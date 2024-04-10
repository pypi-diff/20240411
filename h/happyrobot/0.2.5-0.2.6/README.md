# Comparing `tmp/happyrobot-0.2.5.tar.gz` & `tmp/happyrobot-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyrobot-0.2.5.tar", last modified: Wed Apr  3 23:32:38 2024, max compression
+gzip compressed data, was "happyrobot-0.2.6.tar", last modified: Wed Apr 10 23:23:15 2024, max compression
```

## Comparing `happyrobot-0.2.5.tar` & `happyrobot-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 23:32:38.739736 happyrobot-0.2.5/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       88 2024-04-01 22:36:53.000000 happyrobot-0.2.5/HISTORY.rst
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1299 2024-04-01 22:36:53.000000 happyrobot-0.2.5/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      117 2024-04-01 22:36:53.000000 happyrobot-0.2.5/MANIFEST.in
--rw-r--r--   0 pablo     (1000) pablo     (1000)      783 2024-04-03 23:32:38.739736 happyrobot-0.2.5/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       77 2024-04-01 22:38:42.000000 happyrobot-0.2.5/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 23:32:38.739736 happyrobot-0.2.5/happyrobot/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.5/happyrobot/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 23:32:38.739736 happyrobot-0.2.5/happyrobot/models/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.5/happyrobot/models/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      321 2024-04-03 23:32:23.000000 happyrobot-0.2.5/happyrobot/models/call.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      548 2024-04-01 22:36:53.000000 happyrobot-0.2.5/happyrobot/models/event.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3217 2024-04-02 05:14:49.000000 happyrobot-0.2.5/happyrobot/models/message.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 23:32:38.739736 happyrobot-0.2.5/happyrobot/src/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:58:29.000000 happyrobot-0.2.5/happyrobot/src/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 23:32:38.739736 happyrobot-0.2.5/happyrobot/src/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:40:33.000000 happyrobot-0.2.5/happyrobot/src/utils/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      558 2024-04-02 05:18:42.000000 happyrobot-0.2.5/happyrobot/src/utils/date_utils.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1421 2024-04-01 22:58:52.000000 happyrobot-0.2.5/happyrobot/src/utils/message_utils.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 23:32:38.739736 happyrobot-0.2.5/happyrobot.egg-info/
--rw-r--r--   0 pablo     (1000) pablo     (1000)      783 2024-04-03 23:32:38.000000 happyrobot-0.2.5/happyrobot.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      547 2024-04-03 23:32:38.000000 happyrobot-0.2.5/happyrobot.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-03 23:32:38.000000 happyrobot-0.2.5/happyrobot.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-03 15:51:00.000000 happyrobot-0.2.5/happyrobot.egg-info/not-zip-safe
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       13 2024-04-03 23:32:38.000000 happyrobot-0.2.5/happyrobot.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       11 2024-04-03 23:32:38.000000 happyrobot-0.2.5/happyrobot.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       12 2024-04-02 05:17:09.000000 happyrobot-0.2.5/requirements.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2024-04-03 23:32:38.739736 happyrobot-0.2.5/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1179 2024-04-03 23:32:30.000000 happyrobot-0.2.5/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-10 23:23:15.989020 happyrobot-0.2.6/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       88 2024-04-01 22:36:53.000000 happyrobot-0.2.6/HISTORY.rst
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1299 2024-04-01 22:36:53.000000 happyrobot-0.2.6/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      117 2024-04-01 22:36:53.000000 happyrobot-0.2.6/MANIFEST.in
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      783 2024-04-10 23:23:15.989020 happyrobot-0.2.6/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       77 2024-04-01 22:38:42.000000 happyrobot-0.2.6/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-10 23:23:15.989020 happyrobot-0.2.6/happyrobot/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.6/happyrobot/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-10 23:23:15.989020 happyrobot-0.2.6/happyrobot/models/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.6/happyrobot/models/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      321 2024-04-03 23:32:23.000000 happyrobot-0.2.6/happyrobot/models/call.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      548 2024-04-01 22:36:53.000000 happyrobot-0.2.6/happyrobot/models/event.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3217 2024-04-02 05:14:49.000000 happyrobot-0.2.6/happyrobot/models/message.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-10 23:23:15.989020 happyrobot-0.2.6/happyrobot/src/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:58:29.000000 happyrobot-0.2.6/happyrobot/src/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-10 23:23:15.989020 happyrobot-0.2.6/happyrobot/src/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:40:33.000000 happyrobot-0.2.6/happyrobot/src/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      869 2024-04-08 23:46:20.000000 happyrobot-0.2.6/happyrobot/src/utils/date_utils.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1421 2024-04-01 22:58:52.000000 happyrobot-0.2.6/happyrobot/src/utils/message_utils.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-10 23:23:15.989020 happyrobot-0.2.6/happyrobot.egg-info/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      783 2024-04-10 23:23:15.000000 happyrobot-0.2.6/happyrobot.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      547 2024-04-10 23:23:15.000000 happyrobot-0.2.6/happyrobot.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-10 23:23:15.000000 happyrobot-0.2.6/happyrobot.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-03 15:51:00.000000 happyrobot-0.2.6/happyrobot.egg-info/not-zip-safe
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       13 2024-04-10 23:23:15.000000 happyrobot-0.2.6/happyrobot.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       11 2024-04-10 23:23:15.000000 happyrobot-0.2.6/happyrobot.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       12 2024-04-02 05:17:09.000000 happyrobot-0.2.6/requirements.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2024-04-10 23:23:15.989020 happyrobot-0.2.6/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1179 2024-04-10 23:21:05.000000 happyrobot-0.2.6/setup.py
```

### Comparing `happyrobot-0.2.5/LICENSE` & `happyrobot-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.5/PKG-INFO` & `happyrobot-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happyrobot
-Version: 0.2.5
+Version: 0.2.6
 Summary: This package lets you interact with Happyrobot directly from Python.
 Author: Happyrobot
 Author-email: founders@happyrobot.ai
 Keywords: happyrobot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `happyrobot-0.2.5/happyrobot/models/event.py` & `happyrobot-0.2.6/happyrobot/models/event.py`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.5/happyrobot/models/message.py` & `happyrobot-0.2.6/happyrobot/models/message.py`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.5/happyrobot/src/utils/message_utils.py` & `happyrobot-0.2.6/happyrobot/src/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.5/happyrobot.egg-info/PKG-INFO` & `happyrobot-0.2.6/happyrobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happyrobot
-Version: 0.2.5
+Version: 0.2.6
 Summary: This package lets you interact with Happyrobot directly from Python.
 Author: Happyrobot
 Author-email: founders@happyrobot.ai
 Keywords: happyrobot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `happyrobot-0.2.5/happyrobot.egg-info/SOURCES.txt` & `happyrobot-0.2.6/happyrobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.5/setup.py` & `happyrobot-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def read_requirements(file):
     with open(file) as f:
         return f.read().splitlines()
 
 requirements = read_requirements('requirements.txt')
 
-VERSION = '0.2.5'
+VERSION = '0.2.6'
 
 setup(
     author="Happyrobot",
     author_email='founders@happyrobot.ai',
     name='happyrobot',
     python_requires='>=3.9',
     classifiers=[
```

