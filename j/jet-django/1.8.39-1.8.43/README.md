# Comparing `tmp/jet-django-1.8.39.tar.gz` & `tmp/jet-django-1.8.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jet-django-1.8.39.tar", last modified: Fri Feb  2 12:57:12 2024, max compression
+gzip compressed data, was "dist/jet-django-1.8.43.tar", last modified: Thu Apr 11 10:54:30 2024, max compression
```

## Comparing `jet-django-1.8.39.tar` & `jet-django-1.8.43.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-02-02 12:57:12.000000 jet-django-1.8.39/
--rw-r--r--   0 f1nal      (501) staff       (20)     3927 2024-02-02 12:57:12.000000 jet-django-1.8.39/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-django-1.8.39/LICENSE
--rw-r--r--   0 f1nal      (501) staff       (20)       66 2021-08-25 15:07:30.000000 jet-django-1.8.39/MANIFEST.in
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-02-02 12:57:12.000000 jet-django-1.8.39/jet_django.egg-info/
--rw-r--r--   0 f1nal      (501) staff       (20)     3927 2024-02-02 12:57:11.000000 jet-django-1.8.39/jet_django.egg-info/PKG-INFO
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:49:12.000000 jet-django-1.8.39/jet_django.egg-info/not-zip-safe
--rw-r--r--   0 f1nal      (501) staff       (20)     1266 2024-02-02 12:57:12.000000 jet-django-1.8.39/jet_django.egg-info/SOURCES.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       40 2024-02-02 12:57:11.000000 jet-django-1.8.39/jet_django.egg-info/requires.txt
--rw-r--r--   0 f1nal      (501) staff       (20)       11 2024-02-02 12:57:11.000000 jet-django-1.8.39/jet_django.egg-info/top_level.txt
--rw-r--r--   0 f1nal      (501) staff       (20)        1 2024-02-02 12:57:11.000000 jet-django-1.8.39/jet_django.egg-info/dependency_links.txt
--rw-r--r--   0 f1nal      (501) staff       (20)      974 2024-02-02 01:48:04.000000 jet-django-1.8.39/setup.py
--rw-r--r--   0 f1nal      (501) staff       (20)       38 2024-02-02 12:57:12.000000 jet-django-1.8.39/setup.cfg
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-02-02 12:57:12.000000 jet-django-1.8.39/jet_django/
--rw-r--r--   0 f1nal      (501) staff       (20)    14312 2023-12-30 00:53:53.000000 jet-django-1.8.39/jet_django/configuration.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-02-02 12:57:12.000000 jet-django-1.8.39/jet_django/migrations/
--rw-r--r--   0 f1nal      (501) staff       (20)      761 2022-11-13 04:35:29.000000 jet-django-1.8.39/jet_django/migrations/0002_auto_20181014_2002.py
--rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:35:29.000000 jet-django-1.8.39/jet_django/migrations/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-02-02 12:57:12.000000 jet-django-1.8.39/jet_django/migrations/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     2320 2023-12-30 00:50:00.000000 jet-django-1.8.39/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      771 2023-12-30 00:50:00.000000 jet-django-1.8.39/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1414 2023-12-30 00:50:00.000000 jet-django-1.8.39/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      189 2023-12-30 00:50:00.000000 jet-django-1.8.39/jet_django/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1218 2022-11-13 04:35:29.000000 jet-django-1.8.39/jet_django/migrations/0003_auto_20191007_2005.py
--rw-r--r--   0 f1nal      (501) staff       (20)     5152 2022-11-13 04:35:29.000000 jet-django-1.8.39/jet_django/migrations/0001_initial.py
--rw-r--r--   0 f1nal      (501) staff       (20)       74 2024-02-02 01:48:04.000000 jet-django-1.8.39/jet_django/__init__.py
-drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-02-02 12:57:12.000000 jet-django-1.8.39/jet_django/__pycache__/
--rw-r--r--   0 f1nal      (501) staff       (20)     5789 2023-12-30 00:48:51.000000 jet-django-1.8.39/jet_django/__pycache__/route_view.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     2934 2023-12-30 00:49:52.000000 jet-django-1.8.39/jet_django/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3880 2023-12-30 00:48:49.000000 jet-django-1.8.39/jet_django/__pycache__/urls.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)    14525 2023-12-30 00:48:49.000000 jet-django-1.8.39/jet_django/__pycache__/configuration.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      245 2024-02-02 12:57:11.000000 jet-django-1.8.39/jet_django/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     3311 2023-12-30 00:48:51.000000 jet-django-1.8.39/jet_django/__pycache__/router.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)     1062 2023-12-30 00:48:49.000000 jet-django-1.8.39/jet_django/__pycache__/apps.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      249 2023-08-25 16:50:37.000000 jet-django-1.8.39/jet_django/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      255 2023-12-30 00:48:44.000000 jet-django-1.8.39/jet_django/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 f1nal      (501) staff       (20)      708 2022-11-13 04:35:29.000000 jet-django-1.8.39/jet_django/apps.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4278 2023-12-30 00:53:53.000000 jet-django-1.8.39/jet_django/settings.py
--rw-r--r--   0 f1nal      (501) staff       (20)     4989 2024-01-17 02:57:41.000000 jet-django-1.8.39/jet_django/route_view.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3490 2024-01-17 03:05:40.000000 jet-django-1.8.39/jet_django/router.py
--rw-r--r--   0 f1nal      (501) staff       (20)     5107 2023-09-27 06:21:52.000000 jet-django-1.8.39/jet_django/urls.py
--rw-r--r--   0 f1nal      (501) staff       (20)     3690 2023-04-21 03:52:47.000000 jet-django-1.8.39/README.rst
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-04-11 10:54:30.000000 jet-django-1.8.43/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3927 2024-04-11 10:54:30.000000 jet-django-1.8.43/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2021-08-25 15:07:30.000000 jet-django-1.8.43/LICENSE
+-rw-r--r--   0 f1nal      (501) staff       (20)       66 2021-08-25 15:07:30.000000 jet-django-1.8.43/MANIFEST.in
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django.egg-info/
+-rw-r--r--   0 f1nal      (501) staff       (20)     3927 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django.egg-info/PKG-INFO
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2021-08-26 13:49:12.000000 jet-django-1.8.43/jet_django.egg-info/not-zip-safe
+-rw-r--r--   0 f1nal      (501) staff       (20)     1266 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django.egg-info/SOURCES.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       40 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django.egg-info/requires.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)       11 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django.egg-info/top_level.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)        1 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django.egg-info/dependency_links.txt
+-rw-r--r--   0 f1nal      (501) staff       (20)      974 2024-04-05 19:22:50.000000 jet-django-1.8.43/setup.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       38 2024-04-11 10:54:30.000000 jet-django-1.8.43/setup.cfg
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django/
+-rw-r--r--   0 f1nal      (501) staff       (20)    14373 2024-03-15 19:09:12.000000 jet-django-1.8.43/jet_django/configuration.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django/migrations/
+-rw-r--r--   0 f1nal      (501) staff       (20)      761 2022-11-13 04:35:29.000000 jet-django-1.8.43/jet_django/migrations/0002_auto_20181014_2002.py
+-rw-r--r--   0 f1nal      (501) staff       (20)        0 2022-11-13 04:35:29.000000 jet-django-1.8.43/jet_django/migrations/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django/migrations/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     2320 2023-12-30 00:50:00.000000 jet-django-1.8.43/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      771 2023-12-30 00:50:00.000000 jet-django-1.8.43/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1414 2023-12-30 00:50:00.000000 jet-django-1.8.43/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      189 2023-12-30 00:50:00.000000 jet-django-1.8.43/jet_django/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1218 2022-11-13 04:35:29.000000 jet-django-1.8.43/jet_django/migrations/0003_auto_20191007_2005.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     5152 2022-11-13 04:35:29.000000 jet-django-1.8.43/jet_django/migrations/0001_initial.py
+-rw-r--r--   0 f1nal      (501) staff       (20)       74 2024-04-05 19:22:50.000000 jet-django-1.8.43/jet_django/__init__.py
+drwxr-xr-x   0 f1nal      (501) staff       (20)        0 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django/__pycache__/
+-rw-r--r--   0 f1nal      (501) staff       (20)     5789 2023-12-30 00:48:51.000000 jet-django-1.8.43/jet_django/__pycache__/route_view.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     2934 2023-12-30 00:49:52.000000 jet-django-1.8.43/jet_django/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3880 2023-12-30 00:48:49.000000 jet-django-1.8.43/jet_django/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)    14525 2023-12-30 00:48:49.000000 jet-django-1.8.43/jet_django/__pycache__/configuration.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      245 2024-04-11 10:54:30.000000 jet-django-1.8.43/jet_django/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     3311 2023-12-30 00:48:51.000000 jet-django-1.8.43/jet_django/__pycache__/router.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)     1062 2023-12-30 00:48:49.000000 jet-django-1.8.43/jet_django/__pycache__/apps.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      249 2023-08-25 16:50:37.000000 jet-django-1.8.43/jet_django/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      255 2023-12-30 00:48:44.000000 jet-django-1.8.43/jet_django/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 f1nal      (501) staff       (20)      708 2022-11-13 04:35:29.000000 jet-django-1.8.43/jet_django/apps.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4347 2024-03-15 19:09:12.000000 jet-django-1.8.43/jet_django/settings.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     4989 2024-01-17 02:57:41.000000 jet-django-1.8.43/jet_django/route_view.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3490 2024-01-17 03:05:40.000000 jet-django-1.8.43/jet_django/router.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     5107 2023-09-27 06:21:52.000000 jet-django-1.8.43/jet_django/urls.py
+-rw-r--r--   0 f1nal      (501) staff       (20)     3690 2023-04-21 03:52:47.000000 jet-django-1.8.43/README.rst
```

### Comparing `jet-django-1.8.39/PKG-INFO` & `jet-django-1.8.43/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-django
-Version: 1.8.39
+Version: 1.8.43
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-django
 Author: Denis Kildishev
 Author-email: hello@geex-arts.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `jet-django-1.8.39/jet_django.egg-info/PKG-INFO` & `jet-django-1.8.43/jet_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jet-django
-Version: 1.8.39
+Version: 1.8.43
 Summary: UNKNOWN
 Home-page: https://github.com/jet-admin/jet-django
 Author: Denis Kildishev
 Author-email: hello@geex-arts.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `jet-django-1.8.39/jet_django.egg-info/SOURCES.txt` & `jet-django-1.8.43/jet_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/setup.py` & `jet-django-1.8.43/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     return file.read()
 
 
 def get_install_requires():
     install_requires = [
         'Django',
         'requests',
-        'jet-bridge-base==1.8.39',
+        'jet-bridge-base==1.8.43',
     ]
 
     try:
         from collections import OrderedDict
     except ImportError:
         install_requires.append('ordereddict')
```

### Comparing `jet-django-1.8.39/jet_django/configuration.py` & `jet-django-1.8.43/jet_django/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             'TOKEN': settings.JET_TOKEN,
             'ENVIRONMENT': settings.JET_ENVIRONMENT,
             'CORS_HEADERS': settings.JET_CORS_HEADERS,
             'BASE_URL': settings.JET_BASE_URL,
             'JWT_VERIFY_KEY': settings.JET_JWT_VERIFY_KEY,
             'BEARER_AUTH_KEY': settings.JET_BEARER_AUTH_KEY,
             'ENVIRONMENT_TYPE': settings.JET_ENVIRONMENT_TYPE,
+            'BLACKLIST_HOSTS': settings.JET_BLACKLIST_HOSTS,
             'DATABASE_ENGINE': settings.database_engine,
             'DATABASE_HOST': settings.database_settings.get('HOST'),
             'DATABASE_PORT': settings.database_settings.get('PORT'),
             'DATABASE_USER': settings.database_settings.get('USER'),
             'DATABASE_PASSWORD': settings.database_settings.get('PASSWORD'),
             'DATABASE_NAME': str(settings.database_settings['NAME'])
                 if settings.database_settings.get('NAME') is not None else None,
```

### Comparing `jet-django-1.8.39/jet_django/migrations/0002_auto_20181014_2002.py` & `jet-django-1.8.43/jet_django/migrations/0002_auto_20181014_2002.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc` & `jet-django-1.8.43/jet_django/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc` & `jet-django-1.8.43/jet_django/migrations/__pycache__/0002_auto_20181014_2002.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc` & `jet-django-1.8.43/jet_django/migrations/__pycache__/0003_auto_20191007_2005.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/migrations/0003_auto_20191007_2005.py` & `jet-django-1.8.43/jet_django/migrations/0003_auto_20191007_2005.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/migrations/0001_initial.py` & `jet-django-1.8.43/jet_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/__pycache__/route_view.cpython-310.pyc` & `jet-django-1.8.43/jet_django/__pycache__/route_view.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/__pycache__/settings.cpython-310.pyc` & `jet-django-1.8.43/jet_django/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/__pycache__/urls.cpython-310.pyc` & `jet-django-1.8.43/jet_django/__pycache__/urls.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/__pycache__/configuration.cpython-310.pyc` & `jet-django-1.8.43/jet_django/__pycache__/configuration.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/__pycache__/router.cpython-310.pyc` & `jet-django-1.8.43/jet_django/__pycache__/router.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/__pycache__/apps.cpython-310.pyc` & `jet-django-1.8.43/jet_django/__pycache__/apps.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/apps.py` & `jet-django-1.8.43/jet_django/apps.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/settings.py` & `jet-django-1.8.43/jet_django/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 JET_TOKEN = getattr(settings, 'JET_TOKEN', None)
 JET_ENVIRONMENT = getattr(settings, 'JET_ENVIRONMENT', None)
 JET_CORS_HEADERS = getattr(settings, 'JET_CORS_HEADERS', 'corsheaders' not in settings.INSTALLED_APPS)
 JET_BASE_URL = getattr(settings, 'JET_BASE_URL', None)
 JET_JWT_VERIFY_KEY = getattr(settings, 'JET_JWT_VERIFY_KEY', None)
 JET_BEARER_AUTH_KEY = getattr(settings, 'JET_BEARER_AUTH_KEY', None)
 JET_ENVIRONMENT_TYPE = getattr(settings, 'JET_ENVIRONMENT_TYPE', 'django')
+JET_BLACKLIST_HOSTS = getattr(settings, 'JET_BLACKLIST_HOSTS', None)
 
 JET_BACKEND_API_BASE_URL = getattr(settings, 'JET_BACKEND_API_BASE_URL', 'https://api.jetadmin.io/api')
 JET_BACKEND_WEB_BASE_URL = getattr(settings, 'JET_BACKEND_WEB_BASE_URL', 'https://app.jetadmin.io')
 
 JET_MEDIA_FILE_STORAGE = getattr(settings, 'JET_MEDIA_FILE_STORAGE', settings.DEFAULT_FILE_STORAGE)
 
 JET_DJANGO_DATABASE = getattr(settings, 'JET_DJANGO_DATABASE', 'default')
```

### Comparing `jet-django-1.8.39/jet_django/route_view.py` & `jet-django-1.8.43/jet_django/route_view.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/router.py` & `jet-django-1.8.43/jet_django/router.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/jet_django/urls.py` & `jet-django-1.8.43/jet_django/urls.py`

 * *Files identical despite different names*

### Comparing `jet-django-1.8.39/README.rst` & `jet-django-1.8.43/README.rst`

 * *Files identical despite different names*

