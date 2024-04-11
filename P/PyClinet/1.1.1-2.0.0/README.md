# Comparing `tmp/PyClinet-1.1.1.tar.gz` & `tmp/PyClinet-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyClinet-1.1.1.tar", last modified: Fri Apr  5 08:49:01 2024, max compression
+gzip compressed data, was "PyClinet-2.0.0.tar", last modified: Thu Apr 11 09:39:29 2024, max compression
```

## Comparing `PyClinet-1.1.1.tar` & `PyClinet-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 08:49:01.338945 PyClinet-1.1.1/
--rw-rw-rw-   0        0        0     1091 2024-04-04 15:04:40.000000 PyClinet-1.1.1/LICENCE
--rw-rw-rw-   0        0        0      605 2024-04-05 08:49:01.338945 PyClinet-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 08:49:01.323324 PyClinet-1.1.1/PyClinet/
--rw-rw-rw-   0        0        0     6827 2024-03-30 08:50:58.000000 PyClinet-1.1.1/PyClinet/Encryption.py
--rw-rw-rw-   0        0        0       29 2024-04-05 08:23:40.000000 PyClinet-1.1.1/PyClinet/__init__.py
--rw-rw-rw-   0        0        0    23160 2024-04-05 08:22:37.000000 PyClinet-1.1.1/PyClinet/client.py
-drwxrwxrwx   0        0        0        0 2024-04-05 08:49:01.323324 PyClinet-1.1.1/PyClinet.egg-info/
--rw-rw-rw-   0        0        0      605 2024-04-05 08:49:01.000000 PyClinet-1.1.1/PyClinet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-05 08:49:01.000000 PyClinet-1.1.1/PyClinet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 08:49:01.000000 PyClinet-1.1.1/PyClinet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-05 08:49:01.000000 PyClinet-1.1.1/PyClinet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      170 2024-04-05 07:30:11.000000 PyClinet-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 08:49:01.338945 PyClinet-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      565 2024-04-05 08:47:23.000000 PyClinet-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:39:29.237381 PyClinet-2.0.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 15:04:40.000000 PyClinet-2.0.0/LICENCE
+-rw-rw-rw-   0        0        0      605 2024-04-11 09:39:29.237381 PyClinet-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 09:39:29.237381 PyClinet-2.0.0/PyClinet/
+-rw-rw-rw-   0        0        0     6827 2024-04-06 09:25:47.000000 PyClinet-2.0.0/PyClinet/Encryption.py
+-rw-rw-rw-   0        0        0       29 2024-04-05 08:23:40.000000 PyClinet-2.0.0/PyClinet/__init__.py
+-rw-rw-rw-   0        0        0    35944 2024-04-11 09:29:05.000000 PyClinet-2.0.0/PyClinet/client.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:39:29.237381 PyClinet-2.0.0/PyClinet.egg-info/
+-rw-rw-rw-   0        0        0      605 2024-04-11 09:39:29.000000 PyClinet-2.0.0/PyClinet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-11 09:39:29.000000 PyClinet-2.0.0/PyClinet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:39:29.000000 PyClinet-2.0.0/PyClinet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 09:39:29.000000 PyClinet-2.0.0/PyClinet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      170 2024-04-05 07:30:11.000000 PyClinet-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 09:39:29.237381 PyClinet-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      562 2024-04-10 17:28:11.000000 PyClinet-2.0.0/setup.py
```

### Comparing `PyClinet-1.1.1/LICENCE` & `PyClinet-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `PyClinet-1.1.1/PKG-INFO` & `PyClinet-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyClinet
-Version: 1.1.1
+Version: 2.0.0
 Summary: Luis Rubika libry
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PyClinet-1.1.1/PyClinet/Encryption.py` & `PyClinet-2.0.0/PyClinet/Encryption.py`

 * *Files identical despite different names*

### Comparing `PyClinet-1.1.1/PyClinet.egg-info/PKG-INFO` & `PyClinet-2.0.0/PyClinet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyClinet
-Version: 1.1.1
+Version: 2.0.0
 Summary: Luis Rubika libry
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `PyClinet-1.1.1/setup.py` & `PyClinet-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup,find_packages
 
 setup(
     name='PyClinet',
-    version='1.1.1',
-    packages= find_packages(),
+    version='2.0.0',
+    packages= ['PyClinet'],
     url='https://guides.github.com/features/mastering-markdown/',
     license='MIT',
     author='Luis',
     author_email='mm12mok18@gmail.com',
     description='Luis Rubika libry',
     long_description= open("README.md",'r').read(),
     classifiers=[
```

