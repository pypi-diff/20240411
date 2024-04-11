# Comparing `tmp/lapa_database_structure-0.0.7.tar.gz` & `tmp/lapa_database_structure-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_database_structure-0.0.7.tar", last modified: Sat Apr  6 15:08:10 2024, max compression
+gzip compressed data, was "lapa_database_structure-0.0.8.tar", last modified: Wed Apr 10 17:14:47 2024, max compression
```

## Comparing `lapa_database_structure-0.0.7.tar` & `lapa_database_structure-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.441500 lapa_database_structure-0.0.7/lapa_database_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.441500 lapa_database_structure-0.0.7/lapa_database_structure/lapa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/authentication/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa/file_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/file_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/file_storage/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa/public/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/authentication/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/file_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/file_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/file_storage/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/public/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/lapa_database_structure/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:08:10.441500 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 15:08:10.000000 lapa_database_structure-0.0.7/lapa_database_structure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:08:10.445500 lapa_database_structure-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-06 15:08:01.000000 lapa_database_structure-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.968013 lapa_database_structure-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 17:14:47.968013 lapa_database_structure-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa/file_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/file_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/file_storage/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/public/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/file_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/file_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/file_storage/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.968013 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/public/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:14:47.968013 lapa_database_structure-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/setup.py
```

### Comparing `lapa_database_structure-0.0.7/PKG-INFO` & `lapa_database_structure-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lapa_database_structure
-Version: 0.0.7
+Version: 0.0.8
 Summary: database layer for my personal server.
 Home-page: https://github.com/B21amish/lapa_database_structure
-Author: Amish Palkar, thePmSquare, Lav Sharma,Aaditya Sangishetty
+Author: Amish Palkar, thePmSquare, Lav Sharma, Aaditya Sangishetty
 Author-email: amishpalkar302001@gmail.com, thepmsquare@gmail.com, lavsharma2016@gmail.com, adityasehtty35@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,38 +55,43 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.8
+
+- Overhauled authentication schema, again.
+
 ### v0.0.7
 
--  Overhauled authentication schema, 
-- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and UserLogStatus.
+- Overhauled authentication schema,
+- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and
+  UserLogStatus.
 
 ### v0.0.6
 
 - changed db structure
 - removed game db
 - added testing db which is clone of lapa
 
 ### v0.0.5
 
 - file_storage -> public -> File
-  - change file_extension to file_content_type.
-  - file_system_relative_path default change from "." to "".
+    - change file_extension to file_content_type.
+    - file_system_relative_path default change from "." to "".
 
 ### v.0.0.4
 
 - authentication database added with the below tables
-  - user
-  - user_validation_status
-  - user_registration
-  - hashing_algorithm
+    - user
+    - user_validation_status
+    - user_registration
+    - hashing_algorithm
 
 ### v0.0.3
 
 - Changed package name to lapa_database_structure.
 
 ### v0.0.2
```

### Comparing `lapa_database_structure-0.0.7/README.md` & `lapa_database_structure-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,38 +39,43 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.8
+
+- Overhauled authentication schema, again.
+
 ### v0.0.7
 
--  Overhauled authentication schema, 
-- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and UserLogStatus.
+- Overhauled authentication schema,
+- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and
+  UserLogStatus.
 
 ### v0.0.6
 
 - changed db structure
 - removed game db
 - added testing db which is clone of lapa
 
 ### v0.0.5
 
 - file_storage -> public -> File
-  - change file_extension to file_content_type.
-  - file_system_relative_path default change from "." to "".
+    - change file_extension to file_content_type.
+    - file_system_relative_path default change from "." to "".
 
 ### v.0.0.4
 
 - authentication database added with the below tables
-  - user
-  - user_validation_status
-  - user_registration
-  - hashing_algorithm
+    - user
+    - user_validation_status
+    - user_registration
+    - hashing_algorithm
 
 ### v0.0.3
 
 - Changed package name to lapa_database_structure.
 
 ### v0.0.2
```

### Comparing `lapa_database_structure-0.0.7/lapa_database_structure/lapa/file_storage/tables.py` & `lapa_database_structure-0.0.8/lapa_database_structure/lapa/file_storage/tables.py`

 * *Files identical despite different names*

### Comparing `lapa_database_structure-0.0.7/lapa_database_structure/lapa_testing/file_storage/tables.py` & `lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/file_storage/tables.py`

 * *Files identical despite different names*

### Comparing `lapa_database_structure-0.0.7/lapa_database_structure.egg-info/PKG-INFO` & `lapa_database_structure-0.0.8/lapa_database_structure.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lapa-database-structure
-Version: 0.0.7
+Version: 0.0.8
 Summary: database layer for my personal server.
 Home-page: https://github.com/B21amish/lapa_database_structure
-Author: Amish Palkar, thePmSquare, Lav Sharma,Aaditya Sangishetty
+Author: Amish Palkar, thePmSquare, Lav Sharma, Aaditya Sangishetty
 Author-email: amishpalkar302001@gmail.com, thepmsquare@gmail.com, lavsharma2016@gmail.com, adityasehtty35@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -55,38 +55,43 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.8
+
+- Overhauled authentication schema, again.
+
 ### v0.0.7
 
--  Overhauled authentication schema, 
-- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and UserLogStatus.
+- Overhauled authentication schema,
+- introducing new tables: User, UsernameAuthentication, UserProfile, AuthenticationType, UserAccountStatus, UserLog, and
+  UserLogStatus.
 
 ### v0.0.6
 
 - changed db structure
 - removed game db
 - added testing db which is clone of lapa
 
 ### v0.0.5
 
 - file_storage -> public -> File
-  - change file_extension to file_content_type.
-  - file_system_relative_path default change from "." to "".
+    - change file_extension to file_content_type.
+    - file_system_relative_path default change from "." to "".
 
 ### v.0.0.4
 
 - authentication database added with the below tables
-  - user
-  - user_validation_status
-  - user_registration
-  - hashing_algorithm
+    - user
+    - user_validation_status
+    - user_registration
+    - hashing_algorithm
 
 ### v0.0.3
 
 - Changed package name to lapa_database_structure.
 
 ### v0.0.2
```

### Comparing `lapa_database_structure-0.0.7/lapa_database_structure.egg-info/SOURCES.txt` & `lapa_database_structure-0.0.8/lapa_database_structure.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 lapa_database_structure.egg-info/PKG-INFO
 lapa_database_structure.egg-info/SOURCES.txt
 lapa_database_structure.egg-info/dependency_links.txt
 lapa_database_structure.egg-info/requires.txt
 lapa_database_structure.egg-info/top_level.txt
 lapa_database_structure/lapa/__init__.py
 lapa_database_structure/lapa/authentication/__init__.py
+lapa_database_structure/lapa/authentication/enums.py
 lapa_database_structure/lapa/authentication/tables.py
 lapa_database_structure/lapa/file_storage/__init__.py
 lapa_database_structure/lapa/file_storage/tables.py
 lapa_database_structure/lapa/public/__init__.py
 lapa_database_structure/lapa/public/tables.py
 lapa_database_structure/lapa_testing/__init__.py
 lapa_database_structure/lapa_testing/authentication/__init__.py
+lapa_database_structure/lapa_testing/authentication/enums.py
 lapa_database_structure/lapa_testing/authentication/tables.py
 lapa_database_structure/lapa_testing/file_storage/__init__.py
 lapa_database_structure/lapa_testing/file_storage/tables.py
 lapa_database_structure/lapa_testing/public/__init__.py
 lapa_database_structure/lapa_testing/public/tables.py
```

### Comparing `lapa_database_structure-0.0.7/setup.py` & `lapa_database_structure-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_database_structure"
 
 setup(
     name=package_name,
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     package_data={
         package_name: [],
     },
     install_requires=[
         "sqlalchemy>=2.0.23",
     ],
-    author="Amish Palkar, thePmSquare, Lav Sharma,Aaditya Sangishetty",
+    author="Amish Palkar, thePmSquare, Lav Sharma, Aaditya Sangishetty",
     author_email="amishpalkar302001@gmail.com, thepmsquare@gmail.com, lavsharma2016@gmail.com, "
-                 "adityasehtty35@gmail.com",
+    "adityasehtty35@gmail.com",
     description="database layer for my personal server.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url=f"https://github.com/B21amish/{package_name}",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

