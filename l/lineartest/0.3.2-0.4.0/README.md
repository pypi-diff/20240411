# Comparing `tmp/lineartest-0.3.2.tar.gz` & `tmp/lineartest-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.3.2.tar", max compression
+gzip compressed data, was "lineartest-0.4.0.tar", max compression
```

## Comparing `lineartest-0.3.2.tar` & `lineartest-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.3.2/LICENSE
--rw-r--r--   0        0        0     1963 2024-04-10 17:55:46.854950 lineartest-0.3.2/README.md
--rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.3.2/lineartest/__init__.py
--rw-r--r--   0        0        0      520 2024-04-10 01:05:25.711594 lineartest-0.3.2/lineartest/_log.py
--rw-r--r--   0        0        0     7447 2024-04-11 03:58:58.173204 lineartest-0.3.2/lineartest/client.py
--rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.3.2/lineartest/schedule.py
--rw-r--r--   0        0        0     1196 2024-04-11 04:00:03.700479 lineartest-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 lineartest-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1930 2024-04-11 10:51:08.025696 lineartest-0.4.0/README.md
+-rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.4.0/lineartest/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-10 01:05:25.711594 lineartest-0.4.0/lineartest/_log.py
+-rw-r--r--   0        0        0     7405 2024-04-11 10:46:29.727763 lineartest-0.4.0/lineartest/client.py
+-rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.4.0/lineartest/schedule.py
+-rw-r--r--   0        0        0     1196 2024-04-11 10:51:49.865980 lineartest-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 lineartest-0.4.0/PKG-INFO
```

### Comparing `lineartest-0.3.2/LICENSE` & `lineartest-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.3.2/README.md` & `lineartest-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # LinearTest
-A testing framework working with Starlette TestClient.
+A testing framework working with httpx.
 
 - **Source code**: https://github.com/fanyf22/lineartest/
 - **Documentation**: https://fanyf22.github.io/lineartest/
 
 ## Dependencies
 
 ```requirements
 python>=3.10
-starlette>=0.37.2
 pydantic>=2.6.4
 pyyaml>=6.0.1
 httpx>=0.27.0
 ```
 
 ## Installing
```

### Comparing `lineartest-0.3.2/lineartest/_log.py` & `lineartest-0.4.0/lineartest/_log.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.3.2/lineartest/client.py` & `lineartest-0.4.0/lineartest/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from collections.abc import Mapping
 from typing import IO, Any, TypeVar
 
 import httpx
 import yaml
 from pydantic import BaseModel
-from starlette.testclient import TestClient
 
 from ._log import LoggerBase
 
 BaseModelType = TypeVar('BaseModelType', bound=BaseModel)
 
 
 class LinearClient(LoggerBase):
     """The main entrypoint to use LinearTest."""
 
-    def __init__(self, test_client: TestClient | None = None):
+    def __init__(self, test_client: httpx.Client | None = None):
         """
         Initialize the `LinearClient` instance.
         :param test_client: the Starlette TestClient instance
         """
         super().__init__()
         self.test_client = test_client
```

### Comparing `lineartest-0.3.2/lineartest/schedule.py` & `lineartest-0.4.0/lineartest/schedule.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.3.2/pyproject.toml` & `lineartest-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lineartest"
-version = "0.3.2"
+version = "0.4.0"
 description = "A testing framework working with Starlette TestClient."
 authors = ["Philip Fan <topfyf@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -16,15 +16,14 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-starlette = "^0.37.2"
 pydantic = "^2.6.4"
 pyyaml = "^6.0.1"
 httpx = "^0.27.0"
 
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.21.3"
@@ -34,14 +33,15 @@
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.17"
 
 
 [tool.poetry.group.test.dependencies]
 fastapi = "^0.110.1"
 python-multipart = "^0.0.9"
+starlette = "^0.37.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff.format]
 quote-style = "single"
```

### Comparing `lineartest-0.3.2/PKG-INFO` & `lineartest-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineartest
-Version: 0.3.2
+Version: 0.4.0
 Summary: A testing framework working with Starlette TestClient.
 License: MIT
 Author: Philip Fan
 Author-email: topfyf@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,28 +15,26 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.13
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: starlette (>=0.37.2,<0.38.0)
 Description-Content-Type: text/markdown
 
 # LinearTest
-A testing framework working with Starlette TestClient.
+A testing framework working with httpx.
 
 - **Source code**: https://github.com/fanyf22/lineartest/
 - **Documentation**: https://fanyf22.github.io/lineartest/
 
 ## Dependencies
 
 ```requirements
 python>=3.10
-starlette>=0.37.2
 pydantic>=2.6.4
 pyyaml>=6.0.1
 httpx>=0.27.0
 ```
 
 ## Installing
```

