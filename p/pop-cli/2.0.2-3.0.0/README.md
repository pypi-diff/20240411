# Comparing `tmp/pop_cli-2.0.2.tar.gz` & `tmp/pop_cli-3.0.0.tar.gz`

## Comparing `pop_cli-2.0.2.tar` & `pop_cli-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pop_cli-2.0.2/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/__main__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/config.yaml
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/cli.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/config.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/console.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/init.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/ref.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/state.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_init.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_ref.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-2.0.2/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-2.0.2/README.rst
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pop_cli-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pop_cli-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pop_cli-3.0.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 pop_cli-3.0.0/src/__main__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pop_cli-3.0.0/src/config.yaml
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pop_cli-3.0.0/src/hub/cli.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-3.0.0/src/hub/config.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 pop_cli-3.0.0/src/hub/console.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 pop_cli-3.0.0/src/hub/init.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-3.0.0/src/hub/ref.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pop_cli-3.0.0/src/hub/state.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-3.0.0/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-3.0.0/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-3.0.0/README.rst
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pop_cli-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pop_cli-3.0.0/PKG-INFO
```

### Comparing `pop_cli-2.0.2/.pre-commit-config.yaml` & `pop_cli-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/src/__main__.py` & `pop_cli-3.0.0/src/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 
-import pop.hub
+import cpop.hub
 
 try:
     import uvloop
 
     HAS_UVLOOP = True
 except ImportError:
     HAS_UVLOOP = False
@@ -21,15 +21,15 @@
 
     # Start the async code
     asyncio.run(amain())
 
 
 async def amain():
     # Create the hub within an async context
-    hub = await pop.hub.AsyncHub(cli="cli")
+    hub = await cpop.hub.AsyncHub(cli="cli")
 
     # Start the hub cli
     await hub.cli.init.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pop_cli-2.0.2/src/config.yaml` & `pop_cli-3.0.0/src/config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/src/hub/cli.py` & `pop_cli-3.0.0/src/hub/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/src/hub/config.py` & `pop_cli-3.0.0/src/hub/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/src/hub/console.py` & `pop_cli-3.0.0/src/hub/console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/src/hub/init.py` & `pop_cli-3.0.0/src/hub/init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/src/hub/ref.py` & `pop_cli-3.0.0/src/hub/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/src/hub/state.py` & `pop_cli-3.0.0/src/hub/state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/tests/conftest.py` & `pop_cli-3.0.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pathlib
 import sys
 import unittest.mock as mock
 
-import pop.hub
+import cpop.hub
 import pytest
 
 
 @pytest.fixture(name="hub")
 async def testing_hub():
-    yield await pop.hub.AsyncHub()
+    yield await cpop.hub.AsyncHub()
 
 
 @pytest.fixture(autouse=True, scope="session")
 def tpath():
     code_dir = pathlib.Path(__file__).parent.parent.absolute()
     assert code_dir.exists()
```

### Comparing `pop_cli-2.0.2/tests/integration/test_cli.py` & `pop_cli-3.0.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/tests/integration/test_config.py` & `pop_cli-3.0.0/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/tests/integration/test_console.py` & `pop_cli-3.0.0/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/tests/integration/test_init.py` & `pop_cli-3.0.0/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/tests/integration/test_ref.py` & `pop_cli-3.0.0/tests/integration/test_ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/tests/integration/test_state.py` & `pop_cli-3.0.0/tests/integration/test_state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/.gitignore` & `pop_cli-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/README.rst` & `pop_cli-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.2/pyproject.toml` & `pop_cli-3.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "2.0.2"
+version = "3.0.0"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
 ]
 requires-python = ">=3.10"
 dependencies = [
-    "cPop>=32.0.2",
+    "cPop>=33.0.0",
     "aioconsole",
     "uvloop; sys_platform != 'win32'",
     "prompt-toolkit",
 ]
 
 
 [project.optional-dependencies]
```

### Comparing `pop_cli-2.0.2/PKG-INFO` & `pop_cli-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 2.0.2
+Version: 3.0.0
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Requires-Dist: aioconsole
-Requires-Dist: cpop>=32.0.2
+Requires-Dist: cpop>=33.0.0
 Requires-Dist: prompt-toolkit
 Requires-Dist: uvloop; sys_platform != 'win32'
 Provides-Extra: test
 Requires-Dist: pexpect; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Description-Content-Type: text/x-rst
```

