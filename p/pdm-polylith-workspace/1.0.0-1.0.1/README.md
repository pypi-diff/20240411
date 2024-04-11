# Comparing `tmp/pdm_polylith_workspace-1.0.0.tar.gz` & `tmp/pdm_polylith_workspace-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_polylith_workspace-1.0.0.tar", max compression
+gzip compressed data, was "pdm_polylith_workspace-1.0.1.tar", max compression
```

## Comparing `pdm_polylith_workspace-1.0.0.tar` & `pdm_polylith_workspace-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1008 2024-01-23 21:16:34.627315 pdm_polylith_workspace-1.0.0/README.md
--rw-r--r--   0        0        0      568 2024-04-08 06:18:29.082224 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2194 2024-04-08 06:18:29.083066 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/configuration/core.py
--rw-r--r--   0        0        0      255 2024-04-08 06:18:29.085193 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/__init__.py
--rw-r--r--   0        0        0     1150 2024-04-08 06:18:29.087705 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/core.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/__init__.py
--rw-r--r--   0        0        0      643 2024-04-08 06:18:29.088206 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py
--rw-r--r--   0        0        0     1022 2024-04-08 06:18:29.088916 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.621252 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm_workspace_hooks/__init__.py
--rw-r--r--   0        0        0      465 2024-04-08 06:18:29.084970 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm_workspace_hooks/core.py
--rw-r--r--   0        0        0      545 2024-04-08 06:18:29.086211 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/__init__.py
--rw-r--r--   0        0        0      862 2024-04-08 06:18:29.087058 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/repo.py
--rw-r--r--   0        0        0      467 2024-04-08 06:18:29.083338 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2920 2024-04-08 06:18:29.084564 pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/toml/core.py
--rw-r--r--   0        0        0      645 2024-04-08 06:18:29.081665 pdm_polylith_workspace-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 pdm_polylith_workspace-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1008 2024-01-23 21:16:34.627315 pdm_polylith_workspace-1.0.1/README.md
+-rw-r--r--   0        0        0      568 2024-04-11 15:28:15.485401 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2194 2024-04-11 15:28:15.486256 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/configuration/core.py
+-rw-r--r--   0        0        0      255 2024-04-11 15:28:15.488389 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/__init__.py
+-rw-r--r--   0        0        0     1150 2024-04-11 15:28:15.490864 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/core.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/__init__.py
+-rw-r--r--   0        0        0      643 2024-04-11 15:28:15.491360 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py
+-rw-r--r--   0        0        0     1022 2024-04-11 15:28:15.492077 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py
+-rw-r--r--   0        0        0        0 2024-01-23 21:16:34.621252 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm_workspace_hooks/__init__.py
+-rw-r--r--   0        0        0      465 2024-04-11 15:28:15.488162 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm_workspace_hooks/core.py
+-rw-r--r--   0        0        0      545 2024-04-11 15:28:15.489391 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-11 15:28:15.490231 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/repo.py
+-rw-r--r--   0        0        0      467 2024-04-11 15:28:15.486521 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     2920 2024-04-11 15:28:15.487750 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/toml/core.py
+-rw-r--r--   0        0        0      641 2024-04-11 15:28:15.484828 pdm_polylith_workspace-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1694 1970-01-01 00:00:00.000000 pdm_polylith_workspace-1.0.1/PKG-INFO
```

### Comparing `pdm_polylith_workspace-1.0.0/README.md` & `pdm_polylith_workspace-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/configuration/__init__.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/configuration/core.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/core.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/parsing/rewrite.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/core.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/__init__.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/get.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/repo/repo.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pdm_polylith_workspace/polylith/toml/core.py` & `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/toml/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.0/pyproject.toml` & `pdm_polylith_workspace-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pdm-polylith-workspace"
-version = "1.0.0"
+version = "1.0.1"
 description = "a PDM build hook for a Polylith workspace"
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 authors = ["David Vujic"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     {include = "pdm_polylith_workspace"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-tomlkit = "^0.11.5"
+tomlkit = "0.*"
 
 [tool.poetry.plugins."pdm.build.hook"]
 polylith-workspace = "pdm_polylith_workspace.polylith.pdm_workspace_hooks.core"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pdm_polylith_workspace-1.0.0/PKG-INFO` & `pdm_polylith_workspace-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pdm-polylith-workspace
-Version: 1.0.0
+Version: 1.0.1
 Summary: a PDM build hook for a Polylith workspace
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
 
 # PDM Build Hook for a Polylith workspace
 
 A plugin for [PDM](https://pdm-project.org) and the Polylith Architecture.
```

