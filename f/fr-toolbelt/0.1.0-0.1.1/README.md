# Comparing `tmp/fr-toolbelt-0.1.0.tar.gz` & `tmp/fr-toolbelt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fr-toolbelt-0.1.0.tar", last modified: Tue Apr  9 20:59:28 2024, max compression
+gzip compressed data, was "fr-toolbelt-0.1.1.tar", last modified: Thu Apr 11 17:21:35 2024, max compression
```

## Comparing `fr-toolbelt-0.1.0.tar` & `fr-toolbelt-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 20:59:28.475662 fr-toolbelt-0.1.0/
--rw-rw-rw-   0        0        0     1106 2024-01-22 16:21:01.000000 fr-toolbelt-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    14088 2024-04-09 20:59:28.469145 fr-toolbelt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    11788 2024-02-16 21:09:29.000000 fr-toolbelt-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 20:59:27.968421 fr-toolbelt-0.1.0/fr_toolbelt/
--rw-rw-rw-   0        0        0      400 2024-02-15 15:51:29.000000 fr-toolbelt-0.1.0/fr_toolbelt/__init__.py
--rw-rw-rw-   0        0        0     2738 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.0/fr_toolbelt/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:59:28.074846 fr-toolbelt-0.1.0/fr_toolbelt/api_requests/
--rw-rw-rw-   0        0        0      488 2024-02-15 15:50:35.000000 fr-toolbelt-0.1.0/fr_toolbelt/api_requests/__init__.py
--rw-rw-rw-   0        0        0    11973 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.0/fr_toolbelt/api_requests/get_documents.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:59:28.321987 fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/
--rw-rw-rw-   0        0        0      502 2024-02-09 17:54:43.000000 fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/__init__.py
--rw-rw-rw-   0        0        0    15606 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/agencies.py
--rw-rw-rw-   0        0        0     2368 2024-02-09 18:53:56.000000 fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/dockets.py
--rw-rw-rw-   0        0        0     3210 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/documents.py
--rw-rw-rw-   0        0        0     2649 2024-02-09 18:59:30.000000 fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/fields.py
--rw-rw-rw-   0        0        0     1072 2024-02-09 15:51:31.000000 fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/presidents.py
--rw-rw-rw-   0        0        0     1480 2024-02-09 15:52:01.000000 fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/rin.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:59:28.437908 fr-toolbelt-0.1.0/fr_toolbelt/utils/
--rw-rw-rw-   0        0        0      475 2024-02-16 20:35:20.000000 fr-toolbelt-0.1.0/fr_toolbelt/utils/__init__.py
--rw-rw-rw-   0        0        0     5339 2024-02-17 02:07:49.000000 fr-toolbelt-0.1.0/fr_toolbelt/utils/duplicates.py
--rw-rw-rw-   0        0        0     5282 2024-02-13 21:04:48.000000 fr-toolbelt-0.1.0/fr_toolbelt/utils/format_dates.py
--rw-rw-rw-   0        0        0     4750 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.0/fr_toolbelt/utils/patch_progress.py
-drwxrwxrwx   0        0        0        0 2024-04-09 20:59:28.453519 fr-toolbelt-0.1.0/fr_toolbelt.egg-info/
--rw-rw-rw-   0        0        0    14088 2024-04-09 20:59:27.000000 fr-toolbelt-0.1.0/fr_toolbelt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-04-09 20:59:27.000000 fr-toolbelt-0.1.0/fr_toolbelt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 20:59:27.000000 fr-toolbelt-0.1.0/fr_toolbelt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 20:59:27.000000 fr-toolbelt-0.1.0/fr_toolbelt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 20:59:27.000000 fr-toolbelt-0.1.0/fr_toolbelt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1256 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 20:59:28.475662 fr-toolbelt-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 20:59:28.453519 fr-toolbelt-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-10-16 17:01:26.000000 fr-toolbelt-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      355 2024-02-01 16:31:05.000000 fr-toolbelt-0.1.0/tests/__main__.py
--rw-rw-rw-   0        0        0    20584 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.0/tests/tests.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:21:35.944572 fr-toolbelt-0.1.1/
+-rw-rw-rw-   0        0        0     1106 2024-01-22 16:21:01.000000 fr-toolbelt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    14311 2024-04-11 17:21:35.942535 fr-toolbelt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11989 2024-04-11 14:37:10.000000 fr-toolbelt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 17:21:35.610723 fr-toolbelt-0.1.1/fr_toolbelt/
+-rw-rw-rw-   0        0        0      400 2024-02-15 15:51:29.000000 fr-toolbelt-0.1.1/fr_toolbelt/__init__.py
+-rw-rw-rw-   0        0        0     2738 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.1/fr_toolbelt/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:21:35.715416 fr-toolbelt-0.1.1/fr_toolbelt/api_requests/
+-rw-rw-rw-   0        0        0      488 2024-02-15 15:50:35.000000 fr-toolbelt-0.1.1/fr_toolbelt/api_requests/__init__.py
+-rw-rw-rw-   0        0        0    11973 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.1/fr_toolbelt/api_requests/get_documents.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:21:35.843444 fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/
+-rw-rw-rw-   0        0        0      502 2024-02-09 17:54:43.000000 fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    15586 2024-04-11 14:37:10.000000 fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/agencies.py
+-rw-rw-rw-   0        0        0     2368 2024-02-09 18:53:56.000000 fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/dockets.py
+-rw-rw-rw-   0        0        0     3210 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/documents.py
+-rw-rw-rw-   0        0        0     2649 2024-02-09 18:59:30.000000 fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/fields.py
+-rw-rw-rw-   0        0        0     1072 2024-02-09 15:51:31.000000 fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/presidents.py
+-rw-rw-rw-   0        0        0     1480 2024-02-09 15:52:01.000000 fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/rin.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:21:35.904199 fr-toolbelt-0.1.1/fr_toolbelt/utils/
+-rw-rw-rw-   0        0        0      475 2024-02-16 20:35:20.000000 fr-toolbelt-0.1.1/fr_toolbelt/utils/__init__.py
+-rw-rw-rw-   0        0        0     5339 2024-02-17 02:07:49.000000 fr-toolbelt-0.1.1/fr_toolbelt/utils/duplicates.py
+-rw-rw-rw-   0        0        0     5282 2024-02-13 21:04:48.000000 fr-toolbelt-0.1.1/fr_toolbelt/utils/format_dates.py
+-rw-rw-rw-   0        0        0     4750 2024-04-09 20:58:56.000000 fr-toolbelt-0.1.1/fr_toolbelt/utils/patch_progress.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:21:35.934485 fr-toolbelt-0.1.1/fr_toolbelt.egg-info/
+-rw-rw-rw-   0        0        0    14311 2024-04-11 17:21:35.000000 fr-toolbelt-0.1.1/fr_toolbelt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-04-11 17:21:35.000000 fr-toolbelt-0.1.1/fr_toolbelt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 17:21:35.000000 fr-toolbelt-0.1.1/fr_toolbelt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-11 17:21:35.000000 fr-toolbelt-0.1.1/fr_toolbelt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-11 17:21:35.000000 fr-toolbelt-0.1.1/fr_toolbelt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1269 2024-04-11 17:19:45.000000 fr-toolbelt-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 17:21:35.952647 fr-toolbelt-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 17:21:35.924355 fr-toolbelt-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-16 17:01:26.000000 fr-toolbelt-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      355 2024-02-01 16:31:05.000000 fr-toolbelt-0.1.1/tests/__main__.py
+-rw-rw-rw-   0        0        0    20905 2024-04-11 14:37:10.000000 fr-toolbelt-0.1.1/tests/tests.py
```

### Comparing `fr-toolbelt-0.1.0/LICENSE` & `fr-toolbelt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/PKG-INFO` & `fr-toolbelt-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fr-toolbelt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolbelt of classes and functions written in Python to use with the Federal Register (FR) API.
 Author-email: Mark Febrizio <mfebrizio@gwu.edu>
 Maintainer-email: Mark Febrizio <mfebrizio@gwu.edu>, GW Regulatory Studies Center <regulatorystudies@gwu.edu>
 License: MIT License
         
         Copyright (c) 2024 GW Regulatory Studies Center
         
@@ -35,29 +35,33 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31
 Requires-Dist: pandas>=1.5
+Requires-Dist: numpy
 Requires-Dist: progress>=1.6
 Requires-Dist: cursor>=1.3
 
 # fr-toolbelt
 
+[![PyPI - Version](https://img.shields.io/pypi/v/fr-toolbelt?color=033C5A)](https://pypi.org/project/fr-toolbelt/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fr-toolbelt?color=AA9868)](https://www.python.org/downloads/)
+
 Toolbelt of classes and functions written in Python to use with the [Federal Register API](https://www.federalregister.gov/developers/documentation/api/v1). The Federal Register (FR) is the daily journal of the U.S. government, containing rules, proposed rules, notices, and presidential documents from federal agencies.
 
 Name inspired by the [Requests Toolbelt](https://github.com/requests/toolbelt) package. "FR" is a common shorthand for the Federal Register, in part because document citations take the form of VOLUME FR STARTPAGE (e.g., [88 FR 21879](https://www.federalregister.gov/d/2023-07760)).
 
 ## Installation
 
 Install using pip:
 
 ```bash
-pip install git+https://github.com/regulatorystudies/fr-toolbelt.git
+pip install fr-toolbelt
 ```
 
 This package was developed with Python 3.12 and requires Python 3.10 or higher.
 
 ## Basic Usage
 
 You can run the package as a module to get an illustration of how it processes documents:
```

### Comparing `fr-toolbelt-0.1.0/README.md` & `fr-toolbelt-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # fr-toolbelt
 
+[![PyPI - Version](https://img.shields.io/pypi/v/fr-toolbelt?color=033C5A)](https://pypi.org/project/fr-toolbelt/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fr-toolbelt?color=AA9868)](https://www.python.org/downloads/)
+
 Toolbelt of classes and functions written in Python to use with the [Federal Register API](https://www.federalregister.gov/developers/documentation/api/v1). The Federal Register (FR) is the daily journal of the U.S. government, containing rules, proposed rules, notices, and presidential documents from federal agencies.
 
 Name inspired by the [Requests Toolbelt](https://github.com/requests/toolbelt) package. "FR" is a common shorthand for the Federal Register, in part because document citations take the form of VOLUME FR STARTPAGE (e.g., [88 FR 21879](https://www.federalregister.gov/d/2023-07760)).
 
 ## Installation
 
 Install using pip:
 
 ```bash
-pip install git+https://github.com/regulatorystudies/fr-toolbelt.git
+pip install fr-toolbelt
 ```
 
 This package was developed with Python 3.12 and requires Python 3.10 or higher.
 
 ## Basic Usage
 
 You can run the package as a module to get an illustration of how it processes documents:
```

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/__main__.py` & `fr-toolbelt-0.1.1/fr_toolbelt/__main__.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/api_requests/get_documents.py` & `fr-toolbelt-0.1.1/fr_toolbelt/api_requests/get_documents.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/agencies.py` & `fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/agencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,16 +270,16 @@
         else:
             raise TypeError("Parameter 'return_format' must be `str`, `tuple`, `list`, or `None`.")
         document_copy = document.copy()
         slugs = document_copy.get(slug_key)
         if identify_ira:
                 document_copy["independent_reg_agency"] = self.__identify_independent_reg_agencies(slugs)
         for fmt in return_format:
-            parents = (self.__get_agency_info(slug, return_format) for slug in slugs if slug in self.schema.get("parents"))
-            subagencies = (self.__get_agency_info(slug, return_format) for slug in slugs if slug in self.schema.get("subagencies"))
+            parents = (self.__get_agency_info(slug, fmt) for slug in slugs if slug in self.schema.get("parents"))
+            subagencies = (self.__get_agency_info(slug, fmt) for slug in slugs if slug in self.schema.get("subagencies"))
             if return_values_as_str:
                 document_copy.update({
                     f"parent_{fmt}": self.__return_values_as_str(parents), 
                     f"subagency_{fmt}": self.__return_values_as_str(subagencies), 
                     })
             else:
                 document_copy.update({
```

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/dockets.py` & `fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/dockets.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/documents.py` & `fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/documents.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/fields.py` & `fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/fields.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/presidents.py` & `fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/presidents.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/preprocessing/rin.py` & `fr-toolbelt-0.1.1/fr_toolbelt/preprocessing/rin.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/utils/duplicates.py` & `fr-toolbelt-0.1.1/fr_toolbelt/utils/duplicates.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/utils/format_dates.py` & `fr-toolbelt-0.1.1/fr_toolbelt/utils/format_dates.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt/utils/patch_progress.py` & `fr-toolbelt-0.1.1/fr_toolbelt/utils/patch_progress.py`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt.egg-info/PKG-INFO` & `fr-toolbelt-0.1.1/fr_toolbelt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fr-toolbelt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Toolbelt of classes and functions written in Python to use with the Federal Register (FR) API.
 Author-email: Mark Febrizio <mfebrizio@gwu.edu>
 Maintainer-email: Mark Febrizio <mfebrizio@gwu.edu>, GW Regulatory Studies Center <regulatorystudies@gwu.edu>
 License: MIT License
         
         Copyright (c) 2024 GW Regulatory Studies Center
         
@@ -35,29 +35,33 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31
 Requires-Dist: pandas>=1.5
+Requires-Dist: numpy
 Requires-Dist: progress>=1.6
 Requires-Dist: cursor>=1.3
 
 # fr-toolbelt
 
+[![PyPI - Version](https://img.shields.io/pypi/v/fr-toolbelt?color=033C5A)](https://pypi.org/project/fr-toolbelt/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fr-toolbelt?color=AA9868)](https://www.python.org/downloads/)
+
 Toolbelt of classes and functions written in Python to use with the [Federal Register API](https://www.federalregister.gov/developers/documentation/api/v1). The Federal Register (FR) is the daily journal of the U.S. government, containing rules, proposed rules, notices, and presidential documents from federal agencies.
 
 Name inspired by the [Requests Toolbelt](https://github.com/requests/toolbelt) package. "FR" is a common shorthand for the Federal Register, in part because document citations take the form of VOLUME FR STARTPAGE (e.g., [88 FR 21879](https://www.federalregister.gov/d/2023-07760)).
 
 ## Installation
 
 Install using pip:
 
 ```bash
-pip install git+https://github.com/regulatorystudies/fr-toolbelt.git
+pip install fr-toolbelt
 ```
 
 This package was developed with Python 3.12 and requires Python 3.10 or higher.
 
 ## Basic Usage
 
 You can run the package as a module to get an illustration of how it processes documents:
```

### Comparing `fr-toolbelt-0.1.0/fr_toolbelt.egg-info/SOURCES.txt` & `fr-toolbelt-0.1.1/fr_toolbelt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fr-toolbelt-0.1.0/pyproject.toml` & `fr-toolbelt-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fr-toolbelt"
 #dynamic = ["version"]
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
   "requests>=2.31",
   "pandas>=1.5",
+  "numpy", 
   "progress>=1.6",
   "cursor>=1.3",
 ]
 requires-python = ">= 3.10"
 authors = [
   {name = "Mark Febrizio", email = "mfebrizio@gwu.edu"},
 ]
```

### Comparing `fr-toolbelt-0.1.0/tests/tests.py` & `fr-toolbelt-0.1.1/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import date
+from itertools import product
 import json
 from pathlib import Path
 #from pprint import pprint
 
 from requests import get
 
 from fr_toolbelt.api_requests import (
@@ -408,40 +409,46 @@
         assert key not in processed_keys, f"Failed to delete keys: {key=}"
 
 
 def test_agencies_data_process_return_format_str(
         documents = TEST_DATA, 
         metadata = TEST_METADATA, 
         schema = TEST_SCHEMA, 
-        check_keys = ("agency_slugs", "parent_", "subagency_", "independent_reg_agency")
+        check_keys = ("agency_slugs", "independent_reg_agency", ), 
+        check_prefixes = ("parent_", "subagency_", ), 
+        return_format="short_name", 
 ):
     agency_data = AgencyData(documents=documents, metadata=metadata, schema=schema)
-    processed = agency_data.process_data(return_format="short_name")
+    processed = agency_data.process_data(return_format=return_format)
     assert isinstance(processed, list)
     assert len(processed) > 0
     processed_keys = set((k for d in processed for k in d))
-    for key in check_keys:
-        assert any(pk.startswith(key) for pk in processed_keys), f"Output missing {key=}"
+    checks = list(check_keys) + [f"{p[0]}{p[1]}" for p in product(check_prefixes, (return_format, ))]
+    for key in checks:
+        assert key in processed_keys, f"Output missing {key=}"
     for key in agency_data.field_keys:
         assert key not in processed_keys, f"Failed to delete keys: {key=}"
 
 
 def test_agencies_data_process_return_format_tuple(
         documents = TEST_DATA, 
         metadata = TEST_METADATA, 
         schema = TEST_SCHEMA, 
-        check_keys = ("agency_slugs", "parent_", "subagency_", "independent_reg_agency")
+        check_keys = ("agency_slugs", "independent_reg_agency", ), 
+        check_prefixes = ("parent_", "subagency_", ), 
+        return_format=("short_name", "slug", ), 
 ):
     agency_data = AgencyData(documents=documents, metadata=metadata, schema=schema)
-    processed = agency_data.process_data(return_format=("short_name", "slug"))
+    processed = agency_data.process_data(return_format=return_format)
     assert isinstance(processed, list)
     assert len(processed) > 0
     processed_keys = set((k for d in processed for k in d))
-    for key in check_keys:
-        assert any(pk.startswith(key) for pk in processed_keys), f"Output missing {key=}"
+    checks = list(check_keys) + [f"{p[0]}{p[1]}" for p in product(check_prefixes, return_format)]
+    for key in checks:
+        assert key in processed_keys, f"Output missing {key=}"
     for key in agency_data.field_keys:
         assert key not in processed_keys, f"Failed to delete keys: {key=}"
 
 
 test_agencies = (
     test_agencies_metadata_init, 
     test_agencies_metadata_get,
```

