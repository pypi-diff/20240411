# Comparing `tmp/lookout_config-1.0.2.tar.gz` & `tmp/lookout_config-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lookout_config-1.0.2.tar", last modified: Wed Apr 10 12:28:50 2024, max compression
+gzip compressed data, was "lookout_config-1.0.3.tar", last modified: Thu Apr 11 00:29:32 2024, max compression
```

## Comparing `lookout_config-1.0.2.tar` & `lookout_config-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:28:50.154879 lookout_config-1.0.2/
--rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-10 12:28:50.154879 lookout_config-1.0.2/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      625 2024-04-10 12:27:26.000000 lookout_config-1.0.2/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:28:50.154879 lookout_config-1.0.2/lookout_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2438 2024-04-10 12:27:26.000000 lookout_config-1.0.2/lookout_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     6529 2024-04-10 12:27:26.000000 lookout_config-1.0.2/lookout_config/generate_cameras.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      436 2024-04-10 12:27:26.000000 lookout_config-1.0.2/lookout_config/generate_schemas.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2762 2024-04-10 12:27:26.000000 lookout_config-1.0.2/lookout_config/generate_urdf.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:28:50.154879 lookout_config-1.0.2/lookout_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2769 2024-04-10 12:27:26.000000 lookout_config-1.0.2/lookout_config/schemas/lookout.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:28:50.154879 lookout_config-1.0.2/lookout_config/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-10 12:27:26.000000 lookout_config-1.0.2/lookout_config/test/lookout_config_test.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 12:28:50.154879 lookout_config-1.0.2/lookout_config.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-10 12:28:50.000000 lookout_config-1.0.2/lookout_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      465 2024-04-10 12:28:50.000000 lookout_config-1.0.2/lookout_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:28:50.000000 lookout_config-1.0.2/lookout_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-10 12:28:50.000000 lookout_config-1.0.2/lookout_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2024-04-10 12:28:50.000000 lookout_config-1.0.2/lookout_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 12:28:32.000000 lookout_config-1.0.2/lookout_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      914 2024-04-10 12:28:50.154879 lookout_config-1.0.2/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-10 12:27:26.000000 lookout_config-1.0.2/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-11 00:29:32.297587 lookout_config-1.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-11 00:29:32.297587 lookout_config-1.0.3/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      625 2024-04-11 00:28:21.000000 lookout_config-1.0.3/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-11 00:29:32.297587 lookout_config-1.0.3/lookout_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2438 2024-04-11 00:28:21.000000 lookout_config-1.0.3/lookout_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     6529 2024-04-11 00:28:21.000000 lookout_config-1.0.3/lookout_config/generate_cameras.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      436 2024-04-11 00:28:21.000000 lookout_config-1.0.3/lookout_config/generate_schemas.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2762 2024-04-11 00:28:21.000000 lookout_config-1.0.3/lookout_config/generate_urdf.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-11 00:29:32.297587 lookout_config-1.0.3/lookout_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2769 2024-04-11 00:28:21.000000 lookout_config-1.0.3/lookout_config/schemas/lookout.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-11 00:29:32.297587 lookout_config-1.0.3/lookout_config/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-11 00:28:21.000000 lookout_config-1.0.3/lookout_config/test/lookout_config_test.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-11 00:29:32.297587 lookout_config-1.0.3/lookout_config.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-11 00:29:32.000000 lookout_config-1.0.3/lookout_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      465 2024-04-11 00:29:32.000000 lookout_config-1.0.3/lookout_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-11 00:29:32.000000 lookout_config-1.0.3/lookout_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-11 00:29:32.000000 lookout_config-1.0.3/lookout_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2024-04-11 00:29:32.000000 lookout_config-1.0.3/lookout_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-11 00:29:16.000000 lookout_config-1.0.3/lookout_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      914 2024-04-11 00:29:32.301587 lookout_config-1.0.3/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-11 00:28:21.000000 lookout_config-1.0.3/setup.py
```

### Comparing `lookout_config-1.0.2/PKG-INFO` & `lookout_config-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_config
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library for reading / writing Lookout config files
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_config-1.0.2/README.md` & `lookout_config-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lookout_config-1.0.2/lookout_config/__init__.py` & `lookout_config-1.0.3/lookout_config/__init__.py`

 * *Files identical despite different names*

### Comparing `lookout_config-1.0.2/lookout_config/generate_cameras.py` & `lookout_config-1.0.3/lookout_config/generate_cameras.py`

 * *Files identical despite different names*

### Comparing `lookout_config-1.0.2/lookout_config/generate_urdf.py` & `lookout_config-1.0.3/lookout_config/generate_urdf.py`

 * *Files identical despite different names*

### Comparing `lookout_config-1.0.2/lookout_config/schemas/lookout.schema.json` & `lookout_config-1.0.3/lookout_config/schemas/lookout.schema.json`

 * *Files identical despite different names*

### Comparing `lookout_config-1.0.2/lookout_config.egg-info/PKG-INFO` & `lookout_config-1.0.3/lookout_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_config
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library for reading / writing Lookout config files
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_config-1.0.2/setup.cfg` & `lookout_config-1.0.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lookout_config
-version = 1.0.2
+version = 1.0.3
 url = https://github.com/Greenroom-Robotics/lookout
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

