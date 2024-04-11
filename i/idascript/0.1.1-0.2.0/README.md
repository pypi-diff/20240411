# Comparing `tmp/idascript-0.1.1.tar.gz` & `tmp/idascript-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idascript-0.1.1.tar", last modified: Tue Jan  9 15:44:09 2024, max compression
+gzip compressed data, was "idascript-0.2.0.tar", last modified: Thu Apr 11 16:24:51 2024, max compression
```

## Comparing `idascript-0.1.1.tar` & `idascript-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:44:09.277382 idascript-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-09 15:44:00.000000 idascript-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-01-09 15:44:09.277382 idascript-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-01-09 15:44:00.000000 idascript-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-09 15:44:00.000000 idascript-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 15:44:09.277382 idascript-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:44:09.273383 idascript-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:44:09.273383 idascript-0.1.1/src/idascript/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-09 15:44:00.000000 idascript-0.1.1/src/idascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-01-09 15:44:00.000000 idascript-0.1.1/src/idascript/ida.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-09 15:44:00.000000 idascript-0.1.1/src/idascript/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 15:44:09.277382 idascript-0.1.1/src/idascript.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-01-09 15:44:09.000000 idascript-0.1.1/src/idascript.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-09 15:44:09.000000 idascript-0.1.1/src/idascript.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 15:44:09.000000 idascript-0.1.1/src/idascript.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-09 15:44:09.000000 idascript-0.1.1/src/idascript.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-09 15:44:09.000000 idascript-0.1.1/src/idascript.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:24:51.107523 idascript-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 16:24:45.000000 idascript-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-11 16:24:51.107523 idascript-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-11 16:24:45.000000 idascript-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-11 16:24:45.000000 idascript-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:24:51.107523 idascript-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:24:51.107523 idascript-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:24:51.107523 idascript-0.2.0/src/idascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-11 16:24:45.000000 idascript-0.2.0/src/idascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-04-11 16:24:45.000000 idascript-0.2.0/src/idascript/ida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-11 16:24:45.000000 idascript-0.2.0/src/idascript/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:24:51.107523 idascript-0.2.0/src/idascript.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-11 16:24:51.000000 idascript-0.2.0/src/idascript.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 16:24:51.000000 idascript-0.2.0/src/idascript.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:24:51.000000 idascript-0.2.0/src/idascript.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 16:24:51.000000 idascript-0.2.0/src/idascript.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 16:24:51.000000 idascript-0.2.0/src/idascript.egg-info/top_level.txt
```

### Comparing `idascript-0.1.1/LICENSE` & `idascript-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idascript-0.1.1/PKG-INFO` & `idascript-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idascript
-Version: 0.1.1
+Version: 0.2.0
 Summary: IDA Pro wrapper to launch script on binaries
 Author-email: Robin David <rdavid@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/idascript
 Project-URL: Repository, https://github.com/quarkslab/idascript
 Project-URL: Documentation, https://quarkslab.github.io/diffing-portal/idascript/README.html
 Project-URL: Bug Tracker, https://github.com/quarkslab/idascript/issues
```

### Comparing `idascript-0.1.1/README.md` & `idascript-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `idascript-0.1.1/pyproject.toml` & `idascript-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "idascript"
 description = "IDA Pro wrapper to launch script on binaries"
 authors = [{ name = "Robin David", email = "rdavid@quarkslab.com" }]
 license = { text = "Apache Software License (Apache License, Version 2)" }
 readme = { file = "README.md", content-type = "text/markdown" }
-version = '0.1.1'
+version = '0.2.0'
 requires-python = ">=3.8"
 dependencies = [
     'python-magic; os_name!="nt"',
     'python-magic-bin; os_name=="nt"',
     'click',
     'progressbar2',
 ]
```

### Comparing `idascript-0.1.1/src/idascript/__init__.py` & `idascript-0.2.0/src/idascript/__init__.py`

 * *Files identical despite different names*

### Comparing `idascript-0.1.1/src/idascript/ida.py` & `idascript-0.2.0/src/idascript/ida.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import enum
 import subprocess
 import logging
 from idascript import IDA_BINARY
 from pathlib import Path
-from multiprocessing import Pool, Queue
+from multiprocessing import Pool, Queue, Manager
 import queue
 import os
-from typing import List, Optional, Iterable, Union, Generator, Tuple
+from typing import List, Optional, Iterable, Union, Generator
 
 TIMEOUT_RETURNCODE: int = -1
 
 
 class IDAException(Exception):
     """
     Base class for exceptions in the module.
@@ -242,73 +242,69 @@
 
 class MultiIDA:
     """
     Class to trigger multiple IDA processes concurrently
     on a bunch of files.
     """
 
-    _data_queue = Queue()
-    _script_file: Optional[Path] = None
-    _params: List[str] = []
-    _running: bool = False
-    _timeout: float = None
-
     @staticmethod
-    def _worker_handle(bin_file) -> Tuple[int, str]:
-        """
-        Worker function run concurrently
-
-        :param bin_file: binary file to analyse
-        :return: return code, name of binary file
-        """
+    def _worker(ingress, egress, script_file, params, timeout) -> None:
+        while True:
+            try:
+                file = ingress.get(timeout=0.5)
 
-        ida = IDA(bin_file, MultiIDA._script_file, MultiIDA._params, MultiIDA._timeout)
+                ida = IDA(file, script_file, params, timeout)
+                ida.start()
+                res = ida.wait()
 
-        ida.start()
-        res = ida.wait()
-        MultiIDA._data_queue.put((res, bin_file))
-        
-        return res, bin_file.name
+                egress.put((file, res))
+            except queue.Empty:
+                pass
+            except KeyboardInterrupt:
+                break
 
     @staticmethod
     def map(generator: Iterable[Path],
             script: Union[str, Path] = None,
             params: List[str] = None,
             workers: int = None,
-            timeout: Optional[float] = None) -> Generator[Tuple[int, Path], None, None]:
+            timeout: Optional[float] = None) -> Generator[tuple[int, Path], None, None]:
         """
         Iterator the generator sent and apply the script file on each
         file concurrently on a bunch of IDA workers. The function consume
         the generator as fast as it can occupy all the workers and yield a
         tuple (return code, path file) everytime an IDA process as terminated.
 
         :param generator: Iterable of file paths strings (or Path)
         :param script: path to the script to execute
         :param params: list of parameters to send to the script
         :param workers: number of workers to trigger in parallel
         :param timeout: timeout for IDA runs (-1 means infinity)
         :return: generator of files processed (return code, file path)
         """
 
-        if MultiIDA._running:
-            raise MultiIDAAlreadyRunning()
-
-        MultiIDA._running = True
-
-        MultiIDA._script_file = script
-
-        MultiIDA._params = [] if params is None else params
+        manager = Manager()
+        ingress = manager.Queue()
+        egress = manager.Queue()
+        pool = Pool(workers)
 
-        MultiIDA._timeout = timeout
+        # Launch all workers
+        for i in range(workers):
+            pool.apply_async(MultiIDA._worker, (ingress, egress, script, params, timeout))
+
+        # Pre-fill ingress queue
+        total = 0
+        for file in generator:
+            ingress.put(file)
+            total += 1
 
-        pool = Pool(workers)
-        task = pool.map_async(MultiIDA._worker_handle, generator, chunksize=1)
+        i = 0
         while True:
-            try:
-                data = MultiIDA._data_queue.get(True)
-                if data:
-                    yield data
-            except queue.Empty:
-                pass
-            if task.ready():
+            path, res = egress.get()
+            i += 1
+            yield path, res
+
+            # once all items have been processed
+            if i == total:
                 break
-        MultiIDA._running = False
+
+        pool.terminate()
```

### Comparing `idascript-0.1.1/src/idascript/utils.py` & `idascript-0.2.0/src/idascript/utils.py`

 * *Files identical despite different names*

### Comparing `idascript-0.1.1/src/idascript.egg-info/PKG-INFO` & `idascript-0.2.0/src/idascript.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idascript
-Version: 0.1.1
+Version: 0.2.0
 Summary: IDA Pro wrapper to launch script on binaries
 Author-email: Robin David <rdavid@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/idascript
 Project-URL: Repository, https://github.com/quarkslab/idascript
 Project-URL: Documentation, https://quarkslab.github.io/diffing-portal/idascript/README.html
 Project-URL: Bug Tracker, https://github.com/quarkslab/idascript/issues
```

