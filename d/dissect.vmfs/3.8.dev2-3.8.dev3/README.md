# Comparing `tmp/dissect.vmfs-3.8.dev2.tar.gz` & `tmp/dissect.vmfs-3.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.vmfs-3.8.dev2.tar", last modified: Thu Mar 21 10:17:31 2024, max compression
+gzip compressed data, was "dissect.vmfs-3.8.dev3.tar", last modified: Thu Mar 28 17:24:22 2024, max compression
```

## Comparing `dissect.vmfs-3.8.dev2.tar` & `dissect.vmfs-3.8.dev3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:31.493760 dissect.vmfs-3.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-21 10:17:31.493760 dissect.vmfs-3.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:31.481760 dissect.vmfs-3.8.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:31.485760 dissect.vmfs-3.8.dev2/dissect/vmfs/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/dissect/vmfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/dissect/vmfs/c_vmfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/dissect/vmfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/dissect/vmfs/lvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/dissect/vmfs/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    28019 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/dissect/vmfs/vmfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:31.489760 dissect.vmfs-3.8.dev2/dissect.vmfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-21 10:17:31.000000 dissect.vmfs-3.8.dev2/dissect.vmfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-21 10:17:31.000000 dissect.vmfs-3.8.dev2/dissect.vmfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:17:31.000000 dissect.vmfs-3.8.dev2/dissect.vmfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 10:17:31.000000 dissect.vmfs-3.8.dev2/dissect.vmfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 10:17:31.000000 dissect.vmfs-3.8.dev2/dissect.vmfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-21 10:17:25.000000 dissect.vmfs-3.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:17:31.493760 dissect.vmfs-3.8.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:31.489760 dissect.vmfs-3.8.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:31.489760 dissect.vmfs-3.8.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   531458 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/data/vmfs5.bin.gz
--rw-r--r--   0 runner    (1001) docker     (127)  1054739 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/data/vmfs6.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:17:31.489760 dissect.vmfs-3.8.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/test_lvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tests/test_vmfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-21 10:17:18.000000 dissect.vmfs-3.8.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:24:22.737636 dissect.vmfs-3.8.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-28 17:24:22.737636 dissect.vmfs-3.8.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:24:22.729637 dissect.vmfs-3.8.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:24:22.733636 dissect.vmfs-3.8.dev3/dissect/vmfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/dissect/vmfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/dissect/vmfs/c_vmfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/dissect/vmfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/dissect/vmfs/lvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15221 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/dissect/vmfs/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28019 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/dissect/vmfs/vmfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:24:22.737636 dissect.vmfs-3.8.dev3/dissect.vmfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-28 17:24:22.000000 dissect.vmfs-3.8.dev3/dissect.vmfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 17:24:22.000000 dissect.vmfs-3.8.dev3/dissect.vmfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:24:22.000000 dissect.vmfs-3.8.dev3/dissect.vmfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:24:22.000000 dissect.vmfs-3.8.dev3/dissect.vmfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:24:22.000000 dissect.vmfs-3.8.dev3/dissect.vmfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-28 17:24:17.000000 dissect.vmfs-3.8.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:24:22.737636 dissect.vmfs-3.8.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:24:22.733636 dissect.vmfs-3.8.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:24:22.733636 dissect.vmfs-3.8.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   531458 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/data/vmfs5.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  1054739 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/data/vmfs6.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:24:22.737636 dissect.vmfs-3.8.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/test_lvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tests/test_vmfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:24:09.000000 dissect.vmfs-3.8.dev3/tox.ini
```

### Comparing `dissect.vmfs-3.8.dev2/LICENSE` & `dissect.vmfs-3.8.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/PKG-INFO` & `dissect.vmfs-3.8.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.vmfs
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.vmfs
 Project-URL: repository, https://github.com/fox-it/dissect.vmfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.vmfs-3.8.dev2/README.md` & `dissect.vmfs-3.8.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/dissect/vmfs/c_vmfs.py` & `dissect.vmfs-3.8.dev3/dissect/vmfs/c_vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/dissect/vmfs/lvm.py` & `dissect.vmfs-3.8.dev3/dissect/vmfs/lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/dissect/vmfs/resource.py` & `dissect.vmfs-3.8.dev3/dissect/vmfs/resource.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/dissect/vmfs/vmfs.py` & `dissect.vmfs-3.8.dev3/dissect/vmfs/vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/dissect.vmfs.egg-info/PKG-INFO` & `dissect.vmfs-3.8.dev3/dissect.vmfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.vmfs
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A Dissect module implementing a parser for the VMFS file system, used by VMware virtualization software
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.vmfs
 Project-URL: repository, https://github.com/fox-it/dissect.vmfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.vmfs-3.8.dev2/dissect.vmfs.egg-info/SOURCES.txt` & `dissect.vmfs-3.8.dev3/dissect.vmfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/pyproject.toml` & `dissect.vmfs-3.8.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/tests/data/vmfs5.bin.gz` & `dissect.vmfs-3.8.dev3/tests/data/vmfs5.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/tests/data/vmfs6.bin.gz` & `dissect.vmfs-3.8.dev3/tests/data/vmfs6.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/tests/docs/Makefile` & `dissect.vmfs-3.8.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/tests/docs/conf.py` & `dissect.vmfs-3.8.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/tests/test_address.py` & `dissect.vmfs-3.8.dev3/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/tests/test_lvm.py` & `dissect.vmfs-3.8.dev3/tests/test_lvm.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/tests/test_vmfs.py` & `dissect.vmfs-3.8.dev3/tests/test_vmfs.py`

 * *Files identical despite different names*

### Comparing `dissect.vmfs-3.8.dev2/tox.ini` & `dissect.vmfs-3.8.dev3/tox.ini`

 * *Files identical despite different names*

