# Comparing `tmp/guetwifi-0.1.6.tar.gz` & `tmp/guetwifi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guetwifi-0.1.6.tar", max compression
+gzip compressed data, was "guetwifi-0.1.7.tar", max compression
```

## Comparing `guetwifi-0.1.6.tar` & `guetwifi-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1023 2024-03-20 12:10:24.941893 guetwifi-0.1.6/README.md
--rw-r--r--   0        0        0     3872 2024-03-20 13:01:15.981224 guetwifi-0.1.6/guetwifi/cli.py
--rw-r--r--   0        0        0     4694 2024-03-20 12:55:46.341295 guetwifi-0.1.6/guetwifi/guetwifirunner.py
--rw-r--r--   0        0        0      907 2024-03-20 13:07:38.841139 guetwifi-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 guetwifi-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1023 2024-04-11 09:26:19.098335 guetwifi-0.1.7/README.md
+-rw-r--r--   0        0        0     1148 2024-04-11 10:17:16.861187 guetwifi-0.1.7/guetwifi/cli.py
+-rw-r--r--   0        0        0     2195 2024-04-11 10:17:04.241547 guetwifi-0.1.7/guetwifi/guetwifirunner.py
+-rw-r--r--   0        0        0      907 2024-04-11 10:27:29.875403 guetwifi-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 guetwifi-0.1.7/PKG-INFO
```

### Comparing `guetwifi-0.1.6/README.md` & `guetwifi-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `guetwifi-0.1.6/pyproject.toml` & `guetwifi-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "guetwifi"
-version = "0.1.6"
+version = "0.1.7"
 description = "GUET WiFi Monitor"
 authors = ["PuQing <me@puqing.work>"]
 license = "MIT"
 homepage = "https://github.com/andPuQing/guetwifi"
 repository = "https://github.com/andPuQing/guetwifi.git"
 classifiers = [
     "Environment :: Console",
```

### Comparing `guetwifi-0.1.6/PKG-INFO` & `guetwifi-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guetwifi
-Version: 0.1.6
+Version: 0.1.7
 Summary: GUET WiFi Monitor
 Home-page: https://github.com/andPuQing/guetwifi
 License: MIT
 Author: PuQing
 Author-email: me@puqing.work
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
```

