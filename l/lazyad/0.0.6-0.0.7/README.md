# Comparing `tmp/lazyad-0.0.6.tar.gz` & `tmp/lazyad-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyad-0.0.6.tar", last modified: Sun Mar 24 01:43:28 2024, max compression
+gzip compressed data, was "lazyad-0.0.7.tar", last modified: Thu Apr 11 06:58:11 2024, max compression
```

## Comparing `lazyad-0.0.6.tar` & `lazyad-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-24 01:43:28.323638 lazyad-0.0.6/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-03-24 01:43:28.323409 lazyad-0.0.6/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1311 2024-03-14 02:37:12.000000 lazyad-0.0.6/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-24 01:43:28.321133 lazyad-0.0.6/lazyad/
--rw-r--r--   0 zeroseeker   (501) staff       (20)       23 2024-03-14 03:09:47.000000 lazyad-0.0.6/lazyad/__init__.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-24 01:43:28.322980 lazyad-0.0.6/lazyad/crawlers/
--rw-r--r--   0 zeroseeker   (501) staff       (20)       68 2024-03-19 07:34:32.000000 lazyad-0.0.6/lazyad/crawlers/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2024-03-19 07:35:06.000000 lazyad-0.0.6/lazyad/crawlers/chuangliang.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4540 2024-03-15 02:44:05.000000 lazyad-0.0.6/lazyad/crawlers/oceanengine.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3060 2024-03-24 01:42:41.000000 lazyad-0.0.6/lazyad/crawlers/qq.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-03-24 01:43:28.321910 lazyad-0.0.6/lazyad.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-03-24 01:43:28.000000 lazyad-0.0.6/lazyad.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      298 2024-03-24 01:43:28.000000 lazyad-0.0.6/lazyad.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-03-24 01:43:28.000000 lazyad-0.0.6/lazyad.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       16 2024-03-24 01:43:28.000000 lazyad-0.0.6/lazyad.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        7 2024-03-24 01:43:28.000000 lazyad-0.0.6/lazyad.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-03-24 01:43:28.323689 lazyad-0.0.6/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      893 2024-03-24 01:42:41.000000 lazyad-0.0.6/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.804797 lazyad-0.0.7/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 06:58:11.804597 lazyad-0.0.7/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1311 2024-03-14 02:37:12.000000 lazyad-0.0.7/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.801956 lazyad-0.0.7/lazyad/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       41 2024-04-11 06:24:40.000000 lazyad-0.0.7/lazyad/__init__.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.803872 lazyad-0.0.7/lazyad/crawlers/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       68 2024-03-19 07:34:32.000000 lazyad-0.0.7/lazyad/crawlers/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2024-03-19 07:35:06.000000 lazyad-0.0.7/lazyad/crawlers/chuangliang.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4540 2024-03-15 02:44:05.000000 lazyad-0.0.7/lazyad/crawlers/oceanengine.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3060 2024-03-24 01:42:41.000000 lazyad-0.0.7/lazyad/crawlers/qq.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.804288 lazyad-0.0.7/lazyad/open/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:24:12.000000 lazyad-0.0.7/lazyad/open/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1780 2024-04-11 06:57:50.000000 lazyad-0.0.7/lazyad/open/qq.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:58:11.802854 lazyad-0.0.7/lazyad.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      340 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       16 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        7 2024-04-11 06:58:11.000000 lazyad-0.0.7/lazyad.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-11 06:58:11.804838 lazyad-0.0.7/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      893 2024-04-11 06:57:50.000000 lazyad-0.0.7/setup.py
```

### Comparing `lazyad-0.0.6/PKG-INFO` & `lazyad-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyad
-Version: 0.0.6
+Version: 0.0.7
 Summary: 基于Python的懒人包-适用于广告投放模块
 Home-page: https://gitee.com/ZeroSeeker/lazyad
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazyad-0.0.6/README.md` & `lazyad-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.6/lazyad/crawlers/chuangliang.py` & `lazyad-0.0.7/lazyad/crawlers/chuangliang.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.6/lazyad/crawlers/oceanengine.py` & `lazyad-0.0.7/lazyad/crawlers/oceanengine.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.6/lazyad/crawlers/qq.py` & `lazyad-0.0.7/lazyad/crawlers/qq.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.6/lazyad.egg-info/PKG-INFO` & `lazyad-0.0.7/lazyad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyad
-Version: 0.0.6
+Version: 0.0.7
 Summary: 基于Python的懒人包-适用于广告投放模块
 Home-page: https://gitee.com/ZeroSeeker/lazyad
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazyad-0.0.6/setup.py` & `lazyad-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazyad",
-    version="0.0.6",
+    version="0.0.7",
     description="基于Python的懒人包-适用于广告投放模块",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazyad",
     packages=setuptools.find_packages(),
```

