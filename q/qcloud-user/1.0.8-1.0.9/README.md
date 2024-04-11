# Comparing `tmp/qcloud_user-1.0.8.tar.gz` & `tmp/qcloud_user-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_user-1.0.8.tar", last modified: Mon Jan 22 21:28:53 2024, max compression
+gzip compressed data, was "qcloud_user-1.0.9.tar", last modified: Mon Jan 29 07:21:36 2024, max compression
```

## Comparing `qcloud_user-1.0.8.tar` & `qcloud_user-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2024-01-22 21:28:53.288495 qcloud_user-1.0.8/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.8/LICENSE.txt
--rw-r--r--   0 agilbert   (501) staff       (20)     4775 2024-01-22 21:28:53.288320 qcloud_user-1.0.8/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)     3473 2023-07-12 22:23:41.000000 qcloud_user-1.0.8/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      721 2024-01-22 21:27:00.000000 qcloud_user-1.0.8/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2024-01-22 21:28:53.288125 qcloud_user-1.0.8/qcloud_user.egg-info/
--rw-r--r--   0 agilbert   (501) staff       (20)     4775 2024-01-22 21:28:53.000000 qcloud_user-1.0.8/qcloud_user.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      316 2024-01-22 21:28:53.000000 qcloud_user-1.0.8/qcloud_user.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2024-01-22 21:28:53.000000 qcloud_user-1.0.8/qcloud_user.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       44 2024-01-22 21:28:53.000000 qcloud_user-1.0.8/qcloud_user.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      153 2024-01-22 21:28:53.000000 qcloud_user-1.0.8/qcloud_user.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       12 2024-01-22 21:28:53.000000 qcloud_user-1.0.8/qcloud_user.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2024-01-22 21:28:53.288529 qcloud_user-1.0.8/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      793 2024-01-22 21:26:49.000000 qcloud_user-1.0.8/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2024-01-22 21:28:53.286568 qcloud_user-1.0.8/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2024-01-22 21:28:53.287923 qcloud_user-1.0.8/src/qcloud_user/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.8/src/qcloud_user/__init__.py
--rwxr-x---   0 agilbert   (501) staff       (20)    26550 2024-01-22 21:26:25.000000 qcloud_user-1.0.8/src/qcloud_user/qcloud_user.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2024-01-29 07:21:36.779177 qcloud_user-1.0.9/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.9/LICENSE.txt
+-rw-r--r--   0 agilbert   (501) staff       (20)     4775 2024-01-29 07:21:36.778967 qcloud_user-1.0.9/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)     3473 2023-07-12 22:23:41.000000 qcloud_user-1.0.9/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      721 2024-01-29 07:21:31.000000 qcloud_user-1.0.9/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2024-01-29 07:21:36.778638 qcloud_user-1.0.9/qcloud_user.egg-info/
+-rw-r--r--   0 agilbert   (501) staff       (20)     4775 2024-01-29 07:21:36.000000 qcloud_user-1.0.9/qcloud_user.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      316 2024-01-29 07:21:36.000000 qcloud_user-1.0.9/qcloud_user.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2024-01-29 07:21:36.000000 qcloud_user-1.0.9/qcloud_user.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       44 2024-01-29 07:21:36.000000 qcloud_user-1.0.9/qcloud_user.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      153 2024-01-29 07:21:36.000000 qcloud_user-1.0.9/qcloud_user.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       12 2024-01-29 07:21:36.000000 qcloud_user-1.0.9/qcloud_user.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2024-01-29 07:21:36.779215 qcloud_user-1.0.9/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      793 2024-01-29 07:21:23.000000 qcloud_user-1.0.9/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2024-01-29 07:21:36.777108 qcloud_user-1.0.9/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2024-01-29 07:21:36.778411 qcloud_user-1.0.9/src/qcloud_user/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.9/src/qcloud_user/__init__.py
+-rwxr-x---   0 agilbert   (501) staff       (20)    26551 2024-01-29 07:21:10.000000 qcloud_user-1.0.9/src/qcloud_user/qcloud_user.py
```

### Comparing `qcloud_user-1.0.8/LICENSE.txt` & `qcloud_user-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_user-1.0.8/PKG-INFO` & `qcloud_user-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud_user
-Version: 1.0.8
+Version: 1.0.9
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
```

### Comparing `qcloud_user-1.0.8/README.md` & `qcloud_user-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qcloud_user-1.0.8/pyproject.toml` & `qcloud_user-1.0.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_user"
-version = "1.0.8"
+version = "1.0.9"
 description = "Q-Cloud CLI for users" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_user-1.0.8/qcloud_user.egg-info/PKG-INFO` & `qcloud_user-1.0.9/qcloud_user.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud_user
-Version: 1.0.8
+Version: 1.0.9
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
```

### Comparing `qcloud_user-1.0.8/setup.py` & `qcloud_user-1.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="qcloud_user",
     python_requires='>=3.7',
-    version="1.0.8",
+    version="1.0.9",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="suppor@q-chem.com",
     description="CLI for interacting with Q-Cloud clusters",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=['qcloud_user'],
```

### Comparing `qcloud_user-1.0.8/src/qcloud_user/qcloud_user.py` & `qcloud_user-1.0.9/src/qcloud_user/qcloud_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         else:
            query = f"INSERT INTO jobs VALUES ( ?, ?)"
            self.cursor.execute(query, (id, value))
 
     def remove(self, job_id):
         query = "DELETE FROM jobs WHERE key = ?"
         self.cursor.execute(query, [job_id])
-        self.dump()
+        #self.dump()
  
 
 class JobDB():
     def __init__(self):
         try:
            db_file = os.path.join(pathlib.Path.home(), ".qcloud_jobs.db")
            self.db = dbm.open(db_file,'c')
```

