# Comparing `tmp/beatrica-0.0.4.tar.gz` & `tmp/beatrica-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beatrica-0.0.4.tar", last modified: Thu Apr 11 10:18:32 2024, max compression
+gzip compressed data, was "beatrica-0.0.5.tar", last modified: Thu Apr 11 10:20:07 2024, max compression
```

## Comparing `beatrica-0.0.4.tar` & `beatrica-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:18:32.869487 beatrica-0.0.4/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.4/LICENSE
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13013 2024-04-11 10:18:32.869303 beatrica-0.0.4/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    12484 2024-04-11 09:39:23.000000 beatrica-0.0.4/README.md
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:18:32.867454 beatrica-0.0.4/beatrica/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.4/beatrica/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8472 2024-04-11 09:39:23.000000 beatrica-0.0.4/beatrica/beatrica.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.4/beatrica/prompts.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:18:32.868763 beatrica-0.0.4/beatrica.egg-info/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13013 2024-04-11 10:18:32.000000 beatrica-0.0.4/beatrica.egg-info/PKG-INFO
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 10:18:32.000000 beatrica-0.0.4/beatrica.egg-info/SOURCES.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 10:18:32.000000 beatrica-0.0.4/beatrica.egg-info/dependency_links.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 10:18:32.000000 beatrica-0.0.4/beatrica.egg-info/entry_points.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)      236 2024-04-11 10:18:32.000000 beatrica-0.0.4/beatrica.egg-info/requires.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 10:18:32.000000 beatrica-0.0.4/beatrica.egg-info/top_level.txt
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 10:18:32.869546 beatrica-0.0.4/setup.cfg
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1337 2024-04-11 10:18:30.000000 beatrica-0.0.4/setup.py
-drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:18:32.869005 beatrica-0.0.4/tests/
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.4/tests/__init__.py
--rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.4/tests/test_beatrica.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:20:07.510657 beatrica-0.0.5/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    34523 2024-01-31 16:51:58.000000 beatrica-0.0.5/LICENSE
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13013 2024-04-11 10:20:07.510457 beatrica-0.0.5/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    12484 2024-04-11 09:39:23.000000 beatrica-0.0.5/README.md
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:20:07.508710 beatrica-0.0.5/beatrica/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.5/beatrica/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     8472 2024-04-11 09:39:23.000000 beatrica-0.0.5/beatrica/beatrica.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1641 2024-04-11 09:39:23.000000 beatrica-0.0.5/beatrica/prompts.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:20:07.509724 beatrica-0.0.5/beatrica.egg-info/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)    13013 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/PKG-INFO
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      323 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/SOURCES.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        1 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/dependency_links.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       52 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/entry_points.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)      236 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/requires.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       15 2024-04-11 10:20:07.000000 beatrica-0.0.5/beatrica.egg-info/top_level.txt
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)       38 2024-04-11 10:20:07.510719 beatrica-0.0.5/setup.cfg
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1337 2024-04-11 10:20:02.000000 beatrica-0.0.5/setup.py
+drwxr-xr-x   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 10:20:07.510006 beatrica-0.0.5/tests/
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)        0 2024-04-11 09:39:23.000000 beatrica-0.0.5/tests/__init__.py
+-rw-r--r--   0 evgeniievstafev   (503) staff       (20)     1074 2024-04-11 09:39:23.000000 beatrica-0.0.5/tests/test_beatrica.py
```

### Comparing `beatrica-0.0.4/LICENSE` & `beatrica-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.4/PKG-INFO` & `beatrica-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beatrica
-Version: 0.0.4
+Version: 0.0.5
 Summary: Beatrica is a tool for code review automation using large language models.
 Home-page: https://github.com/chigwell/beatrica
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beatrica-0.0.4/README.md` & `beatrica-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.4/beatrica/beatrica.py` & `beatrica-0.0.5/beatrica/beatrica.py`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.4/beatrica/prompts.py` & `beatrica-0.0.5/beatrica/prompts.py`

 * *Files identical despite different names*

### Comparing `beatrica-0.0.4/beatrica.egg-info/PKG-INFO` & `beatrica-0.0.5/beatrica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beatrica
-Version: 0.0.4
+Version: 0.0.5
 Summary: Beatrica is a tool for code review automation using large language models.
 Home-page: https://github.com/chigwell/beatrica
 Author: Eugene Evstafev
 Author-email: chigwel@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beatrica-0.0.4/setup.py` & `beatrica-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='beatrica',
-    version='0.0.4',
+    version='0.0.5',
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
-        "beatrica-embedding==0.1.0",
+        "beatrica-embedding==0.1.1",
         "langchain-openai==0.1.2",
         "langchain-mistralai==0.1.1",
         "pysqlite-binary",
         "chromadb==0.3.29",
     ],
     extras_require={
         'dev': [
```

### Comparing `beatrica-0.0.4/tests/test_beatrica.py` & `beatrica-0.0.5/tests/test_beatrica.py`

 * *Files identical despite different names*

