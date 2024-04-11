# Comparing `tmp/keria-0.1.3.tar.gz` & `tmp/keria-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keria-0.1.3.tar", last modified: Fri Mar  8 18:04:52 2024, max compression
+gzip compressed data, was "keria-0.2.0.dev0.tar", last modified: Thu Apr 11 17:18:00 2024, max compression
```

## Comparing `keria-0.1.3.tar` & `keria-0.2.0.dev0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.794468 keria-0.1.3/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 03:00:59.000000 keria-0.1.3/LICENSE
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1135 2024-03-08 18:04:52.794247 keria-0.1.3/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4137 2024-03-07 01:18:54.000000 keria-0.1.3/README.md
--rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-03-08 18:04:52.794516 keria-0.1.3/setup.cfg
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3006 2024-03-08 18:04:30.000000 keria-0.1.3/setup.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.784668 keria-0.1.3/src/
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.785848 keria-0.1.3/src/keria/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       98 2024-03-08 18:04:30.000000 keria-0.1.3/src/keria/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      331 2023-04-21 21:16:18.000000 keria-0.1.3/src/keria/__main__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.789512 keria-0.1.3/src/keria/app/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-04-21 21:16:18.000000 keria-0.1.3/src/keria/app/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    44455 2024-03-08 02:06:43.000000 keria-0.1.3/src/keria/app/agenting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    53979 2024-03-07 19:09:12.000000 keria-0.1.3/src/keria/app/aiding.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.789894 keria-0.1.3/src/keria/app/cli/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 03:00:59.000000 keria-0.1.3/src/keria/app/cli/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.790677 keria-0.1.3/src/keria/app/cli/commands/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 03:00:59.000000 keria-0.1.3/src/keria/app/cli/commands/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4243 2024-02-13 21:11:41.000000 keria-0.1.3/src/keria/app/cli/commands/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      623 2024-01-29 20:34:11.000000 keria-0.1.3/src/keria/app/cli/keria.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    37717 2024-03-08 18:04:30.000000 keria-0.1.3/src/keria/app/credentialing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6982 2024-03-07 01:18:54.000000 keria-0.1.3/src/keria/app/delegating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8222 2024-03-08 01:17:17.000000 keria-0.1.3/src/keria/app/grouping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4756 2024-03-07 14:29:22.000000 keria-0.1.3/src/keria/app/indirecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10599 2024-02-13 21:11:41.000000 keria-0.1.3/src/keria/app/ipexing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4254 2024-02-13 21:11:41.000000 keria-0.1.3/src/keria/app/notifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2355 2024-01-29 20:34:11.000000 keria-0.1.3/src/keria/app/specing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)       69 2024-01-29 20:34:11.000000 keria-0.1.3/src/keria/app/watching.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.792017 keria-0.1.3/src/keria/core/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 03:00:59.000000 keria-0.1.3/src/keria/core/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7008 2024-02-13 21:11:41.000000 keria-0.1.3/src/keria/core/authing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1587 2024-01-29 20:34:11.000000 keria-0.1.3/src/keria/core/httping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    14353 2023-05-17 14:10:05.000000 keria-0.1.3/src/keria/core/keeping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    17637 2024-02-26 18:39:13.000000 keria-0.1.3/src/keria/core/longrunning.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.792273 keria-0.1.3/src/keria/db/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-04-24 22:28:34.000000 keria-0.1.3/src/keria/db/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    22428 2024-02-13 21:44:06.000000 keria-0.1.3/src/keria/db/basing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.792982 keria-0.1.3/src/keria/end/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-04-24 22:28:34.000000 keria-0.1.3/src/keria/end/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2510 2024-02-13 21:44:06.000000 keria-0.1.3/src/keria/end/ending.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.793398 keria-0.1.3/src/keria/peer/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-02-13 21:11:41.000000 keria-0.1.3/src/keria/peer/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4875 2024-02-13 21:11:41.000000 keria-0.1.3/src/keria/peer/exchanging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.793751 keria-0.1.3/src/keria/testing/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-06-26 15:18:52.000000 keria-0.1.3/src/keria/testing/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    38007 2024-03-07 01:18:54.000000 keria-0.1.3/src/keria/testing/testing_helper.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-08 18:04:52.793957 keria-0.1.3/src/keria.egg-info/
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1135 2024-03-08 18:04:52.000000 keria-0.1.3/src/keria.egg-info/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1082 2024-03-08 18:04:52.000000 keria-0.1.3/src/keria.egg-info/SOURCES.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-03-08 18:04:52.000000 keria-0.1.3/src/keria.egg-info/dependency_links.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)       51 2024-03-08 18:04:52.000000 keria-0.1.3/src/keria.egg-info/entry_points.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-04-21 21:21:58.000000 keria-0.1.3/src/keria.egg-info/not-zip-safe
--rw-r--r--   0 pfeairheller   (501) staff       (20)      127 2024-03-08 18:04:52.000000 keria-0.1.3/src/keria.egg-info/requires.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        6 2024-03-08 18:04:52.000000 keria-0.1.3/src/keria.egg-info/top_level.txt
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.979848 keria-0.2.0.dev0/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 03:00:59.000000 keria-0.2.0.dev0/LICENSE
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1146 2024-04-11 17:18:00.979683 keria-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4138 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/README.md
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-04-11 17:18:00.979903 keria-0.2.0.dev0/setup.cfg
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3017 2024-04-11 17:02:04.000000 keria-0.2.0.dev0/setup.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.972041 keria-0.2.0.dev0/src/
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.973429 keria-0.2.0.dev0/src/keria/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      103 2024-04-11 17:02:04.000000 keria-0.2.0.dev0/src/keria/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      331 2023-04-21 21:16:18.000000 keria-0.2.0.dev0/src/keria/__main__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.976674 keria-0.2.0.dev0/src/keria/app/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-04-21 21:16:18.000000 keria-0.2.0.dev0/src/keria/app/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    44531 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/app/agenting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    56868 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/app/aiding.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.976931 keria-0.2.0.dev0/src/keria/app/cli/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 03:00:59.000000 keria-0.2.0.dev0/src/keria/app/cli/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.977232 keria-0.2.0.dev0/src/keria/app/cli/commands/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 03:00:59.000000 keria-0.2.0.dev0/src/keria/app/cli/commands/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4720 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/app/cli/commands/start.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      623 2024-01-29 20:34:11.000000 keria-0.2.0.dev0/src/keria/app/cli/keria.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    37927 2024-04-06 20:03:37.000000 keria-0.2.0.dev0/src/keria/app/credentialing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6980 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/app/delegating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8240 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/app/grouping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4762 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/app/indirecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    18584 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/app/ipexing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4254 2024-02-13 21:11:41.000000 keria-0.2.0.dev0/src/keria/app/notifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2355 2024-01-29 20:34:11.000000 keria-0.2.0.dev0/src/keria/app/specing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       69 2024-01-29 20:34:11.000000 keria-0.2.0.dev0/src/keria/app/watching.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.978116 keria-0.2.0.dev0/src/keria/core/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 03:00:59.000000 keria-0.2.0.dev0/src/keria/core/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7008 2024-02-13 21:11:41.000000 keria-0.2.0.dev0/src/keria/core/authing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1587 2024-01-29 20:34:11.000000 keria-0.2.0.dev0/src/keria/core/httping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    14353 2023-05-17 14:10:05.000000 keria-0.2.0.dev0/src/keria/core/keeping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    17632 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/core/longrunning.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.978325 keria-0.2.0.dev0/src/keria/db/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-04-24 22:28:34.000000 keria-0.2.0.dev0/src/keria/db/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    22428 2024-02-13 21:44:06.000000 keria-0.2.0.dev0/src/keria/db/basing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.978733 keria-0.2.0.dev0/src/keria/end/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-04-24 22:28:34.000000 keria-0.2.0.dev0/src/keria/end/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2510 2024-02-13 21:44:06.000000 keria-0.2.0.dev0/src/keria/end/ending.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.979071 keria-0.2.0.dev0/src/keria/peer/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-02-13 21:11:41.000000 keria-0.2.0.dev0/src/keria/peer/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4895 2024-04-06 20:03:11.000000 keria-0.2.0.dev0/src/keria/peer/exchanging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.979270 keria-0.2.0.dev0/src/keria/testing/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-06-26 15:18:52.000000 keria-0.2.0.dev0/src/keria/testing/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    38133 2024-04-08 02:28:32.000000 keria-0.2.0.dev0/src/keria/testing/testing_helper.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-04-11 17:18:00.979454 keria-0.2.0.dev0/src/keria.egg-info/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1146 2024-04-11 17:18:00.000000 keria-0.2.0.dev0/src/keria.egg-info/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1082 2024-04-11 17:18:00.000000 keria-0.2.0.dev0/src/keria.egg-info/SOURCES.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-04-11 17:18:00.000000 keria-0.2.0.dev0/src/keria.egg-info/dependency_links.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       51 2024-04-11 17:18:00.000000 keria-0.2.0.dev0/src/keria.egg-info/entry_points.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-04-21 21:21:58.000000 keria-0.2.0.dev0/src/keria.egg-info/not-zip-safe
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      133 2024-04-11 17:18:00.000000 keria-0.2.0.dev0/src/keria.egg-info/requires.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        6 2024-04-11 17:18:00.000000 keria-0.2.0.dev0/src/keria.egg-info/top_level.txt
```

### Comparing `keria-0.1.3/LICENSE` & `keria-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/PKG-INFO` & `keria-0.2.0.dev0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keria
-Version: 0.1.3
+Version: 0.2.0.dev0
 Summary: KERIA: KERI Agent in the cloud
 Home-page: https://github.com/WebOfTrust/keria
 Author: Philip S. Feairheller
 Author-email: pfeairheller@gmail.com
 License: Apache Software License 2.0
 Project-URL: Issue Tracker, https://github.com/WebOfTrust/keria/issues
 Keywords: secure attribution,authentic data,discovery,resolver
@@ -13,19 +13,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10.4
+Requires-Python: >=3.12.2
 License-File: LICENSE
-Requires-Dist: hio>=0.6.9
-Requires-Dist: keri>=1.1.6
+Requires-Dist: hio>=0.6.12
+Requires-Dist: keri>=1.2.0-dev0
 Requires-Dist: mnemonic>=0.20
 Requires-Dist: multicommand>=1.0.0
-Requires-Dist: falcon>=3.1.0
+Requires-Dist: falcon>=3.1.3
 Requires-Dist: http_sfv>=0.9.8
 Requires-Dist: dataclasses_json>=0.5.7
 Requires-Dist: apispec>=6.3.0
 
 KERIA: KERI Agent in the cloud.
```

### Comparing `keria-0.1.3/README.md` & `keria-0.2.0.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Agents use KERI HIO to handle all of the different asynchronous actions that are occuring. HIO is an efficient and scalable orchestration/processing mechanism that leverages queues, handlers, coroutines, etc.
 All Agent db access is through the associated Agent.
 
 ## Development
 
 ### Setup
 
-* Ensure [Python](https://www.python.org/downloads/) `version 3.10.4+` is installed
+* Ensure [Python](https://www.python.org/downloads/) `version 3.12.14+` is installed
 * Install [Keripy dependency](https://github.com/WebOfTrust/keripy#dependencies) (`libsodium 1.0.18+`)
 
 
 #### Build from source
 
 * Setup virtual environment:
     ```bash
```

### Comparing `keria-0.1.3/setup.py` & `keria-0.2.0.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from os.path import splitext
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='keria',
-    version='0.1.3',  # also change in src/keria/__init__.py
+    version='0.2.0-dev0',  # also change in src/keria/__init__.py
     license='Apache Software License 2.0',
     description='KERIA: KERI Agent in the cloud',
     long_description="KERIA: KERI Agent in the cloud.",
     author='Philip S. Feairheller',
     author_email='pfeairheller@gmail.com',
     url='https://github.com/WebOfTrust/keria',
     packages=find_packages('src'),
@@ -69,21 +69,21 @@
     keywords=[
         "secure attribution",
         "authentic data",
         "discovery",
         "resolver",
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
-    python_requires='>=3.10.4',
+    python_requires='>=3.12.2',
     install_requires=[
-        'hio>=0.6.9',
-        'keri>=1.1.6',
+        'hio>=0.6.12',
+        'keri>=1.2.0-dev0',
         'mnemonic>=0.20',
         'multicommand>=1.0.0',
-        'falcon>=3.1.0',
+        'falcon>=3.1.3',
         'http_sfv>=0.9.8',
         'dataclasses_json>=0.5.7',
         'apispec>=6.3.0',
     ],
     extras_require={
         # eg:
         #   'rst': ['docutils>=0.11'],
```

### Comparing `keria-0.1.3/src/keria/app/agenting.py` & `keria-0.2.0.dev0/src/keria/app/agenting.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 
 """
 import json
 import os
 from dataclasses import asdict
 from urllib.parse import urlparse, urljoin
 
-from keri import kering
-from keri.app.notifying import Notifier
-from keri.app.storing import Mailboxer
 
 import falcon
 from falcon import media
 from hio.base import doing
 from hio.core import http, tcp
 from hio.help import decking
+
+from keri import kering
+from keri import core
+from keri.app.notifying import Notifier
+from keri.app.storing import Mailboxer
+
+
 from keri.app import configing, keeping, habbing, storing, signaling, oobiing, agenting, \
     forwarding, querying, connecting, grouping
 from keri.app.grouping import Counselor
 from keri.app.keeping import Algos
 from keri.core import coring, parsing, eventing, routing, serdering
 from keri.core.coring import Ilks, randomNonce
 from keri.db import dbing
@@ -145,15 +149,15 @@
         server = http.Server(port=port, app=app)
     return server
 
 
 class Agency(doing.DoDoer):
     """
     Agency
-    
+
     """
 
     def __init__(self, name, bran, base="", configFile=None, configDir=None, adb=None, temp=False):
         self.name = name
         self.base = base
         self.bran = bran
         self.temp = temp
@@ -169,15 +173,15 @@
                                          clear=False)
 
         self.agents = dict()
 
         self.adb = adb if adb is not None else basing.AgencyBaser(name="TheAgency", base=base, reopen=True, temp=temp)
         super(Agency, self).__init__(doers=[], always=True)
 
-    def create(self, caid):
+    def create(self, caid, salt=None):
         ks = keeping.Keeper(name=caid,
                             base=self.base,
                             temp=self.temp,
                             reopen=True)
 
         cf = None
         if self.cf is not None:  # Load config file if creating database
@@ -192,15 +196,15 @@
                                     human=False,
                                     temp=self.temp,
                                     reopen=True,
                                     clear=False)
             cf.put(data)
 
         # Create the Hab for the Agent with only 2 AIDs
-        agentHby = habbing.Habery(name=caid, base=self.base, bran=self.bran, ks=ks, cf=cf, temp=self.temp)
+        agentHby = habbing.Habery(name=caid, base=self.base, bran=self.bran, ks=ks, cf=cf, temp=self.temp, salt=salt)
         agentHab = agentHby.makeHab(f"agent-{caid}", ns="agent", transferable=True, delpre=caid)
         agentRgy = Regery(hby=agentHby, name=agentHab.name, base=self.base, temp=self.temp)
 
         agent = Agent(agentHby, agentRgy, agentHab,
                       caid=caid,
                       agency=self,
                       configDir=self.configDir,
@@ -283,15 +287,15 @@
     def __init__(self, hby, rgy, agentHab, agency, caid, **opts):
         self.hby = hby
         self.rgy = rgy
         self.agentHab = agentHab
         self.agency = agency
         self.caid = caid
 
-        self.swain = delegating.Sealer(hby=hby, proxy=agentHab)
+        self.swain = delegating.Anchorer(hby=hby, proxy=agentHab)
         self.counselor = Counselor(hby=hby, swain=self.swain, proxy=agentHab)
         self.org = connecting.Organizer(hby=hby)
 
         oobiery = oobiing.Oobiery(hby=hby)
 
         self.mgr = RemoteManager(hby=hby)
 
@@ -810,15 +814,15 @@
             raise falcon.HTTPBadRequest(title="invalid inception",
                                         description=f'required field "icp" missing from body')
         icp = serdering.SerderKERI(sad=body["icp"])
 
         if "sig" not in body:
             raise falcon.HTTPBadRequest(title="invalid inception",
                                         description=f'required field "sig" missing from body')
-        siger = coring.Siger(qb64=body["sig"])
+        siger = core.Siger(qb64=body["sig"])
 
         caid = icp.pre
 
         if self.agency.get(caid=caid) is not None:
             raise falcon.HTTPBadRequest(title="agent already exists",
                                         description=f"agent for controller {caid} already exists")
 
@@ -968,20 +972,20 @@
         if "pre" not in req.params:
             raise falcon.HTTPBadRequest(description="required parameter 'pre' missing")
 
         pre = req.params.get("pre")
         preb = pre.encode("utf-8")
         events = []
         for fn, dig in agent.hby.db.getFelItemPreIter(preb, fn=0):
-            dgkey = dbing.dgKey(preb, dig)  # get message
-            if not (raw := agent.hby.db.getEvt(key=dgkey)):
+            if not (raw := agent.hby.db.cloneEvtMsg(pre=preb, fn=fn, dig=dig)):
                 raise falcon.HTTPInternalServerError(f"Missing event for dig={dig}.")
 
             serder = serdering.SerderKERI(raw=bytes(raw))
-            events.append(serder.ked)
+            atc = raw[serder.size:]
+            events.append(dict(ked=serder.ked, atc=atc.decode("utf-8")))
 
         rep.status = falcon.HTTP_200
         rep.content_type = "application/json"
         rep.data = json.dumps(events).encode("utf-8")
 
 
 class OOBICollectionEnd:
```

### Comparing `keria-0.1.3/src/keria/app/aiding.py` & `keria-0.2.0.dev0/src/keria/app/aiding.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 import json
 from dataclasses import asdict
 from urllib.parse import urlparse, urljoin
 
 import falcon
 from keri import kering
+from keri import core
 from keri.app import habbing
 from keri.app.keeping import Algos
 from keri.core import coring, serdering
 from keri.core.coring import Ilks
 from keri.db import dbing
 from keri.help import ogler
 from mnemonic import mnemonic
@@ -27,14 +28,15 @@
     groupEnd = AgentResourceEnd(agency=agency, authn=authn)
     app.add_route("/agent/{caid}", groupEnd)
 
     aidsEnd = IdentifierCollectionEnd()
     app.add_route("/identifiers", aidsEnd)
     aidEnd = IdentifierResourceEnd()
     app.add_route("/identifiers/{name}", aidEnd)
+    app.add_route("/identifiers/{name}/events", aidEnd)
 
     aidOOBIsEnd = IdentifierOOBICollectionEnd()
     app.add_route("/identifiers/{name}/oobis", aidOOBIsEnd)
 
     endRolesEnd = EndRoleCollectionEnd()
     app.add_route("/identifiers/{name}/endroles", endRolesEnd)
     app.add_route("/identifiers/{name}/endroles/{role}", endRolesEnd)
@@ -91,15 +93,20 @@
 
         if agent.pre not in agent.hby.kevers:
             raise falcon.HTTPBadRequest(description=f"invalid agent configuration, {agent.pre} not found")
 
         if agent.caid not in agent.hby.kevers:
             raise falcon.HTTPBadRequest(description=f"invalid controller configuration, {agent.caid} not found")
 
-        pidx = agent.hby.db.habs.cntAll()
+        pidx = 0
+        for name, _ in agent.hby.db.names.getItemIter():
+            if name[0] != "agent":
+                pidx += 1
+
+        # pidx = agent.hby.db.habs.cntAll()
 
         state = asdict(agent.hby.kevers[agent.caid].state())
         key = dbing.dgKey(state['i'], state['ee']['d'])  # digest key
         msg = agent.hby.db.getEvt(key)
         eserder = serdering.SerderKERI(raw=bytes(msg))
 
         body = dict(
@@ -151,19 +158,19 @@
         if "keys" not in body:
             raise falcon.HTTPBadRequest(description="required field 'keys' missing from body")
 
         rot = serdering.SerderKERI(sad=body["rot"])
         sigs = body["sigs"]
 
         ctrlHab = agent.hby.habByName(caid, ns="agent")
-        ctrlHab.rotate(serder=rot, sigers=[coring.Siger(qb64=sig) for sig in sigs])
+        ctrlHab.rotate(serder=rot, sigers=[core.Siger(qb64=sig) for sig in sigs])
 
         if not self.authn.verify(req):
             raise falcon.HTTPForbidden(description="invalid signature on request")
-        
+
         sxlt = body["sxlt"]
         agent.mgr.sxlt = sxlt
 
         keys = body["keys"]
         for pre, val in keys.items():
             if "sxlt" in val:
                 if (sp := agent.mgr.rb.sprms.get(pre)) is None:
@@ -206,15 +213,15 @@
 
         if "sigs" not in body:
             raise falcon.HTTPBadRequest(description="required field 'sigs' missing from body")
 
         ked = body['ixn']
         sigs = body['sigs']
         ixn = serdering.SerderKERI(sad=ked)
-        sigers = [coring.Siger(qb64=sig) for sig in sigs]
+        sigers = [core.Siger(qb64=sig) for sig in sigs]
 
         ctrlHab = agent.hby.habByName(caid, ns="agent")
 
         ctrlHab.interact(serder=ixn, sigers=sigers)
         agent.agentHab.kvy.processEvent(serder=ixn, sigers=sigers)
 
         rep.status = falcon.HTTP_204
@@ -265,34 +272,35 @@
             start = 0
             end = 9
         else:
             rep.status = falcon.HTTP_206
             start, end = httping.parseRangeHeader(rng, "aids")
 
         count = agent.hby.db.habs.cntAll()
-        it = agent.hby.db.habs.getItemIter()
+        it = agent.hby.db.names.getItemIter()
         for _ in range(start):
             try:
                 next(it)
             except StopIteration:
                 break
 
-        for name, habord in it:
-            name = ".".join(name)  # detupleize the database key name
+        for (ns, name), pre in it:
+            if ns == "agent":
+                continue
 
-            hab = agent.hby.habByName(name)
+            hab = agent.hby.habs[pre]
             data = info(hab, agent.mgr)
             res.append(data)
 
             if (not end == -1) and len(res) == (end - start) + 1:
                 break
 
         end = start + (len(res) - 1) if len(res) > 0 else 0
         rep.set_header("Accept-Ranges", "aids")
-        rep.set_header("Content-Range", f"aids {start}-{end}/{count}")
+        rep.set_header("Content-Range", f"aids {start}-{end}/{count - 1}")
         rep.content_type = "application/json"
         rep.data = json.dumps(res).encode("utf-8")
 
     @staticmethod
     def on_post(req, rep):
         """ Inception event POST endpoint
 
@@ -306,15 +314,15 @@
             body = req.get_media()
             icp = httping.getRequiredParam(body, "icp")
             name = httping.getRequiredParam(body, "name")
             sigs = httping.getRequiredParam(body, "sigs")
 
             serder = serdering.SerderKERI(sad=icp)
 
-            sigers = [coring.Siger(qb64=sig) for sig in sigs]
+            sigers = [core.Siger(qb64=sig) for sig in sigs]
 
             if agent.hby.habByName(name) is not None:
                 raise falcon.HTTPBadRequest(title=f"AID with name {name} already incepted")
 
             if 'b' in icp:
                 for wit in icp['b']:
                     urls = agent.agentHab.fetchUrls(eid=wit, scheme=kering.Schemes.http)
@@ -346,26 +354,28 @@
                                                             f"event for this group hab.")
 
                 if "ndigs" not in group:
                     raise falcon.HTTPBadRequest(description=f'required field "ndigs" missing from body.group')
                 ndigs = group["ndigs"]
                 digers = [coring.Diger(qb64=ndig) for ndig in ndigs]
 
-                smids = httping.getRequiredParam(body, "smids")
-                rmids = httping.getRequiredParam(body, "rmids")
-
-                hab = agent.hby.makeSignifyGroupHab(name, mhab=mhab, serder=serder, sigers=sigers)
+                states = httping.getRequiredParam(body, "smids")
+                rstates = httping.getRequiredParam(body, "rmids")
+                smids = [state['i'] for state in states]
+                rmids = [rstate['i'] for rstate in rstates]
+                hab = agent.hby.makeSignifyGroupHab(name, mhab=mhab, smids=smids, rmids=rmids, serder=serder,
+                                                    sigers=sigers)
                 try:
                     agent.inceptGroup(pre=serder.pre, mpre=mhab.pre, verfers=verfers, digers=digers)
                 except ValueError as e:
                     agent.hby.deleteHab(name=name)
                     raise falcon.HTTPInternalServerError(description=f"{e.args[0]}")
 
                 # Generate response, a long running operaton indicator for the type
-                agent.groups.append(dict(pre=hab.pre, serder=serder, sigers=sigers, smids=smids, rmids=rmids))
+                agent.groups.append(dict(pre=hab.pre, serder=serder, sigers=sigers, smids=states, rmids=rstates))
                 op = agent.monitor.submit(serder.pre, longrunning.OpTypes.group, metadata=dict(sn=0))
 
                 rep.content_type = "application/json"
                 rep.status = falcon.HTTP_202
                 rep.data = op.to_json().encode("utf-8")
 
             else:
@@ -401,15 +411,15 @@
                 else:
                     raise falcon.HTTPBadRequest(
                         description="invalid request: one of group, rand or salt field required")
 
                 # create Hab and incept the key store (if any)
                 # Generate response, either the serder or a long running operaton indicator for the type
                 rep.content_type = "application/json"
-                if hab.kever.delegator:
+                if hab.kever.delpre:
                     agent.anchors.append(dict(pre=hab.pre, sn=0))
                     op = agent.monitor.submit(hab.kever.prefixer.qb64, longrunning.OpTypes.delegation,
                                               metadata=dict(pre=hab.pre, sn=0))
                     rep.status = falcon.HTTP_202
                     rep.data = op.to_json().encode("utf-8")
 
                 elif hab.kever.wits:
@@ -452,45 +462,97 @@
 
         data = info(hab, agent.mgr, full=True)
         rep.status = falcon.HTTP_200
         rep.content_type = "application/json"
         rep.data = json.dumps(data).encode("utf-8")
 
     def on_put(self, req, rep, name):
-        """ Identifier UPDATE endpoint
+        """ Identifier rename endpoint
+
+        Parameters:
+            req (Request): falcon.Request HTTP request object
+            rep (Response): falcon.Response HTTP response object
+            name (str): human readable name for Hab to rename
+
+        """
+        if not name:
+            raise falcon.HTTPBadRequest(description="name is required")
+        agent = req.context.agent
+        hab = agent.hby.habByName(name)
+
+        if hab is None:
+            raise falcon.HTTPNotFound(title=f"No AID with name {name} found")
+        body = req.get_media()
+        newName = body.get("name")
+        habord = hab.db.habs.get(keys=(hab.pre,))
+        habord.name = newName
+        hab.db.habs.pin(keys=(hab.pre,),
+                        val=habord)
+        hab.db.names.pin(keys=("", newName), val=hab.pre)
+        hab.db.names.rem(keys=("", name))
+        hab.name = newName
+        hab = agent.hby.habByName(newName)
+        data = info(hab, agent.mgr, full=True)
+        rep.status = falcon.HTTP_200
+        rep.content_type = "application/json"
+        rep.data = json.dumps(data).encode("utf-8")
+
+    def on_delete(self, req, rep, name):
+        """ Identifier delete endpoint
+
+        Parameters:
+            req (Request): falcon.Request HTTP request object
+            rep (Response): falcon.Response HTTP response object
+            name (str): human readable name for Hab to delete
+
+        """
+        if not name:
+            raise falcon.HTTPBadRequest(description="name is required")
+        agent = req.context.agent
+        hab = agent.hby.habByName(name)
+        if hab is None:
+            raise falcon.HTTPNotFound(title=f"No AID with name {name} found")
+        agent.hby.deleteHab(name)
+        rep.status = falcon.HTTP_200
+
+    def on_post(self, req, rep, name):
+        """ Identifier events endpoint
 
         Parameters:
             req (Request): falcon.Request HTTP request object
             rep (Response): falcon.Response HTTP response object
             name (str): human readable name for Hab to rotate or interact
 
         """
+        if not name:
+            raise falcon.HTTPBadRequest(description="name is required")
         agent = req.context.agent
         try:
             body = req.get_media()
-            typ = Ilks.ixn if req.params.get("type") == "ixn" else Ilks.rot
-
-            if typ in (Ilks.rot,):
+            if body.get("rot") is not None:
                 op = self.rotate(agent, name, body)
-            else:
+            elif body.get("ixn") is not None:
                 op = self.interact(agent, name, body)
+            else:
+                raise falcon.HTTPBadRequest(title="invalid request",
+                                            description=f"required field 'rot' or 'ixn' missing from request")
 
             rep.status = falcon.HTTP_200
             rep.content_type = "application/json"
             rep.data = op.to_json().encode("utf-8")
 
         except (kering.AuthError, ValueError) as e:
             raise falcon.HTTPBadRequest(description=e.args[0])
 
     @staticmethod
     def rotate(agent, name, body):
         hab = agent.hby.habByName(name)
         if hab is None:
             raise falcon.HTTPNotFound(title=f"No AID with name {name} found")
-               
+
         rot = body.get("rot")
         if rot is None:
             raise falcon.HTTPBadRequest(title="invalid rotation",
                                         description=f"required field 'rot' missing from request")
 
         if 'ba' in rot:
             for wit in rot['ba']:
@@ -500,15 +562,15 @@
 
         sigs = body.get("sigs")
         if sigs is None or len(sigs) == 0:
             raise falcon.HTTPBadRequest(title="invalid rotation",
                                         description=f"required field 'sigs' missing from request")
 
         serder = serdering.SerderKERI(sad=rot)
-        sigers = [coring.Siger(qb64=sig) for sig in sigs]
+        sigers = [core.Siger(qb64=sig) for sig in sigs]
 
         hab.rotate(serder=serder, sigers=sigers)
 
         if Algos.salty in body:
             salt = body[Algos.salty]
             keeper = agent.mgr.get(Algos.salty)
 
@@ -533,15 +595,15 @@
             rmids = httping.getRequiredParam(body, "rmids")
 
             agent.groups.append(dict(pre=hab.pre, serder=serder, sigers=sigers, smids=smids, rmids=rmids))
             op = agent.monitor.submit(serder.pre, longrunning.OpTypes.group, metadata=dict(sn=serder.sn))
 
             return op
 
-        if hab.kever.delegator:
+        if hab.kever.delpre:
             agent.anchors.append(dict(alias=name, pre=hab.pre, sn=serder.sn))
             op = agent.monitor.submit(hab.kever.prefixer.qb64, longrunning.OpTypes.delegation,
                                       metadata=dict(pre=hab.pre, sn=serder.sn))
             return op
 
         if hab.kever.wits:
             agent.witners.append(dict(serder=serder))
@@ -566,15 +628,15 @@
 
         sigs = body.get("sigs")
         if sigs is None or len(sigs) == 0:
             raise falcon.HTTPBadRequest(title="invalid interaction",
                                         description=f"required field 'sigs' missing from request")
 
         serder = serdering.SerderKERI(sad=ixn)
-        sigers = [coring.Siger(qb64=sig) for sig in sigs]
+        sigers = [core.Siger(qb64=sig) for sig in sigs]
 
         hab.interact(serder=serder, sigers=sigers)
 
         if "group" in body:
             agent.groups.append(dict(pre=hab.pre, serder=serder, sigers=sigers))
             op = agent.monitor.submit(serder.pre, longrunning.OpTypes.group, metadata=dict(sn=serder.sn))
 
@@ -607,15 +669,15 @@
 
     if hab.accepted and full:
         kever = hab.kevers[hab.pre]
         data["transferable"] = kever.transferable
         data["state"] = asdict(kever.state())
         dgkey = dbing.dgKey(kever.prefixer.qb64b, kever.serder.saidb)
         wigs = hab.db.getWigs(dgkey)
-        data["windexes"] = [coring.Siger(qb64b=bytes(wig)).index for wig in wigs]
+        data["windexes"] = [core.Siger(qb64b=bytes(wig)).index for wig in wigs]
 
     return data
 
 
 class IdentifierOOBICollectionEnd:
     """
       This class represents the OOBI subresource collection endpoint for identifiers
@@ -645,34 +707,39 @@
 
         role = req.params["role"]
 
         res = dict(role=role)
         if role in (kering.Roles.witness,):  # Fetch URL OOBIs for all witnesses
             oobis = []
             for wit in hab.kever.wits:
-                urls = hab.fetchUrls(eid=wit, scheme=kering.Schemes.http) or hab.fetchUrls(eid=wit, scheme=kering.Schemes.https)
+                urls = hab.fetchUrls(eid=wit, scheme=kering.Schemes.http) or hab.fetchUrls(eid=wit,
+                                                                                           scheme=kering.Schemes.https)
                 if not urls:
                     raise falcon.HTTPNotFound(description=f"unable to query witness {wit}, no http endpoint")
 
                 url = urls[kering.Schemes.http] if kering.Schemes.http in urls else urls[kering.Schemes.https]
                 up = urlparse(url)
                 oobis.append(urljoin(up.geturl(), f"/oobi/{hab.pre}/witness/{wit}"))
             res["oobis"] = oobis
         elif role in (kering.Roles.controller,):  # Fetch any controller URL OOBIs
             oobis = []
-            urls = hab.fetchUrls(eid=hab.pre, scheme=kering.Schemes.http) or hab.fetchUrls(eid=hab.pre, scheme=kering.Schemes.https)
+            urls = hab.fetchUrls(eid=hab.pre, scheme=kering.Schemes.http) or hab.fetchUrls(eid=hab.pre,
+                                                                                           scheme=kering.Schemes.https)
             if not urls:
                 raise falcon.HTTPNotFound(description=f"unable to query controller {hab.pre}, no http endpoint")
 
             url = urls[kering.Schemes.http] if kering.Schemes.http in urls else urls[kering.Schemes.https]
             up = urlparse(url)
             oobis.append(urljoin(up.geturl(), f"/oobi/{hab.pre}/controller"))
             res["oobis"] = oobis
         elif role in (kering.Roles.agent,):  # Fetch URL OOBIs for all witnesses
-            roleUrls = hab.fetchRoleUrls(cid=hab.pre, role=kering.Roles.agent, scheme=kering.Schemes.http) or hab.fetchRoleUrls(cid=hab.pre, role=kering.Roles.agent, scheme=kering.Schemes.https)
+            roleUrls = hab.fetchRoleUrls(cid=hab.pre, role=kering.Roles.agent,
+                                         scheme=kering.Schemes.http) or hab.fetchRoleUrls(cid=hab.pre,
+                                                                                          role=kering.Roles.agent,
+                                                                                          scheme=kering.Schemes.https)
             if kering.Roles.agent not in roleUrls:
                 res['oobis'] = []
             else:
                 aoobis = roleUrls[kering.Roles.agent]
 
                 oobis = list()
                 for agent in set(aoobis.keys()):
@@ -788,15 +855,15 @@
         if hab is None:
             raise falcon.errors.HTTPNotFound(description=f"invalid alias {name}")
 
         if pre != hab.pre:
             raise falcon.errors.HTTPBadRequest(
                 description=f"error trying to create end role for unknown local AID {pre}")
 
-        rsigers = [coring.Siger(qb64=rsig) for rsig in rsigs]
+        rsigers = [core.Siger(qb64=rsig) for rsig in rsigs]
         tsg = (hab.kever.prefixer, coring.Seqner(sn=hab.kever.sn), coring.Saider(qb64=hab.kever.serder.said), rsigers)
         try:
             agent.hby.rvy.processReply(rserder, tsgs=[tsg])
         except kering.UnverifiedReplyError:
             pass
 
         oid = ".".join([pre, role, eid])
@@ -1141,14 +1208,18 @@
             rep.status = falcon.HTTP_200
             rep.data = json.dumps(data).encode("utf-8")
 
     @staticmethod
     def authn(agent, contacts):
         for contact in contacts:
             aid = contact['id']
+
+            ends = agent.agentHab.endsFor(aid)
+            contact['ends'] = ends
+
             accepted = [saider.qb64 for saider in agent.hby.db.chas.get(keys=(aid,))]
             received = [saider.qb64 for saider in agent.hby.db.reps.get(keys=(aid,))]
 
             challenges = []
             for said in received:
                 exn = agent.hby.db.exns.get(keys=(said,))
                 challenges.append(dict(dt=exn.ked['dt'], words=exn.ked['a']['words'], said=said,
```

### Comparing `keria-0.1.3/src/keria/app/cli/commands/start.py` & `keria-0.2.0.dev0/src/keria/app/cli/commands/start.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,19 +56,25 @@
                     help="directory override for configuration data")
 parser.add_argument("--keypath", action="store", required=False, default=None,
                     help="TLS server private key file")
 parser.add_argument("--certpath", action="store", required=False, default=None,
                     help="TLS server signed certificate (public key) file")
 parser.add_argument("--cafilepath", action="store", required=False, default=None,
                     help="TLS server CA certificate chain")
+parser.add_argument("--loglevel", action="store", required=False, default="CRITICAL",
+                    help="Set log level to DEBUG | INFO | WARNING | ERROR | CRITICAL. Default is CRITICAL")
+parser.add_argument("--logfile", action="store", required=False, default=None,
+                    help="path of the log file. If not defined, logs will not be written to the file.")
 
 
 def launch(args):
-    help.ogler.level = logging.CRITICAL
-    help.ogler.reopen(name=args.name, temp=True, clear=True)
+    help.ogler.level = logging.getLevelName(args.loglevel)
+    if(args.logfile != None):
+        help.ogler.headDirPath = args.logfile
+        help.ogler.reopen(name=args.name, temp=False, clear=True)
 
     logger = help.ogler.getLogger()
 
     logger.info("******* Starting Agent for %s listening: admin/%s, http/%s "
                 ".******", args.name, args.admin, args.http)
 
     runAgent(name=args.name,
```

### Comparing `keria-0.1.3/src/keria/app/cli/keria.py` & `keria-0.2.0.dev0/src/keria/app/cli/keria.py`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/src/keria/app/credentialing.py` & `keria-0.2.0.dev0/src/keria/app/credentialing.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,17 @@
         ked = httping.getRequiredParam(body, "ixn")
         ixn = serdering.SerderKERI(sad=ked)
 
         hab = agent.hby.habByName(name)
         if hab is None:
             raise falcon.HTTPNotFound(description="alias is not a valid reference to an identifier")
 
+        if agent.rgy.registryByName(name=rname) is not None:
+            raise falcon.HTTPBadRequest(description=f"registry name {rname} already in use")
+
         registry = agent.rgy.makeSignifyRegistry(name=rname, prefix=hab.pre, regser=vcp)
 
         if hab.kever.estOnly:
             op = self.identifierResource.rotate(agent, name, body)
         else:
             op = self.identifierResource.interact(agent, name, body)
 
@@ -279,14 +282,15 @@
                         description=f"{registryName} is not a valid reference to a credential registry")
 
                 regser = serdering.SerderKERI(raw=bytes(raw))
                 registry = agent.rgy.makeSignifyRegistry(name, hab.pre, regser)
 
         regord = viring.RegistryRecord(registryKey=registry.regk, prefix=hab.pre)
         agent.rgy.reger.regs.pin(keys=(name,), val=regord)
+        agent.rgy.reger.regs.rem(keys=(registryName,))
         registry.name = name
 
         rd = dict(
             name=registry.name,
             regk=registry.regk,
             pre=registry.hab.pre,
             state=asdict(registry.tever.state())
```

### Comparing `keria-0.1.3/src/keria/app/delegating.py` & `keria-0.2.0.dev0/src/keria/app/delegating.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from hio.base import doing
 from keri import kering
 from keri.app import forwarding, agenting, habbing
 from keri.core import coring, serdering
 from keri.db import dbing
 
 
-class Sealer(doing.DoDoer):
+class Anchorer(doing.DoDoer):
     """
     Sends messages to Delegator of an identifier and wait for the anchoring event to
     be processed to ensure the inception or rotation event has been approved by the delegator.
 
     Removes all Doers and exits as Done once the event has been anchored.
 
     """
@@ -28,24 +28,24 @@
         """
         self.hby = hby
         self.postman = forwarding.Poster(hby=hby)
         self.witq = agenting.WitnessInquisitor(hby=hby)
         self.witDoer = agenting.Receiptor(hby=self.hby)
         self.proxy = proxy
 
-        super(Sealer, self).__init__(doers=[self.witq, self.witDoer, self.postman, doing.doify(self.escrowDo)],
+        super(Anchorer, self).__init__(doers=[self.witq, self.witDoer, self.postman, doing.doify(self.escrowDo)],
                                      **kwa)
 
     def delegation(self, pre, sn=None, proxy=None):
         if pre not in self.hby.habs:
             raise kering.ValidationError(f"{pre} is not a valid local AID for delegation")
 
         # load the hab of the delegated identifier to anchor
         hab = self.hby.habs[pre]
-        delpre = hab.kever.delegator  # get the delegator identifier
+        delpre = hab.kever.delpre  # get the delegator identifier
         if delpre not in hab.kevers:
             raise kering.ValidationError(f"delegator {delpre} not found, unable to process delegation")
 
         sn = sn if sn is not None else hab.kever.sner.num
 
         # load the event and signatures
         evt = hab.makeOwnEvent(sn=sn)
@@ -122,15 +122,15 @@
         Process escrow of partially signed multisig group KEL events.  Message
         processing will send this local controllers signature to all other participants
         then this escrow waits for signatures from all other participants
 
         """
         for (pre, said), serder in self.hby.db.dune.getItemIter():  # group partial witness escrow
             kever = self.hby.kevers[pre]
-            dkever = self.hby.kevers[kever.delegator]
+            dkever = self.hby.kevers[kever.delpre]
 
             seal = dict(i=serder.pre, s=serder.snh, d=serder.said)
             if dserder := self.hby.db.findAnchoringSealEvent(dkever.prefixer.qb64, seal=seal):
                 seqner = coring.Seqner(sn=dserder.sn)
                 couple = seqner.qb64b + dserder.saidb
                 dgkey = dbing.dgKey(kever.prefixer.qb64b, kever.serder.saidb)
                 self.hby.db.setAes(dgkey, couple)  # authorizer event seal (delegator/issuer)
```

### Comparing `keria-0.1.3/src/keria/app/grouping.py` & `keria-0.2.0.dev0/src/keria/app/grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 KERIA
 keria.app.grouping module
 
 """
 import json
 
 import falcon
+from keri import core
 from keri.app import habbing
 from keri.core import coring, eventing, serdering
 from keri.kering import SerializeError
 
 from keria.core import httping, longrunning
 
 
@@ -52,15 +53,15 @@
         # grab all of the required parameters
         ked = httping.getRequiredParam(body, "exn")
         serder = serdering.SerderKERI(sad=ked)
         sigs = httping.getRequiredParam(body, "sigs")
         atc = httping.getRequiredParam(body, "atc")
 
         # create sigers from the edge signatures so we can messagize the whole thing
-        sigers = [coring.Siger(qb64=sig) for sig in sigs]
+        sigers = [core.Siger(qb64=sig) for sig in sigs]
 
         # create seal for the proper location to find the signatures
         kever = hab.mhab.kever
         seal = eventing.SealEvent(i=hab.mhab.pre, s="{:x}".format(kever.lastEst.s), d=kever.lastEst.d)
 
         ims = eventing.messagize(serder=serder, sigers=sigers, seal=seal)
         ims.extend(atc.encode("utf-8"))  # add the pathed attachments
@@ -112,15 +113,15 @@
 
         both = list(set(smids + (rmids or [])))
         for recp in both:  # Have to verify we already know all the recipients.
             if recp not in agent.hby.kevers:
                 agent.hby.deleteHab(name=name)
                 raise falcon.HTTPBadRequest(description=f"attempt to merge with unknown AID={recp}")
 
-        sigers = [coring.Siger(qb64=sig) for sig in sigs]
+        sigers = [core.Siger(qb64=sig) for sig in sigs]
         verfers = [coring.Verfer(qb64=k) for k in rot['k']]
         digers = [coring.Diger(qb64=n) for n in rot['n']]
 
         mhab = None
         for mid in both:
             if mid in agent.hby.habs:
                 mhab = agent.hby.habs[mid]
```

### Comparing `keria-0.1.3/src/keria/app/indirecting.py` & `keria-0.2.0.dev0/src/keria/app/indirecting.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 simple indirect mode demo support classes
 """
 import falcon
 from keri.app import httping
 from keri.core import eventing
 from keri.core.coring import Ilks, Sadder
-from keri.kering import Protos
+from keri.kering import Protocols
 
 CESR_DESTINATION_HEADER = "CESR-DESTINATION"
 
 
 class HttpEnd:
     """
     HTTP handler that accepts and KERI events POSTed as the body of a request with all attachments to
@@ -80,15 +80,15 @@
         cr = httping.parseCesrHttpRequest(req=req)
         serder = Sadder(ked=cr.payload, kind=eventing.Serials.json)
         msg = bytearray(serder.raw)
         msg.extend(cr.attachments.encode("utf-8"))
 
         agent.parser.ims.extend(msg)
 
-        if serder.proto == Protos.acdc:
+        if serder.proto == Protocols.acdc:
             rep.status = falcon.HTTP_204
 
         else:
             ilk = serder.ked["t"]
             if ilk in (Ilks.icp, Ilks.rot, Ilks.ixn, Ilks.dip, Ilks.drt, Ilks.exn, Ilks.rpy):
                 rep.status = falcon.HTTP_204
             elif ilk in (Ilks.vcp, Ilks.vrt, Ilks.iss, Ilks.rev, Ilks.bis, Ilks.brv):
```

### Comparing `keria-0.1.3/src/keria/app/notifying.py` & `keria-0.2.0.dev0/src/keria/app/notifying.py`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/src/keria/app/specing.py` & `keria-0.2.0.dev0/src/keria/app/specing.py`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/src/keria/core/authing.py` & `keria-0.2.0.dev0/src/keria/core/authing.py`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/src/keria/core/httping.py` & `keria-0.2.0.dev0/src/keria/core/httping.py`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/src/keria/core/keeping.py` & `keria-0.2.0.dev0/src/keria/core/keeping.py`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/src/keria/core/longrunning.py` & `keria-0.2.0.dev0/src/keria/core/longrunning.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,25 +84,25 @@
 
 class Monitor:
     """  Monitoring and garbage collecting long running operations
 
     Attributes:
         hby (Habery): identifier database environment
         opr(Operator): long running operations database
-        swain(Sealer): Delegation processes tracker
+        swain(Anchorer): Delegation processes tracker
 
     """
 
     def __init__(self, hby, swain, counselor=None, registrar=None, exchanger=None, credentialer=None, opr=None,
                  temp=False):
         """ Create long running operation monitor
 
         Parameters:
             hby (Habery): identifier database environment
-            swain(Sealer): Delegation processes tracker
+            swain(Anchorer): Delegation processes tracker
             opr (Operator): long running operations database
 
         """
         self.hby = hby
         self.swain = swain
         self.counselor = counselor
         self.registrar = registrar
@@ -406,16 +406,16 @@
 
         return operation
 
 
 class OperationCollectionEnd:
     @staticmethod
     def on_get(req, rep):
-        """ Get list of long running operations 
-        
+        """ Get list of long running operations
+
         Parameters:
             req (Request):  Falcon HTTP Request object
             rep (Response): Falcon HTTP Response object
 
         ---
         summary: Get list of long running operations
         parameters:
```

### Comparing `keria-0.1.3/src/keria/db/basing.py` & `keria-0.2.0.dev0/src/keria/db/basing.py`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/src/keria/end/ending.py` & `keria-0.2.0.dev0/src/keria/end/ending.py`

 * *Files identical despite different names*

### Comparing `keria-0.1.3/src/keria/peer/exchanging.py` & `keria-0.2.0.dev0/src/keria/peer/exchanging.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 KERIA
 keria.app.exchanging module
 
 """
 import json
 
 import falcon
+from keri import core
 from keri.core import coring, eventing, serdering
 from keri.peer import exchanging
 
 from keria.core import httping
 
 
 def loadEnds(app):
@@ -54,15 +55,15 @@
 
         for recp in rec:  # Have to verify we already know all the recipients.
             if recp not in agent.hby.kevers:
                 raise falcon.HTTPBadRequest(description=f"attempt to send to unknown AID={recp}")
 
         # use that data to create th Serder and Sigers for the exn
         serder = serdering.SerderKERI(sad=ked)
-        sigers = [coring.Siger(qb64=sig) for sig in sigs]
+        sigers = [core.Siger(qb64=sig) for sig in sigs]
 
         # Now create the stream to send, need the signer seal
         kever = hab.kever
         seal = eventing.SealEvent(i=hab.pre, s="{:x}".format(kever.lastEst.s), d=kever.lastEst.d)
 
         ims = eventing.messagize(serder=serder, sigers=sigers, seal=seal)
```

### Comparing `keria-0.1.3/src/keria/testing/testing_helper.py` & `keria-0.2.0.dev0/src/keria/testing/testing_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Helpers for tests that need KERIA
 """
 import json
 import os
+import pathlib
 import shutil
 from contextlib import contextmanager
 
 import falcon
 from falcon import testing
 from hio.core import http
 from keri import kering
@@ -19,14 +20,16 @@
 from keri.vc import proving
 from keri.vdr import credentialing, verifying
 from keri.vdr import eventing as veventing
 from keri.vdr.credentialing import Regery, Registrar
 
 from keria.app import agenting, indirecting
 
+SCRIPTS_DIR = str(pathlib.Path(str(pathlib.Path(__file__).parent.resolve()), "../../../tests/scripts").resolve())
+
 WitnessUrls = {
     "wan:tcp": "tcp://127.0.0.1:5632/",
     "wan:http": "http://127.0.0.1:5642/",
     "wes:tcp": "tcp://127.0.0.1:5634/",
     "wes:http": "http://127.0.0.1:5644/",
     "wil:tcp": "tcp://127.0.0.1:5633/",
     "wil:http": "http://127.0.0.1:5643/",
@@ -517,15 +520,15 @@
         assert serder.pre == Helpers.controllerAID
 
         if salter is None:
             salt = b'0123456789abcdef'
             salter = coring.Salter(raw=salt)
 
         if cf is None:
-            cf = configing.Configer(name="keria", headDirPath="tests/scripts", reopen=True, clear=False)
+            cf = configing.Configer(name="keria", headDirPath=SCRIPTS_DIR, reopen=True, clear=False)
 
         with habbing.openHby(name="keria", salt=salter.qb64, temp=temp, cf=cf) as hby:
             ims = eventing.messagize(serder, sigers=sigers)
             parsing.Parser(kvy=hby.kvy).parseOne(ims=ims)
 
             agency = agenting.Agency(name="agency", bran=None, temp=True)
             agentHab = hby.makeHab(serder.pre, ns="agent", transferable=True, delpre=serder.pre)
```

### Comparing `keria-0.1.3/src/keria.egg-info/PKG-INFO` & `keria-0.2.0.dev0/src/keria.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keria
-Version: 0.1.3
+Version: 0.2.0.dev0
 Summary: KERIA: KERI Agent in the cloud
 Home-page: https://github.com/WebOfTrust/keria
 Author: Philip S. Feairheller
 Author-email: pfeairheller@gmail.com
 License: Apache Software License 2.0
 Project-URL: Issue Tracker, https://github.com/WebOfTrust/keria/issues
 Keywords: secure attribution,authentic data,discovery,resolver
@@ -13,19 +13,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10.4
+Requires-Python: >=3.12.2
 License-File: LICENSE
-Requires-Dist: hio>=0.6.9
-Requires-Dist: keri>=1.1.6
+Requires-Dist: hio>=0.6.12
+Requires-Dist: keri>=1.2.0-dev0
 Requires-Dist: mnemonic>=0.20
 Requires-Dist: multicommand>=1.0.0
-Requires-Dist: falcon>=3.1.0
+Requires-Dist: falcon>=3.1.3
 Requires-Dist: http_sfv>=0.9.8
 Requires-Dist: dataclasses_json>=0.5.7
 Requires-Dist: apispec>=6.3.0
 
 KERIA: KERI Agent in the cloud.
```

### Comparing `keria-0.1.3/src/keria.egg-info/SOURCES.txt` & `keria-0.2.0.dev0/src/keria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

