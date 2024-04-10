# Comparing `tmp/galileo_protect-0.3.0.tar.gz` & `tmp/galileo_protect-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_protect-0.3.0.tar", max compression
+gzip compressed data, was "galileo_protect-0.4.0.tar", max compression
```

## Comparing `galileo_protect-0.3.0.tar` & `galileo_protect-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    10946 2024-04-09 00:25:55.591543 galileo_protect-0.3.0/LICENSE
--rw-r--r--   0        0        0      118 2024-04-09 00:25:55.591543 galileo_protect-0.3.0/README.md
--rw-r--r--   0        0        0     2529 2024-04-09 00:25:57.499530 galileo_protect-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      395 2024-04-09 00:25:57.499530 galileo_protect-0.3.0/src/galileo_protect/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/constants/__init__.py
--rw-r--r--   0        0        0      269 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/helpers/__init__.py
--rw-r--r--   0        0        0      530 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/helpers/config.py
--rw-r--r--   0        0        0     1402 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/invoke.py
--rw-r--r--   0        0        0      638 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/project.py
--rw-r--r--   0        0        0      665 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/schemas/__init__.py
--rw-r--r--   0        0        0      212 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/schemas/invoke.py
--rw-r--r--   0        0        0      266 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/schemas/rule.py
--rw-r--r--   0        0        0      124 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/schemas/stage.py
--rw-r--r--   0        0        0     1324 2024-04-09 00:25:55.595543 galileo_protect-0.3.0/src/galileo_protect/stage.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/LICENSE
+-rw-r--r--   0        0        0      118 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/README.md
+-rw-r--r--   0        0        0     2529 2024-04-10 20:34:19.719202 galileo_protect-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      422 2024-04-10 20:34:19.723202 galileo_protect-0.4.0/src/galileo_protect/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/constants/__init__.py
+-rw-r--r--   0        0        0      324 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/helpers/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/helpers/config.py
+-rw-r--r--   0        0        0     1402 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/invoke.py
+-rw-r--r--   0        0        0      638 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/project.py
+-rw-r--r--   0        0        0      665 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/schemas/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/schemas/invoke.py
+-rw-r--r--   0        0        0      266 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/schemas/rule.py
+-rw-r--r--   0        0        0      124 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/schemas/stage.py
+-rw-r--r--   0        0        0     3503 2024-04-10 20:34:18.859196 galileo_protect-0.4.0/src/galileo_protect/stage.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 galileo_protect-0.4.0/PKG-INFO
```

### Comparing `galileo_protect-0.3.0/LICENSE` & `galileo_protect-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.3.0/pyproject.toml` & `galileo_protect-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "galileo-protect"
-version = "0.3.0"
+version = "0.4.0"
 description = "🛡️ Secure your Generative AI applications with Galileo Protect!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_protect", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
-galileo-core = "^0.10.0"
+galileo-core = "^0.11.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.3.4"
 pytest-cov = "^5.0.0"
 pytest-xdist = "^3.5.0"
```

### Comparing `galileo_protect-0.3.0/src/galileo_protect/helpers/config.py` & `galileo_protect-0.4.0/src/galileo_protect/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.3.0/src/galileo_protect/invoke.py` & `galileo_protect-0.4.0/src/galileo_protect/invoke.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.3.0/src/galileo_protect/project.py` & `galileo_protect-0.4.0/src/galileo_protect/project.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.3.0/src/galileo_protect/schemas/__init__.py` & `galileo_protect-0.4.0/src/galileo_protect/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `galileo_protect-0.3.0/PKG-INFO` & `galileo_protect-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: galileo-protect
-Version: 0.3.0
+Version: 0.4.0
 Summary: 🛡️ Secure your Generative AI applications with Galileo Protect!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: galileo-core (>=0.10.0,<0.11.0)
+Requires-Dist: galileo-core (>=0.11.0,<0.12.0)
 Description-Content-Type: text/markdown
 
 # galileo-protect
 
 🛡️ Secure your Generative AI applications with [Galileo Protect](https://www.rungalileo.io/).
```

