# Comparing `tmp/dataminer-0.1.1.tar.gz` & `tmp/dataminer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataminer-0.1.1.tar", last modified: Mon Mar 25 07:58:28 2024, max compression
+gzip compressed data, was "dataminer-0.1.2.tar", last modified: Thu Apr 11 08:52:52 2024, max compression
```

## Comparing `dataminer-0.1.1.tar` & `dataminer-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-03-25 07:58:28.180274 dataminer-0.1.1/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)    11357 2024-03-25 06:41:25.000000 dataminer-0.1.1/LICENSE
--rw-r--r--   0 javaite   (1000) javaite   (1000)      494 2024-03-25 07:58:28.180274 dataminer-0.1.1/PKG-INFO
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-03-25 07:08:21.000000 dataminer-0.1.1/README.md
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-03-25 07:58:28.172274 dataminer-0.1.1/dataminer/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-03-25 06:49:34.000000 dataminer-0.1.1/dataminer/__init__.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-03-25 07:58:28.176274 dataminer-0.1.1/dataminer/datax/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-03-25 07:46:19.000000 dataminer-0.1.1/dataminer/datax/__init__.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     4302 2024-03-25 07:50:27.000000 dataminer-0.1.1/dataminer/datax/jobbuilder.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     3558 2024-03-25 07:47:21.000000 dataminer-0.1.1/dataminer/datax/runner.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-03-25 07:58:28.180274 dataminer-0.1.1/dataminer/sqla/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-03-25 07:50:23.000000 dataminer-0.1.1/dataminer/sqla/__init__.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     1624 2024-03-25 07:51:53.000000 dataminer-0.1.1/dataminer/sqla/engine_utils.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      284 2024-03-25 07:55:12.000000 dataminer-0.1.1/dataminer/sqla/query_utils.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-03-25 07:58:28.176274 dataminer-0.1.1/dataminer.egg-info/
--rw-r--r--   0 javaite   (1000) javaite   (1000)      494 2024-03-25 07:58:28.000000 dataminer-0.1.1/dataminer.egg-info/PKG-INFO
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      352 2024-03-25 07:58:28.000000 dataminer-0.1.1/dataminer.egg-info/SOURCES.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        1 2024-03-25 07:58:28.000000 dataminer-0.1.1/dataminer.egg-info/dependency_links.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       10 2024-03-25 07:58:28.000000 dataminer-0.1.1/dataminer.egg-info/top_level.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       38 2024-03-25 07:58:28.180274 dataminer-0.1.1/setup.cfg
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      683 2024-03-25 07:55:54.000000 dataminer-0.1.1/setup.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.755700 dataminer-0.1.2/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)    11357 2024-04-11 08:51:19.000000 dataminer-0.1.2/LICENSE
+-rw-r--r--   0 javaite   (1000) javaite   (1000)      520 2024-04-11 08:52:52.755700 dataminer-0.1.2/PKG-INFO
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:51:19.000000 dataminer-0.1.2/README.md
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.751700 dataminer-0.1.2/dataminer/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/__init__.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.755700 dataminer-0.1.2/dataminer/datax/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/datax/__init__.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     4302 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/datax/job_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     3558 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/datax/runner.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.755700 dataminer-0.1.2/dataminer/sqla/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/sqla/__init__.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     1624 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/sqla/engine_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      332 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/sqla/query_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     1443 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/sqla/table_helpers.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.751700 dataminer-0.1.2/dataminer.egg-info/
+-rw-r--r--   0 javaite   (1000) javaite   (1000)      520 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/PKG-INFO
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      421 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/SOURCES.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        1 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/dependency_links.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       11 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/requires.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       10 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/top_level.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       38 2024-04-11 08:52:52.755700 dataminer-0.1.2/setup.cfg
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      705 2024-04-11 08:51:19.000000 dataminer-0.1.2/setup.py
```

### Comparing `dataminer-0.1.1/LICENSE` & `dataminer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.1/dataminer/datax/jobbuilder.py` & `dataminer-0.1.2/dataminer/datax/job_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.1/dataminer/datax/runner.py` & `dataminer-0.1.2/dataminer/datax/runner.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.1/dataminer/sqla/engine_utils.py` & `dataminer-0.1.2/dataminer/sqla/engine_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.1/setup.py` & `dataminer-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dataminer',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
+        'sqlalchemy',
     ],
     author='javaite',
     author_email='javaite@126.com',
     description='A set of data processing tools.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://gitee.com/javaite_code/dataminer.git',
```

