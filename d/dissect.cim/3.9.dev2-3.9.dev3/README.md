# Comparing `tmp/dissect.cim-3.9.dev2.tar.gz` & `tmp/dissect.cim-3.9.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.cim-3.9.dev2.tar", last modified: Thu Mar 21 09:51:11 2024, max compression
+gzip compressed data, was "dissect.cim-3.9.dev3.tar", last modified: Thu Mar 28 17:21:38 2024, max compression
```

## Comparing `dissect.cim-3.9.dev2.tar` & `dissect.cim-3.9.dev3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:11.581042 dissect.cim-3.9.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-21 09:51:11.581042 dissect.cim-3.9.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:11.569042 dissect.cim-3.9.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:11.573042 dissect.cim-3.9.dev2/dissect/cim/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/c_cim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/cim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/dissect/cim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:11.581042 dissect.cim-3.9.dev2/dissect.cim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-21 09:51:11.000000 dissect.cim-3.9.dev2/dissect.cim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-21 09:51:11.000000 dissect.cim-3.9.dev2/dissect.cim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 09:51:11.000000 dissect.cim-3.9.dev2/dissect.cim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 09:51:11.000000 dissect.cim-3.9.dev2/dissect.cim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 09:51:11.000000 dissect.cim-3.9.dev2/dissect.cim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-21 09:51:06.000000 dissect.cim-3.9.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 09:51:11.581042 dissect.cim-3.9.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:11.573042 dissect.cim-3.9.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:11.577042 dissect.cim-3.9.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)  2018815 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/data/INDEX.BTR.gz
--rw-r--r--   0 runner    (1001) docker     (127)    29367 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/data/MAPPING1.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (127)    29375 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/data/MAPPING2.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (127)    29340 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/data/MAPPING3.MAP.gz
--rw-r--r--   0 runner    (1001) docker     (127)  4105816 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/data/OBJECTS.DATA.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:11.581042 dissect.cim-3.9.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tests/test_cim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-21 09:51:02.000000 dissect.cim-3.9.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:38.456201 dissect.cim-3.9.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-28 17:21:38.456201 dissect.cim-3.9.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:38.440201 dissect.cim-3.9.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:38.444201 dissect.cim-3.9.dev3/dissect/cim/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/c_cim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/cim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/dissect/cim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:38.456201 dissect.cim-3.9.dev3/dissect.cim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-28 17:21:38.000000 dissect.cim-3.9.dev3/dissect.cim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-28 17:21:38.000000 dissect.cim-3.9.dev3/dissect.cim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:38.000000 dissect.cim-3.9.dev3/dissect.cim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:21:38.000000 dissect.cim-3.9.dev3/dissect.cim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:21:38.000000 dissect.cim-3.9.dev3/dissect.cim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-28 17:21:32.000000 dissect.cim-3.9.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:21:38.456201 dissect.cim-3.9.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:38.444201 dissect.cim-3.9.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:38.448202 dissect.cim-3.9.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  2018815 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/data/INDEX.BTR.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    29367 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/data/MAPPING1.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    29375 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/data/MAPPING2.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    29340 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/data/MAPPING3.MAP.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  4105816 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/data/OBJECTS.DATA.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:38.456201 dissect.cim-3.9.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tests/test_cim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:21:26.000000 dissect.cim-3.9.dev3/tox.ini
```

### Comparing `dissect.cim-3.9.dev2/LICENSE` & `dissect.cim-3.9.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/PKG-INFO` & `dissect.cim-3.9.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cim
-Version: 3.9.dev2
+Version: 3.9.dev3
 Summary: A Dissect module implementing a parser for the Windows Common Information Model (CIM) database, used in the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cim
 Project-URL: repository, https://github.com/fox-it/dissect.cim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.cim-3.9.dev2/README.md` & `dissect.cim-3.9.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/dissect/cim/c_cim.py` & `dissect.cim-3.9.dev3/dissect/cim/c_cim.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/dissect/cim/cim.py` & `dissect.cim-3.9.dev3/dissect/cim/cim.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/dissect/cim/classes.py` & `dissect.cim-3.9.dev3/dissect/cim/classes.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/dissect/cim/index.py` & `dissect.cim-3.9.dev3/dissect/cim/index.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/dissect/cim/mappings.py` & `dissect.cim-3.9.dev3/dissect/cim/mappings.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/dissect/cim/objects.py` & `dissect.cim-3.9.dev3/dissect/cim/objects.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/dissect/cim/utils.py` & `dissect.cim-3.9.dev3/dissect/cim/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/dissect.cim.egg-info/PKG-INFO` & `dissect.cim-3.9.dev3/dissect.cim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cim
-Version: 3.9.dev2
+Version: 3.9.dev3
 Summary: A Dissect module implementing a parser for the Windows Common Information Model (CIM) database, used in the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cim
 Project-URL: repository, https://github.com/fox-it/dissect.cim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.cim-3.9.dev2/dissect.cim.egg-info/SOURCES.txt` & `dissect.cim-3.9.dev3/dissect.cim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/pyproject.toml` & `dissect.cim-3.9.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tests/conftest.py` & `dissect.cim-3.9.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tests/data/INDEX.BTR.gz` & `dissect.cim-3.9.dev3/tests/data/INDEX.BTR.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tests/data/MAPPING1.MAP.gz` & `dissect.cim-3.9.dev3/tests/data/MAPPING1.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tests/data/MAPPING2.MAP.gz` & `dissect.cim-3.9.dev3/tests/data/MAPPING2.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tests/data/MAPPING3.MAP.gz` & `dissect.cim-3.9.dev3/tests/data/MAPPING3.MAP.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tests/data/OBJECTS.DATA.gz` & `dissect.cim-3.9.dev3/tests/data/OBJECTS.DATA.gz`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tests/docs/Makefile` & `dissect.cim-3.9.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tests/docs/conf.py` & `dissect.cim-3.9.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.cim-3.9.dev2/tox.ini` & `dissect.cim-3.9.dev3/tox.ini`

 * *Files identical despite different names*

