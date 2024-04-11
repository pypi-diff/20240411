# Comparing `tmp/cykooz.buildout.fixnamespace-2.0.4.tar.gz` & `tmp/cykooz.buildout.fixnamespace-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cykooz.buildout.fixnamespace-2.0.4.tar", last modified: Mon Sep  4 21:48:04 2023, max compression
+gzip compressed data, was "cykooz.buildout.fixnamespace-2.0.6.tar", last modified: Thu Apr 11 13:13:28 2024, max compression
```

## Comparing `cykooz.buildout.fixnamespace-2.0.4.tar` & `cykooz.buildout.fixnamespace-2.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2023-09-04 21:48:04.602662 cykooz.buildout.fixnamespace-2.0.4/
--rw-r--r--   0 cykooz    (1000) cykooz    (1000)      967 2023-09-04 21:45:22.000000 cykooz.buildout.fixnamespace-2.0.4/CHANGES.rst
--rw-r--r--   0 cykooz    (1000) cykooz    (1000)      117 2020-04-14 12:20:54.000000 cykooz.buildout.fixnamespace-2.0.4/MANIFEST.in
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)     2351 2023-09-04 21:48:04.602662 cykooz.buildout.fixnamespace-2.0.4/PKG-INFO
--rw-r--r--   0 cykooz    (1000) cykooz    (1000)      487 2023-07-20 21:08:44.000000 cykooz.buildout.fixnamespace-2.0.4/README.rst
--rw-r--r--   0 cykooz    (1000) cykooz    (1000)        6 2023-09-04 21:45:26.000000 cykooz.buildout.fixnamespace-2.0.4/RELEASE-VERSION
-drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2023-09-04 21:48:04.598662 cykooz.buildout.fixnamespace-2.0.4/cykooz/
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)       65 2023-07-20 20:12:05.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz/__init__.py
-drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2023-09-04 21:48:04.598662 cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)       65 2023-07-20 20:11:59.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/__init__.py
-drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2023-09-04 21:48:04.598662 cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/fixnamespace/
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)       67 2023-07-20 20:11:50.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/fixnamespace/__init__.py
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)     4640 2023-09-04 21:45:01.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/fixnamespace/extension.py
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)      544 2023-09-03 13:40:16.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/fixnamespace/runtests.py
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)     2934 2023-09-04 20:05:18.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/fixnamespace/tests.py
-drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2023-09-04 21:48:04.598662 cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)     2351 2023-09-04 21:48:04.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/PKG-INFO
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)      875 2023-09-04 21:48:04.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/SOURCES.txt
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)        1 2023-09-04 21:48:04.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/dependency_links.txt
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)      172 2023-09-04 21:48:04.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/entry_points.txt
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)        1 2023-07-20 22:53:07.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/not-zip-safe
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)       56 2023-09-04 21:48:04.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/requires.txt
--rw-rw-r--   0 cykooz    (1000) cykooz    (1000)        7 2023-09-04 21:48:04.000000 cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/top_level.txt
--rw-r--r--   0 cykooz    (1000) cykooz    (1000)      513 2023-09-04 21:48:04.602662 cykooz.buildout.fixnamespace-2.0.4/setup.cfg
--rw-r--r--   0 cykooz    (1000) cykooz    (1000)     2870 2023-07-18 19:50:00.000000 cykooz.buildout.fixnamespace-2.0.4/setup.py
--rw-r--r--   0 cykooz    (1000) cykooz    (1000)     5902 2023-07-20 19:33:27.000000 cykooz.buildout.fixnamespace-2.0.4/version.py
+drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2024-04-11 13:13:28.225656 cykooz.buildout.fixnamespace-2.0.6/
+-rw-r--r--   0 cykooz    (1000) cykooz    (1000)     1091 2024-04-11 13:13:24.000000 cykooz.buildout.fixnamespace-2.0.6/CHANGES.rst
+-rw-r--r--   0 cykooz    (1000) cykooz    (1000)      117 2020-04-14 12:20:54.000000 cykooz.buildout.fixnamespace-2.0.6/MANIFEST.in
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)     2475 2024-04-11 13:13:28.225656 cykooz.buildout.fixnamespace-2.0.6/PKG-INFO
+-rw-r--r--   0 cykooz    (1000) cykooz    (1000)      487 2023-07-20 21:08:44.000000 cykooz.buildout.fixnamespace-2.0.6/README.rst
+-rw-r--r--   0 cykooz    (1000) cykooz    (1000)        6 2024-04-11 13:13:28.000000 cykooz.buildout.fixnamespace-2.0.6/RELEASE-VERSION
+drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2024-04-11 13:13:28.221656 cykooz.buildout.fixnamespace-2.0.6/cykooz/
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)       65 2023-07-20 20:12:05.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz/__init__.py
+drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2024-04-11 13:13:28.221656 cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)       65 2023-07-20 20:11:59.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/__init__.py
+drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2024-04-11 13:13:28.225656 cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/fixnamespace/
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)       67 2023-07-20 20:11:50.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/fixnamespace/__init__.py
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)     4832 2024-04-11 13:03:49.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/fixnamespace/extension.py
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)      544 2023-09-03 13:40:16.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/fixnamespace/runtests.py
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)     2970 2024-04-11 13:04:38.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/fixnamespace/tests.py
+drwxrwxr-x   0 cykooz    (1000) cykooz    (1000)        0 2024-04-11 13:13:28.225656 cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)     2475 2024-04-11 13:13:28.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/PKG-INFO
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)      875 2024-04-11 13:13:28.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/SOURCES.txt
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)        1 2024-04-11 13:13:28.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/dependency_links.txt
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)      172 2024-04-11 13:13:28.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/entry_points.txt
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)        1 2023-07-20 22:53:07.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/not-zip-safe
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)       56 2024-04-11 13:13:28.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/requires.txt
+-rw-rw-r--   0 cykooz    (1000) cykooz    (1000)        7 2024-04-11 13:13:28.000000 cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/top_level.txt
+-rw-r--r--   0 cykooz    (1000) cykooz    (1000)      513 2024-04-11 13:13:28.225656 cykooz.buildout.fixnamespace-2.0.6/setup.cfg
+-rw-r--r--   0 cykooz    (1000) cykooz    (1000)     2870 2023-07-18 19:50:00.000000 cykooz.buildout.fixnamespace-2.0.6/setup.py
+-rw-r--r--   0 cykooz    (1000) cykooz    (1000)     5902 2023-07-20 19:33:27.000000 cykooz.buildout.fixnamespace-2.0.6/version.py
```

### Comparing `cykooz.buildout.fixnamespace-2.0.4/CHANGES.rst` & `cykooz.buildout.fixnamespace-2.0.6/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,19 @@
       This identifier MUST be placed in brackets. If a hot fix has not the task identifier then you
       can use the word "HOTFIX" instead of it.
     - At the end of sentence MUST stand a point.
 
 CHANGELOG
 *********
 
+2.0.6 (2024-04-11)
+==================
+
+- Added support of namespaced package with python-files but without subdirectories.
+
 2.0.4 (2023-09-05)
 ==================
 
 - Added support of packages without ``top_level.txt`` file.
 
 2.0.2 (2023-09-03)
 ==================
```

### Comparing `cykooz.buildout.fixnamespace-2.0.4/PKG-INFO` & `cykooz.buildout.fixnamespace-2.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cykooz.buildout.fixnamespace
-Version: 2.0.4
+Version: 2.0.6
 Summary: A zc.buildout extension changes value of NAMESPACE_PACKAGE_INIT constant from setuptools
 Home-page: https://github.com/Cykooz/cykooz.buildout.fixnamespace
 Author: Kirill Kuzminykh
 Author-email: cykooz@gmail.com
 License: MIT
 Keywords: development build
 Classifier: Intended Audience :: Developers
@@ -45,14 +45,19 @@
       This identifier MUST be placed in brackets. If a hot fix has not the task identifier then you
       can use the word "HOTFIX" instead of it.
     - At the end of sentence MUST stand a point.
 
 CHANGELOG
 *********
 
+2.0.6 (2024-04-11)
+==================
+
+- Added support of namespaced package with python-files but without subdirectories.
+
 2.0.4 (2023-09-05)
 ==================
 
 - Added support of packages without ``top_level.txt`` file.
 
 2.0.2 (2023-09-03)
 ==================
```

### Comparing `cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/fixnamespace/extension.py` & `cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/fixnamespace/extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,18 @@
 
 
 def get_namespaces(root_dir: Path):
     dir_names, has_init = get_child_dirs(root_dir)
     if not dir_names:
         if has_init:
             return [None]
+        for name in os.listdir(root_dir):
+            p = root_dir / name
+            if p.is_file() and name.endswith(('.py', '.pyc', '.pyo', '.pyd')):
+                return [root_dir.name]
         return []
     namespaces = set()
     root_name = root_dir.name
     for dir_name in dir_names:
         child_dir = root_dir / dir_name
         child_namespaces = get_namespaces(child_dir)
         for namespace in child_namespaces:
```

### Comparing `cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/fixnamespace/runtests.py` & `cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/fixnamespace/runtests.py`

 * *Files identical despite different names*

### Comparing `cykooz.buildout.fixnamespace-2.0.4/cykooz/buildout/fixnamespace/tests.py` & `cykooz.buildout.fixnamespace-2.0.6/cykooz/buildout/fixnamespace/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             path.mkdir(parents=True, exist_ok=True)
 
 
 @pytest.mark.parametrize(
     ['paths', 'result'],
     [
         ([], []),
+        (['context.py'], ['root']),
         (['sub1'], []),
         (['sub1/__init__.py'], ['root']),
         (['sub1/sub2/__init__.py'], ['root', 'root.sub1']),
         (
                 [
                     'sub1/__init__.py',
                     'sub2',
```

### Comparing `cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/PKG-INFO` & `cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cykooz.buildout.fixnamespace
-Version: 2.0.4
+Version: 2.0.6
 Summary: A zc.buildout extension changes value of NAMESPACE_PACKAGE_INIT constant from setuptools
 Home-page: https://github.com/Cykooz/cykooz.buildout.fixnamespace
 Author: Kirill Kuzminykh
 Author-email: cykooz@gmail.com
 License: MIT
 Keywords: development build
 Classifier: Intended Audience :: Developers
@@ -45,14 +45,19 @@
       This identifier MUST be placed in brackets. If a hot fix has not the task identifier then you
       can use the word "HOTFIX" instead of it.
     - At the end of sentence MUST stand a point.
 
 CHANGELOG
 *********
 
+2.0.6 (2024-04-11)
+==================
+
+- Added support of namespaced package with python-files but without subdirectories.
+
 2.0.4 (2023-09-05)
 ==================
 
 - Added support of packages without ``top_level.txt`` file.
 
 2.0.2 (2023-09-03)
 ==================
```

### Comparing `cykooz.buildout.fixnamespace-2.0.4/cykooz.buildout.fixnamespace.egg-info/SOURCES.txt` & `cykooz.buildout.fixnamespace-2.0.6/cykooz.buildout.fixnamespace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cykooz.buildout.fixnamespace-2.0.4/setup.cfg` & `cykooz.buildout.fixnamespace-2.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `cykooz.buildout.fixnamespace-2.0.4/setup.py` & `cykooz.buildout.fixnamespace-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `cykooz.buildout.fixnamespace-2.0.4/version.py` & `cykooz.buildout.fixnamespace-2.0.6/version.py`

 * *Files identical despite different names*

