# Comparing `tmp/prosperity2submit-0.2.3.tar.gz` & `tmp/prosperity2submit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2submit-0.2.3.tar", last modified: Tue Apr  9 15:27:11 2024, max compression
+gzip compressed data, was "prosperity2submit-0.2.4.tar", last modified: Thu Apr 11 09:12:45 2024, max compression
```

## Comparing `prosperity2submit-0.2.3.tar` & `prosperity2submit-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/prosperity2submit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/prosperity2submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/prosperity2submit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/prosperity2submit/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/prosperity2submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 15:27:08.000000 prosperity2submit-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:45.622817 prosperity2submit-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-11 09:12:45.622817 prosperity2submit-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:45.618817 prosperity2submit-0.2.4/prosperity2submit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/prosperity2submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/prosperity2submit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-04-11 09:12:41.000000 prosperity2submit-0.2.4/prosperity2submit/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:12:45.622817 prosperity2submit-0.2.4/prosperity2submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 09:12:45.000000 prosperity2submit-0.2.4/prosperity2submit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-11 09:12:43.000000 prosperity2submit-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:12:45.622817 prosperity2submit-0.2.4/setup.cfg
```

### Comparing `prosperity2submit-0.2.3/LICENSE` & `prosperity2submit-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.3/PKG-INFO` & `prosperity2submit-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.3
+Version: 0.2.4
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.3/README.md` & `prosperity2submit-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.3/prosperity2submit/__main__.py` & `prosperity2submit-0.2.4/prosperity2submit/__main__.py`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.3/prosperity2submit/core.py` & `prosperity2submit-0.2.4/prosperity2submit/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import keyring
+# This import needs to exist to prevent a 1024-character pasting limit on macOS
+# See https://stackoverflow.com/a/53871077
 import readline
 import requests
+import sys
 import time
 import webbrowser
 from collections import defaultdict
 from functools import partial
 from http.server import HTTPServer, SimpleHTTPRequestHandler
 from pathlib import Path
 from requests_toolbelt import MultipartEncoder
@@ -23,15 +26,15 @@
 From there, click on Local Storage in the sidebar and select the website that appears underneath the sidebar entry.
 Your token is stored in your system's credentials store for convenience.
     """.strip())
 
     token = input("Prosperity ID token: ")
     keyring.set_password(KEYRING_SERVICE, KEYRING_USERNAME, token)
 
-def request_with_token(method: str, url: str, form_data: Optional[dict[str, Any]] = None) -> requests.Response:
+def request_with_token(method: str, url: str, form_data: Optional[dict[str, Any]] = None, attempt: int = 0) -> requests.Response:
     token = keyring.get_password(KEYRING_SERVICE, KEYRING_USERNAME)
     if token is None:
         refresh_token()
         return request_with_token(method, url, form_data)
 
     data = None
     headers = {"Authorization": f"Bearer {token}"}
@@ -43,17 +46,22 @@
 
     response = requests.request(method, url, data=data, headers=headers)
 
     if response.status_code == 403:
         refresh_token()
         return request_with_token(method, url, form_data)
 
+    if response.status_code == 503:
+        print("The Prosperity website is currently in maintenance mode, please try again later")
+        sys.exit(1)
+
     if 500 <= response.status_code < 600:
-        print(f"Received unexpected HTTP {response.status_code} response from the Prosperity API, retrying request")
-        return request_with_token(method, url, form_data)
+        print(f"Received unexpected HTTP {response.status_code} response from the Prosperity API, retrying request after 5 seconds (attempt {attempt + 1})")
+        time.sleep(5)
+        return request_with_token(method, url, form_data, attempt + 1)
 
     response.raise_for_status()
     return response
 
 def format_path(path: Path) -> str:
     cwd = Path.cwd()
     if path.is_relative_to(cwd):
```

### Comparing `prosperity2submit-0.2.3/prosperity2submit.egg-info/PKG-INFO` & `prosperity2submit-0.2.4/prosperity2submit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.3
+Version: 0.2.4
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.3/pyproject.toml` & `prosperity2submit-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2submit"
 description = "Command-line submitter for IMC Prosperity 2 algorithms"
-version = "0.2.3"
+version = "0.2.4"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "submit", "submitter"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

