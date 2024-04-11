# Comparing `tmp/datoso-0.3.8.tar.gz` & `tmp/datoso-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.3.8.tar", last modified: Tue Nov 28 18:47:07 2023, max compression
+gzip compressed data, was "datoso-0.3.9.tar", last modified: Fri Dec  8 03:46:11 2023, max compression
```

## Comparing `datoso-0.3.8.tar` & `datoso-0.3.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.467302 datoso-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-28 18:46:54.000000 datoso-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-28 18:46:54.000000 datoso-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-11-28 18:47:07.467302 datoso-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2023-11-28 18:46:54.000000 datoso-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-11-28 18:46:54.000000 datoso-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-28 18:47:07.467302 datoso-0.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.459302 datoso-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.459302 datoso-0.3.8/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20740 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.463302 datoso-0.3.8/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.463302 datoso-0.3.8/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.463302 datoso-0.3.8/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.463302 datoso-0.3.8/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.463302 datoso-0.3.8/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.463302 datoso-0.3.8/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.467302 datoso-0.3.8/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/helpers/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.467302 datoso-0.3.8/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14809 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.467302 datoso-0.3.8/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (127)    43419 2023-11-28 18:46:54.000000 datoso-0.3.8/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:47:07.463302 datoso-0.3.8/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-11-28 18:47:07.000000 datoso-0.3.8/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-11-28 18:47:07.000000 datoso-0.3.8/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:47:07.000000 datoso-0.3.8/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-28 18:47:07.000000 datoso-0.3.8/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-11-28 18:47:07.000000 datoso-0.3.8/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-28 18:47:07.000000 datoso-0.3.8/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.651119 datoso-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-08 03:46:01.000000 datoso-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-08 03:46:01.000000 datoso-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-12-08 03:46:11.651119 datoso-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2023-12-08 03:46:01.000000 datoso-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-12-08 03:46:01.000000 datoso-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-08 03:46:11.651119 datoso-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.643119 datoso-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.647119 datoso-0.3.9/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20740 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.647119 datoso-0.3.9/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.647119 datoso-0.3.9/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.651119 datoso-0.3.9/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.651119 datoso-0.3.9/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.651119 datoso-0.3.9/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.651119 datoso-0.3.9/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.651119 datoso-0.3.9/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/helpers/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.651119 datoso-0.3.9/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14809 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.651119 datoso-0.3.9/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    43419 2023-12-08 03:46:01.000000 datoso-0.3.9/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 03:46:11.647119 datoso-0.3.9/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2023-12-08 03:46:11.000000 datoso-0.3.9/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-12-08 03:46:11.000000 datoso-0.3.9/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 03:46:11.000000 datoso-0.3.9/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-08 03:46:11.000000 datoso-0.3.9/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2023-12-08 03:46:11.000000 datoso-0.3.9/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-08 03:46:11.000000 datoso-0.3.9/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.3.8/LICENSE` & `datoso-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/PKG-INFO` & `datoso-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.3.8/README.md` & `datoso-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/pyproject.toml` & `datoso-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,26 +31,26 @@
     "requests>=2.31.0",
 ]
 dynamic = ["version"]
 
 
 [project.optional-dependencies]
 all = [
-    "datoso-seed-fbneo>=0.3.2",
+    "datoso-seed-fbneo>=0.3.3",
     "datoso-seed-md-enhanced>=0.3.0",
     "datoso-seed-nointro>=0.3.0",
     "datoso-seed-pleasuredome>=0.3.2",
     "datoso-seed-redump>=0.3.1",
     "datoso-seed-sfc-enhancedcolors>=0.3.0",
     "datoso-seed-sfc-msu1>=0.3.0",
     "datoso-seed-sfc-speedhacks>=0.3.0",
     "datoso-seed-translatedenglish>=0.3.1",
     "datoso-seed-vpinmame>=0.3.0",
     ]
-fbneo = [ "datoso-seed-fbneo>=0.3.2" ]
+fbneo = [ "datoso-seed-fbneo>=0.3.3" ]
 md-enhanced = [ "datoso-seed-md-enhanced>=0.3.0" ]
 nointro = [ "datoso-seed-nointro>=0.3.0" ]
 pleasuredome = [ "datoso-seed-pleasuredome>=0.3.2" ]
 redump = [ "datoso-seed-redump>=0.3.1" ]
 sfc-enhancedcolors = [ "datoso-seed-sfc-enhancedcolors>=0.3.0" ]
 sfc-msu1 = [ "datoso-seed-sfc-msu1>=0.3.0" ]
 sfc-speedhacks = [ "datoso-seed-sfc-speedhacks>=0.3.0" ]
```

### Comparing `datoso-0.3.8/src/datoso/__main__.py` & `datoso-0.3.9/src/datoso/__main__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/actions/processor.py` & `datoso-0.3.9/src/datoso/actions/processor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/commands/doctor.py` & `datoso-0.3.9/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/commands/seed.py` & `datoso-0.3.9/src/datoso/commands/seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/configuration/folder_helper.py` & `datoso-0.3.9/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/configuration/logger.py` & `datoso-0.3.9/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/database/__init__.py` & `datoso-0.3.9/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/database/models/datfile.py` & `datoso-0.3.9/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/database/seeds/dat_repos.py` & `datoso-0.3.9/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/database/seeds/dat_rules.py` & `datoso-0.3.9/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/datoso.ini` & `datoso-0.3.9/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/helpers/__init__.py` & `datoso-0.3.9/src/datoso/helpers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 __all__ = ['downloader']
 from contextlib import suppress
 from enum import Enum
 import re
 import os
 from pathlib import Path
+
 from dateutil import parser
 import shutil
 
 from datoso.helpers.download import downloader
 
 class Bcolors:
     # pylint: disable=anomalous-backslash-in-string
@@ -134,15 +135,18 @@
         os.makedirs(os.path.dirname(destination), exist_ok=True)
         try:
             shutil.move(origin, destination)
         except shutil.Error:
             FileUtils.remove(origin)
 
 class RequestUtils:
-    pass
+    @staticmethod
+    def urljoin(*args):
+        """ Join url parts. """
+        return '/'.join(args).replace('//', '/').replace(':/', '://')
 
 class FileHeaders(Enum):
     XML = '<?xml'
     CLRMAMEPRO = 'clrma'
 
 def show_progress(block_num, block_size, total_size):
     if total_size != -1:
```

### Comparing `datoso-0.3.8/src/datoso/helpers/download.py` & `datoso-0.3.9/src/datoso/helpers/download.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/helpers/executor.py` & `datoso-0.3.9/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/helpers/plugins.py` & `datoso-0.3.9/src/datoso/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/repositories/dat.py` & `datoso-0.3.9/src/datoso/repositories/dat.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/repositories/dedupe.py` & `datoso-0.3.9/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/seeds/unknown_seed.py` & `datoso-0.3.9/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/seeds.txt` & `datoso-0.3.9/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso/systems.json` & `datoso-0.3.9/src/datoso/systems.json`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso.egg-info/PKG-INFO` & `datoso-0.3.9/src/datoso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.3.8/src/datoso.egg-info/SOURCES.txt` & `datoso-0.3.9/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.3.8/src/datoso.egg-info/requires.txt` & `datoso-0.3.9/src/datoso.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 pydantic==1.10.9
 python-dateutil>=2.8.2
 xmltodict>=0.13.0
 tabulate>=0.9.0
 requests>=2.31.0
 
 [all]
-datoso-seed-fbneo>=0.3.2
+datoso-seed-fbneo>=0.3.3
 datoso-seed-md-enhanced>=0.3.0
 datoso-seed-nointro>=0.3.0
 datoso-seed-pleasuredome>=0.3.2
 datoso-seed-redump>=0.3.1
 datoso-seed-sfc-enhancedcolors>=0.3.0
 datoso-seed-sfc-msu1>=0.3.0
 datoso-seed-sfc-speedhacks>=0.3.0
@@ -18,15 +18,15 @@
 datoso-seed-vpinmame>=0.3.0
 
 [dev]
 ruff>=0.0.272
 line_profiler==4.0.3
 
 [fbneo]
-datoso-seed-fbneo>=0.3.2
+datoso-seed-fbneo>=0.3.3
 
 [md-enhanced]
 datoso-seed-md-enhanced>=0.3.0
 
 [nointro]
 datoso-seed-nointro>=0.3.0
```

