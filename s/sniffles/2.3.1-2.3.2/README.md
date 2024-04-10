# Comparing `tmp/sniffles-2.3.1.tar.gz` & `tmp/sniffles-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffles-2.3.1.tar", last modified: Wed Apr 10 19:32:59 2024, max compression
+gzip compressed data, was "sniffles-2.3.2.tar", last modified: Wed Apr 10 23:43:28 2024, max compression
```

## Comparing `sniffles-2.3.1.tar` & `sniffles-2.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.614698 sniffles-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 19:32:49.000000 sniffles-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-10 19:32:59.614698 sniffles-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-10 19:32:49.000000 sniffles-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 19:32:49.000000 sniffles-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 19:32:59.614698 sniffles-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-10 19:32:49.000000 sniffles-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.606698 sniffles-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.610698 sniffles-2.3.1/src/sniffles/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/consensus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25903 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/leadprov.py
--rw-r--r--   0 runner    (1001) docker     (127)    24149 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/snf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21208 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/sniffles
--rwxr-xr-x   0 runner    (1001) docker     (127)    24081 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/sv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.614698 sniffles-2.3.1/src/sniffles/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/utils/resmon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18412 2024-04-10 19:32:49.000000 sniffles-2.3.1/src/sniffles/vcf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:32:59.614698 sniffles-2.3.1/src/sniffles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 19:32:59.000000 sniffles-2.3.1/src/sniffles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.036682 sniffles-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 23:43:24.000000 sniffles-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-10 23:43:28.036682 sniffles-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-10 23:43:24.000000 sniffles-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 23:43:24.000000 sniffles-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 23:43:28.036682 sniffles-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-10 23:43:24.000000 sniffles-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.028682 sniffles-2.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.032682 sniffles-2.3.2/src/sniffles/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/consensus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25903 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/leadprov.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24149 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17736 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/snf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21307 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/sniffles
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24081 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/sv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.036682 sniffles-2.3.2/src/sniffles/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/utils/resmon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18412 2024-04-10 23:43:24.000000 sniffles-2.3.2/src/sniffles/vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:43:28.036682 sniffles-2.3.2/src/sniffles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 23:43:28.000000 sniffles-2.3.2/src/sniffles.egg-info/top_level.txt
```

### Comparing `sniffles-2.3.1/LICENSE` & `sniffles-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/PKG-INFO` & `sniffles-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.3.1
+Version: 2.3.2
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
 Author: Moritz Smolka, Hermann Romanek
 Author-email: moritz.g.smolka@gmail.com, sniffles@romanek.at
 License: MIT
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sniffles-2.3.1/README.md` & `sniffles-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/setup.cfg` & `sniffles-2.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sniffles
-version = 2.3.1
+version = 2.3.2
 author = Moritz Smolka, Hermann Romanek
 author_email = moritz.g.smolka@gmail.com, sniffles@romanek.at
 description = A fast structural variation caller for long-read sequencing data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fritzsedlazeck/Sniffles
 project_urls =
```

### Comparing `sniffles-2.3.1/src/sniffles/cluster.py` & `sniffles-2.3.2/src/sniffles/cluster.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/config.py` & `sniffles-2.3.2/src/sniffles/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import argparse
 
 from typing import Union, Optional
 
 from sniffles import util
 
 VERSION = "Sniffles2"
-BUILD = "2.3.1"
+BUILD = "2.3.2"
 SNF_VERSION = "S2_rc4"
 
 
 class ArgFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
     pass
```

### Comparing `sniffles-2.3.1/src/sniffles/consensus.py` & `sniffles-2.3.2/src/sniffles/consensus.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/leadprov.py` & `sniffles-2.3.2/src/sniffles/leadprov.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/parallel.py` & `sniffles-2.3.2/src/sniffles/parallel.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/postprocessing.py` & `sniffles-2.3.2/src/sniffles/postprocessing.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/result.py` & `sniffles-2.3.2/src/sniffles/result.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/snf.py` & `sniffles-2.3.2/src/sniffles/snf.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/sniffles` & `sniffles-2.3.2/src/sniffles/sniffles`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 #
 import logging
 import logging.config
 from typing import Optional
 
 from sniffles.utils.resmon import ResourceMonitor
 
-DEV_MONITOR_MEM = False
-
 import sys
 
 if not sys.version_info >= (3, 10):
     print(f"Error: Sniffles2 must be run with Python version 3.10 or above (detected Python version: {sys.version_info.major}.{sys.version_info.minor}). Exiting")
     exit(1)
 
 import math
@@ -31,15 +29,15 @@
 from sniffles.config import SnifflesConfig
 from sniffles import vcf
 from sniffles import snf
 from sniffles import parallel
 from sniffles import util
 
 # TODO: Dev/Debugging only - Remove for prod
-DEV_MONITOR_MEM = True
+DEV_MONITOR_MEM = False
 
 if DEV_MONITOR_MEM:
     try:
         import psutil
     except ImportError:
         logging.getLogger('sniffles.memory').warning('psutil not available.')
 
@@ -507,15 +505,16 @@
             'disable_existing_loggers': False,
         })
     except (ValueError, TypeError, AttributeError, ImportError):
         logging.exception(f'Error configuring loggers.')
 
     try:
         Sniffles2_Main(processes)
-    except (util.Sniffles2Exit, SystemExit):
+    except (util.Sniffles2Exit, SystemExit) as exit_code:
+        # print(f'Sniffles exit with code {exit_code}')
         if len(processes):
             # Allow time for child process error messages to propagate
             print("Sniffles2Main: Shutting down workers")
             time.sleep(10)
         for proc in processes:
             try:
                 proc.process.terminate()
@@ -523,10 +522,11 @@
                 pass
 
         for proc in processes:
             try:
                 proc.process.join()
             except:
                 pass
-        exit(1)
+        int_exit_code = exit_code.args[0]
+        exit(int_exit_code)
     except:
         logging.getLogger('sniffles.main').exception(f'Unhandled error while running sniffles.')
```

### Comparing `sniffles-2.3.1/src/sniffles/sv.py` & `sniffles-2.3.2/src/sniffles/sv.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/util.py` & `sniffles-2.3.2/src/sniffles/util.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/utils/resmon.py` & `sniffles-2.3.2/src/sniffles/utils/resmon.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles/vcf.py` & `sniffles-2.3.2/src/sniffles/vcf.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.3.1/src/sniffles.egg-info/PKG-INFO` & `sniffles-2.3.2/src/sniffles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.3.1
+Version: 2.3.2
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
 Author: Moritz Smolka, Hermann Romanek
 Author-email: moritz.g.smolka@gmail.com, sniffles@romanek.at
 License: MIT
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sniffles-2.3.1/src/sniffles.egg-info/SOURCES.txt` & `sniffles-2.3.2/src/sniffles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

