# Comparing `tmp/adif_io-0.4.0.tar.gz` & `tmp/adif_io-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adif_io-0.4.0.tar", last modified: Tue Jun  6 16:45:16 2023, max compression
+gzip compressed data, was "adif_io-0.4.1.tar", last modified: Thu Apr 11 08:38:13 2024, max compression
```

## Comparing `adif_io-0.4.0.tar` & `adif_io-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:16.012039 adif_io-0.4.0/
--rw-r--r--   0 andreas   (1000) andreas   (1000)    11358 2019-10-26 14:11:14.000000 adif_io-0.4.0/LICENSE
--rw-r--r--   0 andreas   (1000) andreas   (1000)      140 2023-06-06 14:24:35.000000 adif_io-0.4.0/NOTICE
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4090 2023-06-06 16:45:16.012039 adif_io-0.4.0/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3508 2023-06-06 12:29:32.000000 adif_io-0.4.0/README.md
--rw-r--r--   0 andreas   (1000) andreas   (1000)       38 2023-06-06 16:45:16.012039 adif_io-0.4.0/setup.cfg
--rw-r--r--   0 andreas   (1000) andreas   (1000)      832 2023-06-06 14:26:34.000000 adif_io-0.4.0/setup.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:15.944039 adif_io-0.4.0/src/
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:15.984039 adif_io-0.4.0/src/adif_io/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6240 2023-06-06 13:49:18.000000 adif_io-0.4.0/src/adif_io/__init__.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:16.000039 adif_io-0.4.0/src/adif_io.egg-info/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     4090 2023-06-06 16:45:15.000000 adif_io-0.4.0/src/adif_io.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)      256 2023-06-06 16:45:15.000000 adif_io-0.4.0/src/adif_io.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2023-06-06 16:45:15.000000 adif_io-0.4.0/src/adif_io.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        8 2023-06-06 16:45:15.000000 adif_io-0.4.0/src/adif_io.egg-info/top_level.txt
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-06-06 16:45:16.004039 adif_io-0.4.0/tests/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     6901 2023-06-06 14:51:51.000000 adif_io-0.4.0/tests/test_adif_import.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)      859 2023-06-06 14:13:26.000000 adif_io-0.4.0/tests/test_degree_translation.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-11 08:38:13.863938 adif_io-0.4.1/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)    11358 2019-10-26 14:11:14.000000 adif_io-0.4.1/LICENSE
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      194 2024-04-11 08:27:22.000000 adif_io-0.4.1/NOTICE
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4090 2024-04-11 08:38:13.863938 adif_io-0.4.1/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     3508 2023-06-06 12:29:32.000000 adif_io-0.4.1/README.md
+-rw-r--r--   0 andreas   (1000) andreas   (1000)       38 2024-04-11 08:38:13.863938 adif_io-0.4.1/setup.cfg
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      832 2024-04-11 08:34:22.000000 adif_io-0.4.1/setup.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-11 08:38:13.775938 adif_io-0.4.1/src/
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-11 08:38:13.819938 adif_io-0.4.1/src/adif_io/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6277 2024-04-11 08:26:04.000000 adif_io-0.4.1/src/adif_io/__init__.py
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-11 08:38:13.863938 adif_io-0.4.1/src/adif_io.egg-info/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     4090 2024-04-11 08:38:13.000000 adif_io-0.4.1/src/adif_io.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      256 2024-04-11 08:38:13.000000 adif_io-0.4.1/src/adif_io.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2024-04-11 08:38:13.000000 adif_io-0.4.1/src/adif_io.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) andreas   (1000)        8 2024-04-11 08:38:13.000000 adif_io-0.4.1/src/adif_io.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2024-04-11 08:38:13.859938 adif_io-0.4.1/tests/
+-rw-r--r--   0 andreas   (1000) andreas   (1000)     6901 2023-06-06 14:51:51.000000 adif_io-0.4.1/tests/test_adif_import.py
+-rw-r--r--   0 andreas   (1000) andreas   (1000)      859 2023-06-06 14:13:26.000000 adif_io-0.4.1/tests/test_degree_translation.py
```

### Comparing `adif_io-0.4.0/LICENSE` & `adif_io-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adif_io-0.4.0/PKG-INFO` & `adif_io-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: adif_io
-Version: 0.4.0
+Version: 0.4.1
 Summary: Basic input of ADIF radio amateur log files.
 Home-page: https://gitlab.com/andreas_krueger_py/adif_io
 Author: Andreas Krüger (DJ3EI)
 Author-email: dj3ei@famsik.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Communications :: Ham Radio
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # This is an ADIF parser in Python.
 
 ## Actual usage
```

### Comparing `adif_io-0.4.0/README.md` & `adif_io-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `adif_io-0.4.0/setup.py` & `adif_io-0.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf_8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adif_io",
-    version="0.4.0",
+    version="0.4.1",
     author="Andreas Krüger (DJ3EI)",
     author_email="dj3ei@famsik.de",
     description="Basic input of ADIF radio amateur log files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
@@ -17,9 +17,9 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Communications :: Ham Radio"
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 )
```

### Comparing `adif_io-0.4.0/src/adif_io/__init__.py` & `adif_io-0.4.1/src/adif_io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # Keys in that dict are ADIF field names in upper case,
 # value for a key is whatever was found in the ADIF, as a string.
 # Order of QSOs in the list is same as in ADIF file.
 
 import math
 import re
 from datetime import datetime, timedelta, timezone
+from typing import Dict, List, Tuple
 
 
 class AdifError(Exception):
     """Base error."""
 
     pass
 
@@ -48,26 +49,26 @@
     """Error for duplicate fileds in one QSO record or in the header."""
 
     pass
 
 
 # Some type definitions:
 
-headers = dict[str, str]
-qso = dict[str, str]
+headers = Dict[str, str]
+qso = Dict[str, str]
 
 
-def read_from_string(adif_string: str) -> tuple[list[qso], headers]:
+def read_from_string(adif_string: str) -> Tuple[List[qso], headers]:
     # The ADIF file header keys and values, if any.
     adif_headers: headers = {}
 
     header_field_re = re.compile(r"<((eoh)|(\w+)\:(\d+)(\:[^>]+)?)>", re.IGNORECASE)
     field_re = re.compile(r"<((eor)|(\w+)\:(\d+)(\:[^>]+)?)>", re.IGNORECASE)
 
-    qsos: list[qso] = []
+    qsos: List[qso] = []
     cursor = 0
     if adif_string[0] != "<":
         # Input has ADIF header. Read all header fields.
         eoh_found = False
         while not eoh_found:
             header_field_mo = header_field_re.search(adif_string, cursor)
             if header_field_mo:
@@ -111,15 +112,15 @@
             one_qso[field] = value
             cursor = value_end
         field_mo = field_re.search(adif_string, cursor)
 
     return (qsos, adif_headers)
 
 
-def read_from_file(filename: str) -> tuple[list[qso], headers]:
+def read_from_file(filename: str) -> Tuple[List[qso], headers]:
     with open(filename) as adif_file:
         adif_string = adif_file.read()
         return read_from_string(adif_string)
 
 
 _ONE_DAY = timedelta(days=1)
```

### Comparing `adif_io-0.4.0/src/adif_io.egg-info/PKG-INFO` & `adif_io-0.4.1/src/adif_io.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: adif-io
-Version: 0.4.0
+Name: adif_io
+Version: 0.4.1
 Summary: Basic input of ADIF radio amateur log files.
 Home-page: https://gitlab.com/andreas_krueger_py/adif_io
 Author: Andreas Krüger (DJ3EI)
 Author-email: dj3ei@famsik.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Communications :: Ham Radio
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # This is an ADIF parser in Python.
 
 ## Actual usage
```

### Comparing `adif_io-0.4.0/tests/test_adif_import.py` & `adif_io-0.4.1/tests/test_adif_import.py`

 * *Files identical despite different names*

### Comparing `adif_io-0.4.0/tests/test_degree_translation.py` & `adif_io-0.4.1/tests/test_degree_translation.py`

 * *Files identical despite different names*

