# Comparing `tmp/daraz_scrapper-0.1.0.tar.gz` & `tmp/daraz-scrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daraz_scrapper-0.1.0.tar", last modified: Thu Apr 11 07:14:46 2024, max compression
+gzip compressed data, was "daraz-scrapper-0.1.1.tar", last modified: Thu Apr 11 10:37:33 2024, max compression
```

## Comparing `daraz_scrapper-0.1.0.tar` & `daraz-scrapper-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 khudi     (1000) khudi     (1000)        0 2024-04-11 07:14:46.821001 daraz_scrapper-0.1.0/
--rw-rw-r--   0 khudi     (1000) khudi     (1000)     1314 2024-04-11 07:14:46.821001 daraz_scrapper-0.1.0/PKG-INFO
--rw-rw-r--   0 khudi     (1000) khudi     (1000)      573 2024-04-11 07:14:43.000000 daraz_scrapper-0.1.0/README.md
-drwxrwxr-x   0 khudi     (1000) khudi     (1000)        0 2024-04-11 07:14:46.821001 daraz_scrapper-0.1.0/daraz_scrapper.egg-info/
--rw-rw-r--   0 khudi     (1000) khudi     (1000)     1314 2024-04-11 07:14:46.000000 daraz_scrapper-0.1.0/daraz_scrapper.egg-info/PKG-INFO
--rw-rw-r--   0 khudi     (1000) khudi     (1000)      286 2024-04-11 07:14:46.000000 daraz_scrapper-0.1.0/daraz_scrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 khudi     (1000) khudi     (1000)        1 2024-04-11 07:14:46.000000 daraz_scrapper-0.1.0/daraz_scrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 khudi     (1000) khudi     (1000)       20 2024-04-11 07:14:46.000000 daraz_scrapper-0.1.0/daraz_scrapper.egg-info/entry_points.txt
--rw-rw-r--   0 khudi     (1000) khudi     (1000)       36 2024-04-11 07:14:46.000000 daraz_scrapper-0.1.0/daraz_scrapper.egg-info/requires.txt
--rw-rw-r--   0 khudi     (1000) khudi     (1000)        6 2024-04-11 07:14:46.000000 daraz_scrapper-0.1.0/daraz_scrapper.egg-info/top_level.txt
--rw-rw-r--   0 khudi     (1000) khudi     (1000)       38 2024-04-11 07:14:46.825001 daraz_scrapper-0.1.0/setup.cfg
--rw-rw-r--   0 khudi     (1000) khudi     (1000)     1307 2024-04-11 07:11:07.000000 daraz_scrapper-0.1.0/setup.py
-drwxrwxr-x   0 khudi     (1000) khudi     (1000)        0 2024-04-11 07:14:46.821001 daraz_scrapper-0.1.0/utils/
--rw-rw-r--   0 khudi     (1000) khudi     (1000)       62 2024-04-11 04:38:45.000000 daraz_scrapper-0.1.0/utils/__init__.py
--rw-rw-r--   0 khudi     (1000) khudi     (1000)     9814 2024-04-11 04:39:17.000000 daraz_scrapper-0.1.0/utils/user_agent.py
+drwxrwxr-x   0 khudi     (1000) khudi     (1000)        0 2024-04-11 10:37:33.027886 daraz-scrapper-0.1.1/
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)     1312 2024-04-11 10:37:33.027886 daraz-scrapper-0.1.1/PKG-INFO
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)      573 2024-04-11 07:14:43.000000 daraz-scrapper-0.1.1/README.md
+drwxrwxr-x   0 khudi     (1000) khudi     (1000)        0 2024-04-11 10:37:33.027886 daraz-scrapper-0.1.1/daraz_scrapper.egg-info/
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)     1312 2024-04-11 10:37:32.000000 daraz-scrapper-0.1.1/daraz_scrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)      245 2024-04-11 10:37:32.000000 daraz-scrapper-0.1.1/daraz_scrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)        1 2024-04-11 10:37:32.000000 daraz-scrapper-0.1.1/daraz_scrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)       36 2024-04-11 10:37:32.000000 daraz-scrapper-0.1.1/daraz_scrapper.egg-info/requires.txt
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)        6 2024-04-11 10:37:32.000000 daraz-scrapper-0.1.1/daraz_scrapper.egg-info/top_level.txt
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)       38 2024-04-11 10:37:33.027886 daraz-scrapper-0.1.1/setup.cfg
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)     1079 2024-04-11 10:36:53.000000 daraz-scrapper-0.1.1/setup.py
+drwxrwxr-x   0 khudi     (1000) khudi     (1000)        0 2024-04-11 10:37:33.027886 daraz-scrapper-0.1.1/utils/
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)       62 2024-04-11 04:38:45.000000 daraz-scrapper-0.1.1/utils/__init__.py
+-rw-rw-r--   0 khudi     (1000) khudi     (1000)     9814 2024-04-11 04:39:17.000000 daraz-scrapper-0.1.1/utils/user_agent.py
```

### Comparing `daraz_scrapper-0.1.0/PKG-INFO` & `daraz-scrapper-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: daraz_scrapper
-Version: 0.1.0
+Name: daraz-scrapper
+Version: 0.1.1
 Summary: A scrapper for Daraz platform
 Home-page: https://github.com/Anas-art-source/daraz_scrapper
-Author: Your Name
-Author-email: your.email@example.com
+Author: Anas Khan
+Author-email: anas985822@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `daraz_scrapper-0.1.0/README.md` & `daraz-scrapper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `daraz_scrapper-0.1.0/daraz_scrapper.egg-info/PKG-INFO` & `daraz-scrapper-0.1.1/daraz_scrapper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: daraz-scrapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A scrapper for Daraz platform
 Home-page: https://github.com/Anas-art-source/daraz_scrapper
-Author: Your Name
-Author-email: your.email@example.com
+Author: Anas Khan
+Author-email: anas985822@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `daraz_scrapper-0.1.0/setup.py` & `daraz-scrapper-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='daraz_scrapper',
-    version='0.1.0',
-    author='Your Name',
-    author_email='your.email@example.com',
+    name='daraz-scrapper',
+    version='0.1.1',
+    author='Anas Khan',
+    author_email='anas985822@gmail.com',
     description='A scrapper for Daraz platform',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Anas-art-source/daraz_scrapper',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'pandas',
         'numpy',
         'bs4',
         'requests',
         'tqdm',
         'lxml'  # Assuming you are using lxml as parser
     ],
-    entry_points={
-        'console_scripts': [
-            # If you have a script meant to be executed directly, you can list it here.
-            # 'daraz-scrapper = daraz_scrapper.scrapper:main_function',
-        ],
-    },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

### Comparing `daraz_scrapper-0.1.0/utils/user_agent.py` & `daraz-scrapper-0.1.1/utils/user_agent.py`

 * *Files identical despite different names*

