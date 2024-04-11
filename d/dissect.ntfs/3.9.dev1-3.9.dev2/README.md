# Comparing `tmp/dissect.ntfs-3.9.dev1.tar.gz` & `tmp/dissect.ntfs-3.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ntfs-3.9.dev1.tar", last modified: Wed Jan 31 14:23:06 2024, max compression
+gzip compressed data, was "dissect.ntfs-3.9.dev2.tar", last modified: Tue Feb 20 13:43:36 2024, max compression
```

## Comparing `dissect.ntfs-3.9.dev1.tar` & `dissect.ntfs-3.9.dev2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:06.020996 dissect.ntfs-3.9.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-01-31 14:23:06.020996 dissect.ntfs-3.9.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:06.012996 dissect.ntfs-3.9.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:06.016996 dissect.ntfs-3.9.dev1/dissect/ntfs/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17840 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/attr.py
--rw-r--r--   0 runner    (1001) docker     (127)    20063 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/c_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/mft.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/ntfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/dissect/ntfs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:06.020996 dissect.ntfs-3.9.dev1/dissect.ntfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-01-31 14:23:05.000000 dissect.ntfs-3.9.dev1/dissect.ntfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-31 14:23:06.000000 dissect.ntfs-3.9.dev1/dissect.ntfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 14:23:05.000000 dissect.ntfs-3.9.dev1/dissect.ntfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-31 14:23:05.000000 dissect.ntfs-3.9.dev1/dissect.ntfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-31 14:23:05.000000 dissect.ntfs-3.9.dev1/dissect.ntfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-31 14:22:57.000000 dissect.ntfs-3.9.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 14:23:06.020996 dissect.ntfs-3.9.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:06.016996 dissect.ntfs-3.9.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:22:55.000000 dissect.ntfs-3.9.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:06.020996 dissect.ntfs-3.9.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/data/boot_2m.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/data/mft.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)   908628 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/data/ntfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/data/ntfs_fragmented_mft.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/data/sds.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/data/sds_complex.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:23:06.020996 dissect.ntfs-3.9.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/test_mft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/test_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/test_secure.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/test_usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-31 14:22:54.000000 dissect.ntfs-3.9.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:36.471138 dissect.ntfs-3.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-02-20 13:43:36.467138 dissect.ntfs-3.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:36.459138 dissect.ntfs-3.9.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:36.463138 dissect.ntfs-3.9.dev2/dissect/ntfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17840 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20063 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/c_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/mft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/dissect/ntfs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:36.467138 dissect.ntfs-3.9.dev2/dissect.ntfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-02-20 13:43:36.000000 dissect.ntfs-3.9.dev2/dissect.ntfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-20 13:43:36.000000 dissect.ntfs-3.9.dev2/dissect.ntfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 13:43:36.000000 dissect.ntfs-3.9.dev2/dissect.ntfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-20 13:43:36.000000 dissect.ntfs-3.9.dev2/dissect.ntfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 13:43:36.000000 dissect.ntfs-3.9.dev2/dissect.ntfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-20 13:43:27.000000 dissect.ntfs-3.9.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 13:43:36.471138 dissect.ntfs-3.9.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:36.467138 dissect.ntfs-3.9.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:20.000000 dissect.ntfs-3.9.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:36.467138 dissect.ntfs-3.9.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/data/boot_2m.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/data/mft.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   908628 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/data/ntfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/data/ntfs_fragmented_mft.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/data/sds.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/data/sds_complex.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:36.467138 dissect.ntfs-3.9.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/test_mft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/test_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/test_secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/test_usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-02-20 13:43:19.000000 dissect.ntfs-3.9.dev2/tox.ini
```

### Comparing `dissect.ntfs-3.9.dev1/LICENSE` & `dissect.ntfs-3.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/PKG-INFO` & `dissect.ntfs-3.9.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.9.dev1
+Version: 3.9.dev2
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ntfs-3.9.dev1/README.md` & `dissect.ntfs-3.9.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/__init__.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/attr.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/c_ntfs.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/c_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/index.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,19 @@
             self._vcn_size_shift = SECTOR_SHIFT
 
         try:
             self._index_stream = self.record.open(self.name, ATTRIBUTE_TYPE_CODE.INDEX_ALLOCATION)
         except FileNotFoundError:
             self._index_stream = None
 
+        self.index_buffer = lru_cache(128)(self.index_buffer)
+
     def __iter__(self) -> Iterator[IndexEntry]:
         return self.entries()
 
-    @lru_cache(128)
     def index_buffer(self, vcn: int) -> IndexBuffer:
         """Return the :class:`IndexBuffer` at the specified cluster number.
 
         Args:
             vcn: The virtual cluster number within the index allocation to read.
 
         Raises:
```

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/mft.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/mft.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         ntfs: An optional NTFS class instance.
     """
 
     def __init__(self, fh: BinaryIO, ntfs: Optional[NTFS] = None):
         self.fh = fh
         self.ntfs = ntfs
 
+        self.get = lru_cache(4096)(self.get)
+
     def __call__(self, ref, *args, **kwargs) -> MftRecord:
         return self.get(ref, *args, **kwargs)
 
     @cached_property
     def root(self) -> MftRecord:
         """Return the root directory MFT record."""
         return self.get(FILE_NUMBER_ROOT)
@@ -85,15 +87,14 @@
             try:
                 node = index.search(part).dereference()
             except KeyError:
                 raise FileNotFoundError(f"File not found: {path}")
 
         return node
 
-    @lru_cache(4096)
     def get(self, ref: Union[int, str, Instance], root: Optional[MftRecord] = None) -> MftRecord:
         """Retrieve an MFT record using a variety of methods.
 
         Supported references are:
             - ``_MFT_SEGMENT_REFERENCE`` cstruct instance
             - integer segment number
             - string file path
```

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/ntfs.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/secure.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/stream.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/usnjrnl.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect/ntfs/util.py` & `dissect.ntfs-3.9.dev2/dissect/ntfs/util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/dissect.ntfs.egg-info/PKG-INFO` & `dissect.ntfs-3.9.dev2/dissect.ntfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.9.dev1
+Version: 3.9.dev2
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ntfs-3.9.dev1/dissect.ntfs.egg-info/SOURCES.txt` & `dissect.ntfs-3.9.dev2/dissect.ntfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/pyproject.toml` & `dissect.ntfs-3.9.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/conftest.py` & `dissect.ntfs-3.9.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/data/boot_2m.bin.gz` & `dissect.ntfs-3.9.dev2/tests/data/boot_2m.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/data/mft.bin.gz` & `dissect.ntfs-3.9.dev2/tests/data/mft.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/data/ntfs.bin.gz` & `dissect.ntfs-3.9.dev2/tests/data/ntfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/data/ntfs_fragmented_mft.csv.gz` & `dissect.ntfs-3.9.dev2/tests/data/ntfs_fragmented_mft.csv.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/data/sds.bin.gz` & `dissect.ntfs-3.9.dev2/tests/data/sds.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/data/sds_complex.bin.gz` & `dissect.ntfs-3.9.dev2/tests/data/sds_complex.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/docs/Makefile` & `dissect.ntfs-3.9.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/docs/conf.py` & `dissect.ntfs-3.9.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/test_attr.py` & `dissect.ntfs-3.9.dev2/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/test_index.py` & `dissect.ntfs-3.9.dev2/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/test_mft.py` & `dissect.ntfs-3.9.dev2/tests/test_mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/test_ntfs.py` & `dissect.ntfs-3.9.dev2/tests/test_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/test_secure.py` & `dissect.ntfs-3.9.dev2/tests/test_secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/test_usnjrnl.py` & `dissect.ntfs-3.9.dev2/tests/test_usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tests/test_util.py` & `dissect.ntfs-3.9.dev2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.9.dev1/tox.ini` & `dissect.ntfs-3.9.dev2/tox.ini`

 * *Files identical despite different names*

