# Comparing `tmp/s3path-0.5.3.tar.gz` & `tmp/s3path-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3path-0.5.3.tar", last modified: Thu Apr 11 08:55:40 2024, max compression
+gzip compressed data, was "s3path-0.5.4.tar", last modified: Thu Apr 11 20:52:10 2024, max compression
```

## Comparing `s3path-0.5.3.tar` & `s3path-0.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:40.421542 s3path-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-11 08:55:32.000000 s3path-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 08:55:32.000000 s3path-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-11 08:55:40.421542 s3path-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-11 08:55:32.000000 s3path-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:40.421542 s3path-0.5.3/s3path/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 08:55:32.000000 s3path-0.5.3/s3path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17211 2024-04-11 08:55:32.000000 s3path-0.5.3/s3path/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28111 2024-04-11 08:55:32.000000 s3path-0.5.3/s3path/current_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    50156 2024-04-11 08:55:32.000000 s3path-0.5.3/s3path/old_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:40.421542 s3path-0.5.3/s3path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 08:55:40.421542 s3path-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-11 08:55:32.000000 s3path-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:40.421542 s3path-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-11 08:55:32.000000 s3path-0.5.3/tests/test_not_supported.py
--rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-11 08:55:32.000000 s3path-0.5.3/tests/test_path_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-11 08:55:32.000000 s3path-0.5.3/tests/test_pure_path_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-11 08:55:32.000000 s3path-0.5.3/tests/test_s3path_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:52:10.987448 s3path-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-11 20:52:05.000000 s3path-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 20:52:05.000000 s3path-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-11 20:52:10.987448 s3path-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-11 20:52:05.000000 s3path-0.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:52:10.987448 s3path-0.5.4/s3path/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 20:52:05.000000 s3path-0.5.4/s3path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17211 2024-04-11 20:52:05.000000 s3path-0.5.4/s3path/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28111 2024-04-11 20:52:05.000000 s3path-0.5.4/s3path/current_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50156 2024-04-11 20:52:05.000000 s3path-0.5.4/s3path/old_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:52:10.987448 s3path-0.5.4/s3path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 20:52:10.991448 s3path-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-11 20:52:05.000000 s3path-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:52:10.987448 s3path-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-11 20:52:05.000000 s3path-0.5.4/tests/test_not_supported.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-11 20:52:05.000000 s3path-0.5.4/tests/test_path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-11 20:52:05.000000 s3path-0.5.4/tests/test_pure_path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-11 20:52:05.000000 s3path-0.5.4/tests/test_s3path_configuration.py
```

### Comparing `s3path-0.5.3/LICENSE` & `s3path-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `s3path-0.5.3/PKG-INFO` & `s3path-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3path
-Version: 0.5.3
+Version: 0.5.4
 Home-page: https://github.com/liormizr/s3path
 Author: Lior Mizrahi
 Author-email: li.mizr@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: boto3>=1.16.35
-Requires-Dist: smart-open
+Requires-Dist: smart-open>=5.1.0
 
 S3Path
 ======
 
 .. image:: https://badgen.net/pypi/v/s3path
     :target: https://pypi.org/project/s3path/
     :alt: Latest version
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: s3path Version: 0.5.3 Home-page: https://
+Metadata-Version: 2.1 Name: s3path Version: 0.5.4 Home-page: https://
 github.com/liormizr/s3path Author: Lior Mizrahi Author-email: li.mizr@gmail.com
 License: Apache 2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
 text/x-rst License-File: LICENSE Requires-Dist: boto3>=1.16.35 Requires-Dist:
-smart-open S3Path ====== .. image:: https://badgen.net/pypi/v/s3path :target:
-https://pypi.org/project/s3path/ :alt: Latest version .. image:: https://
-github.com/liormizr/s3path/actions/workflows/testing.yml/
+smart-open>=5.1.0 S3Path ====== .. image:: https://badgen.net/pypi/v/s3path :
+target: https://pypi.org/project/s3path/ :alt: Latest version .. image:: https:
+//github.com/liormizr/s3path/actions/workflows/testing.yml/
 badge.svg?branch=master&event=push :target: https://github.com/liormizr/s3path/
 actions/workflows/testing.yml :alt: S3Path CI S3Path provide a Python
 convenient File-System/Path like interface for AWS S3 Service using boto3 S3
 resource as a driver. Like pathlib, but for S3 Buckets
 ________________________________ AWS S3 is among the most popular cloud storage
 solutions. It's object storage, is built to store and retrieve various amounts
 of data from anywhere. Currently, Python developers use Boto3 as the default
```

### Comparing `s3path-0.5.3/README.rst` & `s3path-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `s3path-0.5.3/s3path/__init__.py` & `s3path-0.5.4/s3path/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 s3path provides a Pythonic API to S3 by wrapping boto3 with pathlib interface
 """
 import sys
 
 from . import accessor
 
-__version__ = '0.5.3'
+__version__ = '0.5.4'
 __all__ = (
     'register_configuration_parameter',
     'StatResult',
     'PureS3Path',
     'S3Path',
     'VersionedS3Path',
     'PureVersionedS3Path',
```

### Comparing `s3path-0.5.3/s3path/accessor.py` & `s3path-0.5.4/s3path/accessor.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.3/s3path/current_version.py` & `s3path-0.5.4/s3path/current_version.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.3/s3path/old_versions.py` & `s3path-0.5.4/s3path/old_versions.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.3/s3path.egg-info/PKG-INFO` & `s3path-0.5.4/s3path.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3path
-Version: 0.5.3
+Version: 0.5.4
 Home-page: https://github.com/liormizr/s3path
 Author: Lior Mizrahi
 Author-email: li.mizr@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: boto3>=1.16.35
-Requires-Dist: smart-open
+Requires-Dist: smart-open>=5.1.0
 
 S3Path
 ======
 
 .. image:: https://badgen.net/pypi/v/s3path
     :target: https://pypi.org/project/s3path/
     :alt: Latest version
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: s3path Version: 0.5.3 Home-page: https://
+Metadata-Version: 2.1 Name: s3path Version: 0.5.4 Home-page: https://
 github.com/liormizr/s3path Author: Lior Mizrahi Author-email: li.mizr@gmail.com
 License: Apache 2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
 text/x-rst License-File: LICENSE Requires-Dist: boto3>=1.16.35 Requires-Dist:
-smart-open S3Path ====== .. image:: https://badgen.net/pypi/v/s3path :target:
-https://pypi.org/project/s3path/ :alt: Latest version .. image:: https://
-github.com/liormizr/s3path/actions/workflows/testing.yml/
+smart-open>=5.1.0 S3Path ====== .. image:: https://badgen.net/pypi/v/s3path :
+target: https://pypi.org/project/s3path/ :alt: Latest version .. image:: https:
+//github.com/liormizr/s3path/actions/workflows/testing.yml/
 badge.svg?branch=master&event=push :target: https://github.com/liormizr/s3path/
 actions/workflows/testing.yml :alt: S3Path CI S3Path provide a Python
 convenient File-System/Path like interface for AWS S3 Service using boto3 S3
 resource as a driver. Like pathlib, but for S3 Buckets
 ________________________________ AWS S3 is among the most popular cloud storage
 solutions. It's object storage, is built to store and retrieve various amounts
 of data from anywhere. Currently, Python developers use Boto3 as the default
```

### Comparing `s3path-0.5.3/setup.py` & `s3path-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 setup(
     name='s3path',
-    version='0.5.3',
+    version='0.5.4',
     url='https://github.com/liormizr/s3path',
     author='Lior Mizrahi',
     author_email='li.mizr@gmail.com',
     packages=['s3path'],
     install_requires=[
         'boto3>=1.16.35',
-        'smart-open',
+        'smart-open>=5.1.0',
     ],
     license='Apache 2.0',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     python_requires='>=3.8',
     include_package_data=True,
     classifiers=[
```

### Comparing `s3path-0.5.3/tests/test_not_supported.py` & `s3path-0.5.4/tests/test_not_supported.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.3/tests/test_path_operations.py` & `s3path-0.5.4/tests/test_path_operations.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.3/tests/test_pure_path_operations.py` & `s3path-0.5.4/tests/test_pure_path_operations.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.3/tests/test_s3path_configuration.py` & `s3path-0.5.4/tests/test_s3path_configuration.py`

 * *Files identical despite different names*

