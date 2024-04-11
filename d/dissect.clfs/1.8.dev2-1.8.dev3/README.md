# Comparing `tmp/dissect.clfs-1.8.dev2.tar.gz` & `tmp/dissect.clfs-1.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.clfs-1.8.dev2.tar", last modified: Thu Mar 21 09:51:18 2024, max compression
+gzip compressed data, was "dissect.clfs-1.8.dev3.tar", last modified: Thu Mar 28 17:21:43 2024, max compression
```

## Comparing `dissect.clfs-1.8.dev2.tar` & `dissect.clfs-1.8.dev3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:18.379341 dissect.clfs-1.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-21 09:51:18.379341 dissect.clfs-1.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:18.371341 dissect.clfs-1.8.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:18.375341 dissect.clfs-1.8.dev2/dissect/clfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/dissect/clfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/dissect/clfs/blf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/dissect/clfs/c_clfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/dissect/clfs/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/dissect/clfs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:18.379341 dissect.clfs-1.8.dev2/dissect.clfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-21 09:51:18.000000 dissect.clfs-1.8.dev2/dissect.clfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-21 09:51:18.000000 dissect.clfs-1.8.dev2/dissect.clfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 09:51:18.000000 dissect.clfs-1.8.dev2/dissect.clfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-21 09:51:18.000000 dissect.clfs-1.8.dev2/dissect.clfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 09:51:18.000000 dissect.clfs-1.8.dev2/dissect.clfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-21 09:51:13.000000 dissect.clfs-1.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 09:51:18.379341 dissect.clfs-1.8.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:18.375341 dissect.clfs-1.8.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:18.375341 dissect.clfs-1.8.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    65536 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf
--rw-r--r--   0 runner    (1001) docker     (127)   524288 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/data/bad_control_record.blf
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/data/control_record.blf
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/data/invalid_control_record.blf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:51:18.379341 dissect.clfs-1.8.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/test_control_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/test_record_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tests/test_validate_blf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-21 09:51:10.000000 dissect.clfs-1.8.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.031082 dissect.clfs-1.8.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-28 17:21:43.031082 dissect.clfs-1.8.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.023083 dissect.clfs-1.8.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.027083 dissect.clfs-1.8.dev3/dissect/clfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/dissect/clfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/dissect/clfs/blf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/dissect/clfs/c_clfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/dissect/clfs/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/dissect/clfs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.031082 dissect.clfs-1.8.dev3/dissect.clfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-28 17:21:42.000000 dissect.clfs-1.8.dev3/dissect.clfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-28 17:21:43.000000 dissect.clfs-1.8.dev3/dissect.clfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:42.000000 dissect.clfs-1.8.dev3/dissect.clfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 17:21:42.000000 dissect.clfs-1.8.dev3/dissect.clfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:21:42.000000 dissect.clfs-1.8.dev3/dissect.clfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-28 17:21:37.000000 dissect.clfs-1.8.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:21:43.031082 dissect.clfs-1.8.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.027083 dissect.clfs-1.8.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.031082 dissect.clfs-1.8.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    65536 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf
+-rw-r--r--   0 runner    (1001) docker     (127)   524288 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/data/bad_control_record.blf
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/data/control_record.blf
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/data/invalid_control_record.blf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:43.031082 dissect.clfs-1.8.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/test_control_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/test_record_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tests/test_validate_blf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:21:29.000000 dissect.clfs-1.8.dev3/tox.ini
```

### Comparing `dissect.clfs-1.8.dev2/LICENSE` & `dissect.clfs-1.8.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/PKG-INFO` & `dissect.clfs-1.8.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.clfs
-Version: 1.8.dev2
+Version: 1.8.dev3
 Summary: A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.clfs
 Project-URL: repository, https://github.com/fox-it/dissect.clfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.clfs-1.8.dev2/README.md` & `dissect.clfs-1.8.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/dissect/clfs/blf.py` & `dissect.clfs-1.8.dev3/dissect/clfs/blf.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/dissect/clfs/c_clfs.py` & `dissect.clfs-1.8.dev3/dissect/clfs/c_clfs.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/dissect/clfs/container.py` & `dissect.clfs-1.8.dev3/dissect/clfs/container.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/dissect.clfs.egg-info/PKG-INFO` & `dissect.clfs-1.8.dev3/dissect.clfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.clfs
-Version: 1.8.dev2
+Version: 1.8.dev3
 Summary: A Dissect module implementing a parser for the CLFS (Common Log File System) file system of Windows
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.clfs
 Project-URL: repository, https://github.com/fox-it/dissect.clfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.clfs-1.8.dev2/dissect.clfs.egg-info/SOURCES.txt` & `dissect.clfs-1.8.dev3/dissect.clfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/pyproject.toml` & `dissect.clfs-1.8.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/conftest.py` & `dissect.clfs-1.8.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf` & `dissect.clfs-1.8.dev3/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TM.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms` & `dissect.clfs-1.8.dev3/tests/data/DRIVERS{53b39e70-18c4-11ea-a811-000d3aa4692b}.TMContainer00000000000000000001.regtrans-ms`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/data/bad_control_record.blf` & `dissect.clfs-1.8.dev3/tests/data/bad_control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/data/control_record.blf` & `dissect.clfs-1.8.dev3/tests/data/control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/data/invalid_control_record.blf` & `dissect.clfs-1.8.dev3/tests/data/invalid_control_record.blf`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/docs/Makefile` & `dissect.clfs-1.8.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/docs/conf.py` & `dissect.clfs-1.8.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/test_container.py` & `dissect.clfs-1.8.dev3/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/test_control_record.py` & `dissect.clfs-1.8.dev3/tests/test_control_record.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tests/test_record_header.py` & `dissect.clfs-1.8.dev3/tests/test_record_header.py`

 * *Files identical despite different names*

### Comparing `dissect.clfs-1.8.dev2/tox.ini` & `dissect.clfs-1.8.dev3/tox.ini`

 * *Files identical despite different names*

