# Comparing `tmp/tsk_monster-0.0.1.tar.gz` & `tmp/tsk_monster-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsk_monster-0.0.1.tar", max compression
+gzip compressed data, was "tsk_monster-0.0.2.tar", max compression
```

## Comparing `tsk_monster-0.0.1.tar` & `tsk_monster-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-04-09 06:29:21.335344 tsk_monster-0.0.1/README.md
--rw-r--r--   0        0        0      442 2024-04-10 13:36:08.875801 tsk_monster-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2719 2024-04-10 13:31:58.772870 tsk_monster-0.0.1/tsk_monster/__init__.py
--rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 tsk_monster-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 14:44:15.334597 tsk_monster-0.0.2/README.md
+-rw-r--r--   0        0        0      442 2024-04-10 20:13:29.689253 tsk_monster-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2946 2024-04-10 20:12:55.221970 tsk_monster-0.0.2/tsk_monster/__init__.py
+-rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 tsk_monster-0.0.2/PKG-INFO
```

### Comparing `tsk_monster-0.0.1/tsk_monster/__init__.py` & `tsk_monster-0.0.2/tsk_monster/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import asyncio
 import logging
 from collections import defaultdict, deque
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, AsyncGenerator, Awaitable, Callable, Iterable, List
+from typing import (Any, AsyncGenerator, Awaitable, Callable, Iterable, List,
+                    Union)
 
-lg = logging.getLogger('👾')
+lg = logging.getLogger(__name__)
 
 
 @dataclass
-class Need:
+class input:
     val: Any
 
 
 @dataclass
-class Make:
+class output:
     val: Any
 
 
-def changed(path: str | Path):
+def changed(path: Path):
     try:
-        path = Path(path)
         tsk = path.with_suffix('.tsk')
         if not tsk.exists():
             return True
 
         return tsk.stat().st_mtime < path.stat().st_mtime
     finally:
         tsk.touch()
@@ -33,93 +33,98 @@
 def none(items: Iterable[bool]):
     return not any(items)
 
 
 @dataclass
 class Tsk:
     name: str
-    gen: AsyncGenerator
+    gen: AsyncGenerator[Union[input, output, "Tsk"], None]
 
     def __repr__(self):
         return self.name
 
 
 def tsk(
         name: str, action: Callable[[], Awaitable], *,
-        need: List[Path] = [],
-        make: List[Path] = []):
+        inputs: List[Path] = [],
+        outputs: List[Path] = []):
 
     async def gen():
-        always_run = len(need) == len(make) == 0
+        always_run = len(inputs) == len(outputs) == 0
 
-        for n in need:
-            yield Need(n)
+        for n in inputs:
+            yield input(n)
 
-        if any(map(changed, need)) or not all(map(Path.exists, make)) or always_run:
+        if any(map(changed, inputs)) or not all(map(Path.exists, outputs)) or always_run:
+            lg.info(f'STARTING: {name}')
             await action()
+            lg.info(f'DONE: {name}')
 
-        for m in make:
+        else:
+            lg.info(f'SKIPPING: {name}')
+
+        for m in outputs:
             if m.exists():
-                yield Make(m)
+                yield output(m)
             else:
-                lg.warning(f'Failed to make {m}.')
+                lg.warning(f'Failed to create {m}.')
 
     return Tsk(name, gen())
 
 
 def shell(
         cmd: str, *,
-        need: List[Path] = [],
-        make: List[Path] = []):
+        inputs: List[Path] = [],
+        outputs: List[Path] = []):
 
     return tsk(
         cmd, lambda: asyncio.create_subprocess_shell(cmd),
-        need=need,
-        make=make)
-
+        inputs=inputs,
+        outputs=outputs)
 
-async def plan(tsks: Iterable[Tsk], parallelism=1):
 
-    def step(tsk: Tsk):
-        lg.info(f'START: {tsk.name}')
-        return anext(tsk.gen)
+async def runner(tsks: Iterable[Tsk], parallelism=1):
 
     tsks = deque(tsks)
     wait = defaultdict(list)
     done = set()
 
     while tsks:
-        head = [tsks.popleft() for _ in range(min(parallelism, len(tsks)))]
+        batch = [
+            tsks.popleft()
+            for _ in range(min(parallelism, len(tsks)))]
 
         results = await asyncio.gather(
-            *(step(tsk) for tsk in head),
+            *(anext(tsk.gen) for tsk in batch),
             return_exceptions=True)
 
-        assert len(head) == len(results)
+        assert len(batch) == len(results)
 
-        for tsk, res in zip(head, results):
-            if isinstance(res, Need) and res.val not in done:
+        for tsk, res in zip(batch, results):
+            if isinstance(res, input) and res.val not in done:
                 wait[res.val].append(tsk)
 
-            elif isinstance(res, Make):
+            elif isinstance(res, output):
                 done.add(res.val)
                 for w in wait.pop(res.val, []):
                     tsks.append(w)
                 tsks.append(tsk)
 
             elif isinstance(res, Tsk):
                 tsks.append(res)
                 tsks.append(tsk)
 
             elif isinstance(res, StopAsyncIteration):
-                lg.info(f'END: {tsk.name}')
+                pass
 
             else:
                 lg.error(f'Failed to run {tsk.name}: {res}')
 
     if wait:
-        print(f'Could not run all tasks: {wait}')
+        lg.warning(f'Could not run all tasks: {wait.values()}')
+        return
+
+    lg.info('All tasks finished.')
 
-    else:
-        print('All tasks finished.')
 
-    return wait
+def run(*tsks: Tsk, parallelism=1):
+    asyncio.run(runner(tsks, parallelism=parallelism))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

