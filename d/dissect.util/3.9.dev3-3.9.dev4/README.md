# Comparing `tmp/dissect.util-3.9.dev3.tar.gz` & `tmp/dissect.util-3.9.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.util-3.9.dev3.tar", last modified: Tue Jun 27 07:48:30 2023, max compression
+gzip compressed data, was "dissect.util-3.9.dev4.tar", last modified: Wed Jul  5 12:42:33 2023, max compression
```

## Comparing `dissect.util-3.9.dev3.tar` & `dissect.util-3.9.dev4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.170692 dissect.util-3.9.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-27 07:48:30.170692 dissect.util-3.9.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.154692 dissect.util-3.9.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.158692 dissect.util-3.9.dev3/dissect/util/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.162692 dissect.util-3.9.dev3/dissect/util/compression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/compression/lzxpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/compression/lzxpress_huffman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/compression/sevenbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/cpio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.162692 dissect.util-3.9.dev3/dissect/util/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/encoding/surrogateescape.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/plist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/sid.py
--rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.162692 dissect.util-3.9.dev3/dissect/util/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/tools/dump_nskeyedarchiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/dissect/util/xmemoryview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.154692 dissect.util-3.9.dev3/dissect.util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-27 07:48:30.000000 dissect.util-3.9.dev3/dissect.util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 07:48:30.000000 dissect.util-3.9.dev3/dissect.util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:48:30.000000 dissect.util-3.9.dev3/dissect.util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-27 07:48:30.000000 dissect.util-3.9.dev3/dissect.util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:48:30.000000 dissect.util-3.9.dev3/dissect.util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-27 07:48:20.000000 dissect.util-3.9.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:48:30.170692 dissect.util-3.9.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.166692 dissect.util-3.9.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.170692 dissect.util-3.9.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/data/bin.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/data/crc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/data/hpbin.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/data/hpodc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/data/newc.cpio.gz
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/data/odc.cpio.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:30.170692 dissect.util-3.9.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/test_cpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/test_plist.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/test_sid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/test_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tests/test_xmemoryview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:48:15.000000 dissect.util-3.9.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.176804 dissect.util-3.9.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-05 12:42:33.176804 dissect.util-3.9.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.168804 dissect.util-3.9.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.172804 dissect.util-3.9.dev4/dissect/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.172804 dissect.util-3.9.dev4/dissect/util/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/compression/lzxpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/compression/lzxpress_huffman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/compression/sevenbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/cpio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.172804 dissect.util-3.9.dev4/dissect/util/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/encoding/surrogateescape.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18781 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.172804 dissect.util-3.9.dev4/dissect/util/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/tools/dump_nskeyedarchiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/dissect/util/xmemoryview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.168804 dissect.util-3.9.dev4/dissect.util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-05 12:42:33.000000 dissect.util-3.9.dev4/dissect.util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-05 12:42:33.000000 dissect.util-3.9.dev4/dissect.util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:42:33.000000 dissect.util-3.9.dev4/dissect.util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 12:42:33.000000 dissect.util-3.9.dev4/dissect.util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 12:42:33.000000 dissect.util-3.9.dev4/dissect.util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-05 12:42:20.000000 dissect.util-3.9.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:42:33.176804 dissect.util-3.9.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.176804 dissect.util-3.9.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.176804 dissect.util-3.9.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/data/bin.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/data/crc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/data/hpbin.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/data/hpodc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/data/newc.cpio.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/data/odc.cpio.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:42:33.176804 dissect.util-3.9.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16394 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/test_cpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/test_plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/test_sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/test_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tests/test_xmemoryview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-05 12:42:13.000000 dissect.util-3.9.dev4/tox.ini
```

### Comparing `dissect.util-3.9.dev3/LICENSE` & `dissect.util-3.9.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/PKG-INFO` & `dissect.util-3.9.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.util
-Version: 3.9.dev3
+Version: 3.9.dev4
 Summary: A Dissect module implementing various utility functions for the other Dissect modules
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.util
 Project-URL: repository, https://github.com/fox-it/dissect.util
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.util-3.9.dev3/README.md` & `dissect.util-3.9.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/compression/lz4.py` & `dissect.util-3.9.dev4/dissect/util/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/compression/lznt1.py` & `dissect.util-3.9.dev4/dissect/util/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/compression/lzo.py` & `dissect.util-3.9.dev4/dissect/util/compression/lzo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,29 @@
+# References:
+# - https://github.com/FFmpeg/FFmpeg/blob/master/libavutil/lzo.c
+# - https://docs.kernel.org/staging/lzo.html
+# - https://github.com/torvalds/linux/blob/master/lib/lzo/lzo1x_decompress_safe.c
+
 import io
 import struct
 from typing import BinaryIO, Union
 
-
-def _count_zeroes(src: BinaryIO):
-    length = 0
-    val = src.read(1)[0]
-    while val == 0:
-        length += 255
-        val = src.read(1)[0]
-        if length > 2**20:
-            raise ValueError("Too many zeroes")
-
-    return length + val
+MAX_READ_LENGTH = (1 << 32) - 1000
 
 
-def _copy_block(src: BinaryIO, dst: bytearray, length: int, distance: int, trailing: int):
-    remaining = length
+def _read_length(src: BinaryIO, val: int, mask: int) -> int:
+    if (length := val & mask) != 0:
+        return length
 
-    block = dst[-distance:]
-    remaining -= len(block)
-    while remaining > 0:
-        add = block[:remaining]
-        remaining -= len(add)
-        block += add
+    while (val := src.read(1)[0]) == 0:
+        if length >= MAX_READ_LENGTH:
+            raise ValueError("Invalid encoded length")
+        length += 255
 
-    dst.extend(block[:length])
-    dst.extend(src.read(trailing))
+    return length + mask + val
 
 
 def decompress(src: Union[bytes, BinaryIO], header: bool = True, buflen: int = -1) -> bytes:
     """LZO decompress from a file-like object or bytes. Assumes no header.
 
     Arguments are largely compatible with python-lzo API.
 
@@ -52,64 +45,70 @@
         if byte not in [0xF0, 0xF1]:
             raise ValueError("Invalid header value")
         out_len = struct.unpack("<I", src.read(4))
     else:
         out_len = buflen
 
     val = src.read(1)[0]
-    if val == 0x10:
-        raise ValueError("LZOv1")
-    elif val >= 0x12:
-        dst += src.read(val - 0x11)
+    offset = src.tell()
+    if src.seek(5) == 5 and val == 17:
+        src.seek(offset)
+        _ = src.read(1)  # This would be the bitstream version but we don't currently use it
         val = src.read(1)[0]
+    else:
+        src.seek(offset)
 
-    trailing = 0
+    if val > 17:
+        dst += src.read(val - 17)
+        val = src.read(1)[0]
+
+        if val < 16:
+            raise ValueError("Invalid LZO stream")
+
+    state = 0
     while True:
-        if val <= 0xF:
-            if not trailing:
-                if val == 0:
-                    dst += src.read(_count_zeroes(src) + 18)
-                else:
-                    dst += src.read(val + 3)
-            else:
-                h = src.read(1)[0]
-                dist = (h << 2) + (val >> 2) + 1
-                length = 2
-                trailing = val & 3
-                _copy_block(src, dst, length, dist, trailing)
-        elif val <= 0x1F:
-            if val & 7 == 0:
-                length = 9 + _count_zeroes(src)
+        if val > 15:
+            if val > 63:
+                # Copy 3-8 bytes from block within 2kb distance
+                length = (val >> 5) - 1
+                dist = (src.read(1)[0] << 3) + ((val >> 2) & 7) + 1
+            elif val > 31:
+                # Copy of small block within 16kb distance
+                length = _read_length(src, val, 31)
+                val = src.read(1)[0]
+                dist = (src.read(1)[0] << 6) + (val >> 2) + 1
             else:
-                length = (val & 7) + 2
-            ds = struct.unpack("<H", src.read(2))[0]
-            dist = 16384 + ((val & 8) >> 3) + (ds >> 2)
-            if dist == 16384:
-                break
-            trailing = ds & 3
-            _copy_block(src, dst, length, dist, trailing)
-        elif val <= 0x3F:
-            length = val & 31
-            if length == 0:
-                length = _count_zeroes(src) + 31
-            length += 2
-            ds = struct.unpack("<H", src.read(2))[0]
-            dist = 1 + (ds >> 2)
-            trailing = ds & 3
-            _copy_block(src, dst, length, dist, trailing)
+                # Copy of a block within 16...48kB distance
+                length = _read_length(src, val, 7)
+                dist = (1 << 14) + ((val & 8) << 11)
+                val = src.read(1)[0]
+                dist += (src.read(1)[0] << 6) + (val >> 2)
+                if dist == (1 << 14):
+                    if length != 1:
+                        raise ValueError("Invalid LZO stream")
+                    break
+        elif not state:
+            # Copy 4 or more literals, depending on the last 4 bits
+            length = _read_length(src, val, 15)
+            dst += src.read(length + 3)
+            val = src.read(1)[0]
+            if val > 15:
+                continue
+            length = 1
+            dist = (1 << 11) + (src.read(1)[0] << 2) + (val >> 2) + 1
         else:
-            if val <= 0x7F:
-                length = 3 + ((val >> 5) & 1)
-            else:
-                length = 5 + ((val >> 5) & 3)
-            h = src.read(1)[0]
-            d = (val >> 2) & 7
-            dist = (h << 3) + d + 1
-            trailing = val & 3
-            _copy_block(src, dst, length, dist, trailing)
+            length = 0
+            dist = (src.read(1)[0] << 2) + (val >> 2) + 1
+
+        for _ in range(length + 2):
+            dst.append(dst[-dist])
+
+        # State is often encoded in the last 2 bits of the value, and used in subsequent iterations
+        state = length = val & 3
+        dst += src.read(length)
 
         if len(dst) == out_len:
             break
 
         val = src.read(1)[0]
 
     return bytes(dst)
```

### Comparing `dissect.util-3.9.dev3/dissect/util/compression/lzxpress.py` & `dissect.util-3.9.dev4/dissect/util/compression/lzxpress.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/compression/lzxpress_huffman.py` & `dissect.util-3.9.dev4/dissect/util/compression/lzxpress_huffman.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/compression/sevenbit.py` & `dissect.util-3.9.dev4/dissect/util/compression/sevenbit.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/cpio.py` & `dissect.util-3.9.dev4/dissect/util/cpio.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/plist.py` & `dissect.util-3.9.dev4/dissect/util/plist.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/sid.py` & `dissect.util-3.9.dev4/dissect/util/sid.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/stream.py` & `dissect.util-3.9.dev4/dissect/util/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/tools/dump_nskeyedarchiver.py` & `dissect.util-3.9.dev4/dissect/util/tools/dump_nskeyedarchiver.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/ts.py` & `dissect.util-3.9.dev4/dissect/util/ts.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect/util/xmemoryview.py` & `dissect.util-3.9.dev4/dissect/util/xmemoryview.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/dissect.util.egg-info/PKG-INFO` & `dissect.util-3.9.dev4/dissect.util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.util
-Version: 3.9.dev3
+Version: 3.9.dev4
 Summary: A Dissect module implementing various utility functions for the other Dissect modules
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.util
 Project-URL: repository, https://github.com/fox-it/dissect.util
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.util-3.9.dev3/dissect.util.egg-info/SOURCES.txt` & `dissect.util-3.9.dev4/dissect.util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/pyproject.toml` & `dissect.util-3.9.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/data/bin.cpio.gz` & `dissect.util-3.9.dev4/tests/data/bin.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/data/crc.cpio.gz` & `dissect.util-3.9.dev4/tests/data/crc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/data/hpbin.cpio.gz` & `dissect.util-3.9.dev4/tests/data/hpbin.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/data/hpodc.cpio.gz` & `dissect.util-3.9.dev4/tests/data/hpodc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/data/newc.cpio.gz` & `dissect.util-3.9.dev4/tests/data/newc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/data/odc.cpio.gz` & `dissect.util-3.9.dev4/tests/data/odc.cpio.gz`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/docs/Makefile` & `dissect.util-3.9.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/docs/conf.py` & `dissect.util-3.9.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/test_cpio.py` & `dissect.util-3.9.dev4/tests/test_cpio.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/test_plist.py` & `dissect.util-3.9.dev4/tests/test_plist.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/test_sid.py` & `dissect.util-3.9.dev4/tests/test_sid.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/test_stream.py` & `dissect.util-3.9.dev4/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/test_ts.py` & `dissect.util-3.9.dev4/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tests/test_xmemoryview.py` & `dissect.util-3.9.dev4/tests/test_xmemoryview.py`

 * *Files identical despite different names*

### Comparing `dissect.util-3.9.dev3/tox.ini` & `dissect.util-3.9.dev4/tox.ini`

 * *Files identical despite different names*

