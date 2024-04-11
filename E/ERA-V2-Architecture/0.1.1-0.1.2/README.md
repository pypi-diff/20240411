# Comparing `tmp/ERA_V2_Architecture-0.1.1.tar.gz` & `tmp/ERA_V2_Architecture-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ERA_V2_Architecture-0.1.1.tar", last modified: Mon Apr  1 10:34:48 2024, max compression
+gzip compressed data, was "ERA_V2_Architecture-0.1.2.tar", last modified: Thu Apr 11 11:26:07 2024, max compression
```

## Comparing `ERA_V2_Architecture-0.1.1.tar` & `ERA_V2_Architecture-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 10:34:48.907264 ERA_V2_Architecture-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-04-01 10:34:48.875267 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture/
--rw-rw-rw-   0        0        0        0 2024-04-01 10:07:44.000000 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 10:34:48.901262 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture/model/
--rw-rw-rw-   0        0        0       45 2024-03-13 08:56:18.000000 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture/model/__init__.py
--rw-rw-rw-   0        0        0    18509 2024-03-29 07:18:09.000000 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture/model/models.py
-drwxrwxrwx   0        0        0        0 2024-04-01 10:34:48.904265 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture.egg-info/
--rw-rw-rw-   0        0        0      473 2024-04-01 10:34:48.000000 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-04-01 10:34:48.000000 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 10:34:48.000000 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-01 10:34:48.000000 ERA_V2_Architecture-0.1.1/ERA_V2_Architecture.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      473 2024-04-01 10:34:48.905266 ERA_V2_Architecture-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       43 2024-04-01 09:40:59.000000 ERA_V2_Architecture-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 10:34:48.907264 ERA_V2_Architecture-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-04-01 10:33:09.000000 ERA_V2_Architecture-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:26:07.671674 ERA_V2_Architecture-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:26:07.582363 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture/
+-rw-rw-rw-   0        0        0        0 2024-04-01 10:07:44.000000 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:26:07.665275 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture/model/
+-rw-rw-rw-   0        0        0       73 2024-04-11 10:17:05.000000 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture/model/__init__.py
+-rw-rw-rw-   0        0        0    18509 2024-03-29 07:18:09.000000 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture/model/models.py
+-rw-rw-rw-   0        0        0     2915 2024-04-11 10:29:37.000000 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture/model/resnet.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:26:07.667672 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-04-11 11:26:07.000000 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-04-11 11:26:07.000000 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 11:26:07.000000 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-11 11:26:07.000000 ERA_V2_Architecture-0.1.2/ERA_V2_Architecture.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      473 2024-04-11 11:26:07.669671 ERA_V2_Architecture-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2024-04-01 09:40:59.000000 ERA_V2_Architecture-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 11:26:07.671674 ERA_V2_Architecture-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-04-11 11:25:42.000000 ERA_V2_Architecture-0.1.2/setup.py
```

### Comparing `ERA_V2_Architecture-0.1.1/ERA_V2_Architecture/model/models.py` & `ERA_V2_Architecture-0.1.2/ERA_V2_Architecture/model/models.py`

 * *Files identical despite different names*

### Comparing `ERA_V2_Architecture-0.1.1/setup.py` & `ERA_V2_Architecture-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ERA_V2_Architecture",
-    version="0.1.1",
+    version="0.1.2",
     author="Xianping Wu",
     author_email="xianpingwu@hotmail.com",
     description="The ERA-V2 course network architectures",
     long_description=long_description,
     long_description_content_type="text/markdown",    
     url="https://github.com/ping-Mel/ERAV2-Architecture.git",
     packages=find_packages(),
```

