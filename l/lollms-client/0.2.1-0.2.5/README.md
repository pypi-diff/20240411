# Comparing `tmp/lollms_client-0.2.1.tar.gz` & `tmp/lollms_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.2.1.tar", last modified: Thu Apr 11 21:23:46 2024, max compression
+gzip compressed data, was "lollms_client-0.2.5.tar", last modified: Thu Apr 11 21:25:48 2024, max compression
```

## Comparing `lollms_client-0.2.1.tar` & `lollms_client-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 21:23:46.300240 lollms_client-0.2.1/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-04-11 21:23:46.299242 lollms_client-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 21:23:46.273723 lollms_client-0.2.1/lollms_client/
--rw-rw-rw-   0        0        0    12127 2024-04-10 07:06:13.000000 lollms_client-0.2.1/lollms_client/__init__.py
--rw-rw-rw-   0        0        0    12127 2024-04-11 21:17:29.000000 lollms_client-0.2.1/lollms_client/lollms_core.py
--rw-rw-rw-   0        0        0     1457 2024-04-11 21:23:29.000000 lollms_client-0.2.1/lollms_client/lollms_tasks.py
--rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.2.1/lollms_client/lollms_types.py
-drwxrwxrwx   0        0        0        0 2024-04-11 21:23:46.298240 lollms_client-0.2.1/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-04-11 21:23:46.000000 lollms_client-0.2.1/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-04-11 21:23:46.000000 lollms_client-0.2.1/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 21:23:46.000000 lollms_client-0.2.1/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 21:23:46.000000 lollms_client-0.2.1/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-11 21:23:46.000000 lollms_client-0.2.1/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 21:23:46.300240 lollms_client-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-04-11 21:23:34.000000 lollms_client-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 21:25:48.942571 lollms_client-0.2.5/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-04-11 21:25:48.941569 lollms_client-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 21:25:48.922446 lollms_client-0.2.5/lollms_client/
+-rw-rw-rw-   0        0        0      105 2024-04-11 21:24:53.000000 lollms_client-0.2.5/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0    12127 2024-04-11 21:17:29.000000 lollms_client-0.2.5/lollms_client/lollms_core.py
+-rw-rw-rw-   0        0        0     1457 2024-04-11 21:23:29.000000 lollms_client-0.2.5/lollms_client/lollms_tasks.py
+-rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.2.5/lollms_client/lollms_types.py
+drwxrwxrwx   0        0        0        0 2024-04-11 21:25:48.940568 lollms_client-0.2.5/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 21:25:48.942571 lollms_client-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-04-11 21:25:01.000000 lollms_client-0.2.5/setup.py
```

### Comparing `lollms_client-0.2.1/LICENSE` & `lollms_client-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.1/PKG-INFO` & `lollms_client-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.2.1
+Version: 0.2.5
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.2.1/README.md` & `lollms_client-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.1/lollms_client/__init__.py` & `lollms_client-0.2.5/lollms_client/lollms_core.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.1/lollms_client/lollms_tasks.py` & `lollms_client-0.2.5/lollms_client/lollms_tasks.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.1/lollms_client/lollms_types.py` & `lollms_client-0.2.5/lollms_client/lollms_types.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.1/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.2.5/lollms_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.2.1
+Version: 0.2.5
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.2.1/setup.py` & `lollms_client-0.2.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lollms_client",
-    version="0.2.1",
+    version="0.2.5",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

