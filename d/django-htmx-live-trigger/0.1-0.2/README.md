# Comparing `tmp/django-htmx-live-trigger-0.1.tar.gz` & `tmp/django-htmx-live-trigger-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-live-trigger-0.1.tar", last modified: Thu Apr 11 16:02:34 2024, max compression
+gzip compressed data, was "django-htmx-live-trigger-0.2.tar", last modified: Thu Apr 11 16:27:06 2024, max compression
```

## Comparing `django-htmx-live-trigger-0.1.tar` & `django-htmx-live-trigger-0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:02:34.838740 django-htmx-live-trigger-0.1/
--rw-r--r--   0 paulik123   (502) staff       (20)     1093 2024-04-03 17:16:36.000000 django-htmx-live-trigger-0.1/LICENSE
--rw-r--r--   0 paulik123   (502) staff       (20)      225 2024-04-11 14:51:26.000000 django-htmx-live-trigger-0.1/MANIFEST.in
--rw-r--r--   0 paulik123   (502) staff       (20)     1064 2024-04-11 16:02:34.838361 django-htmx-live-trigger-0.1/PKG-INFO
--rw-r--r--   0 paulik123   (502) staff       (20)        4 2024-04-03 17:15:29.000000 django-htmx-live-trigger-0.1/README.rst
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:02:34.830901 django-htmx-live-trigger-0.1/django_htmx_live_trigger/
--rw-r--r--   0 paulik123   (502) staff       (20)      318 2024-04-11 15:36:27.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger/__init__.py
--rw-r--r--   0 paulik123   (502) staff       (20)       63 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger/admin.py
--rw-r--r--   0 paulik123   (502) staff       (20)      202 2024-04-11 14:58:42.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger/apps.py
--rw-r--r--   0 paulik123   (502) staff       (20)      513 2024-04-11 14:41:29.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger/consumers.py
--rw-r--r--   0 paulik123   (502) staff       (20)       57 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger/models.py
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:02:34.820143 django-htmx-live-trigger-0.1/django_htmx_live_trigger/static/
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:02:34.820427 django-htmx-live-trigger-0.1/django_htmx_live_trigger/static/django_htmx_live_trigger/
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:02:34.835907 django-htmx-live-trigger-0.1/django_htmx_live_trigger/static/django_htmx_live_trigger/js/
--rw-r--r--   0 paulik123   (502) staff       (20)     9425 2024-04-09 18:32:30.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger/static/django_htmx_live_trigger/js/htmx-ws-events.js
--rw-r--r--   0 paulik123   (502) staff       (20)       60 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger/tests.py
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:02:34.837046 django-htmx-live-trigger-0.1/django_htmx_live_trigger.egg-info/
--rw-r--r--   0 paulik123   (502) staff       (20)     1064 2024-04-11 16:02:34.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger.egg-info/PKG-INFO
--rw-r--r--   0 paulik123   (502) staff       (20)      592 2024-04-11 16:02:34.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger.egg-info/SOURCES.txt
--rw-r--r--   0 paulik123   (502) staff       (20)        1 2024-04-11 16:02:34.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger.egg-info/dependency_links.txt
--rw-r--r--   0 paulik123   (502) staff       (20)       40 2024-04-11 16:02:34.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger.egg-info/requires.txt
--rw-r--r--   0 paulik123   (502) staff       (20)       25 2024-04-11 16:02:34.000000 django-htmx-live-trigger-0.1/django_htmx_live_trigger.egg-info/top_level.txt
--rw-r--r--   0 paulik123   (502) staff       (20)       88 2024-04-03 17:17:54.000000 django-htmx-live-trigger-0.1/pyproject.toml
--rw-r--r--   0 paulik123   (502) staff       (20)      994 2024-04-11 16:02:34.839883 django-htmx-live-trigger-0.1/setup.cfg
--rw-r--r--   0 paulik123   (502) staff       (20)       37 2024-04-03 17:25:11.000000 django-htmx-live-trigger-0.1/setup.py
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.520079 django-htmx-live-trigger-0.2/
+-rw-r--r--   0 paulik123   (502) staff       (20)     1093 2024-04-03 17:16:36.000000 django-htmx-live-trigger-0.2/LICENSE
+-rw-r--r--   0 paulik123   (502) staff       (20)      225 2024-04-11 14:51:26.000000 django-htmx-live-trigger-0.2/MANIFEST.in
+-rw-r--r--   0 paulik123   (502) staff       (20)     1126 2024-04-11 16:27:06.519823 django-htmx-live-trigger-0.2/PKG-INFO
+-rw-r--r--   0 paulik123   (502) staff       (20)      278 2024-04-11 16:20:20.000000 django-htmx-live-trigger-0.2/README.md
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.512130 django-htmx-live-trigger-0.2/django_htmx_live_trigger/
+-rw-r--r--   0 paulik123   (502) staff       (20)      318 2024-04-11 15:36:27.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/__init__.py
+-rw-r--r--   0 paulik123   (502) staff       (20)       63 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/admin.py
+-rw-r--r--   0 paulik123   (502) staff       (20)      202 2024-04-11 14:58:42.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/apps.py
+-rw-r--r--   0 paulik123   (502) staff       (20)      513 2024-04-11 14:41:29.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/consumers.py
+-rw-r--r--   0 paulik123   (502) staff       (20)       57 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/models.py
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.505355 django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.505495 django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/django_htmx_live_trigger/
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.517912 django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/django_htmx_live_trigger/js/
+-rw-r--r--   0 paulik123   (502) staff       (20)     9425 2024-04-09 18:32:30.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/django_htmx_live_trigger/js/htmx-ws-events.js
+-rw-r--r--   0 paulik123   (502) staff       (20)       60 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/tests.py
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.518825 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/
+-rw-r--r--   0 paulik123   (502) staff       (20)     1126 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/PKG-INFO
+-rw-r--r--   0 paulik123   (502) staff       (20)      591 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/SOURCES.txt
+-rw-r--r--   0 paulik123   (502) staff       (20)        1 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/dependency_links.txt
+-rw-r--r--   0 paulik123   (502) staff       (20)       78 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/requires.txt
+-rw-r--r--   0 paulik123   (502) staff       (20)       25 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/top_level.txt
+-rw-r--r--   0 paulik123   (502) staff       (20)       88 2024-04-03 17:17:54.000000 django-htmx-live-trigger-0.2/pyproject.toml
+-rw-r--r--   0 paulik123   (502) staff       (20)     1034 2024-04-11 16:27:06.521133 django-htmx-live-trigger-0.2/setup.cfg
+-rw-r--r--   0 paulik123   (502) staff       (20)       37 2024-04-03 17:25:11.000000 django-htmx-live-trigger-0.2/setup.py
```

### Comparing `django-htmx-live-trigger-0.1/LICENSE` & `django-htmx-live-trigger-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-live-trigger-0.1/PKG-INFO` & `django-htmx-live-trigger-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-live-trigger
-Version: 0.1
+Version: 0.2
 Summary: Realtime updates in Django using HTMX and websockets.
 Home-page: https://github.com/paulik123
 Author: Cornel Kenef
 Author-email: paul@2na.dev
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -22,9 +22,9 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Django>=4.2
 Requires-Dist: channels>=4.0
 Requires-Dist: daphne>=4.0.0
-
-TODO
+Requires-Dist: django-redis>=5.0
+Requires-Dist: channels-redis>=4.0
```

### Comparing `django-htmx-live-trigger-0.1/django_htmx_live_trigger/consumers.py` & `django-htmx-live-trigger-0.2/django_htmx_live_trigger/consumers.py`

 * *Files identical despite different names*

### Comparing `django-htmx-live-trigger-0.1/django_htmx_live_trigger/static/django_htmx_live_trigger/js/htmx-ws-events.js` & `django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/django_htmx_live_trigger/js/htmx-ws-events.js`

 * *Files identical despite different names*

### Comparing `django-htmx-live-trigger-0.1/django_htmx_live_trigger.egg-info/PKG-INFO` & `django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-live-trigger
-Version: 0.1
+Version: 0.2
 Summary: Realtime updates in Django using HTMX and websockets.
 Home-page: https://github.com/paulik123
 Author: Cornel Kenef
 Author-email: paul@2na.dev
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -22,9 +22,9 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: Django>=4.2
 Requires-Dist: channels>=4.0
 Requires-Dist: daphne>=4.0.0
-
-TODO
+Requires-Dist: django-redis>=5.0
+Requires-Dist: channels-redis>=4.0
```

### Comparing `django-htmx-live-trigger-0.1/django_htmx_live_trigger.egg-info/SOURCES.txt` & `django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 setup.cfg
 setup.py
 django_htmx_live_trigger/__init__.py
 django_htmx_live_trigger/admin.py
 django_htmx_live_trigger/apps.py
 django_htmx_live_trigger/consumers.py
```

### Comparing `django-htmx-live-trigger-0.1/setup.cfg` & `django-htmx-live-trigger-0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-htmx-live-trigger
-version = 0.1
+version = 0.2
 description = Realtime updates in Django using HTMX and websockets.
 long_description = file: README.rst
 url = https://github.com/paulik123
 author = Cornel Kenef
 author_email = paul@2na.dev
 license = MIT
 classifiers = 
@@ -28,12 +28,14 @@
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	Django >= 4.2
 	channels >= 4.0
 	daphne>=4.0.0
+	django-redis>=5.0
+	channels-redis>=4.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

