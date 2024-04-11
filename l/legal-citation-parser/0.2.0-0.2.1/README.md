# Comparing `tmp/legal_citation_parser-0.2.0.tar.gz` & `tmp/legal_citation_parser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legal_citation_parser-0.2.0.tar", last modified: Tue Apr  9 03:12:41 2024, max compression
+gzip compressed data, was "legal_citation_parser-0.2.1.tar", last modified: Thu Apr 11 01:10:47 2024, max compression
```

## Comparing `legal_citation_parser-0.2.0.tar` & `legal_citation_parser-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.2.0/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4756 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4421 2024-04-09 02:49:51.000000 legal_citation_parser-0.2.0/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/legal_citation_parser/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2024-04-07 01:51:59.000000 legal_citation_parser-0.2.0/legal_citation_parser/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    32481 2024-04-07 18:00:32.000000 legal_citation_parser-0.2.0/legal_citation_parser/canlii_constants.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8379 2024-04-09 02:03:30.000000 legal_citation_parser-0.2.0/legal_citation_parser/canlii_rules.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1023 2024-04-08 17:41:14.000000 legal_citation_parser-0.2.0/legal_citation_parser/citation_parser.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3705 2024-04-09 02:09:14.000000 legal_citation_parser-0.2.0/legal_citation_parser/utils.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4756 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-09 03:12:41.000000 legal_citation_parser-0.2.0/legal_citation_parser.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-09 03:12:41.073056 legal_citation_parser-0.2.0/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      703 2024-04-07 18:00:32.000000 legal_citation_parser-0.2.0/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-11 01:10:47.630238 legal_citation_parser-0.2.1/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    35149 2024-03-22 00:07:43.000000 legal_citation_parser-0.2.1/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4894 2024-04-11 01:10:47.630238 legal_citation_parser-0.2.1/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4559 2024-04-10 03:34:07.000000 legal_citation_parser-0.2.1/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-11 01:10:47.626238 legal_citation_parser-0.2.1/legal_citation_parser/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      100 2024-04-07 01:51:59.000000 legal_citation_parser-0.2.1/legal_citation_parser/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    61431 2024-04-10 03:28:29.000000 legal_citation_parser-0.2.1/legal_citation_parser/canlii_constants.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8529 2024-04-10 03:28:29.000000 legal_citation_parser-0.2.1/legal_citation_parser/canlii_rules.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1023 2024-04-08 17:41:14.000000 legal_citation_parser-0.2.1/legal_citation_parser/citation_parser.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     5036 2024-04-10 03:28:29.000000 legal_citation_parser-0.2.1/legal_citation_parser/utils.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-11 01:10:47.630238 legal_citation_parser-0.2.1/legal_citation_parser.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4894 2024-04-11 01:10:47.000000 legal_citation_parser-0.2.1/legal_citation_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      436 2024-04-11 01:10:47.000000 legal_citation_parser-0.2.1/legal_citation_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-11 01:10:47.000000 legal_citation_parser-0.2.1/legal_citation_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        9 2024-04-11 01:10:47.000000 legal_citation_parser-0.2.1/legal_citation_parser.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       22 2024-04-11 01:10:47.000000 legal_citation_parser-0.2.1/legal_citation_parser.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-11 01:10:47.630238 legal_citation_parser-0.2.1/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      703 2024-04-10 03:28:57.000000 legal_citation_parser-0.2.1/setup.py
```

### Comparing `legal_citation_parser-0.2.0/LICENSE` & `legal_citation_parser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.2.0/PKG-INFO` & `legal_citation_parser-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: legal_citation_parser
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extracts metadata from legal citations
 Home-page: https://github.com/646e62/legal_citation_parser
 Author: Daniel Nathan Booy
 Author-email: 444e42@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# legal_citation_parser
+# legal_citation_parser v 0.2.1
 Extracts metadata from legal citations.
 
 Although legal citations are typically short strings, they contain a great deal of information compressed into a relatively small package. This Python module is designed to extract and standardize that data from from legal citation strings. This module can currently handles the following citation types:
 
 * Neutral citations (Canadian);
 * Supreme Court Reader (SCR) citations;
 * CanLII citations.
@@ -130,14 +130,19 @@
     'caseId': {'en': '2018onca494'},
     'title': 'R. v. Ajise',
     'citation': '2018 ONCA 494 (CanLII)'},
     ...
    } 
 ```
 
+## v 0.2.1 updates
+
+* Added functionality to the CanLII API call tool
+* Updated the court code dictionaries using the CanLII API
+
 ## Contributing
 
 Contributions to improve this module are welcome. You can contribute by:
 * Reporting bugs
 * Suggesting enhancements
 * Sending pull requests with bug fixes or new features
```

### Comparing `legal_citation_parser-0.2.0/README.md` & `legal_citation_parser-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# legal_citation_parser
+# legal_citation_parser v 0.2.1
 Extracts metadata from legal citations.
 
 Although legal citations are typically short strings, they contain a great deal of information compressed into a relatively small package. This Python module is designed to extract and standardize that data from from legal citation strings. This module can currently handles the following citation types:
 
 * Neutral citations (Canadian);
 * Supreme Court Reader (SCR) citations;
 * CanLII citations.
@@ -118,14 +118,19 @@
     'caseId': {'en': '2018onca494'},
     'title': 'R. v. Ajise',
     'citation': '2018 ONCA 494 (CanLII)'},
     ...
    } 
 ```
 
+## v 0.2.1 updates
+
+* Added functionality to the CanLII API call tool
+* Updated the court code dictionaries using the CanLII API
+
 ## Contributing
 
 Contributions to improve this module are welcome. You can contribute by:
 * Reporting bugs
 * Suggesting enhancements
 * Sending pull requests with bug fixes or new features
```

### Comparing `legal_citation_parser-0.2.0/legal_citation_parser/canlii_rules.py` & `legal_citation_parser-0.2.1/legal_citation_parser/canlii_rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import re
 
 from .canlii_constants import (
     COURT_HIERARCHY_CRIMINAL,
     COURT_LEVEL_MAPPING,
+    COURT_LEVEL_MAPPING_LEGACY,
     PROVINCE_TERRITORY_ABBREVIATIONS,
 )
 
 from .utils import check_url, canlii_api_call
 
 
 def court_code_corrector(court_code):
@@ -118,14 +119,16 @@
     if uid is None:
         style_of_cause = None
 
     # Extrapolate the court name and jurisdiction from the court code
     if court_code:
         court_code_lower = court_code.lower()
         court_decoded = COURT_LEVEL_MAPPING.get(court_code_lower)
+        if court_decoded is None:
+            court_decoded = COURT_LEVEL_MAPPING_LEGACY.get(court_code_lower, 'scc')
         court_level = COURT_HIERARCHY_CRIMINAL.get(court_code_lower)
         court_name = court_decoded[0]
         jurisdiction = court_decoded[1]
     
     # Each subsequent variable requires court_code, so they are set to None if court_code == None
     else:
         court_decoded = court_name = court_level = jurisdiction = None
```

### Comparing `legal_citation_parser-0.2.0/legal_citation_parser/citation_parser.py` & `legal_citation_parser-0.2.1/legal_citation_parser/citation_parser.py`

 * *Files identical despite different names*

### Comparing `legal_citation_parser-0.2.0/legal_citation_parser.egg-info/PKG-INFO` & `legal_citation_parser-0.2.1/legal_citation_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: legal-citation-parser
-Version: 0.2.0
+Version: 0.2.1
 Summary: Extracts metadata from legal citations
 Home-page: https://github.com/646e62/legal_citation_parser
 Author: Daniel Nathan Booy
 Author-email: 444e42@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# legal_citation_parser
+# legal_citation_parser v 0.2.1
 Extracts metadata from legal citations.
 
 Although legal citations are typically short strings, they contain a great deal of information compressed into a relatively small package. This Python module is designed to extract and standardize that data from from legal citation strings. This module can currently handles the following citation types:
 
 * Neutral citations (Canadian);
 * Supreme Court Reader (SCR) citations;
 * CanLII citations.
@@ -130,14 +130,19 @@
     'caseId': {'en': '2018onca494'},
     'title': 'R. v. Ajise',
     'citation': '2018 ONCA 494 (CanLII)'},
     ...
    } 
 ```
 
+## v 0.2.1 updates
+
+* Added functionality to the CanLII API call tool
+* Updated the court code dictionaries using the CanLII API
+
 ## Contributing
 
 Contributions to improve this module are welcome. You can contribute by:
 * Reporting bugs
 * Suggesting enhancements
 * Sending pull requests with bug fixes or new features
```

### Comparing `legal_citation_parser-0.2.0/setup.py` & `legal_citation_parser-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='legal_citation_parser',
-    version='0.2.0',
+    version='0.2.1',
     description='Extracts metadata from legal citations',
     author='Daniel Nathan Booy',
     url='https://github.com/646e62/legal_citation_parser',
     author_email='444e42@protonmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

