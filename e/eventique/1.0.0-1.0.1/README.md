# Comparing `tmp/eventique-1.0.0.tar.gz` & `tmp/eventique-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventique-1.0.0.tar", last modified: Thu Apr 11 12:12:00 2024, max compression
+gzip compressed data, was "eventique-1.0.1.tar", last modified: Thu Apr 11 12:14:42 2024, max compression
```

## Comparing `eventique-1.0.0.tar` & `eventique-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 12:12:00.799284 eventique-1.0.0/
--rw-rw-rw-   0        0        0       41 2024-04-11 11:58:48.000000 eventique-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2089 2024-04-11 12:12:00.794983 eventique-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1677 2024-04-11 11:43:02.000000 eventique-1.0.0/README.md
--rw-rw-rw-   0        0        0        5 2024-04-11 11:43:02.000000 eventique-1.0.0/VERSION
-drwxrwxrwx   0        0        0        0 2024-04-11 12:12:00.781213 eventique-1.0.0/eventique/
--rw-rw-rw-   0        0        0    11793 2024-04-11 11:43:02.000000 eventique-1.0.0/eventique/EventsHandler.py
--rw-rw-rw-   0        0        0     1905 2024-04-11 11:43:02.000000 eventique-1.0.0/eventique/Listener.py
--rw-rw-rw-   0        0        0      810 2024-04-11 11:43:02.000000 eventique-1.0.0/eventique/ThreadSharedSingleton.py
--rw-rw-rw-   0        0        0        0 2024-04-11 11:43:02.000000 eventique-1.0.0/eventique/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 12:12:00.794473 eventique-1.0.0/eventique.egg-info/
--rw-rw-rw-   0        0        0     2089 2024-04-11 12:12:00.000000 eventique-1.0.0/eventique.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-11 12:12:00.000000 eventique-1.0.0/eventique.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 12:12:00.000000 eventique-1.0.0/eventique.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 12:12:00.000000 eventique-1.0.0/eventique.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-04-11 11:43:02.000000 eventique-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 12:12:00.799715 eventique-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1392 2024-04-11 12:11:45.000000 eventique-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 12:14:42.650273 eventique-1.0.1/
+-rw-rw-rw-   0        0        0       41 2024-04-11 11:58:48.000000 eventique-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2089 2024-04-11 12:14:42.648277 eventique-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1677 2024-04-11 11:43:02.000000 eventique-1.0.1/README.md
+-rw-rw-rw-   0        0        0        5 2024-04-11 12:13:35.000000 eventique-1.0.1/VERSION
+drwxrwxrwx   0        0        0        0 2024-04-11 12:14:42.633363 eventique-1.0.1/eventique/
+-rw-rw-rw-   0        0        0    11793 2024-04-11 11:43:02.000000 eventique-1.0.1/eventique/EventsHandler.py
+-rw-rw-rw-   0        0        0     1905 2024-04-11 11:43:02.000000 eventique-1.0.1/eventique/Listener.py
+-rw-rw-rw-   0        0        0      810 2024-04-11 11:43:02.000000 eventique-1.0.1/eventique/ThreadSharedSingleton.py
+-rw-rw-rw-   0        0        0        0 2024-04-11 11:43:02.000000 eventique-1.0.1/eventique/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 12:14:42.643452 eventique-1.0.1/eventique.egg-info/
+-rw-rw-rw-   0        0        0     2089 2024-04-11 12:14:42.000000 eventique-1.0.1/eventique.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-11 12:14:42.000000 eventique-1.0.1/eventique.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 12:14:42.000000 eventique-1.0.1/eventique.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 12:14:42.000000 eventique-1.0.1/eventique.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-04-11 11:43:02.000000 eventique-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 12:14:42.650273 eventique-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2024-04-11 12:11:45.000000 eventique-1.0.1/setup.py
```

### Comparing `eventique-1.0.0/PKG-INFO` & `eventique-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventique
-Version: 1.0.0
+Version: 1.0.1
 Summary: Light and standalone python events manager.
 Home-page: https://github.com/hadamrd/eventique
 Author: MAJDOUB Khalid
 Author-email: majdoub.khalid@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `eventique-1.0.0/README.md` & `eventique-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `eventique-1.0.0/eventique/EventsHandler.py` & `eventique-1.0.1/eventique/EventsHandler.py`

 * *Files identical despite different names*

### Comparing `eventique-1.0.0/eventique/Listener.py` & `eventique-1.0.1/eventique/Listener.py`

 * *Files identical despite different names*

### Comparing `eventique-1.0.0/eventique/ThreadSharedSingleton.py` & `eventique-1.0.1/eventique/ThreadSharedSingleton.py`

 * *Files identical despite different names*

### Comparing `eventique-1.0.0/eventique.egg-info/PKG-INFO` & `eventique-1.0.1/eventique.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventique
-Version: 1.0.0
+Version: 1.0.1
 Summary: Light and standalone python events manager.
 Home-page: https://github.com/hadamrd/eventique
 Author: MAJDOUB Khalid
 Author-email: majdoub.khalid@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `eventique-1.0.0/setup.py` & `eventique-1.0.1/setup.py`

 * *Files identical despite different names*

