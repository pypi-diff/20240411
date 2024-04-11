# Comparing `tmp/dissect.fat-3.9.dev3.tar.gz` & `tmp/dissect.fat-3.9.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.fat-3.9.dev3.tar", last modified: Thu Mar 28 17:22:01 2024, max compression
+gzip compressed data, was "dissect.fat-3.9.dev4.tar", last modified: Thu Apr 11 11:56:49 2024, max compression
```

## Comparing `dissect.fat-3.9.dev3.tar` & `dissect.fat-3.9.dev4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:01.017264 dissect.fat-3.9.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-28 17:22:01.017264 dissect.fat-3.9.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:00.965264 dissect.fat-3.9.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:00.969264 dissect.fat-3.9.dev3/dissect/fat/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/dissect/fat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/dissect/fat/c_exfat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/dissect/fat/c_fat.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/dissect/fat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/dissect/fat/exfat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14545 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/dissect/fat/fat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:01.017264 dissect.fat-3.9.dev3/dissect.fat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-28 17:22:00.000000 dissect.fat-3.9.dev3/dissect.fat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-28 17:22:00.000000 dissect.fat-3.9.dev3/dissect.fat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:22:00.000000 dissect.fat-3.9.dev3/dissect.fat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:22:00.000000 dissect.fat-3.9.dev3/dissect.fat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:22:00.000000 dissect.fat-3.9.dev3/dissect.fat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-28 17:21:55.000000 dissect.fat-3.9.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:22:01.017264 dissect.fat-3.9.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:00.969264 dissect.fat-3.9.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:00.977264 dissect.fat-3.9.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-03-28 17:21:50.000000 dissect.fat-3.9.dev3/tests/data/exfat.bin
--rw-r--r--   0 runner    (1001) docker     (127)  1474560 2024-03-28 17:21:50.000000 dissect.fat-3.9.dev3/tests/data/fat12.bin
--rw-r--r--   0 runner    (1001) docker     (127)  3072000 2024-03-28 17:21:50.000000 dissect.fat-3.9.dev3/tests/data/fat16.bin
--rw-r--r--   0 runner    (1001) docker     (127) 34304000 2024-03-28 17:21:50.000000 dissect.fat-3.9.dev3/tests/data/fat32.bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:22:01.017264 dissect.fat-3.9.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/tests/test_exfat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/tests/test_fat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:21:49.000000 dissect.fat-3.9.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:49.983239 dissect.fat-3.9.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-11 11:56:49.983239 dissect.fat-3.9.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:49.931239 dissect.fat-3.9.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:49.935239 dissect.fat-3.9.dev4/dissect/fat/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/dissect/fat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/dissect/fat/c_exfat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/dissect/fat/c_fat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/dissect/fat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/dissect/fat/exfat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14545 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/dissect/fat/fat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:49.983239 dissect.fat-3.9.dev4/dissect.fat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-11 11:56:49.000000 dissect.fat-3.9.dev4/dissect.fat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-11 11:56:49.000000 dissect.fat-3.9.dev4/dissect.fat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:49.000000 dissect.fat-3.9.dev4/dissect.fat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 11:56:49.000000 dissect.fat-3.9.dev4/dissect.fat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:56:49.000000 dissect.fat-3.9.dev4/dissect.fat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-11 11:56:44.000000 dissect.fat-3.9.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:56:49.983239 dissect.fat-3.9.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:49.935239 dissect.fat-3.9.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:49.943239 dissect.fat-3.9.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1048576 2024-04-11 11:56:40.000000 dissect.fat-3.9.dev4/tests/data/exfat.bin
+-rw-r--r--   0 runner    (1001) docker     (127)  1474560 2024-04-11 11:56:40.000000 dissect.fat-3.9.dev4/tests/data/fat12.bin
+-rw-r--r--   0 runner    (1001) docker     (127)  3072000 2024-04-11 11:56:41.000000 dissect.fat-3.9.dev4/tests/data/fat16.bin
+-rw-r--r--   0 runner    (1001) docker     (127) 34304000 2024-04-11 11:56:41.000000 dissect.fat-3.9.dev4/tests/data/fat32.bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:49.983239 dissect.fat-3.9.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/tests/test_exfat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/tests/test_fat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-11 11:56:39.000000 dissect.fat-3.9.dev4/tox.ini
```

### Comparing `dissect.fat-3.9.dev3/LICENSE` & `dissect.fat-3.9.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/PKG-INFO` & `dissect.fat-3.9.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.fat
-Version: 3.9.dev3
+Version: 3.9.dev4
 Summary: A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage devices and UEFI partitions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.fat
 Project-URL: repository, https://github.com/fox-it/dissect.fat
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.fat-3.9.dev3/README.md` & `dissect.fat-3.9.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/dissect/fat/__init__.py` & `dissect.fat-3.9.dev4/dissect/fat/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/dissect/fat/c_exfat.py` & `dissect.fat-3.9.dev4/dissect/fat/c_exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/dissect/fat/c_fat.py` & `dissect.fat-3.9.dev4/dissect/fat/c_fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/dissect/fat/exfat.py` & `dissect.fat-3.9.dev4/dissect/fat/exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/dissect/fat/fat.py` & `dissect.fat-3.9.dev4/dissect/fat/fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/dissect.fat.egg-info/PKG-INFO` & `dissect.fat-3.9.dev4/dissect.fat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.fat
-Version: 3.9.dev3
+Version: 3.9.dev4
 Summary: A Dissect module implementing parsers for the FAT and exFAT file systems, commonly used on flash memory based storage devices and UEFI partitions
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.fat
 Project-URL: repository, https://github.com/fox-it/dissect.fat
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.fat-3.9.dev3/dissect.fat.egg-info/SOURCES.txt` & `dissect.fat-3.9.dev4/dissect.fat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/pyproject.toml` & `dissect.fat-3.9.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/conftest.py` & `dissect.fat-3.9.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/data/exfat.bin` & `dissect.fat-3.9.dev4/tests/data/exfat.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/data/fat12.bin` & `dissect.fat-3.9.dev4/tests/data/fat12.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/data/fat16.bin` & `dissect.fat-3.9.dev4/tests/data/fat16.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/data/fat32.bin` & `dissect.fat-3.9.dev4/tests/data/fat32.bin`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/docs/Makefile` & `dissect.fat-3.9.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/docs/conf.py` & `dissect.fat-3.9.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/test_exfat.py` & `dissect.fat-3.9.dev4/tests/test_exfat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tests/test_fat.py` & `dissect.fat-3.9.dev4/tests/test_fat.py`

 * *Files identical despite different names*

### Comparing `dissect.fat-3.9.dev3/tox.ini` & `dissect.fat-3.9.dev4/tox.ini`

 * *Files identical despite different names*

