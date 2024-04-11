# Comparing `tmp/kraken_wrapper-0.36.4.tar.gz` & `tmp/kraken_wrapper-0.36.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.36.4.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.36.5.tar", max compression
```

## Comparing `kraken_wrapper-0.36.4.tar` & `kraken_wrapper-0.36.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      352 2023-12-14 08:55:00.365270 kraken_wrapper-0.36.4/README.md
--rw-r--r--   0        0        0     1536 2024-03-26 12:46:20.042384 kraken_wrapper-0.36.4/pyproject.toml
--rw-r--r--   0        0        0      134 2024-03-26 12:46:20.042503 kraken_wrapper-0.36.4/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     3499 2024-03-17 14:51:02.642573 kraken_wrapper-0.36.4/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     6014 2024-02-16 10:07:48.795871 kraken_wrapper-0.36.4/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     1149 2024-03-17 14:51:02.642772 kraken_wrapper-0.36.4/src/kraken/wrapper/_buildenv_uv.py
--rw-r--r--   0        0        0     9900 2024-03-17 14:51:02.646489 kraken_wrapper-0.36.4/src/kraken/wrapper/_buildenv_venv.py
--rw-r--r--   0        0        0     8229 2024-03-17 14:51:02.646729 kraken_wrapper-0.36.4/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4594 2024-02-02 12:43:51.722281 kraken_wrapper-0.36.4/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     5688 2024-02-02 12:43:51.732077 kraken_wrapper-0.36.4/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0    18670 2024-03-17 14:51:02.647059 kraken_wrapper-0.36.4/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2023-12-13 22:21:55.726884 kraken_wrapper-0.36.4/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 kraken_wrapper-0.36.4/PKG-INFO
+-rw-r--r--   0        0        0      352 2024-04-11 17:13:39.320140 kraken_wrapper-0.36.5/README.md
+-rw-r--r--   0        0        0     1408 2024-04-11 19:39:33.065823 kraken_wrapper-0.36.5/pyproject.toml
+-rw-r--r--   0        0        0      134 2024-04-11 19:39:33.066269 kraken_wrapper-0.36.5/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     3499 2024-04-11 17:13:39.320563 kraken_wrapper-0.36.5/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     6014 2024-04-11 17:13:39.320864 kraken_wrapper-0.36.5/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     1149 2024-04-11 18:13:27.451924 kraken_wrapper-0.36.5/src/kraken/wrapper/_buildenv_uv.py
+-rw-r--r--   0        0        0     9900 2024-04-11 18:13:27.452189 kraken_wrapper-0.36.5/src/kraken/wrapper/_buildenv_venv.py
+-rw-r--r--   0        0        0     8229 2024-04-11 17:13:39.321280 kraken_wrapper-0.36.5/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4594 2024-04-11 17:13:39.321459 kraken_wrapper-0.36.5/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     5688 2024-04-11 17:13:39.321632 kraken_wrapper-0.36.5/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0    18670 2024-04-11 17:13:39.321759 kraken_wrapper-0.36.5/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:13:39.321836 kraken_wrapper-0.36.5/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 kraken_wrapper-0.36.5/PKG-INFO
```

### Comparing `kraken_wrapper-0.36.4/pyproject.toml` & `kraken_wrapper-0.36.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.36.4"
+version = "0.36.5"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   {include = "kraken/wrapper", from = "src"},
 ]
@@ -18,29 +18,22 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kraken-build/kraken-build/issues"
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
 [tool.poetry.dependencies]
-kraken-build = "0.36.4"
+kraken-build = "0.36.5"
 packaging = "^23.1"
 python = ">=3.10"
-termcolor = "^1.1.0"
+termcolor = "^2.0.0"
 uv = "^0.1.0"
 
 [tool.poetry.dev-dependencies]
-black = "^23.10.1"
-flake8 = "^6.1.0"
-isort = "^5.12.0"
-mypy = "^1.6.1"
-pycln = "^2.1.3"
-pylint = "^3.0.2"
 pytest = ">=6.0.0"
-pyupgrade = "^3.15.0"
 
 [tool.poetry.scripts]
 krakenw = "kraken.wrapper.main:main"
 
 [tool.slap]
 typed = true
```

### Comparing `kraken_wrapper-0.36.4/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.36.5/src/kraken/wrapper/_buildenv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.36.4/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.36.5/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.36.4/src/kraken/wrapper/_buildenv_uv.py` & `kraken_wrapper-0.36.5/src/kraken/wrapper/_buildenv_uv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.36.4/src/kraken/wrapper/_buildenv_venv.py` & `kraken_wrapper-0.36.5/src/kraken/wrapper/_buildenv_venv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.36.4/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.36.5/src/kraken/wrapper/_config.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.36.4/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.36.5/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.36.4/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.36.5/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.36.4/src/kraken/wrapper/main.py` & `kraken_wrapper-0.36.5/src/kraken/wrapper/main.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.36.4/PKG-INFO` & `kraken_wrapper-0.36.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.36.4
+Version: 0.36.5
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: kraken-build (==0.36.4)
+Requires-Dist: kraken-build (==0.36.5)
 Requires-Dist: packaging (>=23.1,<24.0)
-Requires-Dist: termcolor (>=1.1.0,<2.0.0)
+Requires-Dist: termcolor (>=2.0.0,<3.0.0)
 Requires-Dist: uv (>=0.1.0,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
 Project-URL: Homepage, https://kraken-build.github.io/kraken-build/
 Project-URL: Repository, https://github.com/kraken-build/kraken-build/
 Description-Content-Type: text/markdown
```

