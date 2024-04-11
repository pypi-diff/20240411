# Comparing `tmp/polytrend-1.0.5.tar.gz` & `tmp/polytrend-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytrend-1.0.5.tar", last modified: Thu Apr 11 20:54:36 2024, max compression
+gzip compressed data, was "polytrend-1.0.6.tar", last modified: Thu Apr 11 21:13:48 2024, max compression
```

## Comparing `polytrend-1.0.5.tar` & `polytrend-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:54:36.025923 polytrend-1.0.5/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.5/LICENSE
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 20:54:36.025923 polytrend-1.0.5/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.5/README.md
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      800 2024-04-11 20:54:26.000000 polytrend-1.0.5/pyproject.toml
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 20:54:36.025923 polytrend-1.0.5/setup.cfg
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      426 2024-04-11 20:54:28.000000 polytrend-1.0.5/setup.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:54:36.015923 polytrend-1.0.5/src/
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:54:36.015923 polytrend-1.0.5/src/polytrend/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      694 2024-04-11 20:21:39.000000 polytrend-1.0.5/src/polytrend/__init__.py
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    10445 2024-04-11 20:20:38.000000 polytrend-1.0.5/src/polytrend/polytrend.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 20:54:36.015923 polytrend-1.0.5/src/polytrend.egg-info/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 20:54:35.000000 polytrend-1.0.5/src/polytrend.egg-info/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      242 2024-04-11 20:54:36.000000 polytrend-1.0.5/src/polytrend.egg-info/SOURCES.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 20:54:35.000000 polytrend-1.0.5/src/polytrend.egg-info/dependency_links.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-11 20:54:35.000000 polytrend-1.0.5/src/polytrend.egg-info/top_level.txt
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 21:13:48.035953 polytrend-1.0.6/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.6/LICENSE
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-11 21:13:48.035953 polytrend-1.0.6/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.6/README.md
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      963 2024-04-11 21:12:19.000000 polytrend-1.0.6/pyproject.toml
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 21:13:48.035953 polytrend-1.0.6/setup.cfg
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 21:08:44.000000 polytrend-1.0.6/setup.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 21:13:48.025953 polytrend-1.0.6/src/
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 21:13:48.025953 polytrend-1.0.6/src/polytrend/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      694 2024-04-11 20:21:39.000000 polytrend-1.0.6/src/polytrend/__init__.py
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    10445 2024-04-11 20:20:38.000000 polytrend-1.0.6/src/polytrend/polytrend.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 21:13:48.035953 polytrend-1.0.6/src/polytrend.egg-info/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3458 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      278 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/SOURCES.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/dependency_links.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      141 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/requires.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-11 21:13:48.000000 polytrend-1.0.6/src/polytrend.egg-info/top_level.txt
```

### Comparing `polytrend-1.0.5/LICENSE` & `polytrend-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.5/PKG-INFO` & `polytrend-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.5
+Version: 1.0.6
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cx_Freeze~=6.15.16
+Requires-Dist: matplotlib~=3.8.3
+Requires-Dist: numpy~=1.26.4
+Requires-Dist: pandas~=2.2.1
+Requires-Dist: PyQt6~=6.6.1
+Requires-Dist: PyQt6_sip~=13.6.0
+Requires-Dist: scikit-learn~=1.4.1.post1
+Requires-Dist: setuptools~=65.5.0
 
 # PolyTrend
 
 PolyTrend is a Python package aimed at facilitating polynomial trend fitting, visualization, and extrapolation. It offers a comprehensive set of functionalities to analyze and interpret data using polynomial regression techniques. Below, we provide an overview of the package along with additional formatting and explanations relevant for PyPI.
 
 ## Introduction
```

### Comparing `polytrend-1.0.5/README.md` & `polytrend-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.5/pyproject.toml` & `polytrend-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polytrend"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Emmanuel Asiimwe", email="asiimwemmanuel47@gmail.com" },
 ]
 description = "PolyTrend is a regression tool that fits polynomial curves to noisy data."
 readme = "README.md"
 requires-python = ">= 3.11.8"
-# dependencies = [
-#   "matplotlib==3.8.3",
-#   "numpy==1.21.5",
-#   "pandas==2.2.2",
-#   "scikit_learn==1.4.1.post1",
-# ]
+dependencies = [
+  "cx_Freeze~=6.15.16",
+  "matplotlib~=3.8.3",
+  "numpy~=1.26.4",
+  "pandas~=2.2.1",
+  "PyQt6~=6.6.1",
+  "PyQt6_sip~=13.6.0",
+  "scikit-learn~=1.4.1.post1",
+  "setuptools~=65.5.0",
+]
+# # TODO remove the version attribute of project if activated
+# dynamic = ["version"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `polytrend-1.0.5/src/polytrend/__init__.py` & `polytrend-1.0.6/src/polytrend/__init__.py`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.5/src/polytrend/polytrend.py` & `polytrend-1.0.6/src/polytrend/polytrend.py`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.5/src/polytrend.egg-info/PKG-INFO` & `polytrend-1.0.6/src/polytrend.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.5
+Version: 1.0.6
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cx_Freeze~=6.15.16
+Requires-Dist: matplotlib~=3.8.3
+Requires-Dist: numpy~=1.26.4
+Requires-Dist: pandas~=2.2.1
+Requires-Dist: PyQt6~=6.6.1
+Requires-Dist: PyQt6_sip~=13.6.0
+Requires-Dist: scikit-learn~=1.4.1.post1
+Requires-Dist: setuptools~=65.5.0
 
 # PolyTrend
 
 PolyTrend is a Python package aimed at facilitating polynomial trend fitting, visualization, and extrapolation. It offers a comprehensive set of functionalities to analyze and interpret data using polynomial regression techniques. Below, we provide an overview of the package along with additional formatting and explanations relevant for PyPI.
 
 ## Introduction
```

