# Comparing `tmp/giExtract-1.0.3.tar.gz` & `tmp/giExtract-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/giExtract-1.0.3.tar", last modified: Mon Mar 11 04:58:57 2024, max compression
+gzip compressed data, was "dist/giExtract-1.0.4.tar", last modified: Thu Apr 11 14:44:15 2024, max compression
```

## Comparing `giExtract-1.0.3.tar` & `giExtract-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 chineduanene   (501) staff       (20)        0 2024-03-11 04:58:57.027783 giExtract-1.0.3/
--rw-r--r--   0 chineduanene   (501) staff       (20)     4711 2024-03-11 04:58:57.027414 giExtract-1.0.3/PKG-INFO
--rw-r--r--   0 chineduanene   (501) staff       (20)     3623 2024-03-08 11:03:19.000000 giExtract-1.0.3/README.md
-drwxr-xr-x   0 chineduanene   (501) staff       (20)        0 2024-03-11 04:58:57.023122 giExtract-1.0.3/bin/
--rw-r--r--   0 chineduanene   (501) staff       (20)     1585 2024-03-05 22:30:10.000000 giExtract-1.0.3/bin/giCube
--rw-r--r--   0 chineduanene   (501) staff       (20)     2031 2024-03-06 17:17:57.000000 giExtract-1.0.3/bin/giExtract
-drwxr-xr-x   0 chineduanene   (501) staff       (20)        0 2024-03-11 04:58:57.024422 giExtract-1.0.3/giExtract/
--rw-r--r--   0 chineduanene   (501) staff       (20)        0 2024-03-06 17:50:34.000000 giExtract-1.0.3/giExtract/__init__.py
--rw-r--r--   0 chineduanene   (501) staff       (20)     8984 2022-01-11 16:46:37.000000 giExtract-1.0.3/giExtract/util.py
-drwxr-xr-x   0 chineduanene   (501) staff       (20)        0 2024-03-11 04:58:57.026876 giExtract-1.0.3/giExtract.egg-info/
--rw-r--r--   0 chineduanene   (501) staff       (20)     4711 2024-03-11 04:58:56.000000 giExtract-1.0.3/giExtract.egg-info/PKG-INFO
--rw-r--r--   0 chineduanene   (501) staff       (20)      247 2024-03-11 04:58:56.000000 giExtract-1.0.3/giExtract.egg-info/SOURCES.txt
--rw-r--r--   0 chineduanene   (501) staff       (20)        1 2024-03-11 04:58:56.000000 giExtract-1.0.3/giExtract.egg-info/dependency_links.txt
--rw-r--r--   0 chineduanene   (501) staff       (20)      101 2024-03-11 04:58:56.000000 giExtract-1.0.3/giExtract.egg-info/requires.txt
--rw-r--r--   0 chineduanene   (501) staff       (20)       10 2024-03-11 04:58:56.000000 giExtract-1.0.3/giExtract.egg-info/top_level.txt
--rw-r--r--   0 chineduanene   (501) staff       (20)       38 2024-03-11 04:58:57.027917 giExtract-1.0.3/setup.cfg
--rw-r--r--   0 chineduanene   (501) staff       (20)     1066 2024-03-11 04:48:11.000000 giExtract-1.0.3/setup.py
+drwxr-xr-x   0 chineduanene   (501) staff       (20)        0 2024-04-11 14:44:15.954097 giExtract-1.0.4/
+-rw-r--r--   0 chineduanene   (501) staff       (20)     4711 2024-04-11 14:44:15.953778 giExtract-1.0.4/PKG-INFO
+-rw-r--r--   0 chineduanene   (501) staff       (20)     3623 2024-03-08 11:03:19.000000 giExtract-1.0.4/README.md
+drwxr-xr-x   0 chineduanene   (501) staff       (20)        0 2024-04-11 14:44:15.949257 giExtract-1.0.4/bin/
+-rw-r--r--   0 chineduanene   (501) staff       (20)     1585 2024-03-05 22:30:10.000000 giExtract-1.0.4/bin/giCube
+-rw-r--r--   0 chineduanene   (501) staff       (20)     2031 2024-03-06 17:17:57.000000 giExtract-1.0.4/bin/giExtract
+drwxr-xr-x   0 chineduanene   (501) staff       (20)        0 2024-04-11 14:44:15.950528 giExtract-1.0.4/giExtract/
+-rw-r--r--   0 chineduanene   (501) staff       (20)        0 2024-03-06 17:50:34.000000 giExtract-1.0.4/giExtract/__init__.py
+-rw-r--r--   0 chineduanene   (501) staff       (20)     8984 2022-01-11 16:46:37.000000 giExtract-1.0.4/giExtract/util.py
+drwxr-xr-x   0 chineduanene   (501) staff       (20)        0 2024-04-11 14:44:15.953136 giExtract-1.0.4/giExtract.egg-info/
+-rw-r--r--   0 chineduanene   (501) staff       (20)     4711 2024-04-11 14:44:15.000000 giExtract-1.0.4/giExtract.egg-info/PKG-INFO
+-rw-r--r--   0 chineduanene   (501) staff       (20)      247 2024-04-11 14:44:15.000000 giExtract-1.0.4/giExtract.egg-info/SOURCES.txt
+-rw-r--r--   0 chineduanene   (501) staff       (20)        1 2024-04-11 14:44:15.000000 giExtract-1.0.4/giExtract.egg-info/dependency_links.txt
+-rw-r--r--   0 chineduanene   (501) staff       (20)       87 2024-04-11 14:44:15.000000 giExtract-1.0.4/giExtract.egg-info/requires.txt
+-rw-r--r--   0 chineduanene   (501) staff       (20)       10 2024-04-11 14:44:15.000000 giExtract-1.0.4/giExtract.egg-info/top_level.txt
+-rw-r--r--   0 chineduanene   (501) staff       (20)       38 2024-04-11 14:44:15.954295 giExtract-1.0.4/setup.cfg
+-rw-r--r--   0 chineduanene   (501) staff       (20)     1066 2024-04-11 14:43:35.000000 giExtract-1.0.4/setup.py
```

### Comparing `giExtract-1.0.3/PKG-INFO` & `giExtract-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giExtract
-Version: 1.0.3
+Version: 1.0.4
 Summary: Digital pathology feature extraction
 Home-page: https://github.com/caanene1/giExtract
 Author: Chinedu A. Anene
 Author-email: caanenedr@outlook.com
 License: UNKNOWN
 Download-URL: https://github.com/caanene1/giExtract/releases/download/1.0.6/giExtract-1.0.1-py3-none-any.whl
 Description: # giExtract
```

### Comparing `giExtract-1.0.3/README.md` & `giExtract-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `giExtract-1.0.3/bin/giCube` & `giExtract-1.0.4/bin/giCube`

 * *Files identical despite different names*

### Comparing `giExtract-1.0.3/bin/giExtract` & `giExtract-1.0.4/bin/giExtract`

 * *Files identical despite different names*

### Comparing `giExtract-1.0.3/giExtract/util.py` & `giExtract-1.0.4/giExtract/util.py`

 * *Files identical despite different names*

### Comparing `giExtract-1.0.3/giExtract.egg-info/PKG-INFO` & `giExtract-1.0.4/giExtract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giExtract
-Version: 1.0.3
+Version: 1.0.4
 Summary: Digital pathology feature extraction
 Home-page: https://github.com/caanene1/giExtract
 Author: Chinedu A. Anene
 Author-email: caanenedr@outlook.com
 License: UNKNOWN
 Download-URL: https://github.com/caanene1/giExtract/releases/download/1.0.6/giExtract-1.0.1-py3-none-any.whl
 Description: # giExtract
```

### Comparing `giExtract-1.0.3/setup.py` & `giExtract-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt") as rq:
     install_requires = rq.read()
 
 
 setuptools.setup(
     name="giExtract",
-    version="1.0.3",
+    version="1.0.4",
     scripts=["bin/giExtract", "bin/giCube"],
     author="Chinedu A. Anene",
     author_email="caanenedr@outlook.com",
     description="Digital pathology feature extraction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/caanene1/giExtract",
```

