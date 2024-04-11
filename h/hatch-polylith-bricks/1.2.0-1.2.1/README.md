# Comparing `tmp/hatch_polylith_bricks-1.2.0.tar.gz` & `tmp/hatch_polylith_bricks-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch_polylith_bricks-1.2.0.tar", max compression
+gzip compressed data, was "hatch_polylith_bricks-1.2.1.tar", max compression
```

## Comparing `hatch_polylith_bricks-1.2.0.tar` & `hatch_polylith_bricks-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3140 2024-01-23 22:26:31.652064 hatch_polylith_bricks-1.2.0/README.md
--rw-r--r--   0        0        0       74 2024-04-08 06:15:46.532447 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/__init__.py
--rw-r--r--   0        0        0      419 2024-04-08 06:15:46.532719 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/core.py
--rw-r--r--   0        0        0        0 2024-01-21 11:02:57.120575 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/hooks/__init__.py
--rw-r--r--   0        0        0     1600 2024-04-08 06:15:46.535651 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py
--rw-r--r--   0        0        0        0 2024-01-21 11:02:57.119034 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch_hooks/__init__.py
--rw-r--r--   0        0        0      192 2024-04-08 06:15:46.532144 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch_hooks/hooks.py
--rw-r--r--   0        0        0      253 2024-04-08 06:15:46.532963 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0      543 2024-04-08 06:15:46.533995 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/__init__.py
--rw-r--r--   0        0        0      861 2024-04-08 06:15:46.534851 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/repo.py
--rw-r--r--   0        0        0      466 2024-04-08 06:15:46.530537 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2919 2024-04-08 06:15:46.531856 hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/toml/core.py
--rw-r--r--   0        0        0      680 2024-04-08 06:15:46.529985 hatch_polylith_bricks-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 hatch_polylith_bricks-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3140 2024-01-23 22:26:31.652064 hatch_polylith_bricks-1.2.1/README.md
+-rw-r--r--   0        0        0       74 2024-04-11 15:26:35.138411 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-11 15:26:35.138667 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/core.py
+-rw-r--r--   0        0        0        0 2024-01-21 11:02:57.120575 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/hooks/__init__.py
+-rw-r--r--   0        0        0     1600 2024-04-11 15:26:35.141601 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py
+-rw-r--r--   0        0        0        0 2024-01-21 11:02:57.119034 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch_hooks/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-11 15:26:35.138145 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch_hooks/hooks.py
+-rw-r--r--   0        0        0      253 2024-04-11 15:26:35.138894 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0      543 2024-04-11 15:26:35.139948 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      861 2024-04-11 15:26:35.140817 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/repo.py
+-rw-r--r--   0        0        0      466 2024-04-11 15:26:35.136568 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     2919 2024-04-11 15:26:35.137889 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/toml/core.py
+-rw-r--r--   0        0        0      676 2024-04-11 15:26:35.136006 hatch_polylith_bricks-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 hatch_polylith_bricks-1.2.1/PKG-INFO
```

### Comparing `hatch_polylith_bricks-1.2.0/README.md` & `hatch_polylith_bricks-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py` & `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/core.py` & `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/parsing/rewrite.py` & `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/__init__.py` & `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/get.py` & `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/repo/repo.py` & `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.0/hatch_polylith_bricks/polylith/toml/core.py` & `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/toml/core.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.0/pyproject.toml` & `hatch_polylith_bricks-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hatch-polylith-bricks"
-version = "1.2.0"
+version = "1.2.1"
 description = "Hatch build hook plugin for Polylith"
 authors = ['David Vujic']
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
 
@@ -15,15 +15,15 @@
 classifiers = [
   "Framework :: Hatch",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 hatchling = "^1.21.0"
-tomlkit = "^0.11.5"
+tomlkit = "0.*"
 
 [tool.poetry.plugins.hatch]
 polylith-bricks = "hatch_polylith_bricks.polylith.hatch_hooks.hooks"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hatch_polylith_bricks-1.2.0/PKG-INFO` & `hatch_polylith_bricks-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hatch-polylith-bricks
-Version: 1.2.0
+Version: 1.2.1
 Summary: Hatch build hook plugin for Polylith
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Hatch
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: hatchling (>=1.21.0,<2.0.0)
-Requires-Dist: tomlkit (>=0.11.5,<0.12.0)
+Requires-Dist: tomlkit (==0.*)
 Project-URL: Repository, https://github.com/davidvujic/python-polylith
 Description-Content-Type: text/markdown
 
 # Hatch Build Hook for Polylith
 
 A plugin for [Hatch](https://hatch.pypa.io/) and the Polylith Architecture.
```

