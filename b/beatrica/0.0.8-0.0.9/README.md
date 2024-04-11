# Comparing `tmp/beatrica-0.0.8.tar.gz` & `tmp/beatrica-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beatrica-0.0.8.tar", last modified: Thu Apr 11 13:10:54 2024, max compression
+gzip compressed data, was "beatrica-0.0.9.tar", last modified: Thu Apr 11 13:12:53 2024, max compression
```

## Comparing `beatrica-0.0.8.tar` & `beatrica-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:10:54.472977 beatrica-0.0.8/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.8/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 13:10:54.472802 beatrica-0.0.8/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13783 2024-04-11 10:25:00.000000 beatrica-0.0.8/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:10:54.471224 beatrica-0.0.8/beatrica/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.8/beatrica/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8476 2024-04-11 13:10:50.000000 beatrica-0.0.8/beatrica/beatrica.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.8/beatrica/prompts.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:10:54.472231 beatrica-0.0.8/beatrica.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      236 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 13:10:54.000000 beatrica-0.0.8/beatrica.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 13:10:54.473018 beatrica-0.0.8/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1337 2024-04-11 13:10:50.000000 beatrica-0.0.8/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:10:54.472433 beatrica-0.0.8/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.8/tests/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.8/tests/test_beatrica.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:12:53.138779 beatrica-0.0.9/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.9/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 13:12:53.138583 beatrica-0.0.9/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13783 2024-04-11 10:25:00.000000 beatrica-0.0.9/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:12:53.137081 beatrica-0.0.9/beatrica/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.9/beatrica/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8476 2024-04-11 13:10:50.000000 beatrica-0.0.9/beatrica/beatrica.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.9/beatrica/prompts.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:12:53.138040 beatrica-0.0.9/beatrica.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    14312 2024-04-11 13:12:53.000000 beatrica-0.0.9/beatrica.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 13:12:53.000000 beatrica-0.0.9/beatrica.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 13:12:53.000000 beatrica-0.0.9/beatrica.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 13:12:53.000000 beatrica-0.0.9/beatrica.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      220 2024-04-11 13:12:53.000000 beatrica-0.0.9/beatrica.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 13:12:53.000000 beatrica-0.0.9/beatrica.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 13:12:53.138824 beatrica-0.0.9/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1310 2024-04-11 13:12:49.000000 beatrica-0.0.9/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 13:12:53.138254 beatrica-0.0.9/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.9/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.9/tests/test_beatrica.py
```

### Comparing `beatrica-0.0.8/LICENSE` & `beatrica-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.8/PKG-INFO` & `beatrica-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beatrica
-Version: 0.0.8
+Version: 0.0.9
 Summary: Beatrica is a tool for code review automation using large language models.
 Home-page: https://github.com/chigwell/beatrica
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beatrica-0.0.8/README.md` & `beatrica-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.8/beatrica/beatrica.py` & `beatrica-0.0.9/beatrica/beatrica.py`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.8/beatrica/prompts.py` & `beatrica-0.0.9/beatrica/prompts.py`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.8/beatrica.egg-info/PKG-INFO` & `beatrica-0.0.9/beatrica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beatrica
-Version: 0.0.8
+Version: 0.0.9
 Summary: Beatrica is a tool for code review automation using large language models.
 Home-page: https://github.com/chigwell/beatrica
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beatrica-0.0.8/setup.py` & `beatrica-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beatrica',
-    version='0.0.8',
+    version='0.0.9',
     author='Eugene Evstafev',
     author_email='chigwel@gmail.com',
     description="Beatrica is a tool for code review automation using large language models.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/chigwell/beatrica',
     packages=find_packages(),
     install_requires=[
         "rich==13.7.1",
         "beatrica-git==0.1.1",
         "beatrica-embedding==0.1.1",
         "langchain-openai==0.1.2",
         "langchain-mistralai==0.1.1",
-        "pysqlite-binary",
         "chromadb==0.3.29",
     ],
     extras_require={
         'dev': [
             'pytest',
             'pytest-cov',
             'pytest-mock',
```

### Comparing `beatrica-0.0.8/tests/test_beatrica.py` & `beatrica-0.0.9/tests/test_beatrica.py`

 * *Files identical despite different names*

