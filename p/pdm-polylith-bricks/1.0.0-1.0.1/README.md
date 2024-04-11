# Comparing `tmp/pdm_polylith_bricks-1.0.0.tar.gz` & `tmp/pdm_polylith_bricks-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_polylith_bricks-1.0.0.tar", max compression
+gzip compressed data, was "pdm_polylith_bricks-1.0.1.tar", max compression
```

## Comparing `pdm_polylith_bricks-1.0.0.tar` & `pdm_polylith_bricks-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2825 2024-01-23 21:16:34.626643 pdm_polylith_bricks-1.0.0/README.md
--rw-r--r--   0        0        0      565 2024-04-08 06:17:20.390842 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2191 2024-04-08 06:17:20.391693 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/configuration/core.py
--rw-r--r--   0        0        0      249 2024-04-08 06:17:20.393823 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/__init__.py
--rw-r--r--   0        0        0     1147 2024-04-08 06:17:20.396272 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/core.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/__init__.py
--rw-r--r--   0        0        0      637 2024-04-08 06:17:20.396787 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py
--rw-r--r--   0        0        0     1019 2024-04-08 06:17:20.398343 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.620904 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm_project_hooks/__init__.py
--rw-r--r--   0        0        0      259 2024-04-08 06:17:20.393602 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm_project_hooks/core.py
--rw-r--r--   0        0        0      539 2024-04-08 06:17:20.394816 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/__init__.py
--rw-r--r--   0        0        0      859 2024-04-08 06:17:20.395648 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/repo.py
--rw-r--r--   0        0        0      464 2024-04-08 06:17:20.391973 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2917 2024-04-08 06:17:20.393228 pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/toml/core.py
--rw-r--r--   0        0        0      618 2024-04-08 06:17:20.390284 pdm_polylith_bricks-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3507 1970-01-01 00:00:00.000000 pdm_polylith_bricks-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2825 2024-01-23 21:16:34.626643 pdm_polylith_bricks-1.0.1/README.md
+-rw-r--r--   0        0        0      565 2024-04-11 15:27:32.081655 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2191 2024-04-11 15:27:32.082518 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/configuration/core.py
+-rw-r--r--   0        0        0      249 2024-04-11 15:27:32.084613 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm/__init__.py
+-rw-r--r--   0        0        0     1147 2024-04-11 15:27:32.087181 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm/core.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm/hooks/__init__.py
+-rw-r--r--   0        0        0      637 2024-04-11 15:27:32.087705 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py
+-rw-r--r--   0        0        0     1019 2024-04-11 15:27:32.089180 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.620904 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm_project_hooks/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-11 15:27:32.084396 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm_project_hooks/core.py
+-rw-r--r--   0        0        0      539 2024-04-11 15:27:32.085627 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      859 2024-04-11 15:27:32.086509 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/repo/repo.py
+-rw-r--r--   0        0        0      464 2024-04-11 15:27:32.082788 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     2917 2024-04-11 15:27:32.084031 pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/toml/core.py
+-rw-r--r--   0        0        0      614 2024-04-11 15:27:32.081072 pdm_polylith_bricks-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 pdm_polylith_bricks-1.0.1/PKG-INFO
```

### Comparing `pdm_polylith_bricks-1.0.0/README.md` & `pdm_polylith_bricks-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/configuration/__init__.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/configuration/core.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/core.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/parsing/rewrite.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/core.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/__init__.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/get.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/repo/repo.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pdm_polylith_bricks/polylith/toml/core.py` & `pdm_polylith_bricks-1.0.1/pdm_polylith_bricks/polylith/toml/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.0/pyproject.toml` & `pdm_polylith_bricks-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pdm-polylith-bricks"
-version = "1.0.0"
+version = "1.0.1"
 description = "a PDM build hook for Polylith"
 authors = ["David Vujic"]
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
 
 packages = [
     {include = "pdm_polylith_bricks"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-tomlkit = "^0.11.5"
+tomlkit = "0.*"
 
 [tool.poetry.plugins."pdm.build.hook"]
 polylith-bricks = "pdm_polylith_bricks.polylith.pdm_project_hooks.core"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pdm_polylith_bricks-1.0.0/PKG-INFO` & `pdm_polylith_bricks-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pdm-polylith-bricks
-Version: 1.0.0
+Version: 1.0.1
 Summary: a PDM build hook for Polylith
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: tomlkit (>=0.11.5,<0.12.0)
+Requires-Dist: tomlkit (==0.*)
 Project-URL: Repository, https://github.com/davidvujic/python-polylith
 Description-Content-Type: text/markdown
 
 # PDM Build Hook for Polylith
 
 A plugin for [PDM](https://pdm-project.org) and the Polylith Architecture.
```

