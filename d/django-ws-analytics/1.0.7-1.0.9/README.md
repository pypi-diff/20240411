# Comparing `tmp/django-ws-analytics-1.0.7.tar.gz` & `tmp/django-ws-analytics-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ws-analytics-1.0.7.tar", last modified: Tue Feb 27 09:43:33 2024, max compression
+gzip compressed data, was "django-ws-analytics-1.0.9.tar", last modified: Mon Mar 11 13:48:24 2024, max compression
```

## Comparing `django-ws-analytics-1.0.7.tar` & `django-ws-analytics-1.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:33.062492 django-ws-analytics-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-02-27 09:43:33.062492 django-ws-analytics-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:33.058493 django-ws-analytics-1.0.7/django_ws_analytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-02-27 09:43:32.000000 django-ws-analytics-1.0.7/django_ws_analytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-27 09:43:33.000000 django-ws-analytics-1.0.7/django_ws_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 09:43:32.000000 django-ws-analytics-1.0.7/django_ws_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-27 09:43:32.000000 django-ws-analytics-1.0.7/django_ws_analytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-27 09:43:32.000000 django-ws-analytics-1.0.7/django_ws_analytics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:33.050492 django-ws-analytics-1.0.7/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/example/asgi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      730 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/example/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/example/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/example/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/example/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-27 09:43:33.062492 django-ws-analytics-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:33.054492 django-ws-analytics-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/tests/asgi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/tests/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:33.058493 django-ws-analytics-1.0.7/ws_analytics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:33.058493 django-ws-analytics-1.0.7/ws_analytics/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 09:43:20.000000 django-ws-analytics-1.0.7/ws_analytics/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:24.282254 django-ws-analytics-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-11 13:48:24.282254 django-ws-analytics-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:24.282254 django-ws-analytics-1.0.9/django_ws_analytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-11 13:48:24.000000 django-ws-analytics-1.0.9/django_ws_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-11 13:48:24.000000 django-ws-analytics-1.0.9/django_ws_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 13:48:24.000000 django-ws-analytics-1.0.9/django_ws_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-11 13:48:24.000000 django-ws-analytics-1.0.9/django_ws_analytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-11 13:48:24.000000 django-ws-analytics-1.0.9/django_ws_analytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:24.278254 django-ws-analytics-1.0.9/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/example/asgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      730 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/example/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/example/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/example/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/example/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-11 13:48:24.282254 django-ws-analytics-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:24.278254 django-ws-analytics-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/tests/asgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:24.282254 django-ws-analytics-1.0.9/ws_analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:24.282254 django-ws-analytics-1.0.9/ws_analytics/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 13:48:15.000000 django-ws-analytics-1.0.9/ws_analytics/views.py
```

### Comparing `django-ws-analytics-1.0.7/LICENSE` & `django-ws-analytics-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/PKG-INFO` & `django-ws-analytics-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ws-analytics
-Version: 1.0.7
+Version: 1.0.9
 Summary: Django WS Analytics Package
 Home-page: https://github.com/windschatten-it/django-ws-analytics
 Author: windschatten.it
 Author-email: fabian@windschatten.it
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `django-ws-analytics-1.0.7/README.rst` & `django-ws-analytics-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/django_ws_analytics.egg-info/PKG-INFO` & `django-ws-analytics-1.0.9/django_ws_analytics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ws-analytics
-Version: 1.0.7
+Version: 1.0.9
 Summary: Django WS Analytics Package
 Home-page: https://github.com/windschatten-it/django-ws-analytics
 Author: windschatten.it
 Author-email: fabian@windschatten.it
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `django-ws-analytics-1.0.7/django_ws_analytics.egg-info/SOURCES.txt` & `django-ws-analytics-1.0.9/django_ws_analytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/example/manage.py` & `django-ws-analytics-1.0.9/example/manage.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/example/settings.py` & `django-ws-analytics-1.0.9/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/example/urls.py` & `django-ws-analytics-1.0.9/example/urls.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/tests/manage.py` & `django-ws-analytics-1.0.9/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/tests/settings.py` & `django-ws-analytics-1.0.9/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/tests/urls.py` & `django-ws-analytics-1.0.9/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/ws_analytics/admin.py` & `django-ws-analytics-1.0.9/ws_analytics/admin.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/ws_analytics/apps.py` & `django-ws-analytics-1.0.9/ws_analytics/apps.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/ws_analytics/middleware.py` & `django-ws-analytics-1.0.9/ws_analytics/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import time
 import uuid
 from importlib import import_module
 
 from django.conf import settings
 from django.contrib.sessions.backends.base import UpdateError
 from django.contrib.sessions.exceptions import SessionInterrupted
@@ -10,18 +11,20 @@
 from django.utils import timezone
 from django.utils.cache import patch_vary_headers
 from django.utils.functional import SimpleLazyObject
 from django.utils.http import http_date
 from django_q.tasks import async_task
 from django_user_agents.utils import get_user_agent
 
-from ws_analytics.models import AnalyticsRequest, AnalyticsDevice
-from ws_analytics.services import get_device_data, get_city_for_geoip, create_analytics_request
+from ws_analytics.models import AnalyticsDevice
+from ws_analytics.services import get_device_data, create_analytics_request
 from ws_analytics.settings import get_config
 
+logger = logging.getLogger('ws_analytics')
+
 
 class AnalyticsMiddleware(SessionMiddleware):
     def __init__(self, get_response):
         super().__init__(get_response)
         self.loggable_view_names = get_config()['LOGGABLE_VIEW_NAMES']
         self.DEVICE_COOKIE_NAME = get_config()['DEVICE_COOKIE_NAME']
 
@@ -61,67 +64,72 @@
 
             if not request.session.session_key:
                 request.session['_device_key'] = request.device.session_key
                 request.session.modified = True
                 request.session.save()
 
     def process_request(self, request):
-        request.user_agent = SimpleLazyObject(lambda: get_user_agent(request))
-        self.process_request_device(request)
-        self.process_request_analytics(request)
+        try:
+            if request.resolver_match.view_name in self.loggable_view_names:
+                request.user_agent = SimpleLazyObject(lambda: get_user_agent(request))
+                self.process_request_device(request)
+                self.process_request_analytics(request)
+        except Exception as e:
+            logger.warning(str(e))
 
     def process_response_device(self, request, response):
 
         try:
             accessed = request.device.accessed
             modified = request.device.modified
             empty = request.device.is_empty()
-        except AttributeError:
-            return response
 
-        if self.DEVICE_COOKIE_NAME in request.COOKIES and empty:
-            response.delete_cookie(
-                self.DEVICE_COOKIE_NAME,
-                path=settings.SESSION_COOKIE_PATH,
-                domain=settings.SESSION_COOKIE_DOMAIN,
-                samesite=settings.SESSION_COOKIE_SAMESITE,
-            )
-            patch_vary_headers(response, ("Cookie",))
-        else:
-            if accessed:
+            if self.DEVICE_COOKIE_NAME in request.COOKIES and empty:
+                response.delete_cookie(
+                    self.DEVICE_COOKIE_NAME,
+                    path=settings.SESSION_COOKIE_PATH,
+                    domain=settings.SESSION_COOKIE_DOMAIN,
+                    samesite=settings.SESSION_COOKIE_SAMESITE,
+                )
                 patch_vary_headers(response, ("Cookie",))
-            if (modified or settings.SESSION_SAVE_EVERY_REQUEST) and not empty:
-                max_age = request.device.get_expiry_age()
-                expires_time = time.time() + max_age
-                expires = http_date(expires_time)
-                # Save the device data and refresh the client cookie.
-                # Skip device save for 5xx responses.
-                if response.status_code < 500:
-                    try:
-                        request.device.save()
-                    except UpdateError:
-                        raise SessionInterrupted(
-                            "The request's decive was deleted before the "
-                            "request completed."
+            else:
+                if accessed:
+                    patch_vary_headers(response, ("Cookie",))
+                if (modified or settings.SESSION_SAVE_EVERY_REQUEST) and not empty:
+                    max_age = request.device.get_expiry_age()
+                    expires_time = time.time() + max_age
+                    expires = http_date(expires_time)
+                    # Save the device data and refresh the client cookie.
+                    # Skip device save for 5xx responses.
+                    if response.status_code < 500:
+                        try:
+                            request.device.save()
+                        except UpdateError:
+                            raise SessionInterrupted(
+                                "The request's decive was deleted before the "
+                                "request completed."
+                            )
+                        response.set_cookie(
+                            self.DEVICE_COOKIE_NAME,
+                            request.device.session_key,
+                            max_age=max_age,
+                            expires=expires,
+                            domain=settings.SESSION_COOKIE_DOMAIN,
+                            path=settings.SESSION_COOKIE_PATH,
+                            secure=settings.SESSION_COOKIE_SECURE or None,
+                            httponly=settings.SESSION_COOKIE_HTTPONLY or None,
+                            samesite=settings.SESSION_COOKIE_SAMESITE,
                         )
-                    response.set_cookie(
-                        self.DEVICE_COOKIE_NAME,
-                        request.device.session_key,
-                        max_age=max_age,
-                        expires=expires,
-                        domain=settings.SESSION_COOKIE_DOMAIN,
-                        path=settings.SESSION_COOKIE_PATH,
-                        secure=settings.SESSION_COOKIE_SECURE or None,
-                        httponly=settings.SESSION_COOKIE_HTTPONLY or None,
-                        samesite=settings.SESSION_COOKIE_SAMESITE,
-                    )
+        except Exception as e:
+            logger.debug(str(e))
+
         return response
 
     def process_response_analytics(self, request, response):
-        if request.resolver_match.view_name in self.loggable_view_names:
+        try:
             end_time = time.time()
             execution_time = end_time - self.start_time
 
             client_ip = request.META.get('HTTP_X_FORWARDED_FOR').split(',')[0].strip() if request.META.get(
                 'HTTP_X_FORWARDED_FOR') else request.META.get('REMOTE_ADDR')
 
             analytics_data = {
@@ -132,15 +140,21 @@
                 'query_params': request.GET.dict(),
                 'status_code': response.status_code,
                 'execution_time': execution_time,
                 'client_ip': client_ip,
                 'session_id': request.session.session_key
             }
             async_task(create_analytics_request, **analytics_data)
+        except Exception as e:
+            logger.debug(str(e))
 
         return response
 
     def process_response(self, request, response):
-        response = self.process_response_device(request, response)
-        response = self.process_response_analytics(request, response)
+        try:
+            if request.resolver_match.view_name in self.loggable_view_names:
+                response = self.process_response_device(request, response)
+                response = self.process_response_analytics(request, response)
+        except Exception as e:
+            logger.warning(str(e))
 
         return response
```

### Comparing `django-ws-analytics-1.0.7/ws_analytics/migrations/0001_initial.py` & `django-ws-analytics-1.0.9/ws_analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/ws_analytics/models.py` & `django-ws-analytics-1.0.9/ws_analytics/models.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/ws_analytics/services.py` & `django-ws-analytics-1.0.9/ws_analytics/services.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/ws_analytics/sessions.py` & `django-ws-analytics-1.0.9/ws_analytics/sessions.py`

 * *Files identical despite different names*

### Comparing `django-ws-analytics-1.0.7/ws_analytics/settings.py` & `django-ws-analytics-1.0.9/ws_analytics/settings.py`

 * *Files identical despite different names*

