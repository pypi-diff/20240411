# Comparing `tmp/dissect.btrfs-1.3.dev3.tar.gz` & `tmp/dissect.btrfs-1.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.btrfs-1.3.dev3.tar", last modified: Thu Mar 28 17:21:37 2024, max compression
+gzip compressed data, was "dissect.btrfs-1.3.dev4.tar", last modified: Thu Apr 11 11:56:22 2024, max compression
```

## Comparing `dissect.btrfs-1.3.dev3.tar` & `dissect.btrfs-1.3.dev4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:37.043482 dissect.btrfs-1.3.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-28 17:21:37.043482 dissect.btrfs-1.3.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:37.027482 dissect.btrfs-1.3.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:37.031482 dissect.btrfs-1.3.dev3/dissect/btrfs/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/dissect/btrfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/dissect/btrfs/btrfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27165 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/dissect/btrfs/c_btrfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/dissect/btrfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/dissect/btrfs/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/dissect/btrfs/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:37.043482 dissect.btrfs-1.3.dev3/dissect.btrfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-28 17:21:36.000000 dissect.btrfs-1.3.dev3/dissect.btrfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-28 17:21:37.000000 dissect.btrfs-1.3.dev3/dissect.btrfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:36.000000 dissect.btrfs-1.3.dev3/dissect.btrfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-28 17:21:36.000000 dissect.btrfs-1.3.dev3/dissect.btrfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:21:36.000000 dissect.btrfs-1.3.dev3/dissect.btrfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-28 17:21:32.000000 dissect.btrfs-1.3.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:21:37.043482 dissect.btrfs-1.3.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:37.031482 dissect.btrfs-1.3.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-28 17:21:26.000000 dissect.btrfs-1.3.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:37.043482 dissect.btrfs-1.3.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   239072 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-compression.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   155198 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-default.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   295784 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-dup-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   302851 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-dup-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   152549 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid0-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   148657 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid0-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   153538 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   151299 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   153589 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid10-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   151358 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid10-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   155315 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c3-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   153018 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c3-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   153018 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c3-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   153982 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c4-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   151612 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c4-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   151610 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c4-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   151614 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c4-4.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   153585 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid5-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   151362 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid5-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   153791 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid6-1.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   151501 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid6-2.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   151499 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-raid6-3.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   174289 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-sparse.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   170186 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-subvolume-custom-default.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   166940 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-subvolume-nested.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   177966 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-subvolume-snapshot.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   170958 2024-03-28 17:21:28.000000 dissect.btrfs-1.3.dev3/tests/data/btrfs-subvolume.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-03-28 17:21:27.000000 dissect.btrfs-1.3.dev3/tests/test_btrfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-28 17:21:27.000000 dissect.btrfs-1.3.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:22.724038 dissect.btrfs-1.3.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-11 11:56:22.724038 dissect.btrfs-1.3.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:22.708038 dissect.btrfs-1.3.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:22.712038 dissect.btrfs-1.3.dev4/dissect/btrfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/dissect/btrfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/dissect/btrfs/btrfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27165 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/dissect/btrfs/c_btrfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/dissect/btrfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/dissect/btrfs/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/dissect/btrfs/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:22.724038 dissect.btrfs-1.3.dev4/dissect.btrfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-11 11:56:22.000000 dissect.btrfs-1.3.dev4/dissect.btrfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-11 11:56:22.000000 dissect.btrfs-1.3.dev4/dissect.btrfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:22.000000 dissect.btrfs-1.3.dev4/dissect.btrfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-11 11:56:22.000000 dissect.btrfs-1.3.dev4/dissect.btrfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 11:56:22.000000 dissect.btrfs-1.3.dev4/dissect.btrfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-11 11:56:17.000000 dissect.btrfs-1.3.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:56:22.724038 dissect.btrfs-1.3.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:22.712038 dissect.btrfs-1.3.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-11 11:56:12.000000 dissect.btrfs-1.3.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:22.724038 dissect.btrfs-1.3.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   239072 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-compression.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   155198 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-default.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   295784 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-dup-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   302851 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-dup-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   152549 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid0-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   148657 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid0-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   153538 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   151299 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   153589 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid10-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   151358 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid10-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   155315 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c3-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   153018 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c3-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   153018 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c3-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   153982 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c4-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   151612 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c4-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   151610 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c4-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   151614 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c4-4.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   153585 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid5-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   151362 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid5-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   153791 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid6-1.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   151501 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid6-2.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   151499 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-raid6-3.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   174289 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-sparse.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   170186 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-subvolume-custom-default.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   166940 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-subvolume-nested.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   177966 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-subvolume-snapshot.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   170958 2024-04-11 11:56:14.000000 dissect.btrfs-1.3.dev4/tests/data/btrfs-subvolume.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-04-11 11:56:13.000000 dissect.btrfs-1.3.dev4/tests/test_btrfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-11 11:56:13.000000 dissect.btrfs-1.3.dev4/tox.ini
```

### Comparing `dissect.btrfs-1.3.dev3/.gitattributes` & `dissect.btrfs-1.3.dev4/.gitattributes`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/LICENSE` & `dissect.btrfs-1.3.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/PKG-INFO` & `dissect.btrfs-1.3.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.btrfs
-Version: 1.3.dev3
+Version: 1.3.dev4
 Summary: A Dissect module implementing a parser for the Btrfs file system, a commonly used Linux filesystem.
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.btrfs
 Project-URL: repository, https://github.com/fox-it/dissect.btrfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.btrfs-1.3.dev3/README.md` & `dissect.btrfs-1.3.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/dissect/btrfs/btrfs.py` & `dissect.btrfs-1.3.dev4/dissect/btrfs/btrfs.py`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/dissect/btrfs/c_btrfs.py` & `dissect.btrfs-1.3.dev4/dissect/btrfs/c_btrfs.py`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/dissect/btrfs/stream.py` & `dissect.btrfs-1.3.dev4/dissect/btrfs/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/dissect/btrfs/tree.py` & `dissect.btrfs-1.3.dev4/dissect/btrfs/tree.py`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/dissect.btrfs.egg-info/PKG-INFO` & `dissect.btrfs-1.3.dev4/dissect.btrfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.btrfs
-Version: 1.3.dev3
+Version: 1.3.dev4
 Summary: A Dissect module implementing a parser for the Btrfs file system, a commonly used Linux filesystem.
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.btrfs
 Project-URL: repository, https://github.com/fox-it/dissect.btrfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.btrfs-1.3.dev3/dissect.btrfs.egg-info/SOURCES.txt` & `dissect.btrfs-1.3.dev4/dissect.btrfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/pyproject.toml` & `dissect.btrfs-1.3.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/conftest.py` & `dissect.btrfs-1.3.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-compression.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-compression.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-default.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-default.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-dup-1.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-dup-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-dup-2.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-dup-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid0-1.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid0-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid0-2.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid0-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1-1.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1-2.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid10-1.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid10-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid10-2.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid10-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c3-1.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c3-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c3-2.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c3-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c3-3.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c3-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c4-1.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c4-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c4-2.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c4-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c4-3.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c4-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid1c4-4.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid1c4-4.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid5-1.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid5-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid5-2.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid5-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid6-1.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid6-1.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid6-2.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid6-2.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-raid6-3.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-raid6-3.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-sparse.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-sparse.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-subvolume-custom-default.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-subvolume-custom-default.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-subvolume-nested.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-subvolume-nested.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-subvolume-snapshot.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-subvolume-snapshot.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/data/btrfs-subvolume.bin.gz` & `dissect.btrfs-1.3.dev4/tests/data/btrfs-subvolume.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tests/test_btrfs.py` & `dissect.btrfs-1.3.dev4/tests/test_btrfs.py`

 * *Files identical despite different names*

### Comparing `dissect.btrfs-1.3.dev3/tox.ini` & `dissect.btrfs-1.3.dev4/tox.ini`

 * *Files identical despite different names*

