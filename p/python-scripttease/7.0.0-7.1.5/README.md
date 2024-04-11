# Comparing `tmp/python-scripttease-7.0.0.tar.gz` & `tmp/python-scripttease-7.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-scripttease-7.0.0.tar", last modified: Mon Apr 17 17:40:24 2023, max compression
+gzip compressed data, was "python-scripttease-7.1.5.tar", last modified: Thu Apr 11 16:33:10 2024, max compression
```

## Comparing `python-scripttease-7.0.0.tar` & `python-scripttease-7.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.646536 python-scripttease-7.0.0/
--rw-r--r--   0 shawn      (501) staff       (20)       87 2019-04-26 18:33:34.000000 python-scripttease-7.0.0/DESCRIPTION.txt
--rw-r--r--   0 shawn      (501) staff       (20)     1516 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/LICENSE.txt
--rw-r--r--   0 shawn      (501) staff       (20)      204 2020-09-02 16:16:51.000000 python-scripttease-7.0.0/MANIFEST.in
--rw-r--r--   0 shawn      (501) staff       (20)     1478 2023-04-17 17:40:24.646216 python-scripttease-7.0.0/PKG-INFO
--rw-r--r--   0 shawn      (501) staff       (20)        5 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/VERSION.txt
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.635827 python-scripttease-7.0.0/python_scripttease.egg-info/
--rw-r--r--   0 shawn      (501) staff       (20)     1478 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/PKG-INFO
--rw-r--r--   0 shawn      (501) staff       (20)     1164 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/SOURCES.txt
--rw-r--r--   0 shawn      (501) staff       (20)        1 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/dependency_links.txt
--rw-r--r--   0 shawn      (501) staff       (20)       56 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/entry_points.txt
--rw-r--r--   0 shawn      (501) staff       (20)        1 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/not-zip-safe
--rw-r--r--   0 shawn      (501) staff       (20)       67 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/requires.txt
--rw-r--r--   0 shawn      (501) staff       (20)       12 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/top_level.txt
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.638343 python-scripttease-7.0.0/scripttease/
--rw-r--r--   0 shawn      (501) staff       (20)        0 2020-07-16 18:21:17.000000 python-scripttease-7.0.0/scripttease/__init__.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.639500 python-scripttease-7.0.0/scripttease/cli/
--rw-r--r--   0 shawn      (501) staff       (20)     3573 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/cli/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)     9590 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/cli/initialize.py
--rw-r--r--   0 shawn      (501) staff       (20)     5349 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/cli/subcommands.py
--rw-r--r--   0 shawn      (501) staff       (20)      314 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/constants.py
--rw-r--r--   0 shawn      (501) staff       (20)       84 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/exceptions.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.640584 python-scripttease-7.0.0/scripttease/lib/
--rw-r--r--   0 shawn      (501) staff       (20)        0 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/__init__.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.643846 python-scripttease-7.0.0/scripttease/lib/commands/
--rw-r--r--   0 shawn      (501) staff       (20)        0 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/commands/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)    24600 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/base.py
--rw-r--r--   0 shawn      (501) staff       (20)     7431 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/centos.py
--rw-r--r--   0 shawn      (501) staff       (20)     5186 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/django.py
--rw-r--r--   0 shawn      (501) staff       (20)     3263 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/messages.py
--rw-r--r--   0 shawn      (501) staff       (20)     7386 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/mysql.py
--rw-r--r--   0 shawn      (501) staff       (20)     8705 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/pgsql.py
--rw-r--r--   0 shawn      (501) staff       (20)      281 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/php.py
--rw-r--r--   0 shawn      (501) staff       (20)    19570 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/posix.py
--rw-r--r--   0 shawn      (501) staff       (20)     2046 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/python.py
--rw-r--r--   0 shawn      (501) staff       (20)     9009 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/ubuntu.py
--rw-r--r--   0 shawn      (501) staff       (20)     2028 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/contexts.py
--rw-r--r--   0 shawn      (501) staff       (20)     4425 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/factories.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.645422 python-scripttease-7.0.0/scripttease/lib/loaders/
--rw-r--r--   0 shawn      (501) staff       (20)      177 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/loaders/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)     7511 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/loaders/base.py
--rw-r--r--   0 shawn      (501) staff       (20)     2919 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/loaders/ini.py
--rw-r--r--   0 shawn      (501) staff       (20)     2176 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/loaders/yaml.py
--rw-r--r--   0 shawn      (501) staff       (20)      213 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/variables.py
--rw-r--r--   0 shawn      (501) staff       (20)       68 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/version.py
--rw-r--r--   0 shawn      (501) staff       (20)       38 2023-04-17 17:40:24.646642 python-scripttease-7.0.0/setup.cfg
--rw-r--r--   0 shawn      (501) staff       (20)     2005 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/setup.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       87 2019-04-26 18:33:34.000000 python-scripttease-7.1.5/DESCRIPTION.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     1516 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/LICENSE.txt
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      204 2020-09-02 16:16:51.000000 python-scripttease-7.1.5/MANIFEST.in
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1352 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/PKG-INFO
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        5 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/VERSION.txt
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/python_scripttease.egg-info/
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1352 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/PKG-INFO
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     1164 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/SOURCES.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        1 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/dependency_links.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       55 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/entry_points.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)        1 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/not-zip-safe
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       67 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/requires.txt
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       12 2024-04-11 16:33:10.000000 python-scripttease-7.1.5/python_scripttease.egg-info/top_level.txt
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2020-07-16 18:21:17.000000 python-scripttease-7.1.5/scripttease/__init__.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/cli/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     3573 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/cli/__init__.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     9590 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/cli/initialize.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5349 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/cli/subcommands.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)      402 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/constants.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)       84 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/exceptions.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/lib/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/__init__.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/lib/commands/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)        0 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/__init__.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    25121 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/base.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     7431 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/centos.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     5186 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/django.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     3874 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/messages.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     7386 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/mysql.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     9099 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/pgsql.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      281 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/php.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)    19745 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/commands/posix.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2046 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/python.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     9009 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/commands/ubuntu.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2028 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/contexts.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     4493 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/factories.py
+drwxrwxr-x   0 shawn     (1000) shawn     (1000)        0 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/scripttease/lib/loaders/
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      177 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/loaders/__init__.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)     7723 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/lib/loaders/base.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2919 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/scripttease/lib/loaders/ini.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2176 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/lib/loaders/yaml.py
+-rw-r--r--   0 shawn     (1000) shawn     (1000)      213 2023-04-04 14:50:40.000000 python-scripttease-7.1.5/scripttease/variables.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       82 2024-04-11 16:31:40.000000 python-scripttease-7.1.5/scripttease/version.py
+-rw-rw-r--   0 shawn     (1000) shawn     (1000)       38 2024-04-11 16:33:10.410574 python-scripttease-7.1.5/setup.cfg
+-rw-r--r--   0 shawn     (1000) shawn     (1000)     2005 2023-04-17 17:40:07.000000 python-scripttease-7.1.5/setup.py
```

### Comparing `python-scripttease-7.0.0/LICENSE.txt` & `python-scripttease-7.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/PKG-INFO` & `python-scripttease-7.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: python-scripttease
-Version: 7.0.0
+Version: 7.1.5
 Summary: A collection of classes and commands for automated command line scripting using Python.
 Home-page: https://develmaycare.com/products/python/scripttease/
+Download-URL: https://gittraction.com/diff6/python-scripttease
 Author: Shawn Davis
 Author-email: shawn@develmaycare.com
-License: UNKNOWN
-Download-URL: https://gittraction.com/diff6/python-scripttease
 Project-URL: Documentation, https://docs.diff6.com/en/python-scripttease/latest/
 Project-URL: Source, https://gittraction.com/diff6/python-scripttease
 Project-URL: Tracker, https://gittraction.com/diff6/python-scripttease/issues
-Description: # Python Script Tease
-        
-        ![](https://img.shields.io/badge/status-active-green.svg)
-        ![](https://img.shields.io/badge/stage-stable-green.svg)
-        ![](https://img.shields.io/badge/coverage-100%25-green.svg)
-        
-        A collection of classes and commands for automated command line scripting using Python.
-        
-        ## Install
-        
-        ```bash
-        pip install python-scripttease;
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Python Script Tease
+
+![](https://img.shields.io/badge/status-active-green.svg)
+![](https://img.shields.io/badge/stage-stable-green.svg)
+![](https://img.shields.io/badge/coverage-100%25-green.svg)
+
+A collection of classes and commands for automated command line scripting using Python.
+
+## Install
+
+```bash
+pip install python-scripttease;
+```
```

### Comparing `python-scripttease-7.0.0/python_scripttease.egg-info/PKG-INFO` & `python-scripttease-7.1.5/python_scripttease.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: python-scripttease
-Version: 7.0.0
+Version: 7.1.5
 Summary: A collection of classes and commands for automated command line scripting using Python.
 Home-page: https://develmaycare.com/products/python/scripttease/
+Download-URL: https://gittraction.com/diff6/python-scripttease
 Author: Shawn Davis
 Author-email: shawn@develmaycare.com
-License: UNKNOWN
-Download-URL: https://gittraction.com/diff6/python-scripttease
 Project-URL: Documentation, https://docs.diff6.com/en/python-scripttease/latest/
 Project-URL: Source, https://gittraction.com/diff6/python-scripttease
 Project-URL: Tracker, https://gittraction.com/diff6/python-scripttease/issues
-Description: # Python Script Tease
-        
-        ![](https://img.shields.io/badge/status-active-green.svg)
-        ![](https://img.shields.io/badge/stage-stable-green.svg)
-        ![](https://img.shields.io/badge/coverage-100%25-green.svg)
-        
-        A collection of classes and commands for automated command line scripting using Python.
-        
-        ## Install
-        
-        ```bash
-        pip install python-scripttease;
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Python Script Tease
+
+![](https://img.shields.io/badge/status-active-green.svg)
+![](https://img.shields.io/badge/stage-stable-green.svg)
+![](https://img.shields.io/badge/coverage-100%25-green.svg)
+
+A collection of classes and commands for automated command line scripting using Python.
+
+## Install
+
+```bash
+pip install python-scripttease;
+```
```

### Comparing `python-scripttease-7.0.0/python_scripttease.egg-info/SOURCES.txt` & `python-scripttease-7.1.5/python_scripttease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/cli/__init__.py` & `python-scripttease-7.1.5/scripttease/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/cli/initialize.py` & `python-scripttease-7.1.5/scripttease/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/cli/subcommands.py` & `python-scripttease-7.1.5/scripttease/cli/subcommands.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/base.py` & `python-scripttease-7.1.5/scripttease/lib/commands/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -787,7 +787,20 @@
 
         return source
 
     @property
     def is_itemized(self):
         # return "$item" in self.target
         return False
+
+'''
+class UnsupportedCommand(Command):
+    """A command class that may be used when a command is not supported on the target operating system."""
+
+    def __init__(self, statement, **kwargs):
+        """Initialize the command."""
+        self._original_statement = statement
+        super().__init__(statement, **kwargs)
+
+        def get_statement(self, cd=True, include_comment=True, include_register=True, include_stop=True):
+            return "The %s command is not supported by the target operating system: %s"
+'''
```

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/centos.py` & `python-scripttease-7.1.5/scripttease/lib/commands/centos.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/django.py` & `python-scripttease-7.1.5/scripttease/lib/commands/django.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/messages.py` & `python-scripttease-7.1.5/scripttease/lib/commands/messages.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,14 +46,35 @@
     :param heading: Optional heading for the output.
     :type heading: str
 
     """
     return Content("explain", message=message, heading=heading, **kwargs)
 
 
+def mattermost(message, url=None, **kwargs):
+    """Send a message to a Mattermost channel.
+
+    :param message: The message to be sent.
+    :type message: str
+
+    :param url: The URL of the Mattermost channel.
+    :type url: str
+
+    """
+    if url is None:
+        raise InvalidInput("mattermost command requires a url parameter.")
+
+    statement = list()
+    statement.append("curl -X POST -H 'Content-type: application/json' --data")
+    statement.append('\'{"text": "%s"}\'' % message)
+    statement.append(url)
+
+    return Command(" ".join(statement), **kwargs)
+
+
 def screenshot(image, caption=None, css=None, height=None, width=None, **kwargs):
     """Create a screenshot for documentation.
 
     :param image: The URL or path to the image file.
     :type image: str
 
     :param caption: A caption for the image.
@@ -86,15 +107,15 @@
         raise InvalidInput("Slack command requires a url parameter.")
 
     statement = list()
     statement.append("curl -X POST -H 'Content-type: application/json' --data")
     statement.append('\'{"text": "%s"}\'' % message)
     statement.append(url)
 
-    return Command(statement, **kwargs)
+    return Command(" ".join(statement), **kwargs)
 
 
 def twist(message, title="Notice", url=None, **kwargs):
     """Send a message to Twist.
 
     :param message: The message to be displayed.
     :type message: str
@@ -117,11 +138,12 @@
     return Command(" ".join(statement), **kwargs)
 
 
 MESSAGE_MAPPINGS = {
     'dialog': dialog,
     'echo': echo,
     'explain': explain,
+    'mattermost': mattermost,
     'screenshot': screenshot,
     'slack': slack,
     'twist': twist,
 }
```

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/mysql.py` & `python-scripttease-7.1.5/scripttease/lib/commands/mysql.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/pgsql.py` & `python-scripttease-7.1.5/scripttease/lib/commands/pgsql.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "PGSQL_MAPPINGS",
     "pgsql_create",
     "pgsql_drop",
     "pgsql_dump",
     "pgsql_exists",
     "pgsql_grant",
     "pgsql_load",
+    "pgsql_sql",
     "pgsql_user",
 )
 
 
 def pgsql(command, *args, excluded_kwargs=None, host="localhost", password=None, port=5432, user="postgres", **kwargs):
     """Get a postgres-related command using commonly required parameters.
 
@@ -96,14 +97,17 @@
 
     if owner is not None:
         kwargs['owner'] = owner
 
     if template is not None:
         kwargs['template'] = template
 
+    # SELECT 'CREATE DATABASE <db_name>'
+    # WHERE NOT EXISTS (SELECT FROM pg_database WHERE datname = '<db_name>')\gexec
+
     # psql -U postgres -tc "SELECT 1 FROM pg_database WHERE datname = '<your db name>'" | grep -q 1 | psql -U postgres -c "CREATE DATABASE <your db name>"
     # first = pgsql("psql", **kwargs)
     #
     # first_query = "SELECT 1 FROM pg_database WHERE datname = '%s'" % database
     # first_statement = '%s -tc "%s" | grep -q 1' % (first.statement, first_query)
     #
     # kwargs_without_password = kwargs.copy()
@@ -235,14 +239,25 @@
 
     kwargs['dbname'] = database
     kwargs['file'] = path
 
     return pgsql("psql", **kwargs)
 
 
+def pgsql_sql(statement, database="template1", **kwargs):
+    kwargs.setdefault("comment", "run SQL statement")
+
+    kwargs['dbname'] = database
+
+    command = pgsql("psql", **kwargs)
+    command.statement += ' -c "%s"' % statement
+
+    return command
+
+
 def pgsql_user(name, admin_pass=None, admin_user="postgres", op="create", password=None, **kwargs):
     """Work with a PostgreSQL user.
 
     :param name: The username.
     :type name: str
 
     :param admin_pass: The password for the user with admin privileges.
@@ -271,15 +286,15 @@
         return command
     elif op in ("drop", "remove"):
         kwargs.setdefault("comment", "remove %s postgres user" % name)
 
         return pgsql("dropuser", name, password=admin_pass, user=admin_user, **kwargs)
     elif op == "exists":
         kwargs.setdefault("comment", "determine if %s postgres user exists" % name)
-        kwargs.setdefault("register", "pgsql_use_exists")
+        kwargs.setdefault("register", "pgsql_user_exists")
 
         command = pgsql("psql", password=admin_pass, user=admin_user, **kwargs)
 
         sql = "SELECT 1 FROM pgsql_roles WHERE rolname='%s'" % name
 
         command.statement += ' -c "%s"' % sql
 
@@ -290,10 +305,10 @@
 
 PGSQL_MAPPINGS = {
     'pgsql.create': pgsql_create,
     'pgsql.drop': pgsql_drop,
     'pgsql.dump': pgsql_dump,
     'pgsql.exists': pgsql_exists,
     'pgsql.grant': pgsql_grant,
-    # 'pgsql.sql': pgsql_exec,
+    'pgsql.sql': pgsql_sql,
     'pgsql.user': pgsql_user,
 }
```

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/posix.py` & `python-scripttease-7.1.5/scripttease/lib/commands/posix.py`

 * *Files 2% similar despite different names*

```diff
@@ -535,14 +535,15 @@
     if links:
         tokens.append("--copy-links")
 
     if delete:
         tokens.append("--delete")
 
     if exclude is not None:
+        # tokens.append("--exclude-from={'%s'}" % exclude)
         tokens.append("--exclude-from=%s" % exclude)
 
     # --partial and --progress
     tokens.append("-P")
 
     if recursive:
         tokens.append("--recursive")
@@ -649,25 +650,27 @@
     kwargs.setdefault("comment", "sync %s with %s" % (source, target))
 
     # rsync -e "ssh -i $(SSH_KEY) -p $(SSH_PORT)" -P -rvzc --delete
     # $(OUTPUTH_PATH) $(SSH_USER)@$(SSH_HOST):$(UPLOAD_PATH) --cvs-exclude;
 
     tokens = list()
     tokens.append("rsync")
-    tokens.append("--cvs-exclude")
+    # tokens.append("--cvs-exclude")
+    tokens.append("--exclude=.git")
     tokens.append("--checksum")
     tokens.append("--compress")
 
     if links:
         tokens.append("--copy-links")
 
     if delete:
         tokens.append("--delete")
 
     if exclude is not None:
+        # tokens.append("--exclude-from={'%s'}" % exclude)
         tokens.append("--exclude-from=%s" % exclude)
 
     # --partial and --progress
     tokens.append("-P")
 
     if recursive:
         tokens.append("--recursive")
@@ -737,14 +740,15 @@
     'copy': copy,
     'dir': directory,
     'extract': extract,
     'link': link,
     'move': move,
     'perms': perms,
     'prompt': prompt,
+    'push': rsync,
     'remove': remove,
     'replace': replace,
     'run': run,
     'rsync': rsync,
     'scopy': scopy,
     'ssl': certbot,
     'sync': sync,
```

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/python.py` & `python-scripttease-7.1.5/scripttease/lib/commands/python.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/lib/commands/ubuntu.py` & `python-scripttease-7.1.5/scripttease/lib/commands/ubuntu.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/lib/contexts.py` & `python-scripttease-7.1.5/scripttease/lib/contexts.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/lib/factories.py` & `python-scripttease-7.1.5/scripttease/lib/factories.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     :param profile: The operating system profile to use for finding commands.
     :type profile: str
 
     :returns: A list of instances that may be Command, ItemizedCommand, or Template.
 
     """
     # Identify the command mappings to be used.
-    if profile == PROFILE.CENTOS:
+    if profile in (PROFILE.CENTOS, PROFILE.FEDORA, PROFILE.REDHAT):
         _mappings = CENTOS_MAPPINGS
-    elif profile == PROFILE.UBUNTU:
+    elif profile in (PROFILE.DEBIAN, PROFILE.POP_OS, PROFILE.UBUNTU):
         _mappings = UBUNTU_MAPPINGS
     else:
         log.error("Unsupported or unrecognized profile: %s" % profile)
         return None
 
     # Update mappings if custom mappings have been supplied.
     if mappings is not None:
```

### Comparing `python-scripttease-7.0.0/scripttease/lib/loaders/base.py` & `python-scripttease-7.1.5/scripttease/lib/loaders/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -217,34 +217,34 @@
 
         """
         if key in ("environments", "environs", "envs", "env"):
             _key = "environments"
             if type(value) in (list, tuple):
                 _value = value
             else:
-                _value = split_csv(value)
+                _value = split_csv(value) if "," in value else split_csv(value, separator=" ")
         elif key in ("func", "function"):
             _key = "function"
             _value = value
         elif key == "groups":
             _key = "groups"
             if type(value) in (list, tuple):
                 _value = value
             else:
-                _value = split_csv(value)
+                _value = split_csv(value) if "," in value else split_csv(value, separator=" ")
         elif key == "items":
             _key = "items"
             if type(value) in (list, tuple):
                 _value = value
             else:
-                _value = split_csv(value)
+                _value = split_csv(value) if "," in value else split_csv(value, separator=" ")
         elif key == "tags":
             _key = "tags"
             if type(value) in (list, tuple):
                 _value = value
             else:
-                _value = split_csv(value)
+                _value = split_csv(value) if "," in value else split_csv(value, separator=" ")
         else:
             _key = key
             _value = smart_cast(value)
 
         return _key, _value
```

### Comparing `python-scripttease-7.0.0/scripttease/lib/loaders/ini.py` & `python-scripttease-7.1.5/scripttease/lib/loaders/ini.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/scripttease/lib/loaders/yaml.py` & `python-scripttease-7.1.5/scripttease/lib/loaders/yaml.py`

 * *Files identical despite different names*

### Comparing `python-scripttease-7.0.0/setup.py` & `python-scripttease-7.1.5/setup.py`

 * *Files identical despite different names*

