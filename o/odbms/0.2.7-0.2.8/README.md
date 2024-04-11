# Comparing `tmp/odbms-0.2.7.tar.gz` & `tmp/odbms-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbms-0.2.7.tar", last modified: Wed Mar  6 10:38:00 2024, max compression
+gzip compressed data, was "odbms-0.2.8.tar", last modified: Thu Apr 11 16:23:33 2024, max compression
```

## Comparing `odbms-0.2.7.tar` & `odbms-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 10:38:00.210399 odbms-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-03-06 10:37:55.000000 odbms-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-06 10:37:55.000000 odbms-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-06 10:38:00.210399 odbms-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-06 10:37:55.000000 odbms-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 10:38:00.206399 odbms-0.2.7/odbms/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/dbms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10731 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/postgresqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-03-06 10:37:55.000000 odbms-0.2.7/odbms/sqlitedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 10:38:00.210399 odbms-0.2.7/odbms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-06 10:38:00.000000 odbms-0.2.7/odbms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-06 10:38:00.000000 odbms-0.2.7/odbms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 10:38:00.000000 odbms-0.2.7/odbms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-06 10:38:00.000000 odbms-0.2.7/odbms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-06 10:38:00.000000 odbms-0.2.7/odbms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 10:38:00.210399 odbms-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-06 10:37:55.000000 odbms-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:23:33.885322 odbms-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-11 16:23:29.000000 odbms-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 16:23:29.000000 odbms-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-11 16:23:33.885322 odbms-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 16:23:29.000000 odbms-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:23:33.881322 odbms-0.2.8/odbms/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/dbms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10731 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/postgresqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-11 16:23:29.000000 odbms-0.2.8/odbms/sqlitedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:23:33.885322 odbms-0.2.8/odbms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-11 16:23:33.000000 odbms-0.2.8/odbms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 16:23:33.000000 odbms-0.2.8/odbms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:23:33.000000 odbms-0.2.8/odbms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 16:23:33.000000 odbms-0.2.8/odbms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 16:23:33.000000 odbms-0.2.8/odbms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:23:33.885322 odbms-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-11 16:23:29.000000 odbms-0.2.8/setup.py
```

### Comparing `odbms-0.2.7/LICENSE` & `odbms-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `odbms-0.2.7/PKG-INFO` & `odbms-0.2.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.2.7
+Version: 0.2.8
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker sqlite mysql mongodb
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dotenv
 Requires-Dist: pymongo
+Requires-Dist: psycopg2
 
 # odbms
 Python package for Managing Mysql, Mongodb and Sqlite instances
 
 ## Installation
 
 ```shell
```

### Comparing `odbms-0.2.7/odbms/database.py` & `odbms-0.2.8/odbms/database.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.7/odbms/dbms.py` & `odbms-0.2.8/odbms/dbms.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.7/odbms/model.py` & `odbms-0.2.8/odbms/model.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.7/odbms/mongodb.py` & `odbms-0.2.8/odbms/mongodb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.7/odbms/mysqldb.py` & `odbms-0.2.8/odbms/mysqldb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.7/odbms/postgresqldb.py` & `odbms-0.2.8/odbms/postgresqldb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.7/odbms/sqlitedb.py` & `odbms-0.2.8/odbms/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `odbms-0.2.7/odbms.egg-info/PKG-INFO` & `odbms-0.2.8/odbms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbms
-Version: 0.2.7
+Version: 0.2.8
 Summary: Database client for Mysql, MongoDB and Sqlite
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/odbms/
 Project-URL: Tracker, https://github.com/theonlyamos/odbms/issues
 Keywords: python3 runit developer serverless architecture docker sqlite mysql mongodb
 Classifier: Development Status :: 3 - Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dotenv
 Requires-Dist: pymongo
+Requires-Dist: psycopg2
 
 # odbms
 Python package for Managing Mysql, Mongodb and Sqlite instances
 
 ## Installation
 
 ```shell
```

### Comparing `odbms-0.2.7/setup.py` & `odbms-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.2.7'
+VERSION = '0.2.8'
 
 with open('README.md', 'rt') as file:
     description = file.read()
 
 setup(
     name='odbms',
     version=VERSION,
@@ -13,15 +13,15 @@
     author_email='theonlyamos@gmail.com',
     description='Database client for Mysql, MongoDB and Sqlite',
     long_description=description,
     packages=find_packages(),
     long_description_content_type = "text/markdown",
     include_package_data=True,
     # install_requires=['python-dotenv','pymongo', 'mysql', 'mysql-connector', 'mysql-connector-python'],
-    install_requires=['python-dotenv','pymongo'],
+    install_requires=['python-dotenv','pymongo', 'psycopg2'],
     keywords='python3 runit developer serverless architecture docker sqlite mysql mongodb',
     project_urls={
         'Source': 'https://github.com/theonlyamos/odbms/',
         'Tracker': 'https://github.com/theonlyamos/odbms/issues',
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
```

