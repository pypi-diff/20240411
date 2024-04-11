# Comparing `tmp/sling-1.2.3.tar.gz` & `tmp/sling-1.2.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sling-1.2.3.tar", last modified: Wed Apr 10 17:18:14 2024, max compression
+gzip compressed data, was "sling-1.2.3.post1.tar", last modified: Wed Apr 10 17:44:32 2024, max compression
```

## Comparing `sling-1.2.3.tar` & `sling-1.2.3.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:14.472063 sling-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 17:15:10.000000 sling-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-10 17:18:14.472063 sling-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-10 17:18:10.000000 sling-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 17:18:10.000000 sling-1.2.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:18:14.472063 sling-1.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-10 17:15:10.000000 sling-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:14.472063 sling-1.2.3/sling/
--rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-04-10 17:15:10.000000 sling-1.2.3/sling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:18:14.472063 sling-1.2.3/sling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 17:18:14.000000 sling-1.2.3/sling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:44:32.917261 sling-1.2.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 17:41:10.000000 sling-1.2.3.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-10 17:44:32.917261 sling-1.2.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-10 17:44:29.000000 sling-1.2.3.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 17:44:29.000000 sling-1.2.3.post1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:44:32.917261 sling-1.2.3.post1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2235 2024-04-10 17:41:10.000000 sling-1.2.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:44:32.913261 sling-1.2.3.post1/sling/
+-rw-r--r--   0 runner    (1001) docker     (127)    14513 2024-04-10 17:41:10.000000 sling-1.2.3.post1/sling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:44:32.917261 sling-1.2.3.post1/sling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-10 17:44:32.000000 sling-1.2.3.post1/sling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-10 17:44:32.000000 sling-1.2.3.post1/sling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:44:32.000000 sling-1.2.3.post1/sling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 17:44:32.000000 sling-1.2.3.post1/sling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 17:44:32.000000 sling-1.2.3.post1/sling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 17:44:32.000000 sling-1.2.3.post1/sling.egg-info/top_level.txt
```

### Comparing `sling-1.2.3/PKG-INFO` & `sling-1.2.3.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sling
-Version: 1.2.3
+Version: 1.2.3.post1
 Summary: Slings data from a source to a target
 Home-page: https://github.com/slingdata-io/sling-python
 Author: Fritz Larco
 Author-email: fritz@slingdata.io
 License: UNKNOWN
 Download-URL: https://github.com/slingdata-io/sling-python/archive/master.zip
 Keywords: sling,etl,elt,extract,load
```

### Comparing `sling-1.2.3/README.md` & `sling-1.2.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `sling-1.2.3/setup.py` & `sling-1.2.3.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 install_requires = []
 if platform.system() == 'Linux':
   if platform.machine() == 'aarch64':
     install_requires = [f'sling-linux-arm64=={SLING_VERSION}']
   else:
     install_requires = [f'sling-linux-amd64=={SLING_VERSION}']
 elif platform.system() == 'Windows':
-  if platform.machine() == 'aarch64':
+  if platform.machine() == 'ARM64':
     install_requires = [f'sling-windows-arm64=={SLING_VERSION}']
   else:
     install_requires = [f'sling-windows-amd64=={SLING_VERSION}']
 elif platform.system() == 'Darwin':
-  if platform.machine() == 'aarch64':
+  if platform.machine() == 'arm64':
     install_requires = [f'sling-mac-arm64=={SLING_VERSION}']
   else:
     install_requires = [f'sling-mac-amd64=={SLING_VERSION}']
 else:
   raise Exception(f'platform "{platform.system()}" ({platform.system()}) not supported.')
 
 setup(
```

### Comparing `sling-1.2.3/sling/__init__.py` & `sling-1.2.3.post1/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `sling-1.2.3/sling.egg-info/PKG-INFO` & `sling-1.2.3.post1/sling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sling
-Version: 1.2.3
+Version: 1.2.3.post1
 Summary: Slings data from a source to a target
 Home-page: https://github.com/slingdata-io/sling-python
 Author: Fritz Larco
 Author-email: fritz@slingdata.io
 License: UNKNOWN
 Download-URL: https://github.com/slingdata-io/sling-python/archive/master.zip
 Keywords: sling,etl,elt,extract,load
```

