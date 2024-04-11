# Comparing `tmp/skale-contracts-1.0.1a5.tar.gz` & `tmp/skale-contracts-1.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale-contracts-1.0.1a5.tar", last modified: Thu Apr  4 15:59:27 2024, max compression
+gzip compressed data, was "skale-contracts-1.0.1a6.tar", last modified: Thu Apr 11 15:44:24 2024, max compression
```

## Comparing `skale-contracts-1.0.1a5.tar` & `skale-contracts-1.0.1a6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.634534 skale-contracts-1.0.1a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/src/skale_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/project_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/src/skale_contracts/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/projects/ima.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/projects/skale_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/projects/skale_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-04 15:59:19.000000 skale-contracts-1.0.1a5/src/skale_contracts/skale_contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:59:27.638534 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 15:59:27.000000 skale-contracts-1.0.1a5/src/skale_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 15:59:25.000000 skale-contracts-1.0.1a5/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:44:24.704180 skale-contracts-1.0.1a6/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-11 15:44:24.704180 skale-contracts-1.0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-11 15:44:24.704180 skale-contracts-1.0.1a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:44:24.700180 skale-contracts-1.0.1a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:44:24.704180 skale-contracts-1.0.1a6/src/skale_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/project_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:44:24.704180 skale-contracts-1.0.1a6/src/skale_contracts/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/projects/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/projects/ima.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/projects/skale_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/projects/skale_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-11 15:44:14.000000 skale-contracts-1.0.1a6/src/skale_contracts/skale_contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:44:24.704180 skale-contracts-1.0.1a6/src/skale_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-11 15:44:24.000000 skale-contracts-1.0.1a6/src/skale_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-11 15:44:24.000000 skale-contracts-1.0.1a6/src/skale_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:44:24.000000 skale-contracts-1.0.1a6/src/skale_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 15:44:24.000000 skale-contracts-1.0.1a6/src/skale_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 15:44:24.000000 skale-contracts-1.0.1a6/src/skale_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 15:44:22.000000 skale-contracts-1.0.1a6/version.txt
```

### Comparing `skale-contracts-1.0.1a5/PKG-INFO` & `skale-contracts-1.0.1a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 1.0.1a5
+Version: 1.0.1a6
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale-contracts-1.0.1a5/setup.cfg` & `skale-contracts-1.0.1a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/instance.py` & `skale-contracts-1.0.1a6/src/skale_contracts/instance.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/metadata.py` & `skale-contracts-1.0.1a6/src/skale_contracts/metadata.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/network.py` & `skale-contracts-1.0.1a6/src/skale_contracts/network.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/project.py` & `skale-contracts-1.0.1a6/src/skale_contracts/project.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/project_factory.py` & `skale-contracts-1.0.1a6/src/skale_contracts/project_factory.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/projects/ima.py` & `skale-contracts-1.0.1a6/src/skale_contracts/projects/ima.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/projects/skale_allocator.py` & `skale-contracts-1.0.1a6/src/skale_contracts/projects/skale_allocator.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/projects/skale_manager.py` & `skale-contracts-1.0.1a6/src/skale_contracts/projects/skale_manager.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts/skale_contracts.py` & `skale-contracts-1.0.1a6/src/skale_contracts/skale_contracts.py`

 * *Files identical despite different names*

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts.egg-info/PKG-INFO` & `skale-contracts-1.0.1a6/src/skale_contracts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 1.0.1a5
+Version: 1.0.1a6
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale-contracts-1.0.1a5/src/skale_contracts.egg-info/SOURCES.txt` & `skale-contracts-1.0.1a6/src/skale_contracts.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 src/skale_contracts/skale_contracts.py
 src/skale_contracts.egg-info/PKG-INFO
 src/skale_contracts.egg-info/SOURCES.txt
 src/skale_contracts.egg-info/dependency_links.txt
 src/skale_contracts.egg-info/requires.txt
 src/skale_contracts.egg-info/top_level.txt
 src/skale_contracts/projects/__init__.py
+src/skale_contracts/projects/context.py
 src/skale_contracts/projects/ima.py
 src/skale_contracts/projects/skale_allocator.py
 src/skale_contracts/projects/skale_manager.py
```

