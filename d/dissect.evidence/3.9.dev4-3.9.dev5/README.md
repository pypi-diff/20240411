# Comparing `tmp/dissect.evidence-3.9.dev4.tar.gz` & `tmp/dissect.evidence-3.9.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.evidence-3.9.dev4.tar", last modified: Wed Apr 10 11:03:52 2024, max compression
+gzip compressed data, was "dissect.evidence-3.9.dev5.tar", last modified: Thu Apr 11 11:56:38 2024, max compression
```

## Comparing `dissect.evidence-3.9.dev4.tar` & `dissect.evidence-3.9.dev5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.922215 dissect.evidence-3.9.dev4/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/dissect/evidence/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/ad1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/dissect/evidence/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/asdf/asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/asdf/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/ewf.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/dissect/evidence/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/dd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 11:03:52.000000 dissect.evidence-3.9.dev4/dissect.evidence.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-10 11:03:47.000000 dissect.evidence-3.9.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.926215 dissect.evidence-3.9.dev4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/data/ad1_long.ad1
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/data/ad1_test.ad1
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/data/ad1_test_compressed.ad1
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/data/ewf.E01
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:03:52.930215 dissect.evidence-3.9.dev4/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/test_ad1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/test_asdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tests/test_ewf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-10 11:03:39.000000 dissect.evidence-3.9.dev4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.129412 dissect.evidence-3.9.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-11 11:56:38.129412 dissect.evidence-3.9.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.121412 dissect.evidence-3.9.dev5/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.125412 dissect.evidence-3.9.dev5/dissect/evidence/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/ad1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.125412 dissect.evidence-3.9.dev5/dissect/evidence/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/asdf/asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/asdf/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/ewf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.125412 dissect.evidence-3.9.dev5/dissect/evidence/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.125412 dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/dd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.129412 dissect.evidence-3.9.dev5/dissect.evidence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-11 11:56:38.000000 dissect.evidence-3.9.dev5/dissect.evidence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-11 11:56:38.000000 dissect.evidence-3.9.dev5/dissect.evidence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:38.000000 dissect.evidence-3.9.dev5/dissect.evidence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-11 11:56:38.000000 dissect.evidence-3.9.dev5/dissect.evidence.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:56:38.000000 dissect.evidence-3.9.dev5/dissect.evidence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:56:38.000000 dissect.evidence-3.9.dev5/dissect.evidence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-11 11:56:33.000000 dissect.evidence-3.9.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:56:38.129412 dissect.evidence-3.9.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.129412 dissect.evidence-3.9.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.129412 dissect.evidence-3.9.dev5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/data/ad1_long.ad1
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/data/ad1_test.ad1
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/data/ad1_test_compressed.ad1
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/data/ewf.E01
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:38.129412 dissect.evidence-3.9.dev5/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/test_ad1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/test_asdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tests/test_ewf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-11 11:56:29.000000 dissect.evidence-3.9.dev5/tox.ini
```

### Comparing `dissect.evidence-3.9.dev4/LICENSE` & `dissect.evidence-3.9.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/PKG-INFO` & `dissect.evidence-3.9.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.evidence
-Version: 3.9.dev4
+Version: 3.9.dev5
 Summary: A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.evidence
 Project-URL: repository, https://github.com/fox-it/dissect.evidence
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.evidence-3.9.dev4/README.md` & `dissect.evidence-3.9.dev5/README.md`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/ad1.py` & `dissect.evidence-3.9.dev5/dissect/evidence/ad1.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/asdf/asdf.py` & `dissect.evidence-3.9.dev5/dissect/evidence/asdf/asdf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/asdf/streams.py` & `dissect.evidence-3.9.dev5/dissect/evidence/asdf/streams.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/ewf.py` & `dissect.evidence-3.9.dev5/dissect/evidence/ewf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/exceptions.py` & `dissect.evidence-3.9.dev5/dissect/evidence/exceptions.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/dd.py` & `dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/dd.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/meta.py` & `dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/meta.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/repair.py` & `dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/repair.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect/evidence/tools/asdf/verify.py` & `dissect.evidence-3.9.dev5/dissect/evidence/tools/asdf/verify.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/dissect.evidence.egg-info/PKG-INFO` & `dissect.evidence-3.9.dev5/dissect.evidence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.evidence
-Version: 3.9.dev4
+Version: 3.9.dev5
 Summary: A Dissect module implementing a parsers for various forensic evidence file containers, currently: AD1, ASDF and EWF
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.evidence
 Project-URL: repository, https://github.com/fox-it/dissect.evidence
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.evidence-3.9.dev4/dissect.evidence.egg-info/SOURCES.txt` & `dissect.evidence-3.9.dev5/dissect.evidence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/pyproject.toml` & `dissect.evidence-3.9.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/conftest.py` & `dissect.evidence-3.9.dev5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/data/ad1_long.ad1` & `dissect.evidence-3.9.dev5/tests/data/ad1_long.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/data/ad1_test.ad1` & `dissect.evidence-3.9.dev5/tests/data/ad1_test.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/data/ad1_test_compressed.ad1` & `dissect.evidence-3.9.dev5/tests/data/ad1_test_compressed.ad1`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/data/ewf.E01` & `dissect.evidence-3.9.dev5/tests/data/ewf.E01`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/docs/Makefile` & `dissect.evidence-3.9.dev5/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/docs/conf.py` & `dissect.evidence-3.9.dev5/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/test_ad1.py` & `dissect.evidence-3.9.dev5/tests/test_ad1.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/test_asdf.py` & `dissect.evidence-3.9.dev5/tests/test_asdf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tests/test_ewf.py` & `dissect.evidence-3.9.dev5/tests/test_ewf.py`

 * *Files identical despite different names*

### Comparing `dissect.evidence-3.9.dev4/tox.ini` & `dissect.evidence-3.9.dev5/tox.ini`

 * *Files identical despite different names*

