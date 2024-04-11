# Comparing `tmp/pytest_xdist_worker_stats-0.1.5.tar.gz` & `tmp/pytest_xdist_worker_stats-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_xdist_worker_stats-0.1.5.tar", max compression
+gzip compressed data, was "pytest_xdist_worker_stats-0.1.6.tar", max compression
```

## Comparing `pytest_xdist_worker_stats-0.1.5.tar` & `pytest_xdist_worker_stats-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/LICENSE
--rw-r--r--   0        0        0     2305 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/README.md
--rw-r--r--   0        0        0     2857 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       75 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/__init__.py
--rw-r--r--   0        0        0      937 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/options.py
--rw-r--r--   0        0        0     3639 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/plugin.py
--rw-r--r--   0        0        0     3299 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2305 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/README.md
+-rw-r--r--   0        0        0     2963 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       75 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/options.py
+-rw-r--r--   0        0        0     3639 2024-04-11 14:39:31.042688 pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/plugin.py
+-rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.6/PKG-INFO
```

### Comparing `pytest_xdist_worker_stats-0.1.5/LICENSE` & `pytest_xdist_worker_stats-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.5/README.md` & `pytest_xdist_worker_stats-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.5/pyproject.toml` & `pytest_xdist_worker_stats-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 [tool.poetry]
 name = "pytest-xdist-worker-stats"
-version = "0.1.5"
+version = "0.1.6"
 description = "A pytest plugin to list worker statistics after a xdist run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_xdist_worker_stats"}]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Testing",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Framework :: Pytest",
 ]
 include = ["LICENSE"]
 repository = "https://github.com/mikicz/pytest-xdist-worker-stats"
 keywords = ["pytest", "xdist", "pytest-xdist"]
 
 [tool.poetry.plugins."pytest11"]
 pytest-xdist-worker-stats = "pytest_xdist_worker_stats"
 
 [tool.poetry.dependencies]
-python = ">3.9"
+python = ">=3.8"
 pytest = ">7.3.2"
 pytest-xdist = "^3.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.9.1"
 ruff = "^0.0.291"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target_version = ['py310', 'py311', 'py312']
+target_version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.git         # exclude a few common directories in the
     | \.tox         # root of the project
     | venv
@@ -79,15 +81,15 @@
     # https://github.com/charliermarsh/ruff#flake8-return-ret
     "RET",
     # https://github.com/charliermarsh/ruff#flake8-simplify-sim
     "SIM",
 ]
 
 line-length = 120
-target-version = "py310"
+target-version = "py38"
 
 # Never enforce...
 ignore = [
     "E501",   # line length violations
     "PT004",  # missing-fixture-name-underscore
     "SIM108", # use-ternary-operator
     "RET505", # superfluous-else-return
```

### Comparing `pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/options.py` & `pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/options.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/plugin.py` & `pytest_xdist_worker_stats-0.1.6/pytest_xdist_worker_stats/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.5/PKG-INFO` & `pytest_xdist_worker_stats-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: pytest-xdist-worker-stats
-Version: 0.1.5
+Version: 0.1.6
 Summary: A pytest plugin to list worker statistics after a xdist run.
 Home-page: https://github.com/mikicz/pytest-xdist-worker-stats
 License: MIT
 Keywords: pytest,xdist,pytest-xdist
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
-Requires-Python: >3.9
+Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: pytest (>7.3.2)
 Requires-Dist: pytest-xdist (>=3.3,<4.0)
 Project-URL: Repository, https://github.com/mikicz/pytest-xdist-worker-stats
```

