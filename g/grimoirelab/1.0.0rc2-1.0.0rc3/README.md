# Comparing `tmp/grimoirelab-1.0.0rc2.tar.gz` & `tmp/grimoirelab-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab-1.0.0rc2.tar", max compression
+gzip compressed data, was "grimoirelab-1.0.0rc3.tar", max compression
```

## Comparing `grimoirelab-1.0.0rc2.tar` & `grimoirelab-1.0.0rc3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35141 2024-04-10 11:00:30.355302 grimoirelab-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     8685 2024-04-10 11:00:30.355302 grimoirelab-1.0.0rc2/README.md
--rw-r--r--   0        0        0       34 2024-04-10 11:00:30.423303 grimoirelab-1.0.0rc2/grimoirelab/__init__.py
--rw-r--r--   0        0        0       91 2024-04-10 11:00:30.423303 grimoirelab-1.0.0rc2/grimoirelab/_version.py
--rwxr-xr-x   0        0        0     1844 2024-04-10 11:00:30.423303 grimoirelab-1.0.0rc2/grimoirelab/grimoirelab.py
--rw-r--r--   0        0        0     1882 2024-04-10 11:00:30.423303 grimoirelab-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0    10171 1970-01-01 00:00:00.000000 grimoirelab-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    35141 2024-04-11 11:34:01.686269 grimoirelab-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0     8685 2024-04-11 11:34:01.686269 grimoirelab-1.0.0rc3/README.md
+-rw-r--r--   0        0        0       34 2024-04-11 11:34:01.754269 grimoirelab-1.0.0rc3/grimoirelab/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-11 11:34:01.754269 grimoirelab-1.0.0rc3/grimoirelab/_version.py
+-rwxr-xr-x   0        0        0     1844 2024-04-11 11:34:01.754269 grimoirelab-1.0.0rc3/grimoirelab/grimoirelab.py
+-rw-r--r--   0        0        0     1882 2024-04-11 11:34:01.754269 grimoirelab-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    10171 1970-01-01 00:00:00.000000 grimoirelab-1.0.0rc3/PKG-INFO
```

### Comparing `grimoirelab-1.0.0rc2/LICENSE` & `grimoirelab-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab-1.0.0rc2/README.md` & `grimoirelab-1.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab-1.0.0rc2/grimoirelab/grimoirelab.py` & `grimoirelab-1.0.0rc3/grimoirelab/grimoirelab.py`

 * *Files identical despite different names*

### Comparing `grimoirelab-1.0.0rc2/pyproject.toml` & `grimoirelab-1.0.0rc3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab"
-version = "1.0.0-rc.2"
+version = "1.0.0-rc.3"
 description = "Tool set for software development analytics"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -35,25 +35,25 @@
 [tool.poetry.scripts]
 'grimoirelab' = 'grimoirelab.grimoirelab:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 grimoirelab-toolkit = {version = ">=1.0.0-rc.2", allow-prereleases = true}
-perceval-mozilla = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-perceval-opnfv = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-perceval-puppet = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-perceval-weblate = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-sortinghat = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-kidash = {version = ">=1.0.0-rc.1", allow-prereleases = true}
+perceval-mozilla = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+perceval-opnfv = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+perceval-puppet = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+perceval-weblate = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+sortinghat = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+kidash = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 grimoirelab-panels = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-grimoire-elk = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-sirmordred = {version = ">=1.0.0-rc.1", allow-prereleases = true}
+grimoire-elk = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+sirmordred = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 cereslib = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-graal = {version = ">=1.0.0-rc.1", allow-prereleases = true}
-perceval = {version = ">=1.0.0-rc.1", allow-prereleases = true}
+graal = {version = ">=1.0.0-rc.2", allow-prereleases = true}
+perceval = {version = ">=1.0.0-rc.2", allow-prereleases = true}
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grimoirelab-1.0.0rc2/PKG-INFO` & `grimoirelab-1.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoirelab
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Tool set for software development analytics
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,26 +13,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Dist: cereslib (>=1.0.0-rc.1)
-Requires-Dist: graal (>=1.0.0-rc.1)
-Requires-Dist: grimoire-elk (>=1.0.0-rc.1)
+Requires-Dist: graal (>=1.0.0-rc.2)
+Requires-Dist: grimoire-elk (>=1.0.0-rc.2)
 Requires-Dist: grimoirelab-panels (>=1.0.0-rc.1)
 Requires-Dist: grimoirelab-toolkit (>=1.0.0-rc.2)
-Requires-Dist: kidash (>=1.0.0-rc.1)
-Requires-Dist: perceval (>=1.0.0-rc.1)
-Requires-Dist: perceval-mozilla (>=1.0.0-rc.1)
-Requires-Dist: perceval-opnfv (>=1.0.0-rc.1)
-Requires-Dist: perceval-puppet (>=1.0.0-rc.1)
-Requires-Dist: perceval-weblate (>=1.0.0-rc.1)
-Requires-Dist: sirmordred (>=1.0.0-rc.1)
-Requires-Dist: sortinghat (>=1.0.0-rc.1)
+Requires-Dist: kidash (>=1.0.0-rc.2)
+Requires-Dist: perceval (>=1.0.0-rc.2)
+Requires-Dist: perceval-mozilla (>=1.0.0-rc.2)
+Requires-Dist: perceval-opnfv (>=1.0.0-rc.2)
+Requires-Dist: perceval-puppet (>=1.0.0-rc.2)
+Requires-Dist: perceval-weblate (>=1.0.0-rc.2)
+Requires-Dist: sirmordred (>=1.0.0-rc.2)
+Requires-Dist: sortinghat (>=1.0.0-rc.2)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab
 Description-Content-Type: text/markdown
 
 # GrimoireLab
 
 [![grimoirelab-showcase](https://user-images.githubusercontent.com/25265451/84442403-30dcce80-ac5b-11ea-9f5b-60266d875ebd.png "GrimoireLab | CHAOSS Bitergia Analytics")](https://chaoss.biterg.io/app/kibana#/dashboard/Overview)
```

