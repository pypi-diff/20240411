# Comparing `tmp/idna-3.5.tar.gz` & `tmp/idna-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idna-3.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idna-3.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idna-3.5.tar` & `idna-3.6.tar`

### file list

```diff
@@ -1,13 +1,21 @@
--rw-r--r--   0        0        0     1541 2023-11-24 17:46:29.733286 idna-3.5/LICENSE.md
--rw-r--r--   0        0        0     8381 2023-11-24 17:37:21.984887 idna-3.5/README.rst
--rw-r--r--   0        0        0      849 2023-06-19 19:05:18.867897 idna-3.5/idna/__init__.py
--rw-r--r--   0        0        0     3426 2023-11-23 02:59:37.252296 idna-3.5/idna/codec.py
--rw-r--r--   0        0        0      321 2023-06-19 19:05:18.868034 idna-3.5/idna/compat.py
--rw-r--r--   0        0        0    12908 2023-11-23 02:59:37.252688 idna-3.5/idna/core.py
--rw-r--r--   0        0        0    44351 2023-11-23 02:59:37.253152 idna-3.5/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2023-06-19 19:05:18.868462 idna-3.5/idna/intranges.py
--rw-r--r--   0        0        0       21 2023-11-24 17:38:24.568938 idna-3.5/idna/package_data.py
--rw-r--r--   0        0        0        0 2023-06-19 19:05:18.868536 idna-3.5/idna/py.typed
--rw-r--r--   0        0        0   206503 2023-11-23 02:59:37.254253 idna-3.5/idna/uts46data.py
--rw-r--r--   0        0        0     1560 2023-08-20 22:08:58.230338 idna-3.5/pyproject.toml
--rw-r--r--   0        0        0     9888 1970-01-01 00:00:00.000000 idna-3.5/PKG-INFO
+-rw-r--r--   0        0        0     1541 2023-11-25 15:32:53.074560 idna-3.6/LICENSE.md
+-rw-r--r--   0        0        0     8381 2023-11-25 15:32:53.074960 idna-3.6/README.rst
+-rw-r--r--   0        0        0      849 2023-06-19 19:05:18.867897 idna-3.6/idna/__init__.py
+-rw-r--r--   0        0        0     3426 2023-11-23 02:59:37.252296 idna-3.6/idna/codec.py
+-rw-r--r--   0        0        0      321 2023-06-19 19:05:18.868034 idna-3.6/idna/compat.py
+-rw-r--r--   0        0        0    12908 2023-11-23 02:59:37.252688 idna-3.6/idna/core.py
+-rw-r--r--   0        0        0    44351 2023-11-23 02:59:37.253152 idna-3.6/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2023-06-19 19:05:18.868462 idna-3.6/idna/intranges.py
+-rw-r--r--   0        0        0       21 2023-11-25 15:34:06.622138 idna-3.6/idna/package_data.py
+-rw-r--r--   0        0        0        0 2023-06-19 19:05:18.868536 idna-3.6/idna/py.typed
+-rw-r--r--   0        0        0   206503 2023-11-23 02:59:37.254253 idna-3.6/idna/uts46data.py
+-rw-r--r--   0        0        0     1580 2023-11-25 15:32:53.075999 idna-3.6/pyproject.toml
+-rw-r--r--   0        0        0   716784 2023-06-19 19:05:18.871644 idna-3.6/tests/IdnaTestV2.txt
+-rw-r--r--   0        0        0        0 2023-06-19 19:05:18.871827 idna-3.6/tests/__init__.py
+-rwxr-xr-x   0        0        0    13182 2023-06-19 19:05:18.871961 idna-3.6/tests/test_idna.py
+-rwxr-xr-x   0        0        0     3684 2023-06-19 19:05:18.872047 idna-3.6/tests/test_idna_codec.py
+-rwxr-xr-x   0        0        0      532 2023-06-19 19:05:18.872115 idna-3.6/tests/test_idna_compat.py
+-rwxr-xr-x   0        0        0      297 2023-06-19 19:05:18.872176 idna-3.6/tests/test_idna_other.py
+-rwxr-xr-x   0        0        0     8192 2023-06-19 19:05:18.872285 idna-3.6/tests/test_idna_uts46.py
+-rw-r--r--   0        0        0     1777 2023-06-19 19:05:18.872359 idna-3.6/tests/test_intranges.py
+-rw-r--r--   0        0        0     9888 1970-01-01 00:00:00.000000 idna-3.6/PKG-INFO
```

### Comparing `idna-3.5/LICENSE.md` & `idna-3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `idna-3.5/README.rst` & `idna-3.6/README.rst`

 * *Files identical despite different names*

### Comparing `idna-3.5/idna/__init__.py` & `idna-3.6/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `idna-3.5/idna/codec.py` & `idna-3.6/idna/codec.py`

 * *Files identical despite different names*

### Comparing `idna-3.5/idna/core.py` & `idna-3.6/idna/core.py`

 * *Files identical despite different names*

### Comparing `idna-3.5/idna/idnadata.py` & `idna-3.6/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `idna-3.5/idna/intranges.py` & `idna-3.6/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `idna-3.5/idna/uts46data.py` & `idna-3.6/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `idna-3.5/pyproject.toml` & `idna-3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -39,7 +39,8 @@
 [project.urls]
 "Source" = "https://github.com/kjd/idna"
 "Changelog" = "https://github.com/kjd/idna/blob/master/HISTORY.rst"
 "Issue tracker" = "https://github.com/kjd/idna/issues"
 
 [tool.flit.sdist]
 exclude = [".gitignore", ".github/"]
+include = ["tests"]
```

### Comparing `idna-3.5/PKG-INFO` & `idna-3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idna
-Version: 3.5
+Version: 3.6
 Summary: Internationalized Domain Names in Applications (IDNA)
 Author-email: Kim Davies <kim+pypi@gumleaf.org>
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

