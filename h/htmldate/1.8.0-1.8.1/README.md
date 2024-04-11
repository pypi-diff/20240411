# Comparing `tmp/htmldate-1.8.0.tar.gz` & `tmp/htmldate-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmldate-1.8.0.tar", last modified: Tue Mar 19 12:44:28 2024, max compression
+gzip compressed data, was "htmldate-1.8.1.tar", last modified: Thu Apr 11 14:49:11 2024, max compression
```

## Comparing `htmldate-1.8.0.tar` & `htmldate-1.8.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-03-19 12:44:28.505176 htmldate-1.8.0/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5987 2024-03-19 12:43:41.000000 htmldate-1.8.0/CHANGELOG.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1127 2020-01-08 18:09:15.000000 htmldate-1.8.0/CONTRIBUTING.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    10173 2024-03-19 12:43:51.000000 htmldate-1.8.0/LICENSE
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      277 2023-01-09 12:35:45.000000 htmldate-1.8.0/MANIFEST.in
--rw-r--r--   0 adbar     (1000) adbar     (1000)    10842 2024-03-19 12:44:28.505176 htmldate-1.8.0/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8064 2024-03-19 12:43:51.000000 htmldate-1.8.0/README.rst
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-03-19 12:44:28.501177 htmldate-1.8.0/htmldate/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      633 2024-03-19 12:43:51.000000 htmldate-1.8.0/htmldate/__init__.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4274 2024-03-19 12:43:51.000000 htmldate-1.8.0/htmldate/cli.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    31834 2024-03-19 12:43:51.000000 htmldate-1.8.0/htmldate/core.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    19147 2024-03-19 12:43:51.000000 htmldate-1.8.0/htmldate/extractors.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1249 2023-10-30 12:40:37.000000 htmldate-1.8.0/htmldate/meta.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        0 2022-07-18 15:53:08.000000 htmldate-1.8.0/htmldate/py.typed
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      748 2024-03-19 12:43:51.000000 htmldate-1.8.0/htmldate/settings.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8955 2024-03-19 12:43:51.000000 htmldate-1.8.0/htmldate/utils.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     6976 2024-03-19 12:43:51.000000 htmldate-1.8.0/htmldate/validators.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-03-19 12:44:28.505176 htmldate-1.8.0/htmldate.egg-info/
--rw-r--r--   0 adbar     (1000) adbar     (1000)    10842 2024-03-19 12:44:28.000000 htmldate-1.8.0/htmldate.egg-info/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      517 2024-03-19 12:44:28.000000 htmldate-1.8.0/htmldate.egg-info/SOURCES.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-03-19 12:44:28.000000 htmldate-1.8.0/htmldate.egg-info/dependency_links.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       47 2024-03-19 12:44:28.000000 htmldate-1.8.0/htmldate.egg-info/entry_points.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2023-09-05 14:06:48.000000 htmldate-1.8.0/htmldate.egg-info/not-zip-safe
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      584 2024-03-19 12:44:28.000000 htmldate-1.8.0/htmldate.egg-info/requires.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        9 2024-03-19 12:44:28.000000 htmldate-1.8.0/htmldate.egg-info/top_level.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-11-15 14:02:12.000000 htmldate-1.8.0/pytest.ini
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2024-03-19 12:44:28.505176 htmldate-1.8.0/setup.cfg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4534 2024-03-19 12:43:51.000000 htmldate-1.8.0/setup.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-03-19 12:44:28.501177 htmldate-1.8.0/tests/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       25 2023-12-08 14:53:32.000000 htmldate-1.8.0/tests/testlist.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    55100 2024-01-16 12:32:59.000000 htmldate-1.8.0/tests/unit_tests.py
+drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-04-11 14:49:11.575361 htmldate-1.8.1/
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)     6152 2024-04-11 14:44:00.000000 htmldate-1.8.1/CHANGELOG.md
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)     1872 2024-03-25 19:06:10.000000 htmldate-1.8.1/CONTRIBUTING.md
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)    10173 2024-03-19 12:43:51.000000 htmldate-1.8.1/LICENSE
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)      277 2023-01-09 12:35:45.000000 htmldate-1.8.1/MANIFEST.in
+-rw-r--r--   0 adbar     (1001) adbar     (1005)    10842 2024-04-11 14:49:11.575361 htmldate-1.8.1/PKG-INFO
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)     8064 2024-04-11 14:44:42.000000 htmldate-1.8.1/README.rst
+drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-04-11 14:49:11.571361 htmldate-1.8.1/htmldate/
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)      633 2024-04-11 14:45:00.000000 htmldate-1.8.1/htmldate/__init__.py
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)     4274 2024-03-19 12:43:51.000000 htmldate-1.8.1/htmldate/cli.py
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)    31834 2024-03-19 12:43:51.000000 htmldate-1.8.1/htmldate/core.py
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)    19160 2024-04-08 15:49:31.000000 htmldate-1.8.1/htmldate/extractors.py
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)     1249 2023-10-30 12:40:37.000000 htmldate-1.8.1/htmldate/meta.py
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)        0 2022-07-18 15:53:08.000000 htmldate-1.8.1/htmldate/py.typed
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)      748 2024-03-19 12:43:51.000000 htmldate-1.8.1/htmldate/settings.py
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)     8955 2024-03-19 12:43:51.000000 htmldate-1.8.1/htmldate/utils.py
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)     6976 2024-03-19 12:43:51.000000 htmldate-1.8.1/htmldate/validators.py
+drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-04-11 14:49:11.575361 htmldate-1.8.1/htmldate.egg-info/
+-rw-r--r--   0 adbar     (1001) adbar     (1005)    10842 2024-04-11 14:49:11.000000 htmldate-1.8.1/htmldate.egg-info/PKG-INFO
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)      517 2024-04-11 14:49:11.000000 htmldate-1.8.1/htmldate.egg-info/SOURCES.txt
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)        1 2024-04-11 14:49:11.000000 htmldate-1.8.1/htmldate.egg-info/dependency_links.txt
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)       47 2024-04-11 14:49:11.000000 htmldate-1.8.1/htmldate.egg-info/entry_points.txt
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)        1 2024-04-11 14:49:11.000000 htmldate-1.8.1/htmldate.egg-info/not-zip-safe
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)      584 2024-04-11 14:49:11.000000 htmldate-1.8.1/htmldate.egg-info/requires.txt
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)        9 2024-04-11 14:49:11.000000 htmldate-1.8.1/htmldate.egg-info/top_level.txt
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)       40 2021-11-15 14:02:12.000000 htmldate-1.8.1/pytest.ini
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)       38 2024-04-11 14:49:11.575361 htmldate-1.8.1/setup.cfg
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)     4534 2024-04-11 14:44:42.000000 htmldate-1.8.1/setup.py
+drwxrwxr-x   0 adbar     (1001) adbar     (1005)        0 2024-04-11 14:49:11.575361 htmldate-1.8.1/tests/
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)       25 2023-12-08 14:53:32.000000 htmldate-1.8.1/tests/testlist.txt
+-rw-rw-r--   0 adbar     (1001) adbar     (1005)    55100 2024-04-08 15:45:16.000000 htmldate-1.8.1/tests/unit_tests.py
```

### Comparing `htmldate-1.8.0/CHANGELOG.md` & `htmldate-1.8.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 ## Changelog
 
+
+## 1.8.1
+- fix: more restrictive YYYYMM pattern to prevent ValueError with @b3n4kh (#145)
+- maintenance: add pre-commit with checks with @nadasuhailAyesh12 (#142)
+
 ## 1.8.0
 - change license to Apache 2.0 (#140)
 - compile XPath expressions (#136)
 - update docs with @EkaterineSheshelidze (#135)
 
 ## 1.7.0
 - fix meta property updated vs. original behavior (#121)
```

### Comparing `htmldate-1.8.0/LICENSE` & `htmldate-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/PKG-INFO` & `htmldate-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmldate
-Version: 1.8.0
+Version: 1.8.1
 Summary: Fast and robust extraction of original and updated publication dates from URLs and web pages.
 Home-page: https://htmldate.readthedocs.io
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: Apache-2.0
 Project-URL: Source, https://github.com/adbar/htmldate
 Project-URL: Tracker, https://github.com/adbar/htmldate/issues
```

### Comparing `htmldate-1.8.0/README.rst` & `htmldate-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/htmldate/__init__.py` & `htmldate-1.8.1/htmldate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # meta
 __title__ = "htmldate"
 __author__ = "Adrien Barbaresi"
 __license__ = "Apache-2.0"
 __copyright__ = "Copyright 2017-2024, Adrien Barbaresi"
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 
 import logging
 
 from datetime import datetime
 
 try:
```

### Comparing `htmldate-1.8.0/htmldate/cli.py` & `htmldate-1.8.1/htmldate/cli.py`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/htmldate/core.py` & `htmldate-1.8.1/htmldate/core.py`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/htmldate/extractors.py` & `htmldate-1.8.1/htmldate/extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,16 +203,16 @@
     r"(\D19[0-9]{2}[01][0-9][0-3][0-9]\D|\D20[0-9]{2}[01][0-9][0-3][0-9]\D)"
 )
 DATESTRINGS_CATCH = re.compile(rf"({YEAR_RE})([01][0-9])([0-3][0-9])")
 SLASHES_PATTERN = re.compile(
     r"\D([0-3]?[0-9]/[01]?[0-9]/[0129][0-9]|[0-3][0-9]\.[01][0-9]\.[0129][0-9])\D"
 )
 SLASHES_YEAR = re.compile(r"([0-9]{2})$")
-YYYYMM_PATTERN = re.compile(r"\D([12][0-9]{3}[/.-][01][0-9])\D")
-YYYYMM_CATCH = re.compile(rf"({YEAR_RE})[/.-]([01][0-9])")
+YYYYMM_PATTERN = re.compile(r"\D([12][0-9]{3}[/.-](?:1[0-2]|0[1-9]))\D")
+YYYYMM_CATCH = re.compile(rf"({YEAR_RE})[/.-](1[0-2]|0[1-9]|)")
 MMYYYY_PATTERN = re.compile(r"\D([01]?[0-9][/.-][12][0-9]{3})\D")
 MMYYYY_YEAR = re.compile(rf"({YEAR_RE})\D?$")
 SIMPLE_PATTERN = re.compile(rf"(?<!w3.org)\D({YEAR_RE})\D")
 
 
 def discard_unwanted(tree: HtmlElement) -> Tuple[HtmlElement, List[HtmlElement]]:
     """Delete unwanted sections of an HTML document and return them as a list"""
```

### Comparing `htmldate-1.8.0/htmldate/meta.py` & `htmldate-1.8.1/htmldate/meta.py`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/htmldate/settings.py` & `htmldate-1.8.1/htmldate/settings.py`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/htmldate/utils.py` & `htmldate-1.8.1/htmldate/utils.py`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/htmldate/validators.py` & `htmldate-1.8.1/htmldate/validators.py`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/htmldate.egg-info/PKG-INFO` & `htmldate-1.8.1/htmldate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htmldate
-Version: 1.8.0
+Version: 1.8.1
 Summary: Fast and robust extraction of original and updated publication dates from URLs and web pages.
 Home-page: https://htmldate.readthedocs.io
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: Apache-2.0
 Project-URL: Source, https://github.com/adbar/htmldate
 Project-URL: Tracker, https://github.com/adbar/htmldate/issues
```

### Comparing `htmldate-1.8.0/htmldate.egg-info/SOURCES.txt` & `htmldate-1.8.1/htmldate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/htmldate.egg-info/requires.txt` & `htmldate-1.8.1/htmldate.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/setup.py` & `htmldate-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `htmldate-1.8.0/tests/unit_tests.py` & `htmldate-1.8.1/tests/unit_tests.py`

 * *Files identical despite different names*

