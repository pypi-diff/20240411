# Comparing `tmp/luxos-0.0.0.0.tar.gz` & `tmp/luxos-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "luxos-0.0.1.tar", last modified: Wed Apr 10 23:11:04 2024, max compression
```

## Comparing `luxos-0.0.0.0.tar` & `luxos-0.0.1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 luxos-0.0.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 luxos-0.0.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 luxos-0.0.0.0/DEVELOP.md
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 luxos-0.0.0.0/config.yaml
--rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 luxos-0.0.0.0/health-checker.pyz
--rw-r--r--   0        0        0    16246 2020-02-02 00:00:00.000000 luxos-0.0.0.0/luxos.pyz
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 luxos-0.0.0.0/make.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 luxos-0.0.0.0/.github/pull_request_template.md
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 luxos-0.0.0.0/.github/workflows/pull-python-luxos.yml
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 luxos-0.0.0.0/.github/workflows/push-main.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/__main__.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/api.json
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/api.py
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/asyncops.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/exceptions.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/misc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/scripts/__init__.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/scripts/async_luxos.py
--rw-r--r--   0        0        0    31019 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/scripts/health_checker.py
--rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 luxos-0.0.0.0/src/luxos/scripts/luxos.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 luxos-0.0.0.0/tests/conftest.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 luxos-0.0.0.0/tests/requirements.txt
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 luxos-0.0.0.0/tests/test_luxos.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 luxos-0.0.0.0/tests/test_luxos_asyncops.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 luxos-0.0.0.0/tests/test_luxos_misc.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 luxos-0.0.0.0/tests/data/echopool.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 luxos-0.0.0.0/.gitignore
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 luxos-0.0.0.0/README.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 luxos-0.0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 luxos-0.0.0.0/PKG-INFO
+drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     3628 2024-04-10 23:11:04.270379 luxos-0.0.1/PKG-INFO
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     2799 2024-04-10 16:28:21.000000 luxos-0.0.1/README.md
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     1724 2024-04-10 23:11:02.000000 luxos-0.0.1/pyproject.toml
+-rw-r--r--   0 antonio   (1000) antonio   (1000)       38 2024-04-10 23:11:04.270379 luxos-0.0.1/setup.cfg
+drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.267045 luxos-0.0.1/src/
+drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/src/luxos/
+-rw-r--r--   0 antonio   (1000) antonio   (1000)       75 2024-04-10 23:11:02.000000 luxos-0.0.1/src/luxos/__init__.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)       75 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/__main__.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     3501 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/api.json
+-rw-r--r--   0 antonio   (1000) antonio   (1000)      803 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/api.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     9601 2024-04-10 23:06:11.000000 luxos-0.0.1/src/luxos/asyncops.py
+drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/src/luxos/cli/
+-rw-r--r--   0 antonio   (1000) antonio   (1000)        0 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/cli/__init__.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     4546 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/cli/v1.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)      645 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/exceptions.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)      755 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/misc.py
+drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/src/luxos/scripts/
+-rw-r--r--   0 antonio   (1000) antonio   (1000)        0 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/scripts/__init__.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     1639 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)    30158 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)    12195 2024-04-10 16:28:21.000000 luxos-0.0.1/src/luxos/scripts/luxos.py
+drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/src/luxos.egg-info/
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     3628 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 antonio   (1000) antonio   (1000)      632 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 antonio   (1000) antonio   (1000)        1 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 antonio   (1000) antonio   (1000)      102 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 antonio   (1000) antonio   (1000)       33 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 antonio   (1000) antonio   (1000)        6 2024-04-10 23:11:04.000000 luxos-0.0.1/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 antonio   (1000) antonio   (1000)        0 2024-04-10 23:11:04.270379 luxos-0.0.1/tests/
+-rw-r--r--   0 antonio   (1000) antonio   (1000)      555 2024-04-10 16:28:21.000000 luxos-0.0.1/tests/test_cli.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)      478 2024-04-10 16:28:21.000000 luxos-0.0.1/tests/test_luxos.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)     5796 2024-04-10 23:06:11.000000 luxos-0.0.1/tests/test_luxos_asyncops.py
+-rw-r--r--   0 antonio   (1000) antonio   (1000)      558 2024-04-10 16:28:21.000000 luxos-0.0.1/tests/test_luxos_misc.py
```

### Comparing `luxos-0.0.0.0/src/luxos/api.py` & `luxos-0.0.1/src/luxos/api.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from __future__ import annotations
-
-import logging
-import json
-import importlib.resources
-
-log = logging.getLogger(__name__)
-
-
-COMMANDS = json.loads(
-    (importlib.resources.files("luxos") / "api.json")
-    .read_text()
-)
-
-
-def logon_required(cmd: str, commands_list=COMMANDS) -> bool | None:
-    # Check if the command requires logon to LuxOS API
-
-    if cmd not in COMMANDS:
-        log.info("%s command is not supported. "
-                 "Try again with a different command.", cmd)
-        return None
-
-    return COMMANDS[cmd]["logon_required"]
-
-
-# TODO timeouts should be float | None
-def execute_command(host: str, port: int, timeout: int, cmd: str, params: list[str], verbose: bool):
-    from .scripts import luxos
-    return luxos.execute_command(host, port, timeout, cmd, params, verbose)
-
-
+from __future__ import annotations
+
+import logging
+import json
+import importlib.resources
+
+log = logging.getLogger(__name__)
+
+
+COMMANDS = json.loads(
+    (importlib.resources.files("luxos") / "api.json")
+    .read_text()
+)
+
+
+def logon_required(cmd: str, commands_list=COMMANDS) -> bool | None:
+    # Check if the command requires logon to LuxOS API
+
+    if cmd not in COMMANDS:
+        log.info("%s command is not supported. "
+                 "Try again with a different command.", cmd)
+        return None
+
+    return COMMANDS[cmd]["logon_required"]
+
+
+# TODO timeouts should be float | None
+def execute_command(host: str, port: int, timeout: int, cmd: str, params: list[str], verbose: bool):
+    from .scripts import luxos
+    return luxos.execute_command(host, port, timeout, cmd, params, verbose)
+
+
```

### Comparing `luxos-0.0.0.0/src/luxos/exceptions.py` & `luxos-0.0.1/src/luxos/exceptions.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-class LuxosBaseException(Exception):
-    pass
-
-
-class MinerConnectionError(LuxosBaseException):
-    def __init__(self, host: str, port: int, *args, **kwargs):
-        super().__init__(host, port, *args, **kwargs)
-        self.address = (host, port)
-
-    def __str__(self):
-        return (f"<{self.address[0]}:{self.address[1]}>: {self.__class__.__name__}, "
-                f"{self.args[2] if self.args[2:] else 'unknown reason'}")
-
-
-class MinerCommandSessionAlreadyActive(MinerConnectionError):
-    pass
-
-
-class MinerCommandTimeoutError(MinerConnectionError):
-    pass
-
-
-class MinerCommandMalformedMessageError(MinerConnectionError):
-    pass
+class LuxosBaseException(Exception):
+    pass
+
+
+class MinerConnectionError(LuxosBaseException):
+    def __init__(self, host: str, port: int, *args, **kwargs):
+        super().__init__(host, port, *args, **kwargs)
+        self.address = (host, port)
+
+    def __str__(self):
+        return (f"<{self.address[0]}:{self.address[1]}>: {self.__class__.__name__}, "
+                f"{self.args[2] if self.args[2:] else 'unknown reason'}")
+
+
+class MinerCommandSessionAlreadyActive(MinerConnectionError):
+    pass
+
+
+class MinerCommandTimeoutError(MinerConnectionError):
+    pass
+
+
+class MinerCommandMalformedMessageError(MinerConnectionError):
+    pass
```

### Comparing `luxos-0.0.0.0/src/luxos/misc.py` & `luxos-0.0.1/src/luxos/misc.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# catch-all module (find later a better place)
-from __future__ import annotations
-import sys
-import itertools
-
-
-if sys.version_info >= (3, 12):
-    batched = itertools.batched
-else:
-    def batched(iterable, n):
-        if n < 1:
-            raise ValueError("n must be at least one")
-        it = iter(iterable)
-        while batch := tuple(itertools.islice(it, n)):
-            yield batch
-
-
-def indent(txt: str, pre: str = " " * 2) -> str:
-    """simple text indentation"""
-
-    from textwrap import dedent
-
-    txt = dedent(txt)
-    if txt.endswith("\n"):
-        last_eol = "\n"
-        txt = txt[:-1]
-    else:
-        last_eol = ""
-
-    result = pre + txt.replace("\n", "\n" + pre) + last_eol
+# catch-all module (find later a better place)
+from __future__ import annotations
+import sys
+import itertools
+
+
+if sys.version_info >= (3, 12):
+    batched = itertools.batched
+else:
+    def batched(iterable, n):
+        if n < 1:
+            raise ValueError("n must be at least one")
+        it = iter(iterable)
+        while batch := tuple(itertools.islice(it, n)):
+            yield batch
+
+
+def indent(txt: str, pre: str = " " * 2) -> str:
+    """simple text indentation"""
+
+    from textwrap import dedent
+
+    txt = dedent(txt)
+    if txt.endswith("\n"):
+        last_eol = "\n"
+        txt = txt[:-1]
+    else:
+        last_eol = ""
+
+    result = pre + txt.replace("\n", "\n" + pre) + last_eol
     return result if result.strip() else result.strip()
```

### Comparing `luxos-0.0.0.0/src/luxos/scripts/async_luxos.py` & `luxos-0.0.1/src/luxos/scripts/async_luxos.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from __future__ import annotations
-import asyncio
-import json
-
-from .. import misc
-from .. import asyncops
-
-
-async def run(
-    ip_list: list[str],
-    port: int,
-    cmd: str,
-    params: list[str],
-    timeout: float,
-    delay: float | None,
-    details: bool,
-    batchsize: int = 0,
-) -> None:
-    result = {}
-    batchsize = max(batchsize, 2)
-
-    for grupid, addresses in enumerate(
-        misc.batched([(ip, port) for ip in ip_list], n=batchsize)
-    ):
-        tasks = []
-        for host, port in addresses:
-            tasks.append(
-                asyncops.execute_command(
-                    host, port, timeout, cmd, params, add_address=True
-                )
-            )
-        result[grupid] = await asyncio.gather(*tasks, return_exceptions=True)
-
-        # runs only on batchsize, wait delay then proceed onto the next batch
-        if delay:
-            await asyncio.sleep(delay)
-
-    alltasks = [task for group in result.values() for task in group]
-    successes = [task for task in alltasks if not isinstance(task, Exception)]
-    failures = [task for task in alltasks if isinstance(task, Exception)]
-
-    # print a nice report
-    print(f"task executed sucessfully: {len(successes)}")
-    if details:
-        for (host, port), task in successes:  # type: ignore
-            print(f"  > {host}:{port}")
-            print(misc.indent(json.dumps(task, indent=2, sort_keys=True), pre="  | "))
-    print(f"task executed failures: {len(failures)}")
-    for failure in failures:
-        print(f"  {failure}")
-
-
-def main(*args, **kwargs) -> None:
-    asyncio.run(run(*args, **kwargs))
+from __future__ import annotations
+import asyncio
+import json
+
+from .. import misc
+from .. import asyncops
+
+
+async def run(
+    ipaddresses: list[str],
+    port: int,
+    cmd: str,
+    params: list[str],
+    timeout: float,
+    delay: float | None,
+    details: bool,
+    batchsize: int = 0,
+) -> None:
+    result = {}
+    batchsize = max(batchsize, 2)
+
+    for grupid, addresses in enumerate(
+        misc.batched([(ip, port) for ip in ipaddresses], n=batchsize)
+    ):
+        tasks = []
+        for host, port in addresses:
+            tasks.append(
+                asyncops.execute_command(
+                    host, port, timeout, cmd, params, add_address=True
+                )
+            )
+        result[grupid] = await asyncio.gather(*tasks, return_exceptions=True)
+
+        # runs only on batchsize, wait delay then proceed onto the next batch
+        if delay:
+            await asyncio.sleep(delay)
+
+    alltasks = [task for group in result.values() for task in group]
+    successes = [task for task in alltasks if not isinstance(task, Exception)]
+    failures = [task for task in alltasks if isinstance(task, Exception)]
+
+    # print a nice report
+    print(f"task executed sucessfully (use -a|--all for details): {len(successes)}")
+    if details:
+        for (host, port), task in successes:  # type: ignore
+            print(f"  > {host}:{port}")
+            print(misc.indent(json.dumps(task, indent=2, sort_keys=True), pre="  | "))
+    print(f"task executed failures: {len(failures)}")
+    for failure in failures:
+        print(f"  {failure}")
+
+
+def main(*args, **kwargs) -> None:
+    asyncio.run(run(*args, **kwargs))
```

### Comparing `luxos-0.0.0.0/README.md` & `luxos-0.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,75 @@
-# LuxOS Tools Repository
-
-> **WARNING** There are references into the PR luxos-code-refactoring
-
-This repository contains scripts we built to operate and troubleshoot miners running LuxOS.
-
-## Install
-
-There are few ways to install the luxos package:
-
-1. Using pip (suggested for end-users):
-   ```shell
-   pip install luxos
-   pip install git+https://github.com/LuxorLabs/luxos-tooling.git@pr/luxos-code-refactoring  
-   ```
-   Using pip gives you access to the cli commands `luxos` and `health-checker` as well
-   the ability to import in python the `import luxos.api` api for luxos.
-
-2. A single drop in file (for support):
-   ```shell
-   curl -LO https://github.com/LuxorLabs/luxos-tooling/raw/pr/luxos-code-refactoring/luxos.pyz
-   ```
-   These are two standalone [zipapp](https://docs.python.org/3/library/zipapp.html) files, you can use
-   from the command line as `python luxos.pyz`, no dependencies beside a recent-*ish* python
-   version (eg. >= 3.10)
-
-3. From the [github](https://github.com/LuxorLabs/luxos-tooling) source checkout (for devs):
-   ```shell
-   python -m venv venv 
-   source venv/bin/activate # for Windows: .\myenv\Scripts\activate)
-
-   pip install -r tests/requirements.txt
-   
-   export PYTHONPATH=$(pwd)/src # for Windows: SET PYTHONPATH=%CD%\src
-   (or)
-   pip install -e .
-   ```
-
-## LuxOS API Wrapper - luxos
-
-This tool offers a convenient way to interact with LuxOS through a command-line interface (CLI) or as Python packages for more advanced integrations.
-
-**CLI Usage**
-
-The luxos.py script serves as a versatile LuxOS API wrapper, allowing users to interact with LuxOS features directly from the command line. Below are some basic examples:
-
-```bash
-python3 -m luxos --ipfile miners.csv --cmd rebootdevice --timeout 2
-python3 -m luxos --range_start 192.168.1.0 --range_end 192.168.1.255 --cmd rebootdevice --verbose True
-```
-
-> **NOTE** Please don't forget to set the PYTHONPATH.
-
-**Library Usage**
-
-If you prefer to integrate LuxOS functionality into your Python applications or scripts, luxos.py can also be used as a Python package. Here's a quick example:
-
-```python
-from luxos.api import (execute_command)
-
-execute_command("192.168.1.1", 4028, 2, "rebootdevice", "", False)
-```
-
-## LuxOS HealthChecker - health_checker.py
-
-The HealthChecker script is designed to continuously pull miner data from LuxOS, providing valuable insights into the health of your mining machines.
-
-You can customize the HealthChecker params using the `config.yaml` file provided. 
-To run the HealthChecker you can use `health-checker` if you installed using pip, or
-the cli `python3 -m luxos.scripts.health_checker`.
-
----
-
-Feel free to explore and customize these tools to suit your specific needs. 
-If you encounter any issues or have suggestions for improvement, please open an issue or submit a pull request.
-
-You can find LuxOS API documentation [here](https://docs.luxor.tech/firmware/api/intro).
+# LuxOS Tools Repository
+
+This repository contains scripts we built to operate and troubleshoot miners running LuxOS.
+
+## Install
+
+There are few ways to install the luxos package:
+
+1. Using pip (suggested for end-users):
+   ```shell
+   pip install luxos
+   pip install git+https://github.com/LuxorLabs/luxos-tooling.git 
+   ```
+   Using pip gives you access to the cli commands `luxos` and `health-checker` as well
+   the ability to import in python the `import luxos.api` api for luxos.
+
+2. A single drop in file (for support):
+   ```shell
+   curl -LO https://github.com/LuxorLabs/luxos-tooling/raw/luxos.pyz
+   ```
+   These are two standalone [zipapp](https://docs.python.org/3/library/zipapp.html) files, you can use
+   from the command line as `python luxos.pyz`, no dependencies beside a recent-*ish* python
+   version (eg. >= 3.10)
+
+3. From the [github](https://github.com/LuxorLabs/luxos-tooling) source checkout (for devs):
+   ```shell
+   python -m venv venv 
+   source venv/bin/activate # for Windows: .\myenv\Scripts\activate)
+
+   pip install -r tests/requirements.txt
+   
+   export PYTHONPATH=$(pwd)/src # for Windows: SET PYTHONPATH=%CD%\src
+   (or)
+   pip install -e .
+   ```
+
+## LuxOS API Wrapper - luxos
+
+This tool offers a convenient way to interact with LuxOS through a command-line interface (CLI) or as Python packages for more advanced integrations.
+
+**CLI Usage**
+
+The luxos.py script serves as a versatile LuxOS API wrapper, allowing users to interact with LuxOS features directly from the command line. Below are some basic examples:
+
+```bash
+python3 -m luxos --ipfile miners.csv --cmd rebootdevice --timeout 2
+python3 -m luxos --range_start 192.168.1.0 --range_end 192.168.1.255 --cmd rebootdevice --verbose True
+```
+
+> **NOTE** Please don't forget to set the PYTHONPATH.
+
+**Library Usage**
+
+If you prefer to integrate LuxOS functionality into your Python applications or scripts, luxos.py can also be used as a Python package. Here's a quick example:
+
+```python
+from luxos.api import (execute_command)
+
+execute_command("192.168.1.1", 4028, 2, "rebootdevice", "", False)
+```
+
+## LuxOS HealthChecker - health_checker.py
+
+The HealthChecker script is designed to continuously pull miner data from LuxOS, providing valuable insights into the health of your mining machines.
+
+You can customize the HealthChecker params using the `config.yaml` file provided. 
+To run the HealthChecker you can use `health-checker` if you installed using pip, or
+the cli `python3 -m luxos.scripts.health_checker`.
+
+---
+
+Feel free to explore and customize these tools to suit your specific needs. 
+If you encounter any issues or have suggestions for improvement, please open an issue or submit a pull request.
+
+You can find LuxOS API documentation [here](https://docs.luxor.tech/firmware/api/intro).
```

### Comparing `luxos-0.0.0.0/pyproject.toml` & `luxos-0.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,85 @@
-[build-system]
-requires = ["hatchling>=1.1.0",]
-build-backend = "hatchling.build"
-
-[project]
-name = "luxos"
-version = "0.0.0.0"
-description = "The all encompassing LuxOS python library."
-readme = "README.md"
-license = { text = "MIT" }  # TODO I don't think this is a MIT??
-requires-python = ">= 3.9"
-
-authors = [
-  { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
-]
-
-# TODO more classifiers
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-]
-
-dependencies = [
-  "tqdm",
-  "asyncpg",
-  "pandas",
-  "pyyaml",
-  "httpx"
-]
-
-[project.urls]
-Source = "https://github.com/LuxorLabs/firmware-biz-tools"
-Issues = "https://github.com/LuxorLabs/firmware-biz-tools/issues"
-
-[project.scripts]
-luxos = "luxos.scripts.luxos:main"
-health-checker = "luxos.scripts.health_checker:main"
-
-[tool.ruff]
-target-version = "py39"
-line-length = 88
-
-
-[tool.ruff.format]
-quote-style = "double"
-
-[tool.mypy]
-disallow_untyped_defs = false
-follow_imports = "normal"
-ignore_missing_imports = true
-pretty = true
-show_column_numbers = true
-show_error_codes = true
-warn_no_return = false
-warn_unused_ignores = true
-
-[tool.coverage.run]
-branch = true
-
-[tool.coverage.paths]
-source = [
-  "src/",
-]
-
-[tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
-
-[tool.pytest.ini_options]
-markers = [
-    "manual: marks tests unsafe for auto-run (eg. better run them manually)",
-]
+[build-system]
+requires = ["setuptools>=68.0"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
+name = "luxos"
+version = "0.0.1"
+description = "The all encompassing LuxOS python library."
+readme = "README.md"
+license = { text = "MIT" }  # TODO I don't think this is a MIT??
+requires-python = ">= 3.9"
+
+authors = [
+  { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
+]
+
+# TODO more classifiers
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+]
+
+dependencies = [
+  "tqdm",
+  "asyncpg",
+  "pandas",
+  "pyyaml",
+  "httpx"
+]
+
+[project.urls]
+Source = "https://github.com/LuxorLabs/firmware-biz-tools"
+Issues = "https://github.com/LuxorLabs/firmware-biz-tools/issues"
+
+[project.scripts]
+luxos = "luxos.scripts.luxos:main"
+health-checker = "luxos.scripts.health_checker:main"
+
+[tool.setuptools.package-data]
+'luxos' = ['*.json']
+
+
+[tool.ruff]
+target-version = "py39"
+line-length = 88
+
+
+[tool.ruff.format]
+quote-style = "double"
+
+[tool.mypy]
+disallow_untyped_defs = false
+follow_imports = "normal"
+ignore_missing_imports = true
+pretty = true
+show_column_numbers = true
+show_error_codes = true
+warn_no_return = false
+warn_unused_ignores = true
+
+[tool.coverage.run]
+branch = true
+
+[tool.coverage.paths]
+source = [
+  "src/",
+]
+
+[tool.coverage.report]
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
+
+[tool.pytest.ini_options]
+markers = [
+    "manual: marks tests unsafe for auto-run (eg. better run them manually)",
+]
```

### Comparing `luxos-0.0.0.0/PKG-INFO` & `luxos-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.0.0
+Version: 0.0.1
 Summary: The all encompassing LuxOS python library.
-Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
-Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
+Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
+Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: tqdm
 Requires-Dist: asyncpg
-Requires-Dist: httpx
 Requires-Dist: pandas
 Requires-Dist: pyyaml
-Requires-Dist: tqdm
-Description-Content-Type: text/markdown
+Requires-Dist: httpx
 
 # LuxOS Tools Repository
 
-> **WARNING** There are references into the PR luxos-code-refactoring
-
 This repository contains scripts we built to operate and troubleshoot miners running LuxOS.
 
 ## Install
 
 There are few ways to install the luxos package:
 
 1. Using pip (suggested for end-users):
    ```shell
    pip install luxos
-   pip install git+https://github.com/LuxorLabs/luxos-tooling.git@pr/luxos-code-refactoring  
+   pip install git+https://github.com/LuxorLabs/luxos-tooling.git 
    ```
    Using pip gives you access to the cli commands `luxos` and `health-checker` as well
    the ability to import in python the `import luxos.api` api for luxos.
 
 2. A single drop in file (for support):
    ```shell
-   curl -LO https://github.com/LuxorLabs/luxos-tooling/raw/pr/luxos-code-refactoring/luxos.pyz
+   curl -LO https://github.com/LuxorLabs/luxos-tooling/raw/luxos.pyz
    ```
    These are two standalone [zipapp](https://docs.python.org/3/library/zipapp.html) files, you can use
    from the command line as `python luxos.pyz`, no dependencies beside a recent-*ish* python
    version (eg. >= 3.10)
 
 3. From the [github](https://github.com/LuxorLabs/luxos-tooling) source checkout (for devs):
    ```shell
```

