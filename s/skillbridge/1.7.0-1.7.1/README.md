# Comparing `tmp/skillbridge-1.7.0.tar.gz` & `tmp/skillbridge-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillbridge-1.7.0.tar", last modified: Mon Feb 19 13:30:01 2024, max compression
+gzip compressed data, was "skillbridge-1.7.1.tar", last modified: Thu Apr 11 09:10:48 2024, max compression
```

## Comparing `skillbridge-1.7.0.tar` & `skillbridge-1.7.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:30:01.391861 skillbridge-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-19 13:29:48.000000 skillbridge-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-19 13:29:48.000000 skillbridge-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-02-19 13:30:01.387861 skillbridge-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-19 13:29:48.000000 skillbridge-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-02-19 13:29:48.000000 skillbridge-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 13:30:01.391861 skillbridge-1.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:30:01.383861 skillbridge-1.7.0/skillbridge/
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:30:01.387861 skillbridge-1.7.0/skillbridge/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/hints.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/var.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:30:01.387861 skillbridge-1.7.0/skillbridge/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/server/python_server.il
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/server/python_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:30:01.387861 skillbridge-1.7.0/skillbridge/test/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/test/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/test/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-02-19 13:29:48.000000 skillbridge-1.7.0/skillbridge/test/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-19 13:29:55.000000 skillbridge-1.7.0/skillbridge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:30:01.387861 skillbridge-1.7.0/skillbridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-02-19 13:30:01.000000 skillbridge-1.7.0/skillbridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-19 13:30:01.000000 skillbridge-1.7.0/skillbridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 13:30:01.000000 skillbridge-1.7.0/skillbridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-19 13:30:01.000000 skillbridge-1.7.0/skillbridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-19 13:30:01.000000 skillbridge-1.7.0/skillbridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-19 13:30:01.000000 skillbridge-1.7.0/skillbridge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 13:30:01.387861 skillbridge-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-02-19 13:29:48.000000 skillbridge-1.7.0/tests/test_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-02-19 13:29:48.000000 skillbridge-1.7.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-02-19 13:29:48.000000 skillbridge-1.7.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-19 13:29:48.000000 skillbridge-1.7.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-19 13:29:48.000000 skillbridge-1.7.0/tests/test_test_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-02-19 13:29:48.000000 skillbridge-1.7.0/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-19 13:29:48.000000 skillbridge-1.7.0/tests/test_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-19 13:29:48.000000 skillbridge-1.7.0/tests/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.320073 skillbridge-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-11 09:10:35.000000 skillbridge-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 09:10:35.000000 skillbridge-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-11 09:10:48.320073 skillbridge-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-11 09:10:35.000000 skillbridge-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-11 09:10:35.000000 skillbridge-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:10:48.320073 skillbridge-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.312073 skillbridge-1.7.1/skillbridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.316073 skillbridge-1.7.1/skillbridge/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.316073 skillbridge-1.7.1/skillbridge/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/server/python_server.il
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/server/python_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.316073 skillbridge-1.7.1/skillbridge/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/test/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/test/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-11 09:10:35.000000 skillbridge-1.7.1/skillbridge/test/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 09:10:45.000000 skillbridge-1.7.1/skillbridge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.320073 skillbridge-1.7.1/skillbridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12733 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 09:10:48.000000 skillbridge-1.7.1/skillbridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:10:48.320073 skillbridge-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_test_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 09:10:35.000000 skillbridge-1.7.1/tests/test_workspace.py
```

### Comparing `skillbridge-1.7.0/LICENSE` & `skillbridge-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/PKG-INFO` & `skillbridge-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillbridge
-Version: 1.7.0
+Version: 1.7.1
 Summary: A seamless Python remote bridge to Cadence's Skill in Virtuoso
 Author-email: Niels Buwen <dev@niels-buwen.de>, Tobias Markus <tobias_markus@gmx.net>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -285,7 +285,20 @@
 
 ##### Reading properties
 
 ```python
 >>> print(cell_view.b_box)
 [[0, 10], [2, 8]]
 ```
+
+##### Call any SKILL function
+
+```python
+>>> ws['plus'](3, 4)
+7
+```
+
+*equivalent to:*
+
+```lisp
+(plus 3 4)
+```
```

### Comparing `skillbridge-1.7.0/README.md` & `skillbridge-1.7.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -88,7 +88,20 @@
 
 ##### Reading properties
 
 ```python
 >>> print(cell_view.b_box)
 [[0, 10], [2, 8]]
 ```
+
+##### Call any SKILL function
+
+```python
+>>> ws['plus'](3, 4)
+7
+```
+
+*equivalent to:*
+
+```lisp
+(plus 3 4)
+```
```

### Comparing `skillbridge-1.7.0/pyproject.toml` & `skillbridge-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
     "ISC001",
     "N999",
     "PD901",
     "PLR0911", "PLR6301",
     "PLW1641", "PLW3201",
     "PT001", "PT013",
     "PTH123",
-    "Q000",
     "S101", "S108", "S310", "S311", "S404",
     "T201",
     "TCH001", "TCH002", "TCH003",
     "TID252",
     "TRY003", "TRY004", "TRY400",
 ]
 
@@ -148,14 +147,17 @@
     "S603",
     "S607",
 ]
 "docs/conf.py" = [
     "INP001",
     "A001",
 ]
+"*" = [
+    "Q000",
+]
 
 [tool.ruff.lint.pylint]
 max-args = 7
 
 [tool.ruff.format]
 docstring-code-format = true
 quote-style = "preserve"
```

### Comparing `skillbridge-1.7.0/skillbridge/__init__.py` & `skillbridge-1.7.1/skillbridge/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import contextlib
 from keyword import iskeyword
 from os import chdir
 from pathlib import Path
 from re import fullmatch, sub
 from sys import executable, version_info
+from typing import Any
 
 from .client.functions import FunctionCollection, keys
 from .client.globals import Globals, GlobalVar
 from .client.hints import Function, Key, SkillCode, SkillList, SkillTuple, Symbol
 from .client.objects import LazyList, RemoteObject, RemoteTable, RemoteVector
 from .client.translator import ParseError
 from .client.var import Var
@@ -38,26 +41,36 @@
 ]
 
 loop_var = Var('i')
 loop_var_i = loop_var
 loop_var_j = Var('j')
 
 
-def generate_static_completion() -> None:
-    from mypy.stubgen import Options, generate_stubs  # noqa: PLC0415
+def import_stub_gen() -> tuple[Any, Any]:
+    # the cpython parser wrongly parses a python3.8-valid syntax as invalid
+    # the newest mypy version uses that parser
+    # this syntax occurs in the mypy source code
+    # -> mypy detects a syntax error in its own code base
+    # this can only be ignored by hiding the import code behind an exec call
+    scope: dict[str, Any] = {}
+    exec("from mypy.stubgen import Options, generate_stubs", scope, scope)  # noqa: S102
+    return scope['Options'], scope['generate_stubs']
 
+
+def generate_static_completion() -> None:
+    options, generate_stubs = import_stub_gen()
     base = Path(__file__).parent.absolute() / 'client'
     annotation = base / 'workspace.pyi'
 
     with contextlib.suppress(FileNotFoundError):
         annotation.unlink()
 
     chdir(base)
 
-    o = Options(
+    o = options(
         (version_info.major, version_info.minor),
         no_import=True,
         doc_dir='',
         search_path=[],
         interpreter=executable,
         parse_only=False,
         ignore_errors=False,
```

### Comparing `skillbridge-1.7.0/skillbridge/__main__.py` & `skillbridge-1.7.1/skillbridge/__main__.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/client/channel.py` & `skillbridge-1.7.1/skillbridge/client/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             message = b''.join(self._receive_all(length))
         except Exception as e:  # noqa: BLE001
             return e
         return message.decode()
 
     def close(self) -> None:
         if self.connected:
-            self.socket.sendall(b'         5close')
+            self.socket.sendall(b'         5$close')
             self.socket.close()
             self.connected = False
 
     def flush(self) -> None:
         while True:
             read, _, _ = select([self.socket], [], [], 0.1)
             if read:
```

### Comparing `skillbridge-1.7.0/skillbridge/client/functions.py` & `skillbridge-1.7.1/skillbridge/client/functions.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/client/globals.py` & `skillbridge-1.7.1/skillbridge/client/globals.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/client/hints.py` & `skillbridge-1.7.1/skillbridge/client/hints.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/client/objects.py` & `skillbridge-1.7.1/skillbridge/client/objects.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/client/remote.py` & `skillbridge-1.7.1/skillbridge/client/remote.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/client/translator.py` & `skillbridge-1.7.1/skillbridge/client/translator.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/client/var.py` & `skillbridge-1.7.1/skillbridge/client/var.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/client/workspace.py` & `skillbridge-1.7.1/skillbridge/client/workspace.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,23 +33,14 @@
 
 
 _no_workspace = cast('Workspace', _NoWorkspace())
 current_workspace: Workspace
 current_workspace = _no_workspace
 
 
-def _register_well_known_functions(ws: Workspace) -> None:
-    @ws.register
-    def db_check(d_cellview: Any) -> None:
-        """
-        Checks the integrity of the database.
-        """
-        _ = d_cellview
-
-
 _unbound = Symbol('unbound')
 
 
 class Workspace:
     _var_counter = 0
 
     abe: FunctionCollection
@@ -197,16 +188,14 @@
 
         for key in Workspace.__annotations__:
             value = FunctionCollection(channel, key, self._translator)
             setattr(self, key, value)
 
         self.user = FunctionCollection(channel, 'user', self._translator)
 
-        _register_well_known_functions(self)
-
     def _prepare_default_translator(self) -> DefaultTranslator:
         translator = DefaultTranslator()
         types = [('Remote', RemoteObject), ('Table', RemoteTable), ('Vector', RemoteVector)]
 
         for name, typ in types:
             construct = partial(typ, self._channel, translator)
             translator.register_remote_variable_type(name, construct)
```

### Comparing `skillbridge-1.7.0/skillbridge/server/python_server.il` & `skillbridge-1.7.1/skillbridge/server/python_server.il`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/server/python_server.py` & `skillbridge-1.7.1/skillbridge/server/python_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         logger.debug(f"got length {length}")
 
         length = int(length)
         command = b''.join(self.receive_all(length))
 
         logger.debug(f"received {len(command)} bytes")
 
-        if command.startswith(b'close'):
+        if command.startswith(b'$close'):
             logger.debug(f"client {self.client_address} disconnected")
             return False
         logger.debug(f"got data {command[:1000].decode()}")
 
         send_to_skill(command.decode())
         logger.debug("sent data to skill")
         result = read_from_skill(self.server.skill_timeout).encode()  # type: ignore[attr-defined]
```

### Comparing `skillbridge-1.7.0/skillbridge/test/channel.py` & `skillbridge-1.7.1/skillbridge/test/channel.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/test/translator.py` & `skillbridge-1.7.1/skillbridge/test/translator.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge/test/workspace.py` & `skillbridge-1.7.1/skillbridge/test/workspace.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/skillbridge.egg-info/PKG-INFO` & `skillbridge-1.7.1/skillbridge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillbridge
-Version: 1.7.0
+Version: 1.7.1
 Summary: A seamless Python remote bridge to Cadence's Skill in Virtuoso
 Author-email: Niels Buwen <dev@niels-buwen.de>, Tobias Markus <tobias_markus@gmx.net>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -285,7 +285,20 @@
 
 ##### Reading properties
 
 ```python
 >>> print(cell_view.b_box)
 [[0, 10], [2, 8]]
 ```
+
+##### Call any SKILL function
+
+```python
+>>> ws['plus'](3, 4)
+7
+```
+
+*equivalent to:*
+
+```lisp
+(plus 3 4)
+```
```

### Comparing `skillbridge-1.7.0/skillbridge.egg-info/SOURCES.txt` & `skillbridge-1.7.1/skillbridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/tests/test_channel.py` & `skillbridge-1.7.1/tests/test_channel.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/tests/test_integration.py` & `skillbridge-1.7.1/tests/test_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 from time import sleep
 from warnings import warn
 
-from pytest import fixture, raises, skip
+from pytest import fixture, mark, raises, skip
 
 from skillbridge import LazyList, RemoteObject, RemoteTable, SkillCode, Symbol, Var, Workspace
 
 here = Path(__file__).parent
 
 
 @fixture(scope='module')
@@ -232,15 +232,36 @@
     variable = 'skillbridge_script_args'
     ws['set'](Symbol(variable), 0)
     assert ws['pyRunScript'](str(here / 'script.py'), args=(variable, '42', '0.25'), block=True)
 
     assert ws['plus'](Var(variable), 1) == 43
 
 
+@mark.skip
 def test_form_vectors_have_dir(ws: Workspace) -> None:
     form = ws.hi.get_current_form()
     assert 'button_layout' in dir(form)
 
 
+@mark.skip
 def test_form_vectors_have_getattr(ws: Workspace) -> None:
     form = ws.hi.get_current_form()
     assert isinstance(form.button_layout, list)
+
+
+def test_outstring(ws: Workspace) -> None:
+    outstring = ws['outstring']
+    get_outstring = ws['getOutstring']
+    close = ws['close']
+    fprintf = ws['fprintf']
+
+    s = outstring()
+    assert get_outstring(s) == ""  # noqa: PLC1901
+
+    assert fprintf(s, "Hello ")
+    assert get_outstring(s) == "Hello "
+
+    assert fprintf(s, "World")
+    assert get_outstring(s) == "Hello World"
+
+    assert close(s)
+    assert get_outstring(s) is None
```

### Comparing `skillbridge-1.7.0/tests/test_misc.py` & `skillbridge-1.7.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/tests/test_server.py` & `skillbridge-1.7.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/tests/test_test_channel.py` & `skillbridge-1.7.1/tests/test_test_channel.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/tests/test_translator.py` & `skillbridge-1.7.1/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/tests/test_var.py` & `skillbridge-1.7.1/tests/test_var.py`

 * *Files identical despite different names*

### Comparing `skillbridge-1.7.0/tests/test_workspace.py` & `skillbridge-1.7.1/tests/test_workspace.py`

 * *Files identical despite different names*

