# Comparing `tmp/polytrend-1.0.0.tar.gz` & `tmp/polytrend-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytrend-1.0.0.tar", last modified: Thu Apr 11 19:09:09 2024, max compression
+gzip compressed data, was "polytrend-1.0.1.tar", last modified: Thu Apr 11 19:42:15 2024, max compression
```

## Comparing `polytrend-1.0.0.tar` & `polytrend-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,12 @@
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:09:09.295775 polytrend-1.0.0/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.0/LICENSE
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3329 2024-04-11 19:09:09.295775 polytrend-1.0.0/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.0/README.md
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      788 2024-04-11 19:08:59.000000 polytrend-1.0.0/pyproject.toml
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 19:09:09.295775 polytrend-1.0.0/setup.cfg
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:09:09.295775 polytrend-1.0.0/src/
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:09:09.295775 polytrend-1.0.0/src/polytrend/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       33 2024-04-11 19:01:45.000000 polytrend-1.0.0/src/polytrend/__init__.py
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     8728 2024-04-11 19:01:45.000000 polytrend-1.0.0/src/polytrend/polytrend.py
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:09:09.295775 polytrend-1.0.0/src/polytrend.egg-info/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3329 2024-04-11 19:09:09.000000 polytrend-1.0.0/src/polytrend.egg-info/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      269 2024-04-11 19:09:09.000000 polytrend-1.0.0/src/polytrend.egg-info/SOURCES.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 19:09:09.000000 polytrend-1.0.0/src/polytrend.egg-info/dependency_links.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       72 2024-04-11 19:09:09.000000 polytrend-1.0.0/src/polytrend.egg-info/requires.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       10 2024-04-11 19:09:09.000000 polytrend-1.0.0/src/polytrend.egg-info/top_level.txt
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:42:15.475819 polytrend-1.0.1/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.1/LICENSE
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 19:42:15.475819 polytrend-1.0.1/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.1/README.md
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:42:15.475819 polytrend-1.0.1/polytrend.egg-info/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 19:42:15.000000 polytrend-1.0.1/polytrend.egg-info/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      173 2024-04-11 19:42:15.000000 polytrend-1.0.1/polytrend.egg-info/SOURCES.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 19:42:15.000000 polytrend-1.0.1/polytrend.egg-info/dependency_links.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 19:42:15.000000 polytrend-1.0.1/polytrend.egg-info/top_level.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      800 2024-04-11 19:36:12.000000 polytrend-1.0.1/pyproject.toml
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 19:42:15.475819 polytrend-1.0.1/setup.cfg
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      273 2024-04-11 19:37:41.000000 polytrend-1.0.1/setup.py
```

### Comparing `polytrend-1.0.0/LICENSE` & `polytrend-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.0/PKG-INFO` & `polytrend-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.0
+Version: 1.0.1
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
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: numpy==1.21.5
-Requires-Dist: pandas==2.2.2
-Requires-Dist: scikit_learn==1.4.1.post1
 
 # PolyTrend
 
 PolyTrend is a Python package aimed at facilitating polynomial trend fitting, visualization, and extrapolation. It offers a comprehensive set of functionalities to analyze and interpret data using polynomial regression techniques. Below, we provide an overview of the package along with additional formatting and explanations relevant for PyPI.
 
 ## Introduction
```

### Comparing `polytrend-1.0.0/README.md` & `polytrend-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.0/pyproject.toml` & `polytrend-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "polytrend"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Emmanuel Asiimwe", email="asiimwemmanuel47@gmail.com" },
 ]
 description = "PolyTrend is a regression tool that fits polynomial curves to noisy data."
 readme = "README.md"
 requires-python = ">= 3.11.8"
-dependencies = [
-  "matplotlib==3.8.3",
-  "numpy==1.21.5",
-  "pandas==2.2.2",
-  "scikit_learn==1.4.1.post1",
-]
+# dependencies = [
+#   "matplotlib==3.8.3",
+#   "numpy==1.21.5",
+#   "pandas==2.2.2",
+#   "scikit_learn==1.4.1.post1",
+# ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `polytrend-1.0.0/src/polytrend.egg-info/PKG-INFO` & `polytrend-1.0.1/polytrend.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.0
+Version: 1.0.1
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
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: numpy==1.21.5
-Requires-Dist: pandas==2.2.2
-Requires-Dist: scikit_learn==1.4.1.post1
 
 # PolyTrend
 
 PolyTrend is a Python package aimed at facilitating polynomial trend fitting, visualization, and extrapolation. It offers a comprehensive set of functionalities to analyze and interpret data using polynomial regression techniques. Below, we provide an overview of the package along with additional formatting and explanations relevant for PyPI.
 
 ## Introduction
```

