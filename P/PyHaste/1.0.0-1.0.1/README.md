# Comparing `tmp/pyhaste-1.0.0.tar.gz` & `tmp/pyhaste-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhaste-1.0.0.tar", max compression
+gzip compressed data, was "pyhaste-1.0.1.tar", max compression
```

## Comparing `pyhaste-1.0.0.tar` & `pyhaste-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1506 2024-04-10 17:21:09.860530 pyhaste-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     7927 2024-04-10 17:21:09.860530 pyhaste-1.0.0/README.md
--rw-r--r--   0        0        0      177 2024-04-10 17:21:09.860530 pyhaste-1.0.0/pyhaste/__init__.py
--rw-r--r--   0        0        0     2175 2024-04-10 17:21:09.860530 pyhaste-1.0.0/pyhaste/analyzer.py
--rw-r--r--   0        0        0      343 2024-04-10 17:21:09.860530 pyhaste-1.0.0/pyhaste/test_analyzer.py
--rw-r--r--   0        0        0      878 2024-04-10 17:21:37.388809 pyhaste-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8659 1970-01-01 00:00:00.000000 pyhaste-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2024-04-10 17:24:17.748694 pyhaste-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     7977 2024-04-10 17:24:17.748694 pyhaste-1.0.1/README.md
+-rw-r--r--   0        0        0      177 2024-04-10 17:24:17.748694 pyhaste-1.0.1/pyhaste/__init__.py
+-rw-r--r--   0        0        0     2175 2024-04-10 17:24:17.748694 pyhaste-1.0.1/pyhaste/analyzer.py
+-rw-r--r--   0        0        0      343 2024-04-10 17:24:17.748694 pyhaste-1.0.1/pyhaste/test_analyzer.py
+-rw-r--r--   0        0        0      878 2024-04-10 17:24:43.629260 pyhaste-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8709 1970-01-01 00:00:00.000000 pyhaste-1.0.1/PKG-INFO
```

### Comparing `pyhaste-1.0.0/LICENSE.md` & `pyhaste-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhaste-1.0.0/README.md` & `pyhaste-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/cocreators-ee/pyhaste/blob/master/.pre-commit-config.yaml)
 [![PyPI](https://img.shields.io/pypi/v/pyhaste)](https://pypi.org/project/pyhaste/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyhaste)](https://pypi.org/project/pyhaste/)
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 Python code speed analyzer.
 
-![PyHaste screenshot](pyhaste.png)
+![PyHaste screenshot](https://github.com/cocreators-ee/pyhaste/raw/main/pyhaste.png)
 
 Monitor the performance of your scripts etc. tools and understand where time is spent.
 
 ## Installation
 
 It's a Python library, what do you expect?
```

### Comparing `pyhaste-1.0.0/pyhaste/analyzer.py` & `pyhaste-1.0.1/pyhaste/analyzer.py`

 * *Files identical despite different names*

### Comparing `pyhaste-1.0.0/pyproject.toml` & `pyhaste-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyHaste"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python code speed analyzer"
 authors = ["Janne Enberg <janne.enberg@lietu.net>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/cocreators-ee/pyhaste/"
 repository = "https://github.com/cocreators-ee/pyhaste/"
 documentation = "https://github.com/cocreators-ee/pyhaste/"
```

### Comparing `pyhaste-1.0.0/PKG-INFO` & `pyhaste-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHaste
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python code speed analyzer
 Home-page: https://github.com/cocreators-ee/pyhaste/
 License: BSD-3-Clause
 Keywords: performance,measuring,benchmark,benchmarking,analyzer
 Author: Janne Enberg
 Author-email: janne.enberg@lietu.net
 Requires-Python: >=3.11,<4.0
@@ -24,15 +24,15 @@
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/cocreators-ee/pyhaste/blob/master/.pre-commit-config.yaml)
 [![PyPI](https://img.shields.io/pypi/v/pyhaste)](https://pypi.org/project/pyhaste/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyhaste)](https://pypi.org/project/pyhaste/)
 [![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 Python code speed analyzer.
 
-![PyHaste screenshot](pyhaste.png)
+![PyHaste screenshot](https://github.com/cocreators-ee/pyhaste/raw/main/pyhaste.png)
 
 Monitor the performance of your scripts etc. tools and understand where time is spent.
 
 ## Installation
 
 It's a Python library, what do you expect?
```

