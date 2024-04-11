# Comparing `tmp/dissect.regf-3.9.dev1.tar.gz` & `tmp/dissect.regf-3.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.regf-3.9.dev1.tar", last modified: Wed Jan 31 14:21:47 2024, max compression
+gzip compressed data, was "dissect.regf-3.9.dev2.tar", last modified: Tue Feb 20 13:43:08 2024, max compression
```

## Comparing `dissect.regf-3.9.dev1.tar` & `dissect.regf-3.9.dev2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:47.646245 dissect.regf-3.9.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-01-31 14:21:47.646245 dissect.regf-3.9.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:47.638245 dissect.regf-3.9.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:47.638245 dissect.regf-3.9.dev1/dissect/regf/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/dissect/regf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/dissect/regf/c_regf.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/dissect/regf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17271 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/dissect/regf/regf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:47.646245 dissect.regf-3.9.dev1/dissect.regf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-01-31 14:21:47.000000 dissect.regf-3.9.dev1/dissect.regf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-01-31 14:21:47.000000 dissect.regf-3.9.dev1/dissect.regf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 14:21:47.000000 dissect.regf-3.9.dev1/dissect.regf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-31 14:21:47.000000 dissect.regf-3.9.dev1/dissect.regf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-31 14:21:47.000000 dissect.regf-3.9.dev1/dissect.regf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:47.642245 dissect.regf-3.9.dev1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/examples/walkhive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-01-31 14:21:38.000000 dissect.regf-3.9.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 14:21:47.646245 dissect.regf-3.9.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:47.642245 dissect.regf-3.9.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:47.642245 dissect.regf-3.9.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1969086 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/tests/data/SYSTEM.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 14:21:47.642245 dissect.regf-3.9.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/tests/test_regf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-31 14:21:34.000000 dissect.regf-3.9.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:08.730948 dissect.regf-3.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-20 13:43:08.730948 dissect.regf-3.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:08.722948 dissect.regf-3.9.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:08.726948 dissect.regf-3.9.dev2/dissect/regf/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/dissect/regf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/dissect/regf/c_regf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/dissect/regf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17299 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/dissect/regf/regf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:08.730948 dissect.regf-3.9.dev2/dissect.regf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-20 13:43:08.000000 dissect.regf-3.9.dev2/dissect.regf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-20 13:43:08.000000 dissect.regf-3.9.dev2/dissect.regf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 13:43:08.000000 dissect.regf-3.9.dev2/dissect.regf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-20 13:43:08.000000 dissect.regf-3.9.dev2/dissect.regf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 13:43:08.000000 dissect.regf-3.9.dev2/dissect.regf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:08.726948 dissect.regf-3.9.dev2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/examples/walkhive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-02-20 13:43:00.000000 dissect.regf-3.9.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 13:43:08.730948 dissect.regf-3.9.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:08.726948 dissect.regf-3.9.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:08.726948 dissect.regf-3.9.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1969086 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/tests/data/SYSTEM.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 13:43:08.730948 dissect.regf-3.9.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/tests/test_regf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-02-20 13:42:57.000000 dissect.regf-3.9.dev2/tox.ini
```

### Comparing `dissect.regf-3.9.dev1/LICENSE` & `dissect.regf-3.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.9.dev1/PKG-INFO` & `dissect.regf-3.9.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.regf
-Version: 3.9.dev1
+Version: 3.9.dev2
 Summary: A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.regf
 Project-URL: repository, https://github.com/fox-it/dissect.regf
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.regf-3.9.dev1/README.md` & `dissect.regf-3.9.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.9.dev1/dissect/regf/c_regf.py` & `dissect.regf-3.9.dev2/dissect/regf/c_regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.9.dev1/dissect/regf/regf.py` & `dissect.regf-3.9.dev2/dissect/regf/regf.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,17 @@
                 f"The hive {self.filename!r} is undergoing a transaction, "
                 "may not be able to read keys and values properly."
             )
         else:
             log.debug(f"Hive {self.filename!r} is not undergoing any transactions.")
 
         self.hbin_offset = 4096
+
+        self.cell = lru_cache(4096)(self.cell)
+
         self._root = self.cell(self.header.root_key_offset)
 
     def root(self):
         return self._root
 
     def read_cell_data(self, offset):
         self.fh.seek(self.hbin_offset + offset)
@@ -101,15 +104,14 @@
             raise NotImplementedError(repr(sig))
 
         if sig == b"db":
             raise NotImplementedError(repr(sig))
 
         raise NotImplementedError(repr(sig))
 
-    @lru_cache(4096)
     def cell(self, offset):
         return self.read_cell(offset)
 
     def open(self, path):
         path = path.strip("\\")
         if path:
             parts = path.split("\\")
```

### Comparing `dissect.regf-3.9.dev1/dissect.regf.egg-info/PKG-INFO` & `dissect.regf-3.9.dev2/dissect.regf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.regf
-Version: 3.9.dev1
+Version: 3.9.dev2
 Summary: A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.regf
 Project-URL: repository, https://github.com/fox-it/dissect.regf
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.regf-3.9.dev1/pyproject.toml` & `dissect.regf-3.9.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.9.dev1/tests/data/SYSTEM.gz` & `dissect.regf-3.9.dev2/tests/data/SYSTEM.gz`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.9.dev1/tests/docs/Makefile` & `dissect.regf-3.9.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.9.dev1/tests/docs/conf.py` & `dissect.regf-3.9.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.9.dev1/tests/test_regf.py` & `dissect.regf-3.9.dev2/tests/test_regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.9.dev1/tox.ini` & `dissect.regf-3.9.dev2/tox.ini`

 * *Files identical despite different names*

