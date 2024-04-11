# Comparing `tmp/ryzen-master-commander-0.1.2.tar.gz` & `tmp/ryzen-master-commander-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryzen-master-commander-0.1.2.tar", last modified: Thu Apr 11 20:21:29 2024, max compression
+gzip compressed data, was "ryzen-master-commander-0.1.4.tar", last modified: Thu Apr 11 20:31:00 2024, max compression
```

## Comparing `ryzen-master-commander-0.1.2.tar` & `ryzen-master-commander-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:21:29.583412 ryzen-master-commander-0.1.2/
--rw-r--r--   0 sam       (1000) sam       (1000)    11357 2024-04-11 19:38:16.000000 ryzen-master-commander-0.1.2/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)       88 2024-04-11 20:21:29.582412 ryzen-master-commander-0.1.2/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     2634 2024-04-11 20:11:01.000000 ryzen-master-commander-0.1.2/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:21:29.582412 ryzen-master-commander-0.1.2/app/
--rw-r--r--   0 sam       (1000) sam       (1000)       22 2024-04-11 20:18:47.000000 ryzen-master-commander-0.1.2/app/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1800 2024-04-11 19:04:29.000000 ryzen-master-commander-0.1.2/app/graphs.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7027 2024-04-11 20:06:15.000000 ryzen-master-commander-0.1.2/app/main_window.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6193 2024-04-11 19:28:04.000000 ryzen-master-commander-0.1.2/app/profile_manager.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1580 2024-04-11 19:19:29.000000 ryzen-master-commander-0.1.2/app/system_utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:21:29.582412 ryzen-master-commander-0.1.2/ryzen_master_commander.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)       88 2024-04-11 20:21:29.000000 ryzen-master-commander-0.1.2/ryzen_master_commander.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      396 2024-04-11 20:21:29.000000 ryzen-master-commander-0.1.2/ryzen_master_commander.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2024-04-11 20:21:29.000000 ryzen-master-commander-0.1.2/ryzen_master_commander.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       52 2024-04-11 20:21:29.000000 ryzen-master-commander-0.1.2/ryzen_master_commander.egg-info/entry_points.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       24 2024-04-11 20:21:29.000000 ryzen-master-commander-0.1.2/ryzen_master_commander.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        4 2024-04-11 20:21:29.000000 ryzen-master-commander-0.1.2/ryzen_master_commander.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       38 2024-04-11 20:21:29.583412 ryzen-master-commander-0.1.2/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)      330 2024-04-11 20:20:27.000000 ryzen-master-commander-0.1.2/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/
+-rw-r--r--   0 sam       (1000) sam       (1000)    11357 2024-04-11 19:38:16.000000 ryzen-master-commander-0.1.4/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)       88 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     2634 2024-04-11 20:11:01.000000 ryzen-master-commander-0.1.4/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/app/
+-rw-r--r--   0 sam       (1000) sam       (1000)      212 2024-04-11 20:25:49.000000 ryzen-master-commander-0.1.4/app/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1800 2024-04-11 19:04:29.000000 ryzen-master-commander-0.1.4/app/graphs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7027 2024-04-11 20:06:15.000000 ryzen-master-commander-0.1.4/app/main_window.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6193 2024-04-11 19:28:04.000000 ryzen-master-commander-0.1.4/app/profile_manager.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1580 2024-04-11 19:19:29.000000 ryzen-master-commander-0.1.4/app/system_utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)       88 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      396 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       52 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/entry_points.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       24 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        4 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       38 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)      330 2024-04-11 20:30:51.000000 ryzen-master-commander-0.1.4/setup.py
```

### Comparing `ryzen-master-commander-0.1.2/LICENSE` & `ryzen-master-commander-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.2/README.md` & `ryzen-master-commander-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.2/app/graphs.py` & `ryzen-master-commander-0.1.4/app/graphs.py`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.2/app/main_window.py` & `ryzen-master-commander-0.1.4/app/main_window.py`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.2/app/profile_manager.py` & `ryzen-master-commander-0.1.4/app/profile_manager.py`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.2/app/system_utils.py` & `ryzen-master-commander-0.1.4/app/system_utils.py`

 * *Files identical despite different names*

