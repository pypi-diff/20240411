# Comparing `tmp/better_rtplot-0.1.5.tar.gz` & `tmp/better_rtplot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_rtplot-0.1.5.tar", max compression
+gzip compressed data, was "better_rtplot-0.1.6.tar", max compression
```

## Comparing `better_rtplot-0.1.5.tar` & `better_rtplot-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-11 01:15:37.992109 better_rtplot-0.1.5/LICENSE
--rwxr-xr-x   0        0        0    12535 2023-08-17 22:19:46.960932 better_rtplot-0.1.5/README.md
--rwxr-xr-x   0        0        0      646 2024-04-11 01:24:27.850580 better_rtplot-0.1.5/pyproject.toml
--rwxr-xr-x   0        0        0     9251 2024-04-11 01:16:00.456553 better_rtplot-0.1.5/rtplot/client.py
--rwxr-xr-x   0        0        0     6252 2023-08-17 22:15:47.496837 better_rtplot-0.1.5/rtplot/example_code.py
--rwxr-xr-x   0        0        0     1564 2023-08-16 23:13:59.843588 better_rtplot-0.1.5/rtplot/plot_log.py
--rw-r--r--   0        0        0       71 2024-04-11 01:15:37.992109 better_rtplot-0.1.5/rtplot/saved_plots/.gitignore
--rwxr-xr-x   0        0        0    26529 2023-08-17 22:17:18.462393 better_rtplot-0.1.5/rtplot/server.py
--rw-r--r--   0        0        0    13287 1970-01-01 00:00:00.000000 better_rtplot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-11 01:15:37.992109 better_rtplot-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0    12535 2023-08-17 22:19:46.960932 better_rtplot-0.1.6/README.md
+-rwxr-xr-x   0        0        0      647 2024-04-11 01:39:42.916614 better_rtplot-0.1.6/pyproject.toml
+-rwxr-xr-x   0        0        0     9251 2024-04-11 01:16:00.456553 better_rtplot-0.1.6/rtplot/client.py
+-rwxr-xr-x   0        0        0     6252 2023-08-17 22:15:47.496837 better_rtplot-0.1.6/rtplot/example_code.py
+-rwxr-xr-x   0        0        0     1564 2023-08-16 23:13:59.843588 better_rtplot-0.1.6/rtplot/plot_log.py
+-rw-r--r--   0        0        0       71 2024-04-11 01:15:37.992109 better_rtplot-0.1.6/rtplot/saved_plots/.gitignore
+-rwxr-xr-x   0        0        0    26529 2023-08-17 22:17:18.462393 better_rtplot-0.1.6/rtplot/server.py
+-rw-r--r--   0        0        0    13288 1970-01-01 00:00:00.000000 better_rtplot-0.1.6/PKG-INFO
```

### Comparing `better_rtplot-0.1.5/LICENSE` & `better_rtplot-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.5/README.md` & `better_rtplot-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.5/pyproject.toml` & `better_rtplot-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "better-rtplot"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["jmontp <jmontp@umich.edu>"]
 license = "GPL V3.0"
 readme = "README.md"
 packages = [{include = "rtplot"}]
 
 [tool.poetry.dependencies]
-python = ">= 3.9, < 3.12"
+python = ">= 3.9, <= 3.12"
 numpy = ">= 1.23.5"
 pyzmq = ">= 25.0.0"
 
 pandas = {version = ">= 1.5.3", optional = true}
 pyarrow = {version=">= 11.0.0", optional = true}
 pyqtgraph = {version = ">= 0.13.0", optional = true}
 pyside6 = {version = "> 6.4.0", optional = true}
```

### Comparing `better_rtplot-0.1.5/rtplot/client.py` & `better_rtplot-0.1.6/rtplot/client.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.5/rtplot/example_code.py` & `better_rtplot-0.1.6/rtplot/example_code.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.5/rtplot/plot_log.py` & `better_rtplot-0.1.6/rtplot/plot_log.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.5/rtplot/server.py` & `better_rtplot-0.1.6/rtplot/server.py`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.5/PKG-INFO` & `better_rtplot-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: better-rtplot
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: GPL V3.0
 Author: jmontp
 Author-email: jmontp@umich.edu
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<=3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: server
 Requires-Dist: numpy (>=1.23.5)
```

