# Comparing `tmp/telemetrx-0.1.0.tar.gz` & `tmp/telemetrx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telemetrx-0.1.0.tar", last modified: Thu Apr 11 13:09:13 2024, max compression
+gzip compressed data, was "telemetrx-0.1.1.tar", last modified: Thu Apr 11 13:39:20 2024, max compression
```

## Comparing `telemetrx-0.1.0.tar` & `telemetrx-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-11 13:09:13.396771 telemetrx-0.1.0/
--rw-r--r--   0 anpapath   (501) staff       (20)     1617 2024-04-11 11:37:58.000000 telemetrx-0.1.0/LICENSE
--rw-r--r--   0 anpapath   (501) staff       (20)     2283 2024-04-11 13:09:13.396317 telemetrx-0.1.0/PKG-INFO
--rw-r--r--   0 anpapath   (501) staff       (20)     1792 2024-04-11 13:08:40.000000 telemetrx-0.1.0/README.md
--rw-r--r--   0 anpapath   (501) staff       (20)       38 2024-04-11 13:09:13.396890 telemetrx-0.1.0/setup.cfg
--rw-r--r--   0 anpapath   (501) staff       (20)      708 2024-04-11 11:45:48.000000 telemetrx-0.1.0/setup.py
-drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-11 13:09:13.393655 telemetrx-0.1.0/telemetrx/
--rw-r--r--   0 anpapath   (501) staff       (20)     4094 2024-04-11 11:31:34.000000 telemetrx-0.1.0/telemetrx/TelemetrX.py
--rw-r--r--   0 anpapath   (501) staff       (20)       37 2024-04-11 12:55:25.000000 telemetrx-0.1.0/telemetrx/__init__.py
-drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-11 13:09:13.395726 telemetrx-0.1.0/telemetrx.egg-info/
--rw-r--r--   0 anpapath   (501) staff       (20)     2283 2024-04-11 13:09:13.000000 telemetrx-0.1.0/telemetrx.egg-info/PKG-INFO
--rw-r--r--   0 anpapath   (501) staff       (20)      235 2024-04-11 13:09:13.000000 telemetrx-0.1.0/telemetrx.egg-info/SOURCES.txt
--rw-r--r--   0 anpapath   (501) staff       (20)        1 2024-04-11 13:09:13.000000 telemetrx-0.1.0/telemetrx.egg-info/dependency_links.txt
--rw-r--r--   0 anpapath   (501) staff       (20)       22 2024-04-11 13:09:13.000000 telemetrx-0.1.0/telemetrx.egg-info/requires.txt
--rw-r--r--   0 anpapath   (501) staff       (20)       10 2024-04-11 13:09:13.000000 telemetrx-0.1.0/telemetrx.egg-info/top_level.txt
+drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-11 13:39:20.127270 telemetrx-0.1.1/
+-rw-r--r--   0 anpapath   (501) staff       (20)     1617 2024-04-11 11:37:58.000000 telemetrx-0.1.1/LICENSE
+-rw-r--r--   0 anpapath   (501) staff       (20)     2204 2024-04-11 13:39:20.126793 telemetrx-0.1.1/PKG-INFO
+-rw-r--r--   0 anpapath   (501) staff       (20)     1792 2024-04-11 13:36:19.000000 telemetrx-0.1.1/README.md
+-rw-r--r--   0 anpapath   (501) staff       (20)      456 2024-04-11 13:38:58.000000 telemetrx-0.1.1/pyproject.toml
+-rw-r--r--   0 anpapath   (501) staff       (20)       38 2024-04-11 13:39:20.127396 telemetrx-0.1.1/setup.cfg
+drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-11 13:39:20.123386 telemetrx-0.1.1/telemetrx/
+-rw-r--r--   0 anpapath   (501) staff       (20)     4094 2024-04-11 11:31:34.000000 telemetrx-0.1.1/telemetrx/TelemetrX.py
+-rw-r--r--   0 anpapath   (501) staff       (20)       37 2024-04-11 12:55:25.000000 telemetrx-0.1.1/telemetrx/__init__.py
+drwxr-xr-x   0 anpapath   (501) staff       (20)        0 2024-04-11 13:39:20.126197 telemetrx-0.1.1/telemetrx.egg-info/
+-rw-r--r--   0 anpapath   (501) staff       (20)     2204 2024-04-11 13:39:20.000000 telemetrx-0.1.1/telemetrx.egg-info/PKG-INFO
+-rw-r--r--   0 anpapath   (501) staff       (20)      241 2024-04-11 13:39:20.000000 telemetrx-0.1.1/telemetrx.egg-info/SOURCES.txt
+-rw-r--r--   0 anpapath   (501) staff       (20)        1 2024-04-11 13:39:20.000000 telemetrx-0.1.1/telemetrx.egg-info/dependency_links.txt
+-rw-r--r--   0 anpapath   (501) staff       (20)       22 2024-04-11 13:39:20.000000 telemetrx-0.1.1/telemetrx.egg-info/requires.txt
+-rw-r--r--   0 anpapath   (501) staff       (20)       10 2024-04-11 13:39:20.000000 telemetrx-0.1.1/telemetrx.egg-info/top_level.txt
```

### Comparing `telemetrx-0.1.0/LICENSE` & `telemetrx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telemetrx-0.1.0/PKG-INFO` & `telemetrx-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: telemetrx
-Version: 0.1.0
-Summary: A package to send telemetry data asynchronously to TelemetrX platform
-Author: Vivek Singh
-Author-email: vivekksi@cisco.com
-License: Proprietary
+Version: 0.1.1
+Summary: a package for sending app telemetry data to the TelemetrX backend.
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: Other/Proprietary License
-Requires-Python: >=3.7
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: python-dotenv
 
-# telemetrx-0.1.0
+# telemetrx-0.1.1
 
 telemetrx is a Python library which facilitates the sending of App telemetry data to the TelemetrX platform, leveraging the TelemetrX API. 
 
 ## Features
 
 The library features the function send_telemetrx() which helps app owners to send telemetry data to the TelemetrX platform with a single line of code.
```

### Comparing `telemetrx-0.1.0/README.md` & `telemetrx-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# telemetrx-0.1.0
+# telemetrx-0.1.1
 
 telemetrx is a Python library which facilitates the sending of App telemetry data to the TelemetrX platform, leveraging the TelemetrX API. 
 
 ## Features
 
 The library features the function send_telemetrx() which helps app owners to send telemetry data to the TelemetrX platform with a single line of code.
```

### Comparing `telemetrx-0.1.0/telemetrx/TelemetrX.py` & `telemetrx-0.1.1/telemetrx/TelemetrX.py`

 * *Files identical despite different names*

### Comparing `telemetrx-0.1.0/telemetrx.egg-info/PKG-INFO` & `telemetrx-0.1.1/telemetrx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: telemetrx
-Version: 0.1.0
-Summary: A package to send telemetry data asynchronously to TelemetrX platform
-Author: Vivek Singh
-Author-email: vivekksi@cisco.com
-License: Proprietary
+Version: 0.1.1
+Summary: a package for sending app telemetry data to the TelemetrX backend.
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: Other/Proprietary License
-Requires-Python: >=3.7
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: python-dotenv
 
-# telemetrx-0.1.0
+# telemetrx-0.1.1
 
 telemetrx is a Python library which facilitates the sending of App telemetry data to the TelemetrX platform, leveraging the TelemetrX API. 
 
 ## Features
 
 The library features the function send_telemetrx() which helps app owners to send telemetry data to the TelemetrX platform with a single line of code.
```

