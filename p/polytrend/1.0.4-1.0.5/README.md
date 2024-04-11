# Comparing `tmp/polytrend-1.0.4.tar.gz` & `tmp/polytrend-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytrend-1.0.4.tar", last modified: Thu Apr 11 20:40:30 2024, max compression
+gzip compressed data, was "polytrend-1.0.5.tar", last modified: Thu Apr 11 20:54:36 2024, max compression
```

## Comparing `polytrend-1.0.4.tar` & `polytrend-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:40:30.365902 polytrend-1.0.4/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.4/LICENSE
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 20:40:30.365902 polytrend-1.0.4/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.4/README.md
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      800 2024-04-11 20:40:17.000000 polytrend-1.0.4/pyproject.toml
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 20:40:30.365902 polytrend-1.0.4/setup.cfg
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      426 2024-04-11 20:40:18.000000 polytrend-1.0.4/setup.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:40:30.365902 polytrend-1.0.4/src/
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:40:30.365902 polytrend-1.0.4/src/polytrend/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      694 2024-04-11 20:21:39.000000 polytrend-1.0.4/src/polytrend/__init__.py
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    10445 2024-04-11 20:20:38.000000 polytrend-1.0.4/src/polytrend/polytrend.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:40:30.365902 polytrend-1.0.4/src/polytrend.egg-info/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 20:40:30.000000 polytrend-1.0.4/src/polytrend.egg-info/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      242 2024-04-11 20:40:30.000000 polytrend-1.0.4/src/polytrend.egg-info/SOURCES.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 20:40:30.000000 polytrend-1.0.4/src/polytrend.egg-info/dependency_links.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-11 20:40:30.000000 polytrend-1.0.4/src/polytrend.egg-info/top_level.txt
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:54:36.025923 polytrend-1.0.5/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.5/LICENSE
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 20:54:36.025923 polytrend-1.0.5/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.5/README.md
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      800 2024-04-11 20:54:26.000000 polytrend-1.0.5/pyproject.toml
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 20:54:36.025923 polytrend-1.0.5/setup.cfg
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      426 2024-04-11 20:54:28.000000 polytrend-1.0.5/setup.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:54:36.015923 polytrend-1.0.5/src/
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:54:36.015923 polytrend-1.0.5/src/polytrend/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      694 2024-04-11 20:21:39.000000 polytrend-1.0.5/src/polytrend/__init__.py
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    10445 2024-04-11 20:20:38.000000 polytrend-1.0.5/src/polytrend/polytrend.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:54:36.015923 polytrend-1.0.5/src/polytrend.egg-info/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 20:54:35.000000 polytrend-1.0.5/src/polytrend.egg-info/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      242 2024-04-11 20:54:36.000000 polytrend-1.0.5/src/polytrend.egg-info/SOURCES.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 20:54:35.000000 polytrend-1.0.5/src/polytrend.egg-info/dependency_links.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-11 20:54:35.000000 polytrend-1.0.5/src/polytrend.egg-info/top_level.txt
```

### Comparing `polytrend-1.0.4/LICENSE` & `polytrend-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.4/PKG-INFO` & `polytrend-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.4
+Version: 1.0.5
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `polytrend-1.0.4/README.md` & `polytrend-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.4/pyproject.toml` & `polytrend-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polytrend"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Emmanuel Asiimwe", email="asiimwemmanuel47@gmail.com" },
 ]
 description = "PolyTrend is a regression tool that fits polynomial curves to noisy data."
 readme = "README.md"
 requires-python = ">= 3.11.8"
 # dependencies = [
```

### Comparing `polytrend-1.0.4/src/polytrend/__init__.py` & `polytrend-1.0.5/src/polytrend/__init__.py`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.4/src/polytrend/polytrend.py` & `polytrend-1.0.5/src/polytrend/polytrend.py`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.4/src/polytrend.egg-info/PKG-INFO` & `polytrend-1.0.5/src/polytrend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.4
+Version: 1.0.5
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

