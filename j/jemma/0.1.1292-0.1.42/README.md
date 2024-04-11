# Comparing `tmp/jemma-0.1.1292.tar.gz` & `tmp/jemma-0.1.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.1292.tar", last modified: Wed Apr 10 01:45:42 2024, max compression
+gzip compressed data, was "jemma-0.1.42.tar", last modified: Wed Apr 10 02:16:21 2024, max compression
```

## Comparing `jemma-0.1.1292.tar` & `jemma-0.1.42.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.886420 jemma-0.1.1292/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:45:42.886040 jemma-0.1.1292/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      797 2024-04-09 23:33:37.000000 jemma-0.1.1292/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.870072 jemma-0.1.1292/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.1292/jemma/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.874730 jemma-0.1.1292/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.1292/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.876198 jemma-0.1.1292/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.1292/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.1292/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.878277 jemma-0.1.1292/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.1292/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.1292/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.1292/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.879765 jemma-0.1.1292/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.1292/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.1292/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.881099 jemma-0.1.1292/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.1292/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.1292/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.884247 jemma-0.1.1292/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.1292/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.1292/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 01:17:50.000000 jemma-0.1.1292/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.1292/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.1292/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5439 2024-04-10 01:45:32.000000 jemma-0.1.1292/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.1292/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.885452 jemma-0.1.1292/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.1292/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.1292/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 01:45:42.873613 jemma-0.1.1292/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-10 01:45:42.000000 jemma-0.1.1292/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-10 01:45:42.886536 jemma-0.1.1292/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-10 01:45:39.000000 jemma-0.1.1292/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.286081 jemma-0.1.42/
+-rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-10 02:16:21.285615 jemma-0.1.42/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      797 2024-04-09 23:33:37.000000 jemma-0.1.42/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.263654 jemma-0.1.42/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.42/jemma/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.268390 jemma-0.1.42/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.42/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.269619 jemma-0.1.42/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.42/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.42/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.274154 jemma-0.1.42/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.42/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.42/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.42/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.276028 jemma-0.1.42/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.42/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.42/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.277745 jemma-0.1.42/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.42/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.42/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.282765 jemma-0.1.42/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.42/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.42/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 01:17:50.000000 jemma-0.1.42/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.42/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.42/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5439 2024-04-10 01:45:32.000000 jemma-0.1.42/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.42/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.284599 jemma-0.1.42/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.42/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.42/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.267764 jemma-0.1.42/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-10 02:16:21.286214 jemma-0.1.42/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      468 2024-04-10 02:16:07.000000 jemma-0.1.42/setup.py
```

### Comparing `jemma-0.1.1292/README.md` & `jemma-0.1.42/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/prompt/business/owner.py` & `jemma-0.1.42/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/prompt/engineer/clarify.py` & `jemma-0.1.42/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/prompt/engineer/code.py` & `jemma-0.1.42/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/prompt/tester/test.py` & `jemma-0.1.42/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/requirements/feature.py` & `jemma-0.1.42/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/team/business_owner.py` & `jemma-0.1.42/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/team/engineer.py` & `jemma-0.1.42/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/team/project_manager.py` & `jemma-0.1.42/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/team/tester.py` & `jemma-0.1.42/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/thinker.py` & `jemma-0.1.42/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/tools.py` & `jemma-0.1.42/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma/work/flow.py` & `jemma-0.1.42/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.1292/jemma.egg-info/SOURCES.txt` & `jemma-0.1.42/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

