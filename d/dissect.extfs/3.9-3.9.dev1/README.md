# Comparing `tmp/dissect.extfs-3.9.tar.gz` & `tmp/dissect.extfs-3.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.extfs-3.9.tar", last modified: Thu Mar  7 15:18:49 2024, max compression
+gzip compressed data, was "dissect.extfs-3.9.dev1.tar", last modified: Wed Jan 31 14:23:09 2024, max compression
```

## Comparing `dissect.extfs-3.9.tar` & `dissect.extfs-3.9.dev1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:18:49.051159 dissect.extfs-3.9/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-07 15:18:39.000000 dissect.extfs-3.9/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-07 15:18:39.000000 dissect.extfs-3.9/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-07 15:18:39.000000 dissect.extfs-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-07 15:18:39.000000 dissect.extfs-3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-07 15:18:49.047159 dissect.extfs-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-07 15:18:39.000000 dissect.extfs-3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:18:49.043159 dissect.extfs-3.9/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:18:49.047159 dissect.extfs-3.9/dissect/extfs/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-07 15:18:39.000000 dissect.extfs-3.9/dissect/extfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23393 2024-03-07 15:18:39.000000 dissect.extfs-3.9/dissect/extfs/c_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-07 15:18:39.000000 dissect.extfs-3.9/dissect/extfs/c_jdb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-07 15:18:39.000000 dissect.extfs-3.9/dissect/extfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19254 2024-03-07 15:18:39.000000 dissect.extfs-3.9/dissect/extfs/extfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-03-07 15:18:39.000000 dissect.extfs-3.9/dissect/extfs/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:18:49.047159 dissect.extfs-3.9/dissect.extfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-07 15:18:48.000000 dissect.extfs-3.9/dissect.extfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-07 15:18:49.000000 dissect.extfs-3.9/dissect.extfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 15:18:48.000000 dissect.extfs-3.9/dissect.extfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-07 15:18:48.000000 dissect.extfs-3.9/dissect.extfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-07 15:18:48.000000 dissect.extfs-3.9/dissect.extfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-07 15:18:39.000000 dissect.extfs-3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 15:18:49.051159 dissect.extfs-3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:18:49.047159 dissect.extfs-3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:18:49.047159 dissect.extfs-3.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/data/ext4.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/data/ext4_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/data/ext4_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/data/ext4_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/data/ext4_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 15:18:49.047159 dissect.extfs-3.9/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tests/test_ext4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-07 15:18:39.000000 dissect.extfs-3.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:09.073319 dissect.extfs-3.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-01-31 14:23:09.073319 dissect.extfs-3.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:09.069319 dissect.extfs-3.9.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:09.073319 dissect.extfs-3.9.dev1/dissect/extfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/dissect/extfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23393 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/dissect/extfs/c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/dissect/extfs/c_jdb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/dissect/extfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19254 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/dissect/extfs/extfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/dissect/extfs/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:09.073319 dissect.extfs-3.9.dev1/dissect.extfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-01-31 14:23:09.000000 dissect.extfs-3.9.dev1/dissect.extfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-01-31 14:23:09.000000 dissect.extfs-3.9.dev1/dissect.extfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 14:23:09.000000 dissect.extfs-3.9.dev1/dissect.extfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-31 14:23:09.000000 dissect.extfs-3.9.dev1/dissect.extfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-31 14:23:09.000000 dissect.extfs-3.9.dev1/dissect.extfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-31 14:23:00.000000 dissect.extfs-3.9.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 14:23:09.073319 dissect.extfs-3.9.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:09.073319 dissect.extfs-3.9.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:09.073319 dissect.extfs-3.9.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/data/ext4.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/data/ext4_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/data/ext4_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/data/ext4_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/data/ext4_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:09.073319 dissect.extfs-3.9.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tests/test_ext4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-31 14:22:55.000000 dissect.extfs-3.9.dev1/tox.ini
```

### Comparing `dissect.extfs-3.9/LICENSE` & `dissect.extfs-3.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/PKG-INFO` & `dissect.extfs-3.9.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.9
+Version: 3.9.dev1
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.extfs-3.9/README.md` & `dissect.extfs-3.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/dissect/extfs/c_ext.py` & `dissect.extfs-3.9.dev1/dissect/extfs/c_ext.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/dissect/extfs/c_jdb2.py` & `dissect.extfs-3.9.dev1/dissect/extfs/c_jdb2.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/dissect/extfs/extfs.py` & `dissect.extfs-3.9.dev1/dissect/extfs/extfs.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/dissect/extfs/journal.py` & `dissect.extfs-3.9.dev1/dissect/extfs/journal.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/dissect.extfs.egg-info/PKG-INFO` & `dissect.extfs-3.9.dev1/dissect.extfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.extfs
-Version: 3.9
+Version: 3.9.dev1
 Summary: A Dissect module implementing a parser for the ExtFS file system, the native filesystem for Linux operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.extfs
 Project-URL: repository, https://github.com/fox-it/dissect.extfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.extfs-3.9/dissect.extfs.egg-info/SOURCES.txt` & `dissect.extfs-3.9.dev1/dissect.extfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/pyproject.toml` & `dissect.extfs-3.9.dev1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -46,7 +46,8 @@
 [tool.setuptools]
 license-files = ["LICENSE", "COPYRIGHT"]
 
 [tool.setuptools.packages.find]
 include = ["dissect.*"]
 
 [tool.setuptools_scm]
+local_scheme = "no-local-version"
```

### Comparing `dissect.extfs-3.9/tests/conftest.py` & `dissect.extfs-3.9.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tests/data/ext4.bin.gz` & `dissect.extfs-3.9.dev1/tests/data/ext4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tests/data/ext4_sparse.bin.gz` & `dissect.extfs-3.9.dev1/tests/data/ext4_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tests/data/ext4_symlink_test1.bin.gz` & `dissect.extfs-3.9.dev1/tests/data/ext4_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tests/data/ext4_symlink_test2.bin.gz` & `dissect.extfs-3.9.dev1/tests/data/ext4_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tests/data/ext4_symlink_test3.bin.gz` & `dissect.extfs-3.9.dev1/tests/data/ext4_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tests/docs/Makefile` & `dissect.extfs-3.9.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tests/docs/conf.py` & `dissect.extfs-3.9.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tests/test_ext4.py` & `dissect.extfs-3.9.dev1/tests/test_ext4.py`

 * *Files identical despite different names*

### Comparing `dissect.extfs-3.9/tox.ini` & `dissect.extfs-3.9.dev1/tox.ini`

 * *Files identical despite different names*

