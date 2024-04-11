# Comparing `tmp/django-htmx-live-trigger-0.2.tar.gz` & `tmp/django-htmx-live-trigger-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-live-trigger-0.2.tar", last modified: Thu Apr 11 16:27:06 2024, max compression
+gzip compressed data, was "django-htmx-live-trigger-0.3.tar", last modified: Thu Apr 11 19:31:30 2024, max compression
```

## Comparing `django-htmx-live-trigger-0.2.tar` & `django-htmx-live-trigger-0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.520079 django-htmx-live-trigger-0.2/
--rw-r--r--   0 paulik123   (502) staff       (20)     1093 2024-04-03 17:16:36.000000 django-htmx-live-trigger-0.2/LICENSE
--rw-r--r--   0 paulik123   (502) staff       (20)      225 2024-04-11 14:51:26.000000 django-htmx-live-trigger-0.2/MANIFEST.in
--rw-r--r--   0 paulik123   (502) staff       (20)     1126 2024-04-11 16:27:06.519823 django-htmx-live-trigger-0.2/PKG-INFO
--rw-r--r--   0 paulik123   (502) staff       (20)      278 2024-04-11 16:20:20.000000 django-htmx-live-trigger-0.2/README.md
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.512130 django-htmx-live-trigger-0.2/django_htmx_live_trigger/
--rw-r--r--   0 paulik123   (502) staff       (20)      318 2024-04-11 15:36:27.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/__init__.py
--rw-r--r--   0 paulik123   (502) staff       (20)       63 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/admin.py
--rw-r--r--   0 paulik123   (502) staff       (20)      202 2024-04-11 14:58:42.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/apps.py
--rw-r--r--   0 paulik123   (502) staff       (20)      513 2024-04-11 14:41:29.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/consumers.py
--rw-r--r--   0 paulik123   (502) staff       (20)       57 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/models.py
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.505355 django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.505495 django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/django_htmx_live_trigger/
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.517912 django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/django_htmx_live_trigger/js/
--rw-r--r--   0 paulik123   (502) staff       (20)     9425 2024-04-09 18:32:30.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/django_htmx_live_trigger/js/htmx-ws-events.js
--rw-r--r--   0 paulik123   (502) staff       (20)       60 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger/tests.py
-drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 16:27:06.518825 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/
--rw-r--r--   0 paulik123   (502) staff       (20)     1126 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/PKG-INFO
--rw-r--r--   0 paulik123   (502) staff       (20)      591 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/SOURCES.txt
--rw-r--r--   0 paulik123   (502) staff       (20)        1 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/dependency_links.txt
--rw-r--r--   0 paulik123   (502) staff       (20)       78 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/requires.txt
--rw-r--r--   0 paulik123   (502) staff       (20)       25 2024-04-11 16:27:06.000000 django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/top_level.txt
--rw-r--r--   0 paulik123   (502) staff       (20)       88 2024-04-03 17:17:54.000000 django-htmx-live-trigger-0.2/pyproject.toml
--rw-r--r--   0 paulik123   (502) staff       (20)     1034 2024-04-11 16:27:06.521133 django-htmx-live-trigger-0.2/setup.cfg
--rw-r--r--   0 paulik123   (502) staff       (20)       37 2024-04-03 17:25:11.000000 django-htmx-live-trigger-0.2/setup.py
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 19:31:30.072092 django-htmx-live-trigger-0.3/
+-rw-r--r--   0 paulik123   (502) staff       (20)     1093 2024-04-03 17:16:36.000000 django-htmx-live-trigger-0.3/LICENSE
+-rw-r--r--   0 paulik123   (502) staff       (20)      225 2024-04-11 14:51:26.000000 django-htmx-live-trigger-0.3/MANIFEST.in
+-rw-r--r--   0 paulik123   (502) staff       (20)     1126 2024-04-11 19:31:30.071770 django-htmx-live-trigger-0.3/PKG-INFO
+-rw-r--r--   0 paulik123   (502) staff       (20)     2366 2024-04-11 19:30:01.000000 django-htmx-live-trigger-0.3/README.md
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 19:31:30.060911 django-htmx-live-trigger-0.3/django_htmx_live_trigger/
+-rw-r--r--   0 paulik123   (502) staff       (20)      318 2024-04-11 15:36:27.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger/__init__.py
+-rw-r--r--   0 paulik123   (502) staff       (20)       63 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger/admin.py
+-rw-r--r--   0 paulik123   (502) staff       (20)      202 2024-04-11 14:58:42.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger/apps.py
+-rw-r--r--   0 paulik123   (502) staff       (20)      513 2024-04-11 14:41:29.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger/consumers.py
+-rw-r--r--   0 paulik123   (502) staff       (20)       57 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger/models.py
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 19:31:30.036747 django-htmx-live-trigger-0.3/django_htmx_live_trigger/static/
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 19:31:30.037126 django-htmx-live-trigger-0.3/django_htmx_live_trigger/static/django_htmx_live_trigger/
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 19:31:30.069448 django-htmx-live-trigger-0.3/django_htmx_live_trigger/static/django_htmx_live_trigger/js/
+-rw-r--r--   0 paulik123   (502) staff       (20)     9425 2024-04-09 18:32:30.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger/static/django_htmx_live_trigger/js/htmx-ws-events.js
+-rw-r--r--   0 paulik123   (502) staff       (20)       60 2024-04-03 16:51:57.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger/tests.py
+drwxr-xr-x   0 paulik123   (502) staff       (20)        0 2024-04-11 19:31:30.070699 django-htmx-live-trigger-0.3/django_htmx_live_trigger.egg-info/
+-rw-r--r--   0 paulik123   (502) staff       (20)     1126 2024-04-11 19:31:30.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger.egg-info/PKG-INFO
+-rw-r--r--   0 paulik123   (502) staff       (20)      591 2024-04-11 19:31:30.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger.egg-info/SOURCES.txt
+-rw-r--r--   0 paulik123   (502) staff       (20)        1 2024-04-11 19:31:30.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger.egg-info/dependency_links.txt
+-rw-r--r--   0 paulik123   (502) staff       (20)       78 2024-04-11 19:31:30.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger.egg-info/requires.txt
+-rw-r--r--   0 paulik123   (502) staff       (20)       25 2024-04-11 19:31:30.000000 django-htmx-live-trigger-0.3/django_htmx_live_trigger.egg-info/top_level.txt
+-rw-r--r--   0 paulik123   (502) staff       (20)       88 2024-04-03 17:17:54.000000 django-htmx-live-trigger-0.3/pyproject.toml
+-rw-r--r--   0 paulik123   (502) staff       (20)     1034 2024-04-11 19:31:30.073555 django-htmx-live-trigger-0.3/setup.cfg
+-rw-r--r--   0 paulik123   (502) staff       (20)       37 2024-04-03 17:25:11.000000 django-htmx-live-trigger-0.3/setup.py
```

### Comparing `django-htmx-live-trigger-0.2/LICENSE` & `django-htmx-live-trigger-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-live-trigger-0.2/PKG-INFO` & `django-htmx-live-trigger-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-live-trigger
-Version: 0.2
+Version: 0.3
 Summary: Realtime updates in Django using HTMX and websockets.
 Home-page: https://github.com/paulik123
 Author: Cornel Kenef
 Author-email: paul@2na.dev
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-htmx-live-trigger-0.2/django_htmx_live_trigger/consumers.py` & `django-htmx-live-trigger-0.3/django_htmx_live_trigger/consumers.py`

 * *Files identical despite different names*

### Comparing `django-htmx-live-trigger-0.2/django_htmx_live_trigger/static/django_htmx_live_trigger/js/htmx-ws-events.js` & `django-htmx-live-trigger-0.3/django_htmx_live_trigger/static/django_htmx_live_trigger/js/htmx-ws-events.js`

 * *Files identical despite different names*

### Comparing `django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/PKG-INFO` & `django-htmx-live-trigger-0.3/django_htmx_live_trigger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-live-trigger
-Version: 0.2
+Version: 0.3
 Summary: Realtime updates in Django using HTMX and websockets.
 Home-page: https://github.com/paulik123
 Author: Cornel Kenef
 Author-email: paul@2na.dev
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `django-htmx-live-trigger-0.2/django_htmx_live_trigger.egg-info/SOURCES.txt` & `django-htmx-live-trigger-0.3/django_htmx_live_trigger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-htmx-live-trigger-0.2/setup.cfg` & `django-htmx-live-trigger-0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-htmx-live-trigger
-version = 0.2
+version = 0.3
 description = Realtime updates in Django using HTMX and websockets.
 long_description = file: README.rst
 url = https://github.com/paulik123
 author = Cornel Kenef
 author_email = paul@2na.dev
 license = MIT
 classifiers =
```

