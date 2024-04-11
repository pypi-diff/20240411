# Comparing `tmp/vedro-httpx-0.4.0.tar.gz` & `tmp/vedro-httpx-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-httpx-0.4.0.tar", last modified: Sun Apr  7 14:34:57 2024, max compression
+gzip compressed data, was "vedro-httpx-0.4.1.tar", last modified: Thu Apr 11 15:53:11 2024, max compression
```

## Comparing `vedro-httpx-0.4.0.tar` & `vedro-httpx-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.985721 vedro-httpx-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_async_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_format_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_print_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_sync_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.985721 vedro-httpx-0.4.0/vedro_httpx/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_async_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_render_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_sync_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_vedro_httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/vedro_httpx/recorder/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_async_har_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_base_har_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_har_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_request_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_sync_har_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/vedro_httpx/recorder/har/
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/har/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/vedro_httpx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:53:11.931309 vedro-httpx-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-11 15:53:11.931309 vedro-httpx-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-11 15:53:11.931309 vedro-httpx-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:53:11.927309 vedro-httpx-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/tests/test_async_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/tests/test_format_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/tests/test_print_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/tests/test_sync_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:53:11.931309 vedro-httpx-0.4.1/vedro_httpx/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/_async_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/_render_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/_sync_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/_vedro_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:53:11.931309 vedro-httpx-0.4.1/vedro_httpx/recorder/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/recorder/_async_har_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/recorder/_base_har_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/recorder/_har_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/recorder/_request_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/recorder/_sync_har_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:53:11.931309 vedro-httpx-0.4.1/vedro_httpx/recorder/har/
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-04-11 15:53:04.000000 vedro-httpx-0.4.1/vedro_httpx/recorder/har/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:53:11.931309 vedro-httpx-0.4.1/vedro_httpx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-11 15:53:11.000000 vedro-httpx-0.4.1/vedro_httpx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-11 15:53:11.000000 vedro-httpx-0.4.1/vedro_httpx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:53:11.000000 vedro-httpx-0.4.1/vedro_httpx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 15:53:11.000000 vedro-httpx-0.4.1/vedro_httpx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 15:53:11.000000 vedro-httpx-0.4.1/vedro_httpx.egg-info/top_level.txt
```

### Comparing `vedro-httpx-0.4.0/LICENSE` & `vedro-httpx-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/PKG-INFO` & `vedro-httpx-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.4.0
+Version: 0.4.1
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/docs/integrations/httpx-client
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx<1.0,>=0.23
+Requires-Dist: httpx<1.0,>=0.24
 Requires-Dist: vedro<2.0,>=1.7
 
 # vedro-httpx
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-httpx/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-httpx)
 [![PyPI](https://img.shields.io/pypi/v/vedro-httpx.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-httpx?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
```

### Comparing `vedro-httpx-0.4.0/README.md` & `vedro-httpx-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/setup.cfg` & `vedro-httpx-0.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.0
+current_version = 0.4.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-httpx-0.4.0/setup.py` & `vedro-httpx-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-httpx",
-    version="0.4.0",
+    version="0.4.1",
     description="Vedro + HTTPX",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/vedro-universe/vedro-httpx",
```

### Comparing `vedro-httpx-0.4.0/tests/test_async_interface.py` & `vedro-httpx-0.4.1/tests/test_async_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/tests/test_format_response.py` & `vedro-httpx-0.4.1/tests/test_format_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/tests/test_plugin.py` & `vedro-httpx-0.4.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/tests/test_print_response.py` & `vedro-httpx-0.4.1/tests/test_print_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/tests/test_response.py` & `vedro-httpx-0.4.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/tests/test_sync_interface.py` & `vedro-httpx-0.4.1/tests/test_sync_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/vedro_httpx/_vedro_httpx.py` & `vedro-httpx-0.4.1/vedro_httpx/_vedro_httpx.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.4.0/vedro_httpx/recorder/har/__init__.py` & `vedro-httpx-0.4.1/vedro_httpx/recorder/har/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-# http://www.softwareishard.com/blog/har-12-spec/
+"""
+This code defines TypedDict classes for constructing HTTP Archive (HAR) format logs.
+These classes adhere to the HAR 1.2 Specification, which structures the way HTTP transactions
+are logged in browsers. More details on the specification can be found at:
+http://www.softwareishard.com/blog/har-12-spec/
+"""
 import sys
 from typing import List, TypedDict
 
 if sys.version_info < (3, 11):
     from typing_extensions import NotRequired
 else:
     from typing import NotRequired
@@ -43,15 +48,15 @@
 
 
 class Page(TypedDict):
     # Date and time stamp for the beginning of the page load
     # (ISO 8601 - YYYY-MM-DDThh:mm:ss.sTZD, e.g. 2009-07-24T19:20:30.45+01:00).
     startedDateTime: str
 
-    # Unique identifier of a page within the <log>. Entries use it to refer the parent page.
+    # Unique identifier of a page within the log. Entries use it to refer the parent page.
     id: str
 
     # Page title.
     title: str
 
     # Detailed timing info about page load.
     pageTimings: PageTimings
@@ -73,18 +78,18 @@
     #  The host of the cookie.
     domain: NotRequired[str]
 
     # Cookie expiration time.
     # (ISO 8601 - YYYY-MM-DDThh:mm:ss.sTZD, e.g. 2009-07-24T19:20:30.123+02:00).
     expires: NotRequired[str]
 
-    # Set to true if the cookie is HTTP only, false otherwise.
+    # Set to true if the cookie is HTTP-only, false otherwise.
     httpOnly: NotRequired[bool]
 
-    # True if the cookie was transmitted over ssl, false otherwise.
+    # True if the cookie was transmitted over SSL, false otherwise.
     secure: NotRequired[bool]
 
     # A comment provided by the user or the application.
     comment: NotRequired[str]
 
 
 class Header(TypedDict):
@@ -109,15 +114,15 @@
     comment: NotRequired[str]
 
 
 class PostParam(TypedDict):
     # Name of a posted parameter.
     name: str
 
-    # Value of a posted parameter or content of a posted file.
+    # Value of a posted parameter, or content of a posted file.
     value: str
 
     # Name of a posted file.
     fileName: NotRequired[str]
 
     # Content type of a posted file.
     contentType: NotRequired[str]
```

### Comparing `vedro-httpx-0.4.0/vedro_httpx.egg-info/PKG-INFO` & `vedro-httpx-0.4.1/vedro_httpx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.4.0
+Version: 0.4.1
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/docs/integrations/httpx-client
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx<1.0,>=0.23
+Requires-Dist: httpx<1.0,>=0.24
 Requires-Dist: vedro<2.0,>=1.7
 
 # vedro-httpx
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-httpx/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-httpx)
 [![PyPI](https://img.shields.io/pypi/v/vedro-httpx.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-httpx?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
```

### Comparing `vedro-httpx-0.4.0/vedro_httpx.egg-info/SOURCES.txt` & `vedro-httpx-0.4.1/vedro_httpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

