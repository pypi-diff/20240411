# Comparing `tmp/open_parser-0.0.3.tar.gz` & `tmp/open_parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_parser-0.0.3.tar", max compression
+gzip compressed data, was "open_parser-0.0.4.tar", max compression
```

## Comparing `open_parser-0.0.3.tar` & `open_parser-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1419 2024-04-06 00:51:24.943032 open_parser-0.0.3/README.md
--rw-r--r--   0        0        0       89 2024-04-07 02:41:57.793424 open_parser-0.0.3/open_parser/__init__.py
--rw-r--r--   0        0        0     3487 2024-04-07 02:39:17.470054 open_parser-0.0.3/open_parser/base.py
--rw-r--r--   0        0        0      394 2024-04-07 02:41:57.794218 open_parser-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 open_parser-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1419 2024-04-06 00:51:24.943032 open_parser-0.0.4/README.md
+-rw-r--r--   0        0        0       89 2024-04-11 02:28:46.122963 open_parser-0.0.4/open_parser/__init__.py
+-rw-r--r--   0        0        0     3487 2024-04-11 02:28:46.123221 open_parser-0.0.4/open_parser/base.py
+-rw-r--r--   0        0        0      394 2024-04-11 02:28:46.123602 open_parser-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 open_parser-0.0.4/PKG-INFO
```

### Comparing `open_parser-0.0.3/README.md` & `open_parser-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `open_parser-0.0.3/open_parser/base.py` & `open_parser-0.0.4/open_parser/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 
 import requests
 
 CAMBIO_UPLOAD_URL = (
-    "https://nl6h9ycq39.execute-api.us-west-2.amazonaws.com/v1/cambio_api/upload"
+    "https://qreije6m7l.execute-api.us-west-2.amazonaws.com/v1/cambio_api/upload"
 )
 CAMBIO_EXTRACT_URL = (
-    "https://nl6h9ycq39.execute-api.us-west-2.amazonaws.com/v1/cambio_api/extract"
+    "https://qreije6m7l.execute-api.us-west-2.amazonaws.com/v1/cambio_api/extract"
 )
 CAMBIO_PARSE_URL = (
-    "https://nl6h9ycq39.execute-api.us-west-2.amazonaws.com/v1/cambio_api/parse"
+    "https://qreije6m7l.execute-api.us-west-2.amazonaws.com/v1/cambio_api/parse"
 )
 
 
 class OpenParser:
     def __init__(self, apiKey) -> None:
         self._uploadurl = CAMBIO_UPLOAD_URL
         self._extracturl = CAMBIO_EXTRACT_URL
```

### Comparing `open_parser-0.0.3/PKG-INFO` & `open_parser-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-parser
-Version: 0.0.3
+Version: 0.0.4
 Summary: Open parser for all.
 Author: CambioML
 Author-email: wanwanaiai45@gmail.com
 Maintainer: Rachel Hu
 Maintainer-email: goldpiggy@berkeley.edu
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
```

