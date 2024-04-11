# Comparing `tmp/mercadolibre-sdk-0.0.8.tar.gz` & `tmp/mercadolibre-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercadolibre-sdk-0.0.8.tar", last modified: Sat Feb  3 15:48:59 2024, max compression
+gzip compressed data, was "mercadolibre-sdk-0.0.9.tar", last modified: Sat Feb  3 15:54:04 2024, max compression
```

## Comparing `mercadolibre-sdk-0.0.8.tar` & `mercadolibre-sdk-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2024-02-03 15:48:59.832259 mercadolibre-sdk-0.0.8/
--rw-rw-r--   0 sandro    (1000) sandro    (1000)     2953 2024-02-03 15:48:59.828258 mercadolibre-sdk-0.0.8/PKG-INFO
--rw-rw-r--   0 sandro    (1000) sandro    (1000)     2732 2024-02-02 22:56:49.000000 mercadolibre-sdk-0.0.8/README.md
-drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2024-02-03 15:48:59.828258 mercadolibre-sdk-0.0.8/mercadolibre/
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      249 2024-02-02 22:51:15.000000 mercadolibre-sdk-0.0.8/mercadolibre/__init__.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)     4968 2024-02-03 15:48:49.000000 mercadolibre-sdk-0.0.8/mercadolibre/_authentication.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)     2058 2024-02-03 15:35:57.000000 mercadolibre-sdk-0.0.8/mercadolibre/api.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      182 2024-02-03 15:48:49.000000 mercadolibre-sdk-0.0.8/mercadolibre/authentication.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)     3141 2024-02-03 00:03:35.000000 mercadolibre-sdk-0.0.8/mercadolibre/authorization.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      310 2024-02-03 15:40:50.000000 mercadolibre-sdk-0.0.8/mercadolibre/category.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      195 2023-10-02 00:22:52.000000 mercadolibre-sdk-0.0.8/mercadolibre/item.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      426 2023-10-05 01:05:35.000000 mercadolibre-sdk-0.0.8/mercadolibre/product.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      200 2023-10-02 00:54:28.000000 mercadolibre-sdk-0.0.8/mercadolibre/review.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)     1120 2024-02-03 15:35:57.000000 mercadolibre-sdk-0.0.8/mercadolibre/search.py
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      195 2023-10-02 00:36:30.000000 mercadolibre-sdk-0.0.8/mercadolibre/user.py
-drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2024-02-03 15:48:59.828258 mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/
--rw-rw-r--   0 sandro    (1000) sandro    (1000)     2953 2024-02-03 15:48:59.000000 mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      535 2024-02-03 15:48:59.000000 mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 sandro    (1000) sandro    (1000)        1 2024-02-03 15:48:59.000000 mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 sandro    (1000) sandro    (1000)       80 2024-02-03 15:48:59.000000 mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 sandro    (1000) sandro    (1000)       64 2024-02-03 15:48:59.000000 mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/requires.txt
--rw-rw-r--   0 sandro    (1000) sandro    (1000)       13 2024-02-03 15:48:59.000000 mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/top_level.txt
--rw-rw-r--   0 sandro    (1000) sandro    (1000)       38 2024-02-03 15:48:59.832259 mercadolibre-sdk-0.0.8/setup.cfg
--rw-rw-r--   0 sandro    (1000) sandro    (1000)      622 2024-02-03 15:48:58.000000 mercadolibre-sdk-0.0.8/setup.py
+drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2024-02-03 15:54:04.665514 mercadolibre-sdk-0.0.9/
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     2953 2024-02-03 15:54:04.665514 mercadolibre-sdk-0.0.9/PKG-INFO
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     2732 2024-02-02 22:56:49.000000 mercadolibre-sdk-0.0.9/README.md
+drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2024-02-03 15:54:04.665514 mercadolibre-sdk-0.0.9/mercadolibre/
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      249 2024-02-02 22:51:15.000000 mercadolibre-sdk-0.0.9/mercadolibre/__init__.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     4968 2024-02-03 15:48:49.000000 mercadolibre-sdk-0.0.9/mercadolibre/_authentication.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     2050 2024-02-03 15:54:03.000000 mercadolibre-sdk-0.0.9/mercadolibre/api.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      182 2024-02-03 15:48:49.000000 mercadolibre-sdk-0.0.9/mercadolibre/authentication.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     3141 2024-02-03 00:03:35.000000 mercadolibre-sdk-0.0.9/mercadolibre/authorization.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      267 2024-02-03 15:54:03.000000 mercadolibre-sdk-0.0.9/mercadolibre/category.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      195 2023-10-02 00:22:52.000000 mercadolibre-sdk-0.0.9/mercadolibre/item.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      426 2023-10-05 01:05:35.000000 mercadolibre-sdk-0.0.9/mercadolibre/product.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      200 2023-10-02 00:54:28.000000 mercadolibre-sdk-0.0.9/mercadolibre/review.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     1120 2024-02-03 15:35:57.000000 mercadolibre-sdk-0.0.9/mercadolibre/search.py
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      195 2023-10-02 00:36:30.000000 mercadolibre-sdk-0.0.9/mercadolibre/user.py
+drwxrwxr-x   0 sandro    (1000) sandro    (1000)        0 2024-02-03 15:54:04.665514 mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)     2953 2024-02-03 15:54:04.000000 mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      535 2024-02-03 15:54:04.000000 mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)        1 2024-02-03 15:54:04.000000 mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)       80 2024-02-03 15:54:04.000000 mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)       64 2024-02-03 15:54:04.000000 mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/requires.txt
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)       13 2024-02-03 15:54:04.000000 mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)       38 2024-02-03 15:54:04.665514 mercadolibre-sdk-0.0.9/setup.cfg
+-rw-rw-r--   0 sandro    (1000) sandro    (1000)      622 2024-02-03 15:54:03.000000 mercadolibre-sdk-0.0.9/setup.py
```

### Comparing `mercadolibre-sdk-0.0.8/PKG-INFO` & `mercadolibre-sdk-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercadolibre-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Description of your package
 Home-page: https://github.com/mercadoradar/mercadolibre-sdk
 Author: Mercado Radar
 Description-Content-Type: text/markdown
 
 # Mercado Libre - SDK (unofficial)
```

### Comparing `mercadolibre-sdk-0.0.8/README.md` & `mercadolibre-sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mercadolibre-sdk-0.0.8/mercadolibre/_authentication.py` & `mercadolibre-sdk-0.0.9/mercadolibre/_authentication.py`

 * *Files identical despite different names*

### Comparing `mercadolibre-sdk-0.0.8/mercadolibre/api.py` & `mercadolibre-sdk-0.0.9/mercadolibre/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from mercadolibre import Authentication
 
 
 class MercadoLibreAPI:
     BASE_URL = 'https://api.mercadolibre.com'
 
-    def _make_request(self, method: str,
-                      path: str,
-                      params: dict = None,
-                      data: dict = None) -> list | dict | bytes:
+    def make_request(self, method: str,
+                     path: str,
+                     params: dict = None,
+                     data: dict = None) -> list | dict | bytes:
         access_token = Authentication().get_access_token()
         headers = {
             'Authorization': f'Bearer {access_token}',
             'Content-Type': 'application/json',
         }
         url = f'{self.BASE_URL}{path}'
         response = request(method, url, headers=headers, params=params, data=data)
@@ -23,32 +23,32 @@
 
         if response.headers.get('Content-Type') == 'text/csv':
             return response.content
 
         return response.json()
 
     def create_request(self, path: str, data: list | dict) -> dict:
-        return self._make_request(method='POST', path=path, data=data)
+        return self.make_request(method='POST', path=path, data=data)
 
     def list_request(self, path: str, limit: int = 50, offset: int = 0, params: dict = None) -> list | dict:
         params = self._set_pagination(limit, offset, params)
-        return self._make_request(method='GET', path=path, params=params)
+        return self.make_request(method='GET', path=path, params=params)
 
     @staticmethod
     def _set_pagination(limit, offset, params):
         if not params:
             params = dict()
         if limit:
             params['limit'] = limit
         if offset:
             params['offset'] = offset
         return params
 
     def retrieve_request(self, path: str, id: str, params=None):
         path = f'{path}/{id}/'
-        return self._make_request(method='GET', path=path, params=params)
+        return self.make_request(method='GET', path=path, params=params)
 
     def action_request(self, path: str, action: str, id: str, limit: int = 50, offset: int = 0,
                        params: dict = None) -> list | dict:
         path = f'{path}/{id}/{action}'
         params = self._set_pagination(limit, offset, params)
-        return self._make_request(method='GET', path=path, params=params)
+        return self.make_request(method='GET', path=path, params=params)
```

### Comparing `mercadolibre-sdk-0.0.8/mercadolibre/authorization.py` & `mercadolibre-sdk-0.0.9/mercadolibre/authorization.py`

 * *Files identical despite different names*

### Comparing `mercadolibre-sdk-0.0.8/mercadolibre/search.py` & `mercadolibre-sdk-0.0.9/mercadolibre/search.py`

 * *Files identical despite different names*

### Comparing `mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/PKG-INFO` & `mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercadolibre-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Description of your package
 Home-page: https://github.com/mercadoradar/mercadolibre-sdk
 Author: Mercado Radar
 Description-Content-Type: text/markdown
 
 # Mercado Libre - SDK (unofficial)
```

### Comparing `mercadolibre-sdk-0.0.8/mercadolibre_sdk.egg-info/SOURCES.txt` & `mercadolibre-sdk-0.0.9/mercadolibre_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercadolibre-sdk-0.0.8/setup.py` & `mercadolibre-sdk-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mercadolibre-sdk',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[
         'requests==2.31.0', 'redis==5.0.1', 'flask==3.0.0', 'python-dotenv==1.0.0'
     ],
     entry_points={
         'console_scripts': [
             'mercadolibre.authorize = mercadolibre.authorization:authorize',
```

