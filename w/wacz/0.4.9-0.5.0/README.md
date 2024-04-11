# Comparing `tmp/wacz-0.4.9.tar.gz` & `tmp/wacz-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wacz-0.4.9.tar", last modified: Thu Jun 29 16:42:54 2023, max compression
+gzip compressed data, was "wacz-0.5.0.tar", last modified: Thu Apr 11 20:21:57 2024, max compression
```

## Comparing `wacz-0.4.9.tar` & `wacz-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:54.841309 wacz-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 16:42:43.000000 wacz-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-29 16:42:54.841309 wacz-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-29 16:42:43.000000 wacz-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:42:54.841309 wacz-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-29 16:42:43.000000 wacz-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:54.837309 wacz-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_create_wacz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_create_wacz_hash_in_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_create_wacz_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_optional_flags_wacz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_validate_wacz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_verify_signed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-29 16:42:43.000000 wacz-0.4.9/tests/test_wacz_indexer_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:54.841309 wacz-0.4.9/wacz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-29 16:42:43.000000 wacz-0.4.9/wacz/waczindexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:42:54.841309 wacz-0.4.9/wacz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:42:54.000000 wacz-0.4.9/wacz.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:21:57.341918 wacz-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 20:21:49.000000 wacz-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-11 20:21:57.341918 wacz-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-11 20:21:49.000000 wacz-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:21:57.341918 wacz-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-11 20:21:49.000000 wacz-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:21:57.337917 wacz-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/test_create_wacz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/test_create_wacz_hash_in_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/test_create_wacz_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26697 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/test_optional_flags_wacz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/test_validate_wacz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/test_verify_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-11 20:21:49.000000 wacz-0.5.0/tests/test_wacz_indexer_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:21:57.341918 wacz-0.5.0/wacz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:21:49.000000 wacz-0.5.0/wacz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 20:21:49.000000 wacz-0.5.0/wacz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-11 20:21:49.000000 wacz-0.5.0/wacz/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-11 20:21:49.000000 wacz-0.5.0/wacz/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-04-11 20:21:49.000000 wacz-0.5.0/wacz/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14549 2024-04-11 20:21:49.000000 wacz-0.5.0/wacz/waczindexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:21:57.341918 wacz-0.5.0/wacz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-11 20:21:57.000000 wacz-0.5.0/wacz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-11 20:21:57.000000 wacz-0.5.0/wacz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:21:57.000000 wacz-0.5.0/wacz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 20:21:57.000000 wacz-0.5.0/wacz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-11 20:21:57.000000 wacz-0.5.0/wacz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 20:21:57.000000 wacz-0.5.0/wacz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:21:57.000000 wacz-0.5.0/wacz.egg-info/zip-safe
```

### Comparing `wacz-0.4.9/LICENSE` & `wacz-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/PKG-INFO` & `wacz-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wacz
-Version: 0.4.9
+Version: 0.5.0
 Summary: WACZ Format Tools
 Home-page: https://github.com/webrecorder/py-wacz
 Author: Ilya Kreymer, Emma Dickson
 Author-email: info@webrecorder.net
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -80,14 +80,30 @@
 
 Overrides the pages index generation with the passed jsonl pages.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl
 ```
 
+### -e --extra-pages
+
+Overrides the extra pages index generation with the passed extra jsonl pages.
+
+```
+wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl -e extra_pages.jsonl
+```
+
+### -c --copy-pages
+
+Overrides the behavior of --pages and --extra-pages options to copy existing pages.jsonl and/or extraPages.jsonl as-is directly into the WACZ rather than attempting to match each page to WARC record. The files are still parsed for basic correctness.
+
+```
+wacz create tests/fixtures/example-collection.warc --pages pages/pages.jsonl --extra-pages pages/extraPages.jsonl --copy-pages
+```
+
 ### -t --text
 
 You can add a full text index by including the --text tag.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl --text
 ```
```

### Comparing `wacz-0.4.9/README.md` & `wacz-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -67,14 +67,30 @@
 
 Overrides the pages index generation with the passed jsonl pages.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl
 ```
 
+### -e --extra-pages
+
+Overrides the extra pages index generation with the passed extra jsonl pages.
+
+```
+wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl -e extra_pages.jsonl
+```
+
+### -c --copy-pages
+
+Overrides the behavior of --pages and --extra-pages options to copy existing pages.jsonl and/or extraPages.jsonl as-is directly into the WACZ rather than attempting to match each page to WARC record. The files are still parsed for basic correctness.
+
+```
+wacz create tests/fixtures/example-collection.warc --pages pages/pages.jsonl --extra-pages pages/extraPages.jsonl --copy-pages
+```
+
 ### -t --text
 
 You can add a full text index by including the --text tag.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl --text
 ```
```

### Comparing `wacz-0.4.9/setup.py` & `wacz-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # vim: set sw=4 et:
 from setuptools import setup, find_packages
 
-__version__ = "0.4.9"
+__version__ = "0.5.0"
 
 def load_requirements(filename):
     with open(filename, "rt") as fh:
         return fh.read().rstrip().split("\n")
 
 def long_description():
     with open("README.md") as f:
@@ -20,15 +20,15 @@
     license="Apache 2.0",
     packages=find_packages(exclude=["test"]),
     url="https://github.com/webrecorder/py-wacz",
     description="WACZ Format Tools",
     long_description=long_description(),
     long_description_content_type="text/markdown",
     install_requires=load_requirements("requirements.txt"),
-    extras_require={"signing": ["authsign>=0.3.1", "requests"]},
+    extras_require={"signing": ["authsign>=0.5.1", "requests"]},
     zip_safe=True,
     setup_requires=["pytest-runner"],
     entry_points="""
         [console_scripts]
         wacz = wacz.main:main
     """,
 )
```

### Comparing `wacz-0.4.9/tests/test_create_wacz.py` & `wacz-0.5.0/tests/test_create_wacz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import unittest, os, zipfile, sys, gzip, json, tempfile
 from wacz.main import main, now
 from unittest.mock import patch
-from wacz.util import hash_stream
+from wacz.util import hash_file
 from frictionless import validate, Report
 
 TEST_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), "fixtures")
 
 
-def hash_file(type_, filename):
-    with open(filename, "rb") as fh:
-        size_, hash_ = hash_stream(type_, fh)
-
-    return hash_
-
-
 class TestWaczFormat(unittest.TestCase):
     def find_resource(self, resource_list, filename):
         for file in resource_list:
             if filename in file["path"]:
                 return file
 
     @classmethod
```

### Comparing `wacz-0.4.9/tests/test_create_wacz_hash_in_page.py` & `wacz-0.5.0/tests/test_create_wacz_hash_in_page.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/tests/test_create_wacz_indexing.py` & `wacz-0.5.0/tests/test_create_wacz_indexing.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/tests/test_optional_flags_wacz.py` & `wacz-0.5.0/tests/test_optional_flags_wacz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import unittest
 import tempfile
 import os
 import zipfile, json, gzip
 from wacz.main import main, now
+from wacz.util import hash_file
 from unittest.mock import patch
 import jsonlines
 
 TEST_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), "fixtures")
+PAGES_DIR = os.path.join(TEST_DIR, "pages")
 
 
 class TestWaczFormat(unittest.TestCase):
     def test_warc_with_invalid_passed_pages(self):
         """If a user passes an invalid file using --page we should return an error"""
         with tempfile.TemporaryDirectory() as tmpdir:
             fp = tempfile.NamedTemporaryFile()
@@ -31,14 +33,103 @@
                         "-p",
                         os.path.join(tmpdir, fp.name),
                     ]
                 ),
                 0,
             )
 
+    def test_invalid_passed_pages_copy_pages(self):
+        """If a user passes an invalid pages.jsonl file using --page --copy-pages we should return an error"""
+        with tempfile.TemporaryDirectory() as tmpdir:
+            self.assertEqual(
+                main(
+                    [
+                        "create",
+                        "-f",
+                        os.path.join(TEST_DIR, "example-collection.warc"),
+                        "-o",
+                        os.path.join(
+                            tmpdir, "example-collection-invalid-copy-pages.wacz"
+                        ),
+                        "-p",
+                        os.path.join(PAGES_DIR, "invalid.jsonl"),
+                        "--copy-pages",
+                    ]
+                ),
+                1,
+            )
+
+            self.assertEqual(
+                main(
+                    [
+                        "create",
+                        "-f",
+                        os.path.join(TEST_DIR, "example-collection.warc"),
+                        "-o",
+                        os.path.join(
+                            tmpdir, "example-collection-invalid-copy-pages-txt.wacz"
+                        ),
+                        "-p",
+                        os.path.join(PAGES_DIR, "invalid.txt"),
+                        "--copy-pages",
+                    ]
+                ),
+                1,
+            )
+
+    def test_invalid_passed_extra_pages_copy_pages(self):
+        """If a user passes an invalid extarPages.jsonl file using -e --copy-pages we still create WACZ without extra pages"""
+        with tempfile.TemporaryDirectory() as tmpdir:
+            self.assertEqual(
+                main(
+                    [
+                        "create",
+                        "-f",
+                        os.path.join(TEST_DIR, "example-collection.warc"),
+                        "-o",
+                        os.path.join(
+                            tmpdir, "example-collection-invalid-copy-extra-pages.wacz"
+                        ),
+                        "-p",
+                        os.path.join(PAGES_DIR, "pages.jsonl"),
+                        "-e",
+                        os.path.join(PAGES_DIR, "invalid.txt"),
+                        "--copy-pages",
+                    ]
+                ),
+                0,
+            )
+
+            with zipfile.ZipFile(
+                os.path.join(
+                    tmpdir, "example-collection-invalid-copy-extra-pages.wacz"
+                ),
+                "r",
+            ) as zip_ref:
+                zip_ref.extractall(os.path.join(tmpdir, "wacz_no_extra_pages"))
+                zip_ref.close()
+
+            self.assertEqual(
+                main(
+                    [
+                        "validate",
+                        "-f",
+                        os.path.join(
+                            tmpdir, "example-collection-invalid-copy-extra-pages.wacz"
+                        ),
+                    ]
+                ),
+                0,
+            )
+
+            self.assertFalse(
+                "extraPages.jsonl"
+                in os.listdir(os.path.join(tmpdir, "wacz_no_extra_pages/pages/"))
+            )
+
     @patch("wacz.main.now")
     def test_warc_with_pages_flag(self, mock_now):
         """When passing the pages flag with a valid pages.jsonl file a pages/pages.jsonl file should be created"""
         mock_now.return_value = (2020, 10, 7, 22, 29, 10)
 
         with tempfile.TemporaryDirectory() as tmpdir:
             fp = tempfile.NamedTemporaryFile()
@@ -92,14 +183,78 @@
                     obj = json.loads(line)
                     self.assertTrue("id" in obj.keys())
                     self.assertTrue("ts" in obj.keys())
                     self.assertTrue("url" in obj.keys())
                     self.assertTrue(obj["url"].encode() in cdx_content)
 
     @patch("wacz.main.now")
+    def test_warc_with_copy_pages(self, mock_now):
+        """When passing the pages and extra-pages flags with copy-pages, the files should end up in the WACZ exactly as-is"""
+        mock_now.return_value = (2020, 10, 7, 22, 29, 10)
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            self.assertEqual(
+                main(
+                    [
+                        "create",
+                        "-f",
+                        os.path.join(TEST_DIR, "example-collection.warc"),
+                        "-o",
+                        os.path.join(tmpdir, "example-collection-copy-pages.wacz"),
+                        "-p",
+                        os.path.join(PAGES_DIR, "pages.jsonl"),
+                        "-e",
+                        os.path.join(PAGES_DIR, "extraPages.jsonl"),
+                        "--copy-pages",
+                    ]
+                ),
+                0,
+            )
+
+            with zipfile.ZipFile(
+                os.path.join(tmpdir, "example-collection-copy-pages.wacz"), "r"
+            ) as zip_ref:
+                zip_ref.extractall(os.path.join(tmpdir, "unzipped_copy_pages"))
+                zip_ref.close()
+
+            self.assertEqual(
+                main(
+                    [
+                        "validate",
+                        "-f",
+                        os.path.join(tmpdir, "example-collection-copy-pages.wacz"),
+                    ]
+                ),
+                0,
+            )
+
+            wacz_pages = os.path.join(tmpdir, "unzipped_copy_pages/pages/pages.jsonl")
+            wacz_extra_pages = os.path.join(
+                tmpdir, "unzipped_copy_pages/pages/extraPages.jsonl"
+            )
+
+            self.assertTrue(
+                "pages.jsonl"
+                in os.listdir(os.path.join(tmpdir, "unzipped_copy_pages/pages/"))
+            )
+            self.assertTrue(
+                "extraPages.jsonl"
+                in os.listdir(os.path.join(tmpdir, "unzipped_copy_pages/pages/"))
+            )
+
+            self.assertEqual(
+                hash_file("sha256", wacz_pages),
+                hash_file("sha256", os.path.join(PAGES_DIR, "pages.jsonl")),
+            )
+            self.assertEqual(
+                hash_file("sha256", wacz_extra_pages),
+                hash_file("sha256", os.path.join(PAGES_DIR, "extraPages.jsonl")),
+            )
+
+    @patch("wacz.main.now")
     def test_warc_with_detect_pages_flag(self, mock_now):
         """When passing the text index flag pages/pages.jsonl should be generated."""
         mock_now.return_value = (2020, 10, 7, 22, 29, 10)
         with tempfile.TemporaryDirectory() as tmpdir:
             self.assertEqual(
                 main(
                     [
```

### Comparing `wacz-0.4.9/tests/test_util.py` & `wacz-0.5.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/tests/test_validate_wacz.py` & `wacz-0.5.0/tests/test_validate_wacz.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/tests/test_verify_signed.py` & `wacz-0.5.0/tests/test_verify_signed.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/tests/test_wacz_indexer_functions.py` & `wacz-0.5.0/tests/test_wacz_indexer_functions.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/wacz/main.py` & `wacz-0.5.0/wacz/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser, RawTextHelpFormatter
 from io import BytesIO, StringIO, TextIOWrapper
 import os, json, datetime, shutil, zipfile, sys, gzip, pkg_resources
 from wacz.waczindexer import WACZIndexer
 from wacz.util import now, WACZ_VERSION, construct_passed_pages_dict
 from wacz.validate import Validation, OUTDATED_WACZ
-from wacz.util import validateJSON, get_py_wacz_version
+from wacz.util import validateJSON, get_py_wacz_version, validate_pages_jsonl_file
 from warcio.timeutils import iso_date_to_timestamp
 
 """
 WACZ Generator
 """
 
 PAGE_INDEX = "pages/pages.jsonl"
@@ -56,14 +56,21 @@
         "-d",
         "--detect-pages",
         help="Generates pages.jsonl without a text index",
         action="store_true",
     )
 
     create.add_argument(
+        "-c",
+        "--copy-pages",
+        help="Overrides the pages/extra-pages options by copying files to WACZ without parsing",
+        action="store_true",
+    )
+
+    create.add_argument(
         "--hash-type",
         choices=["sha256", "md5"],
         help="Allows the user to specify the hash type used. Currently we allow sha256 and md5",
     )
 
     create.add_argument(
         "-l",
@@ -125,36 +132,36 @@
     validate = Validation(
         res.file, verify_auth=res.verify_auth, verifier_url=res.verifier_url
     )
     version = validate.version
     validation_tests = []
 
     if version == OUTDATED_WACZ:
-        print("Validation Succeeded the passed Wacz is outdate but valid")
+        print("Validation succeeded, the passed WACZ is outdated but valid")
         return 0
 
     elif version == WACZ_VERSION:
         validation_tests += [
             validate.check_required_contents,
             validate.frictionless_validate,
             validate.check_file_paths,
             validate.check_file_hashes,
             validate.check_data_package_hash_and_sig,
         ]
     else:
-        print("Validation Failed the passed Wacz is invalid")
+        print("Validation failed, the passed WACZ is invalid")
         return 1
 
     for func in validation_tests:
         success = func()
         if success is False:
-            print("Validation Failed the passed Wacz is invalid")
+            print("Validation failed, the passed WACZ is invalid")
             return 1
 
-    print("Validation Succeeded the passed Wacz is valid")
+    print("Validation succeeded, the passed WACZ is valid")
     return 0
 
 
 def create_wacz(res):
     wacz = zipfile.ZipFile(res.output, "w")
 
     # write index
@@ -167,49 +174,73 @@
 
     text_wrap = TextIOWrapper(index_buff, "utf-8", write_through=True)
 
     wacz_indexer = None
 
     passed_pages_dict = {}
 
-    # If the flag for passed pages has been passed
+    # Handle pages
     if res.pages != None:
-        print("Validating passed pages.jsonl file")
-        passed_content = []
-        with open(res.pages, "rb") as fh:
-            for line in fh:
-                if not line:
-                    continue
-
-                try:
-                    line = line.decode("utf-8")
-                    passed_content.append(line)
-                except:
-                    print("Page data not utf-8 encoded, skipping", line)
+        if res.copy_pages:
+            print("Copying passed pages.jsonl file to WACZ")
+
+            if not validate_pages_jsonl_file(res.pages):
+                print("Unable to create WACZ without valid pages.jsonl file, quitting")
+                wacz.close()
+                return 1
+
+            with open(res.pages, "rb") as fh:
+                pages_jsonl = zipfile.ZipInfo("pages/pages.jsonl", now())
+                with wacz.open(pages_jsonl, "w") as pages_file:
+                    shutil.copyfileobj(fh, pages_file)
+
+        else:
+            print("Validating passed pages.jsonl file")
+            passed_content = []
+            with open(res.pages, "rb") as fh:
+                for line in fh:
+                    if not line:
+                        continue
+
+                    try:
+                        line = line.decode("utf-8")
+                        passed_content.append(line)
+                    except:
+                        print("Page data not utf-8 encoded, skipping", line)
 
-        # Create a dict of the passed pages that will be used in the construction of the index
-        passed_pages_dict = construct_passed_pages_dict(passed_content)
+            # Create a dict of the passed pages that will be used in the construction of the index
+            passed_pages_dict = construct_passed_pages_dict(passed_content)
 
     if res.extra_pages:
-        print("Validating extra pages file")
-        extra_page_data = []
-        with open(res.extra_pages) as fh:
-            data = fh.read()
-            for page_str in data.strip().split("\n"):
-                page_json = validateJSON(page_str)
-
-                if not page_json:
-                    print("Warning: Ignoring invalid extra page\n %s" % page_str)
-                    continue
-
-                extra_page_data.append(page_str.encode("utf-8"))
-
-        extra_pages_file = zipfile.ZipInfo(EXTRA_PAGES_INDEX, now())
-        with wacz.open(extra_pages_file, "w") as efh:
-            efh.write(b"\n".join(extra_page_data))
+        if res.copy_pages:
+            print("Copying passed extraPages.jsonl file to WACZ")
+            if validate_pages_jsonl_file(res.extra_pages):
+                extra_pages_jsonl = zipfile.ZipInfo("pages/extraPages.jsonl", now())
+                with open(res.extra_pages, "rb") as fh:
+                    with wacz.open(extra_pages_jsonl, "w") as extra_pages_file:
+                        shutil.copyfileobj(fh, extra_pages_file)
+            else:
+                print("Ignoring invalid extraPages.jsonl file")
+        else:
+            print("Validating extra pages file")
+            extra_page_data = []
+            with open(res.extra_pages) as fh:
+                data = fh.read()
+                for page_str in data.strip().split("\n"):
+                    page_json = validateJSON(page_str)
+
+                    if not page_json:
+                        print("Warning: Ignoring invalid extra page\n %s" % page_str)
+                        continue
+
+                    extra_page_data.append(page_str.encode("utf-8"))
+
+            extra_pages_file = zipfile.ZipInfo(EXTRA_PAGES_INDEX, now())
+            with wacz.open(extra_pages_file, "w") as efh:
+                efh.write(b"\n".join(extra_page_data))
 
     print("Reading and Indexing All WARCs")
     with wacz.open(data_file, "w") as data:
         wacz_indexer = WACZIndexer(
             text_wrap,
             res.inputs,
             sort=True,
@@ -263,29 +294,29 @@
                 log_path, "logs/{}".format(log_file)
             )
             with wacz.open(log_wacz_file, "w") as out_fh:
                 with open(log_path, "rb") as in_fh:
                     shutil.copyfileobj(in_fh, out_fh)
                     path = "logs/{}".format(log_file)
 
-    if len(wacz_indexer.pages) > 0 and res.pages == None:
+    if len(wacz_indexer.pages) > 0 and res.pages == None and not res.copy_pages:
         print("Generating page index...")
         # generate pages/text
         wacz_indexer.write_page_list(
             wacz,
             PAGE_INDEX,
             wacz_indexer.serialize_json_pages(
                 wacz_indexer.pages.values(),
                 id="pages",
                 title="Pages",
                 has_text=wacz_indexer.has_text,
             ),
         )
 
-    if len(wacz_indexer.pages) > 0 and res.pages != None:
+    if len(wacz_indexer.pages) > 0 and res.pages != None and not res.copy_pages:
         print("Generating page index from passed pages...")
         # Initially set the default value of the header id and title
         id_value = "pages"
         title_value = "Pages"
 
         # If the user has provided a title or an id in a header of their file we will use those instead of our default.
         try:
@@ -308,27 +339,27 @@
                 wacz_indexer.pages.values(),
                 id=id_value,
                 title=title_value,
                 has_text=wacz_indexer.has_text,
             ),
         )
 
-    if len(wacz_indexer.extra_pages) > 0:
+    if len(wacz_indexer.extra_pages) > 0 and not res.copy_pages:
         wacz_indexer.write_page_list(
             wacz,
             EXTRA_PAGES_INDEX,
             wacz_indexer.serialize_json_pages(
                 wacz_indexer.extra_pages.values(),
                 id="extra-pages",
                 title="Extra Pages",
                 has_text=wacz_indexer.has_text,
             ),
         )
 
-    if len(wacz_indexer.extra_page_lists) > 0:
+    if len(wacz_indexer.extra_page_lists) > 0 and not res.copy_pages:
         print("Generating extra page lists...")
 
         for name, pagelist in wacz_indexer.extra_page_lists.items():
             if name == "pages":
                 name = shortuuid.uuid()
             filename = PAGE_INDEX_TEMPLATE.format(name)
```

### Comparing `wacz-0.4.9/wacz/validate.py` & `wacz-0.5.0/wacz/validate.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/wacz/waczindexer.py` & `wacz-0.5.0/wacz/waczindexer.py`

 * *Files identical despite different names*

### Comparing `wacz-0.4.9/wacz.egg-info/PKG-INFO` & `wacz-0.5.0/wacz.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wacz
-Version: 0.4.9
+Version: 0.5.0
 Summary: WACZ Format Tools
 Home-page: https://github.com/webrecorder/py-wacz
 Author: Ilya Kreymer, Emma Dickson
 Author-email: info@webrecorder.net
 License: Apache 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -80,14 +80,30 @@
 
 Overrides the pages index generation with the passed jsonl pages.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl
 ```
 
+### -e --extra-pages
+
+Overrides the extra pages index generation with the passed extra jsonl pages.
+
+```
+wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl -e extra_pages.jsonl
+```
+
+### -c --copy-pages
+
+Overrides the behavior of --pages and --extra-pages options to copy existing pages.jsonl and/or extraPages.jsonl as-is directly into the WACZ rather than attempting to match each page to WARC record. The files are still parsed for basic correctness.
+
+```
+wacz create tests/fixtures/example-collection.warc --pages pages/pages.jsonl --extra-pages pages/extraPages.jsonl --copy-pages
+```
+
 ### -t --text
 
 You can add a full text index by including the --text tag.
 
 ```
 wacz create tests/fixtures/example-collection.warc -p passed_pages.jsonl --text
 ```
```

### Comparing `wacz-0.4.9/wacz.egg-info/SOURCES.txt` & `wacz-0.5.0/wacz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

