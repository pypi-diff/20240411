# Comparing `tmp/pyprtg-api-0.0.8.tar.gz` & `tmp/pyprtg-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprtg-api-0.0.8.tar", last modified: Mon Aug 22 21:06:23 2022, max compression
+gzip compressed data, was "pyprtg-api-0.0.9.tar", last modified: Sat Nov 12 04:57:26 2022, max compression
```

## Comparing `pyprtg-api-0.0.8.tar` & `pyprtg-api-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 cabox     (1000) cabox     (1000)        0 2022-08-22 21:06:23.346031 pyprtg-api-0.0.8/
--rw-r--r--   0 cabox     (1000) cabox     (1000)     1088 2022-08-01 21:40:33.000000 pyprtg-api-0.0.8/LICENSE
--rw-r--r--   0 cabox     (1000) cabox     (1000)     2567 2022-08-22 21:06:23.346031 pyprtg-api-0.0.8/PKG-INFO
--rw-r--r--   0 cabox     (1000) cabox     (1000)     2336 2022-08-01 22:06:35.000000 pyprtg-api-0.0.8/README.md
-drwxr-xr-x   0 cabox     (1000) cabox     (1000)        0 2022-08-22 21:06:23.342031 pyprtg-api-0.0.8/prtg/
--rw-r--r--   0 cabox     (1000) cabox     (1000)    20101 2022-08-22 21:03:55.000000 pyprtg-api-0.0.8/prtg/__init__.py
--rw-r--r--   0 cabox     (1000) cabox     (1000)      360 2022-08-01 19:29:37.000000 pyprtg-api-0.0.8/prtg/exception.py
--rw-r--r--   0 cabox     (1000) cabox     (1000)     3054 2022-08-01 04:39:22.000000 pyprtg-api-0.0.8/prtg/icon.py
--rw-r--r--   0 cabox     (1000) cabox     (1000)      254 2022-08-22 20:50:47.000000 pyprtg-api-0.0.8/pyproject.toml
-drwxr-xr-x   0 cabox     (1000) cabox     (1000)        0 2022-08-22 21:06:23.345031 pyprtg-api-0.0.8/pyprtg_api.egg-info/
--rw-r--r--   0 cabox     (1000) cabox     (1000)     2567 2022-08-22 21:06:23.000000 pyprtg-api-0.0.8/pyprtg_api.egg-info/PKG-INFO
--rw-r--r--   0 cabox     (1000) cabox     (1000)      249 2022-08-22 21:06:23.000000 pyprtg-api-0.0.8/pyprtg_api.egg-info/SOURCES.txt
--rw-r--r--   0 cabox     (1000) cabox     (1000)        1 2022-08-22 21:06:23.000000 pyprtg-api-0.0.8/pyprtg_api.egg-info/dependency_links.txt
--rw-r--r--   0 cabox     (1000) cabox     (1000)        9 2022-08-22 21:06:23.000000 pyprtg-api-0.0.8/pyprtg_api.egg-info/requires.txt
--rw-r--r--   0 cabox     (1000) cabox     (1000)        5 2022-08-22 21:06:23.000000 pyprtg-api-0.0.8/pyprtg_api.egg-info/top_level.txt
--rw-r--r--   0 cabox     (1000) cabox     (1000)       38 2022-08-22 21:06:23.346031 pyprtg-api-0.0.8/setup.cfg
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-11-12 04:57:26.724249 pyprtg-api-0.0.9/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1088 2022-11-12 04:10:25.000000 pyprtg-api-0.0.9/LICENSE
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2615 2022-11-12 04:57:26.720248 pyprtg-api-0.0.9/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2336 2022-11-12 04:10:25.000000 pyprtg-api-0.0.9/README.md
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-11-12 04:57:26.720248 pyprtg-api-0.0.9/prtg/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       24 2022-11-12 04:10:25.000000 pyprtg-api-0.0.9/prtg/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    20186 2022-11-12 04:48:18.000000 pyprtg-api-0.0.9/prtg/api.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      360 2022-11-12 04:10:25.000000 pyprtg-api-0.0.9/prtg/exception.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3054 2022-11-12 04:10:25.000000 pyprtg-api-0.0.9/prtg/icon.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      395 2022-11-12 04:56:42.000000 pyprtg-api-0.0.9/pyproject.toml
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2022-11-12 04:57:26.720248 pyprtg-api-0.0.9/pyprtg_api.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2615 2022-11-12 04:57:26.000000 pyprtg-api-0.0.9/pyprtg_api.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      261 2022-11-12 04:57:26.000000 pyprtg-api-0.0.9/pyprtg_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2022-11-12 04:57:26.000000 pyprtg-api-0.0.9/pyprtg_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        9 2022-11-12 04:57:26.000000 pyprtg-api-0.0.9/pyprtg_api.egg-info/requires.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        5 2022-11-12 04:57:26.000000 pyprtg-api-0.0.9/pyprtg_api.egg-info/top_level.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       38 2022-11-12 04:57:26.724249 pyprtg-api-0.0.9/setup.cfg
```

### Comparing `pyprtg-api-0.0.8/LICENSE` & `pyprtg-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprtg-api-0.0.8/PKG-INFO` & `pyprtg-api-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pyprtg-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: API to communicate with PRTG instance.
 Author-email: Jonny Le <jonny.le@computacenter.com>
 License: MIT
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PRTG API
 
 Module to make it easier to communicate with PRTG instances. This module leverages PRTG's existing API and wraps it into an easy to understand Python class, PrtgApi.
```

### Comparing `pyprtg-api-0.0.8/README.md` & `pyprtg-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyprtg-api-0.0.8/prtg/__init__.py` & `pyprtg-api-0.0.9/prtg/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 import urllib.parse
 import xml.etree.ElementTree as ET
 
 import requests
 
-from prtg.icon import Icon
 from prtg.exception import DuplicateObject, ObjectNotFound, Unauthorized
 
 class PrtgApi:
     """Class to communicate with PRTG instance using PRTG API.
     Validates credentials on __init__.
 
     Attributes:
@@ -28,21 +27,23 @@
 
     def __init__(self, 
             url, 
             username, 
             password, 
             template_group = None, 
             template_device = None, 
-            is_passhash = False):
+            is_passhash = False,
+            requests_verify = True):
         self.url = url
         self.username = username
         self.password = password
         self.template_group = template_group
         self.template_device = template_device
         self.is_passhash = is_passhash
+        self.requests_verify = requests_verify
         self._validate_cred()
     
     def _requests_get(self, endpoint, params=None):
         """Wraps function `requests.get` to add credentials
         to parameter and capture specific response error codes.
 
         Args:
@@ -58,15 +59,15 @@
             requests.Resposne: response of GET API
         """
         url = self.url + endpoint
         key = 'passhash' if self.is_passhash else 'password'
         auth = {'username': self.username, key: self.password}
         if params:
             auth.update(params)
-        response = requests.get(url, auth)
+        response = requests.get(url, auth, verify=self.requests_verify)
         try:
             response.raise_for_status()
         except requests.HTTPError as e:
             if response.status_code == 400:
                 root = ET.fromstring(response.text)
                 error_msg = root.find('error').text
                 raise requests.HTTPError(error_msg)
```

### Comparing `pyprtg-api-0.0.8/prtg/icon.py` & `pyprtg-api-0.0.9/prtg/icon.py`

 * *Files identical despite different names*

### Comparing `pyprtg-api-0.0.8/pyprtg_api.egg-info/PKG-INFO` & `pyprtg-api-0.0.9/pyprtg_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: pyprtg-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: API to communicate with PRTG instance.
 Author-email: Jonny Le <jonny.le@computacenter.com>
 License: MIT
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PRTG API
 
 Module to make it easier to communicate with PRTG instances. This module leverages PRTG's existing API and wraps it into an easy to understand Python class, PrtgApi.
```

