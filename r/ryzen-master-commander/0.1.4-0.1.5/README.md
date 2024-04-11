# Comparing `tmp/ryzen-master-commander-0.1.4.tar.gz` & `tmp/ryzen-master-commander-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryzen-master-commander-0.1.4.tar", last modified: Thu Apr 11 20:31:00 2024, max compression
+gzip compressed data, was "ryzen-master-commander-0.1.5.tar", last modified: Thu Apr 11 20:35:16 2024, max compression
```

## Comparing `ryzen-master-commander-0.1.4.tar` & `ryzen-master-commander-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/
--rw-r--r--   0 sam       (1000) sam       (1000)    11357 2024-04-11 19:38:16.000000 ryzen-master-commander-0.1.4/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)       88 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     2634 2024-04-11 20:11:01.000000 ryzen-master-commander-0.1.4/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/app/
--rw-r--r--   0 sam       (1000) sam       (1000)      212 2024-04-11 20:25:49.000000 ryzen-master-commander-0.1.4/app/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1800 2024-04-11 19:04:29.000000 ryzen-master-commander-0.1.4/app/graphs.py
--rw-r--r--   0 sam       (1000) sam       (1000)     7027 2024-04-11 20:06:15.000000 ryzen-master-commander-0.1.4/app/main_window.py
--rw-r--r--   0 sam       (1000) sam       (1000)     6193 2024-04-11 19:28:04.000000 ryzen-master-commander-0.1.4/app/profile_manager.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1580 2024-04-11 19:19:29.000000 ryzen-master-commander-0.1.4/app/system_utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)       88 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      396 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       52 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/entry_points.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       24 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        4 2024-04-11 20:31:00.000000 ryzen-master-commander-0.1.4/ryzen_master_commander.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       38 2024-04-11 20:31:00.500397 ryzen-master-commander-0.1.4/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)      330 2024-04-11 20:30:51.000000 ryzen-master-commander-0.1.4/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:35:16.950986 ryzen-master-commander-0.1.5/
+-rw-r--r--   0 sam       (1000) sam       (1000)    11357 2024-04-11 19:38:16.000000 ryzen-master-commander-0.1.5/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)       88 2024-04-11 20:35:16.950986 ryzen-master-commander-0.1.5/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     2634 2024-04-11 20:11:01.000000 ryzen-master-commander-0.1.5/README.md
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:35:16.949986 ryzen-master-commander-0.1.5/app/
+-rw-r--r--   0 sam       (1000) sam       (1000)      241 2024-04-11 20:33:33.000000 ryzen-master-commander-0.1.5/app/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1800 2024-04-11 19:04:29.000000 ryzen-master-commander-0.1.5/app/graphs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     7027 2024-04-11 20:06:15.000000 ryzen-master-commander-0.1.5/app/main_window.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     6193 2024-04-11 19:28:04.000000 ryzen-master-commander-0.1.5/app/profile_manager.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1580 2024-04-11 19:19:29.000000 ryzen-master-commander-0.1.5/app/system_utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2024-04-11 20:35:16.949986 ryzen-master-commander-0.1.5/ryzen_master_commander.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)       88 2024-04-11 20:35:16.000000 ryzen-master-commander-0.1.5/ryzen_master_commander.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      396 2024-04-11 20:35:16.000000 ryzen-master-commander-0.1.5/ryzen_master_commander.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2024-04-11 20:35:16.000000 ryzen-master-commander-0.1.5/ryzen_master_commander.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       52 2024-04-11 20:35:16.000000 ryzen-master-commander-0.1.5/ryzen_master_commander.egg-info/entry_points.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       24 2024-04-11 20:35:16.000000 ryzen-master-commander-0.1.5/ryzen_master_commander.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        4 2024-04-11 20:35:16.000000 ryzen-master-commander-0.1.5/ryzen_master_commander.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       38 2024-04-11 20:35:16.950986 ryzen-master-commander-0.1.5/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)      330 2024-04-11 20:33:44.000000 ryzen-master-commander-0.1.5/setup.py
```

### Comparing `ryzen-master-commander-0.1.4/LICENSE` & `ryzen-master-commander-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.4/README.md` & `ryzen-master-commander-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.4/app/graphs.py` & `ryzen-master-commander-0.1.5/app/graphs.py`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.4/app/main_window.py` & `ryzen-master-commander-0.1.5/app/main_window.py`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.4/app/profile_manager.py` & `ryzen-master-commander-0.1.5/app/profile_manager.py`

 * *Files identical despite different names*

### Comparing `ryzen-master-commander-0.1.4/app/system_utils.py` & `ryzen-master-commander-0.1.5/app/system_utils.py`

 * *Files identical despite different names*

