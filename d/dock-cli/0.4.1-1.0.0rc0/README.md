# Comparing `tmp/dock-cli-0.4.1.tar.gz` & `tmp/dock-cli-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-cli-0.4.1.tar", last modified: Wed Apr 10 03:15:20 2024, max compression
+gzip compressed data, was "dock-cli-1.0.0rc0.tar", last modified: Thu Apr 11 09:49:11 2024, max compression
```

## Comparing `dock-cli-0.4.1.tar` & `dock-cli-1.0.0rc0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-10 03:15:20.559459 dock-cli-0.4.1/
--rw-r--r--   0 posen      (501) staff       (20)     1062 2024-03-05 06:48:54.000000 dock-cli-0.4.1/LICENSE
--rw-r--r--   0 posen      (501) staff       (20)     3516 2024-04-10 03:15:20.559207 dock-cli-0.4.1/PKG-INFO
--rw-r--r--   0 posen      (501) staff       (20)     3252 2024-04-10 02:52:04.000000 dock-cli-0.4.1/README.md
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-10 03:15:20.555271 dock-cli-0.4.1/dock_cli/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.4.1/dock_cli/__init__.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-10 03:15:20.557097 dock-cli-0.4.1/dock_cli/cli/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.4.1/dock_cli/cli/__init__.py
--rw-r--r--   0 posen      (501) staff       (20)     4041 2024-04-09 16:22:11.000000 dock-cli-0.4.1/dock_cli/cli/chart.py
--rw-r--r--   0 posen      (501) staff       (20)     5715 2024-04-10 03:04:21.000000 dock-cli-0.4.1/dock_cli/cli/image.py
--rw-r--r--   0 posen      (501) staff       (20)     2246 2024-04-09 17:50:45.000000 dock-cli-0.4.1/dock_cli/main.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-10 03:15:20.558621 dock-cli-0.4.1/dock_cli/utils/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.4.1/dock_cli/utils/__init__.py
--rw-r--r--   0 posen      (501) staff       (20)      853 2024-04-10 02:12:30.000000 dock-cli-0.4.1/dock_cli/utils/callback.py
--rw-r--r--   0 posen      (501) staff       (20)      629 2024-03-21 16:14:08.000000 dock-cli-0.4.1/dock_cli/utils/commands.py
--rw-r--r--   0 posen      (501) staff       (20)     5357 2024-04-10 03:08:28.000000 dock-cli-0.4.1/dock_cli/utils/helpers.py
--rw-r--r--   0 posen      (501) staff       (20)      530 2024-04-02 03:22:43.000000 dock-cli-0.4.1/dock_cli/utils/schema.py
--rw-r--r--   0 posen      (501) staff       (20)     2199 2024-04-10 02:13:11.000000 dock-cli-0.4.1/dock_cli/utils/utils.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-10 03:15:20.558952 dock-cli-0.4.1/dock_cli.egg-info/
--rw-r--r--   0 posen      (501) staff       (20)     3516 2024-04-10 03:15:20.000000 dock-cli-0.4.1/dock_cli.egg-info/PKG-INFO
--rw-r--r--   0 posen      (501) staff       (20)      483 2024-04-10 03:15:20.000000 dock-cli-0.4.1/dock_cli.egg-info/SOURCES.txt
--rw-r--r--   0 posen      (501) staff       (20)        1 2024-04-10 03:15:20.000000 dock-cli-0.4.1/dock_cli.egg-info/dependency_links.txt
--rw-r--r--   0 posen      (501) staff       (20)       43 2024-04-10 03:15:20.000000 dock-cli-0.4.1/dock_cli.egg-info/entry_points.txt
--rw-r--r--   0 posen      (501) staff       (20)       13 2024-04-10 03:15:20.000000 dock-cli-0.4.1/dock_cli.egg-info/requires.txt
--rw-r--r--   0 posen      (501) staff       (20)        9 2024-04-10 03:15:20.000000 dock-cli-0.4.1/dock_cli.egg-info/top_level.txt
--rw-r--r--   0 posen      (501) staff       (20)       38 2024-04-10 03:15:20.559508 dock-cli-0.4.1/setup.cfg
--rw-r--r--   0 posen      (501) staff       (20)      619 2024-04-10 01:50:43.000000 dock-cli-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:49:11.633998 dock-cli-1.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-11 09:49:11.633998 dock-cli-1.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:49:11.629998 dock-cli-1.0.0rc0/dock_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:49:11.629998 dock-cli-1.0.0rc0/dock_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/cli/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:49:11.633998 dock-cli-1.0.0rc0/dock_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/dock_cli/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:49:11.633998 dock-cli-1.0.0rc0/dock_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-11 09:49:11.000000 dock-cli-1.0.0rc0/dock_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-11 09:49:11.000000 dock-cli-1.0.0rc0/dock_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:49:11.000000 dock-cli-1.0.0rc0/dock_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 09:49:11.000000 dock-cli-1.0.0rc0/dock_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 09:49:11.000000 dock-cli-1.0.0rc0/dock_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 09:49:11.000000 dock-cli-1.0.0rc0/dock_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:49:11.633998 dock-cli-1.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-11 09:48:59.000000 dock-cli-1.0.0rc0/setup.py
```

### Comparing `dock-cli-0.4.1/LICENSE` & `dock-cli-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/PKG-INFO` & `dock-cli-1.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 0.4.1
+Version: 1.0.0rc0
 Summary: CLI for manage container applications
 Author: Posen
 Author-email: posen2101024@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `dock-cli-0.4.1/README.md` & `dock-cli-1.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli/cli/chart.py` & `dock-cli-1.0.0rc0/dock_cli/cli/chart.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli/cli/image.py` & `dock-cli-1.0.0rc0/dock_cli/cli/image.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli/main.py` & `dock-cli-1.0.0rc0/dock_cli/main.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli/utils/callback.py` & `dock-cli-1.0.0rc0/dock_cli/utils/callback.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli/utils/commands.py` & `dock-cli-1.0.0rc0/dock_cli/utils/commands.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli/utils/helpers.py` & `dock-cli-1.0.0rc0/dock_cli/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli/utils/schema.py` & `dock-cli-1.0.0rc0/dock_cli/utils/schema.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli/utils/utils.py` & `dock-cli-1.0.0rc0/dock_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.4.1/dock_cli.egg-info/PKG-INFO` & `dock-cli-1.0.0rc0/dock_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 0.4.1
+Version: 1.0.0rc0
 Summary: CLI for manage container applications
 Author: Posen
 Author-email: posen2101024@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `dock-cli-0.4.1/setup.py` & `dock-cli-1.0.0rc0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='dock-cli',
-    version='0.4.1',
+    version='1.0.0rc0',
     author='Posen',
     author_email='posen2101024@gmail.com',
     description='CLI for manage container applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
```

