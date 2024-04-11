# Comparing `tmp/dissect.xfs-3.9.dev2.tar.gz` & `tmp/dissect.xfs-3.9.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.xfs-3.9.dev2.tar", last modified: Thu Mar 21 10:20:47 2024, max compression
+gzip compressed data, was "dissect.xfs-3.9.dev3.tar", last modified: Thu Mar 28 17:25:16 2024, max compression
```

## Comparing `dissect.xfs-3.9.dev2.tar` & `dissect.xfs-3.9.dev3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:20:47.718561 dissect.xfs-3.9.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-21 10:20:47.718561 dissect.xfs-3.9.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:20:47.710561 dissect.xfs-3.9.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:20:47.714561 dissect.xfs-3.9.dev2/dissect/xfs/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/dissect/xfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41820 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/dissect/xfs/c_xfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/dissect/xfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22085 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/dissect/xfs/xfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:20:47.718561 dissect.xfs-3.9.dev2/dissect.xfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-21 10:20:47.000000 dissect.xfs-3.9.dev2/dissect.xfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-21 10:20:47.000000 dissect.xfs-3.9.dev2/dissect.xfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:20:47.000000 dissect.xfs-3.9.dev2/dissect.xfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 10:20:47.000000 dissect.xfs-3.9.dev2/dissect.xfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 10:20:47.000000 dissect.xfs-3.9.dev2/dissect.xfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-21 10:20:41.000000 dissect.xfs-3.9.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:20:47.718561 dissect.xfs-3.9.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:20:47.718561 dissect.xfs-3.9.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:20:47.718561 dissect.xfs-3.9.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    41799 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/data/xfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42673 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/data/xfs_bigtime.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    45520 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/data/xfs_sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42284 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/data/xfs_symlink_test1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    42015 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/data/xfs_symlink_test2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)    41936 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/data/xfs_symlink_test3.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:20:47.718561 dissect.xfs-3.9.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tests/test_xfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-21 10:20:33.000000 dissect.xfs-3.9.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:25:16.540034 dissect.xfs-3.9.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-28 17:25:16.540034 dissect.xfs-3.9.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:25:16.532034 dissect.xfs-3.9.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:25:16.536034 dissect.xfs-3.9.dev3/dissect/xfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/dissect/xfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41820 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/dissect/xfs/c_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/dissect/xfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22085 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/dissect/xfs/xfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:25:16.540034 dissect.xfs-3.9.dev3/dissect.xfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-28 17:25:16.000000 dissect.xfs-3.9.dev3/dissect.xfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-28 17:25:16.000000 dissect.xfs-3.9.dev3/dissect.xfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:25:16.000000 dissect.xfs-3.9.dev3/dissect.xfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:25:16.000000 dissect.xfs-3.9.dev3/dissect.xfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:25:16.000000 dissect.xfs-3.9.dev3/dissect.xfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-28 17:25:11.000000 dissect.xfs-3.9.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:25:16.540034 dissect.xfs-3.9.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:25:16.536034 dissect.xfs-3.9.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:25:16.536034 dissect.xfs-3.9.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    41799 2024-03-28 17:25:08.000000 dissect.xfs-3.9.dev3/tests/data/xfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42673 2024-03-28 17:25:08.000000 dissect.xfs-3.9.dev3/tests/data/xfs_bigtime.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    45520 2024-03-28 17:25:08.000000 dissect.xfs-3.9.dev3/tests/data/xfs_sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42284 2024-03-28 17:25:08.000000 dissect.xfs-3.9.dev3/tests/data/xfs_symlink_test1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    42015 2024-03-28 17:25:08.000000 dissect.xfs-3.9.dev3/tests/data/xfs_symlink_test2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    41936 2024-03-28 17:25:08.000000 dissect.xfs-3.9.dev3/tests/data/xfs_symlink_test3.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:25:16.540034 dissect.xfs-3.9.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/tests/test_xfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:25:07.000000 dissect.xfs-3.9.dev3/tox.ini
```

### Comparing `dissect.xfs-3.9.dev2/LICENSE` & `dissect.xfs-3.9.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/PKG-INFO` & `dissect.xfs-3.9.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.9.dev2
+Version: 3.9.dev3
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.xfs-3.9.dev2/README.md` & `dissect.xfs-3.9.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/dissect/xfs/c_xfs.py` & `dissect.xfs-3.9.dev3/dissect/xfs/c_xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/dissect/xfs/xfs.py` & `dissect.xfs-3.9.dev3/dissect/xfs/xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/dissect.xfs.egg-info/PKG-INFO` & `dissect.xfs-3.9.dev3/dissect.xfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.xfs
-Version: 3.9.dev2
+Version: 3.9.dev3
 Summary: A Dissect module implementing a parser for the XFS file system, commonly used by RedHat Linux distributions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.xfs
 Project-URL: repository, https://github.com/fox-it/dissect.xfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.xfs-3.9.dev2/dissect.xfs.egg-info/SOURCES.txt` & `dissect.xfs-3.9.dev3/dissect.xfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/pyproject.toml` & `dissect.xfs-3.9.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/data/xfs.bin.gz` & `dissect.xfs-3.9.dev3/tests/data/xfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/data/xfs_bigtime.bin.gz` & `dissect.xfs-3.9.dev3/tests/data/xfs_bigtime.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/data/xfs_sparse.bin.gz` & `dissect.xfs-3.9.dev3/tests/data/xfs_sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/data/xfs_symlink_test1.bin.gz` & `dissect.xfs-3.9.dev3/tests/data/xfs_symlink_test1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/data/xfs_symlink_test2.bin.gz` & `dissect.xfs-3.9.dev3/tests/data/xfs_symlink_test2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/data/xfs_symlink_test3.bin.gz` & `dissect.xfs-3.9.dev3/tests/data/xfs_symlink_test3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/docs/Makefile` & `dissect.xfs-3.9.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/docs/conf.py` & `dissect.xfs-3.9.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tests/test_xfs.py` & `dissect.xfs-3.9.dev3/tests/test_xfs.py`

 * *Files identical despite different names*

### Comparing `dissect.xfs-3.9.dev2/tox.ini` & `dissect.xfs-3.9.dev3/tox.ini`

 * *Files identical despite different names*

