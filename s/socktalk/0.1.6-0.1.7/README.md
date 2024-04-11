# Comparing `tmp/socktalk-0.1.6.tar.gz` & `tmp/socktalk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socktalk-0.1.6.tar", last modified: Thu Apr 11 12:03:15 2024, max compression
+gzip compressed data, was "socktalk-0.1.7.tar", last modified: Thu Apr 11 14:44:26 2024, max compression
```

## Comparing `socktalk-0.1.6.tar` & `socktalk-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 12:03:15.628796 socktalk-0.1.6/
--rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.6/LICENSE
--rw-r--r--   0 mike      (1000) mike      (1000)     4136 2024-04-11 12:03:15.628796 socktalk-0.1.6/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3648 2024-04-11 12:01:29.000000 socktalk-0.1.6/README.md
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 12:03:15.624796 socktalk-0.1.6/server_client/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.6/server_client/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5390 2024-04-11 11:39:20.000000 socktalk-0.1.6/server_client/ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.6/server_client/client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.6/server_client/server.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.1.6/server_client/start_server_with_ai_client.py
--rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-11 12:03:15.628796 socktalk-0.1.6/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     1002 2024-04-11 12:03:03.000000 socktalk-0.1.6/setup.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 12:03:15.628796 socktalk-0.1.6/socktalk.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     4136 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/entry_points.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-11 12:03:15.000000 socktalk-0.1.6/socktalk.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 14:44:26.723447 socktalk-0.1.7/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    16725 2024-03-31 10:42:32.000000 socktalk-0.1.7/LICENSE
+-rw-r--r--   0 mike      (1000) mike      (1000)     4136 2024-04-11 14:44:26.719447 socktalk-0.1.7/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3648 2024-04-11 12:01:29.000000 socktalk-0.1.7/README.md
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 14:44:26.719447 socktalk-0.1.7/server_client/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2024-03-25 12:32:15.000000 socktalk-0.1.7/server_client/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5390 2024-04-11 11:39:20.000000 socktalk-0.1.7/server_client/ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6133 2024-04-10 10:18:17.000000 socktalk-0.1.7/server_client/client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3984 2024-04-10 09:06:22.000000 socktalk-0.1.7/server_client/server.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3456 2024-04-11 11:27:09.000000 socktalk-0.1.7/server_client/start_server_with_ai_client.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)       38 2024-04-11 14:44:26.723447 socktalk-0.1.7/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1002 2024-04-11 14:43:17.000000 socktalk-0.1.7/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-04-11 14:44:26.719447 socktalk-0.1.7/socktalk.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     4136 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      366 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      157 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/entry_points.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       30 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       14 2024-04-11 14:44:26.000000 socktalk-0.1.7/socktalk.egg-info/top_level.txt
```

### Comparing `socktalk-0.1.6/LICENSE` & `socktalk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.6/PKG-INFO` & `socktalk-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/socktalk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `socktalk-0.1.6/README.md` & `socktalk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.6/server_client/ai_client.py` & `socktalk-0.1.7/server_client/ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.6/server_client/client.py` & `socktalk-0.1.7/server_client/client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.6/server_client/server.py` & `socktalk-0.1.7/server_client/server.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.6/server_client/start_server_with_ai_client.py` & `socktalk-0.1.7/server_client/start_server_with_ai_client.py`

 * *Files identical despite different names*

### Comparing `socktalk-0.1.6/setup.py` & `socktalk-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='socktalk',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     project_urls={
         'Source': 'https://github.com/mdkmk/socktalk'
     },
     install_requires=[
         'PyQt5==5.15.10',
         'openai==1.14.2'
```

### Comparing `socktalk-0.1.6/socktalk.egg-info/PKG-INFO` & `socktalk-0.1.7/socktalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socktalk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Socket-based AI chat server and multi-user chat client
 Project-URL: Source, https://github.com/mdkmk/socktalk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

