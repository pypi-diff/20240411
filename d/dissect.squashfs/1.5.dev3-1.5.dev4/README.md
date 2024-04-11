# Comparing `tmp/dissect.squashfs-1.5.dev3.tar.gz` & `tmp/dissect.squashfs-1.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.squashfs-1.5.dev3.tar", last modified: Thu Mar 28 17:23:18 2024, max compression
+gzip compressed data, was "dissect.squashfs-1.5.dev4.tar", last modified: Thu Apr 11 11:57:57 2024, max compression
```

## Comparing `dissect.squashfs-1.5.dev3.tar` & `dissect.squashfs-1.5.dev4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:23:18.518959 dissect.squashfs-1.5.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-03-28 17:23:18.514959 dissect.squashfs-1.5.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:23:18.510959 dissect.squashfs-1.5.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:23:18.510959 dissect.squashfs-1.5.dev3/dissect/squashfs/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/dissect/squashfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/dissect/squashfs/c_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/dissect/squashfs/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/dissect/squashfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/dissect/squashfs/squashfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:23:18.514959 dissect.squashfs-1.5.dev3/dissect.squashfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-03-28 17:23:18.000000 dissect.squashfs-1.5.dev3/dissect.squashfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-28 17:23:18.000000 dissect.squashfs-1.5.dev3/dissect.squashfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:23:18.000000 dissect.squashfs-1.5.dev3/dissect.squashfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 17:23:18.000000 dissect.squashfs-1.5.dev3/dissect.squashfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:23:18.000000 dissect.squashfs-1.5.dev3/dissect.squashfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-28 17:23:12.000000 dissect.squashfs-1.5.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:23:18.518959 dissect.squashfs-1.5.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:23:18.514959 dissect.squashfs-1.5.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:23:18.514959 dissect.squashfs-1.5.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/data/gzip-opts.sqfs
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/data/gzip.sqfs
--rw-r--r--   0 runner    (1001) docker     (127)    24576 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/data/lz4.sqfs
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/data/lzma.sqfs
--rw-r--r--   0 runner    (1001) docker     (127)    28672 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/data/lzo.sqfs
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/data/xz.sqfs
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/data/zstd.sqfs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:23:18.514959 dissect.squashfs-1.5.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tests/test_squashfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-28 17:23:03.000000 dissect.squashfs-1.5.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:57.861802 dissect.squashfs-1.5.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-11 11:57:57.861802 dissect.squashfs-1.5.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:57.853802 dissect.squashfs-1.5.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:57.857802 dissect.squashfs-1.5.dev4/dissect/squashfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/dissect/squashfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/dissect/squashfs/c_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/dissect/squashfs/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/dissect/squashfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15504 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/dissect/squashfs/squashfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:57.861802 dissect.squashfs-1.5.dev4/dissect.squashfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-11 11:57:57.000000 dissect.squashfs-1.5.dev4/dissect.squashfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-11 11:57:57.000000 dissect.squashfs-1.5.dev4/dissect.squashfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:57:57.000000 dissect.squashfs-1.5.dev4/dissect.squashfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 11:57:57.000000 dissect.squashfs-1.5.dev4/dissect.squashfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:57:57.000000 dissect.squashfs-1.5.dev4/dissect.squashfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-11 11:57:52.000000 dissect.squashfs-1.5.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:57:57.861802 dissect.squashfs-1.5.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:57.857802 dissect.squashfs-1.5.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:57.861802 dissect.squashfs-1.5.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/data/gzip-opts.sqfs
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/data/gzip.sqfs
+-rw-r--r--   0 runner    (1001) docker     (127)    24576 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/data/lz4.sqfs
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/data/lzma.sqfs
+-rw-r--r--   0 runner    (1001) docker     (127)    28672 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/data/lzo.sqfs
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/data/xz.sqfs
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/data/zstd.sqfs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:57:57.861802 dissect.squashfs-1.5.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tests/test_squashfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-11 11:57:42.000000 dissect.squashfs-1.5.dev4/tox.ini
```

### Comparing `dissect.squashfs-1.5.dev3/LICENSE` & `dissect.squashfs-1.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/PKG-INFO` & `dissect.squashfs-1.5.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.5.dev3
+Version: 1.5.dev4
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.squashfs-1.5.dev3/README.md` & `dissect.squashfs-1.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/dissect/squashfs/c_squashfs.py` & `dissect.squashfs-1.5.dev4/dissect/squashfs/c_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/dissect/squashfs/compression.py` & `dissect.squashfs-1.5.dev4/dissect/squashfs/compression.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/dissect/squashfs/squashfs.py` & `dissect.squashfs-1.5.dev4/dissect/squashfs/squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/dissect.squashfs.egg-info/PKG-INFO` & `dissect.squashfs-1.5.dev4/dissect.squashfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.squashfs
-Version: 1.5.dev3
+Version: 1.5.dev4
 Summary: A Dissect module implementing a parser for the SquashFS file system, commonly used in appliance or device firmware
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.squashfs
 Project-URL: repository, https://github.com/fox-it/dissect.squashfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.squashfs-1.5.dev3/dissect.squashfs.egg-info/SOURCES.txt` & `dissect.squashfs-1.5.dev4/dissect.squashfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/pyproject.toml` & `dissect.squashfs-1.5.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/conftest.py` & `dissect.squashfs-1.5.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/data/gzip-opts.sqfs` & `dissect.squashfs-1.5.dev4/tests/data/gzip-opts.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/data/gzip.sqfs` & `dissect.squashfs-1.5.dev4/tests/data/gzip.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/data/lz4.sqfs` & `dissect.squashfs-1.5.dev4/tests/data/lz4.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/data/lzma.sqfs` & `dissect.squashfs-1.5.dev4/tests/data/lzma.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/data/lzo.sqfs` & `dissect.squashfs-1.5.dev4/tests/data/lzo.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/data/xz.sqfs` & `dissect.squashfs-1.5.dev4/tests/data/xz.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/data/zstd.sqfs` & `dissect.squashfs-1.5.dev4/tests/data/zstd.sqfs`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/docs/Makefile` & `dissect.squashfs-1.5.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/docs/conf.py` & `dissect.squashfs-1.5.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tests/test_squashfs.py` & `dissect.squashfs-1.5.dev4/tests/test_squashfs.py`

 * *Files identical despite different names*

### Comparing `dissect.squashfs-1.5.dev3/tox.ini` & `dissect.squashfs-1.5.dev4/tox.ini`

 * *Files identical despite different names*

