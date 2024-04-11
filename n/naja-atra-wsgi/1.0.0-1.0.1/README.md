# Comparing `tmp/naja-atra-wsgi-1.0.0.tar.gz` & `tmp/naja-atra-wsgi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naja-atra-wsgi-1.0.0.tar", last modified: Wed Apr 10 01:05:17 2024, max compression
+gzip compressed data, was "naja-atra-wsgi-1.0.1.tar", last modified: Thu Apr 11 03:16:31 2024, max compression
```

## Comparing `naja-atra-wsgi-1.0.0.tar` & `naja-atra-wsgi-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-10 01:05:17.832180 naja-atra-wsgi-1.0.0/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1066 2024-03-08 03:08:45.000000 naja-atra-wsgi-1.0.0/LICENSE
--rw-r--r--   0 keijack   (1000) keijack   (1000)     2964 2024-04-10 01:05:17.832180 naja-atra-wsgi-1.0.0/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1060 2024-04-09 12:19:42.000000 naja-atra-wsgi-1.0.0/README.md
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-10 01:05:17.828178 naja-atra-wsgi-1.0.0/naja_atra_wsgi/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     2428 2024-04-09 12:19:12.000000 naja-atra-wsgi-1.0.0/naja_atra_wsgi/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     7304 2024-03-08 02:31:48.000000 naja-atra-wsgi-1.0.0/naja_atra_wsgi/wsgi_request_handler.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-10 01:05:17.828178 naja-atra-wsgi-1.0.0/naja_atra_wsgi.egg-info/
--rw-r--r--   0 keijack   (1000) keijack   (1000)     2964 2024-04-10 01:05:17.000000 naja-atra-wsgi-1.0.0/naja_atra_wsgi.egg-info/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)      325 2024-04-10 01:05:17.000000 naja-atra-wsgi-1.0.0/naja_atra_wsgi.egg-info/SOURCES.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2024-04-10 01:05:17.000000 naja-atra-wsgi-1.0.0/naja_atra_wsgi.egg-info/dependency_links.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       25 2024-04-10 01:05:17.000000 naja-atra-wsgi-1.0.0/naja_atra_wsgi.egg-info/requires.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       15 2024-04-10 01:05:17.000000 naja-atra-wsgi-1.0.0/naja_atra_wsgi.egg-info/top_level.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)      942 2024-03-11 01:20:30.000000 naja-atra-wsgi-1.0.0/pyproject.toml
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2024-04-10 01:05:17.832180 naja-atra-wsgi-1.0.0/setup.cfg
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       62 2024-03-08 01:49:06.000000 naja-atra-wsgi-1.0.0/setup.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-10 01:05:17.828178 naja-atra-wsgi-1.0.0/tests/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     4141 2024-04-08 06:15:00.000000 naja-atra-wsgi-1.0.0/tests/test_all_ctrls_wsgi.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-11 03:16:31.302317 naja-atra-wsgi-1.0.1/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1066 2024-03-08 03:08:45.000000 naja-atra-wsgi-1.0.1/LICENSE
+-rw-r--r--   0 keijack   (1000) keijack   (1000)     2964 2024-04-11 03:16:31.298315 naja-atra-wsgi-1.0.1/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1060 2024-04-09 12:19:42.000000 naja-atra-wsgi-1.0.1/README.md
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-11 03:16:31.290311 naja-atra-wsgi-1.0.1/naja_atra_wsgi/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     2422 2024-04-11 03:14:21.000000 naja-atra-wsgi-1.0.1/naja_atra_wsgi/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     7304 2024-04-11 03:11:15.000000 naja-atra-wsgi-1.0.1/naja_atra_wsgi/wsgi_request_handler.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-11 03:16:31.298315 naja-atra-wsgi-1.0.1/naja_atra_wsgi.egg-info/
+-rw-r--r--   0 keijack   (1000) keijack   (1000)     2964 2024-04-11 03:16:31.000000 naja-atra-wsgi-1.0.1/naja_atra_wsgi.egg-info/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      325 2024-04-11 03:16:31.000000 naja-atra-wsgi-1.0.1/naja_atra_wsgi.egg-info/SOURCES.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2024-04-11 03:16:31.000000 naja-atra-wsgi-1.0.1/naja_atra_wsgi.egg-info/dependency_links.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       25 2024-04-11 03:16:31.000000 naja-atra-wsgi-1.0.1/naja_atra_wsgi.egg-info/requires.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       15 2024-04-11 03:16:31.000000 naja-atra-wsgi-1.0.1/naja_atra_wsgi.egg-info/top_level.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      942 2024-03-11 01:20:30.000000 naja-atra-wsgi-1.0.1/pyproject.toml
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2024-04-11 03:16:31.302317 naja-atra-wsgi-1.0.1/setup.cfg
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       62 2024-03-08 01:49:06.000000 naja-atra-wsgi-1.0.1/setup.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-11 03:16:31.298315 naja-atra-wsgi-1.0.1/tests/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     4141 2024-04-08 06:15:00.000000 naja-atra-wsgi-1.0.1/tests/test_all_ctrls_wsgi.py
```

### Comparing `naja-atra-wsgi-1.0.0/LICENSE` & `naja-atra-wsgi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naja-atra-wsgi-1.0.0/PKG-INFO` & `naja-atra-wsgi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naja-atra-wsgi
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is a simple http server, use MVC like design.
 Author-email: keijack <keijack.wu@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Keijack Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naja-atra-wsgi-1.0.0/README.md` & `naja-atra-wsgi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `naja-atra-wsgi-1.0.0/naja_atra_wsgi/__init__.py` & `naja-atra-wsgi-1.0.1/naja_atra_wsgi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 
 from typing import Dict
 import asyncio
 
-from naja_atra import SessionFactory, AppConf
+from naja_atra import HttpSessionFactory, AppConf
 from naja_atra import get_app_conf, set_session_factory
-from naja_atra.models.model_bindings import ModelBindingConf
+from naja_atra import ModelBindingConf
 from naja_atra.http_servers.routing_server import RoutingServer
 from naja_atra.request_handlers.http_session_local_impl import LocalSessionFactory
 from .wsgi_request_handler import WSGIRequestHandler
 
 
-version = "1.0.0"
+version = "1.0.1"
 
 
 class WSGIProxy(RoutingServer):
 
     def __init__(self, res_conf, model_binding_conf: ModelBindingConf = ModelBindingConf()):
         super().__init__(res_conf=res_conf, model_binding_conf=model_binding_conf)
 
@@ -23,15 +23,15 @@
         return asyncio.run(self.async_app_proxy(environment, start_response))
 
     async def async_app_proxy(self, environment, start_response):
         request_handler = WSGIRequestHandler(self, environment, start_response)
         return await request_handler.handle_request()
 
 
-def __fill_proxy(proxy: RoutingServer, session_factory: SessionFactory, app_conf: AppConf):
+def __fill_proxy(proxy: RoutingServer, session_factory: HttpSessionFactory, app_conf: AppConf):
     appconf = app_conf or get_app_conf()
     set_session_factory(
         session_factory or appconf.session_factory or LocalSessionFactory())
     filters = appconf._get_filters()
     # filter configuration
     for ft in filters:
         proxy.map_filter(ft)
@@ -47,26 +47,26 @@
         proxy.map_websocket_handler(hander)
 
     err_pages = appconf._get_error_pages()
     for code, func in err_pages.items():
         proxy.map_error_page(code, func)
 
 
-def new_wsgi_proxy(resources: Dict[str, str] = {}, session_factory: SessionFactory = None, app_conf: AppConf = None) -> WSGIProxy:
+def new_wsgi_proxy(resources: Dict[str, str] = {}, session_factory: HttpSessionFactory = None, app_conf: AppConf = None) -> WSGIProxy:
     appconf = app_conf or get_app_conf()
     proxy = WSGIProxy(res_conf=resources,
                       model_binding_conf=appconf.model_binding_conf)
     __fill_proxy(proxy, session_factory, appconf)
     return proxy
 
 
 _proxy: WSGIProxy = None
 
 
-def config(resources: Dict[str, str] = {}, session_factory: SessionFactory = None, app_conf: AppConf = None):
+def config(resources: Dict[str, str] = {}, session_factory: HttpSessionFactory = None, app_conf: AppConf = None):
     global _proxy
     _proxy = new_wsgi_proxy(resources, session_factory, app_conf)
 
 
 def app(environment, start_response):
     if _proxy is None:
         config()
```

### Comparing `naja-atra-wsgi-1.0.0/naja_atra_wsgi/wsgi_request_handler.py` & `naja-atra-wsgi-1.0.1/naja_atra_wsgi/wsgi_request_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 import html
 
 from typing import Any, Dict, List
 from http import HTTPStatus
 
-from naja_atra.request_handlers.http_request_handler import HTTPRequestHandler
+from naja_atra.request_handlers.http_request_handler import HttpRequestHandler
 from naja_atra.utils import http_utils
 from naja_atra.utils.logger import get_logger
 
 
 _logger = get_logger("naja_atra_wsgi.wsgi_request_handler")
 
 
@@ -109,15 +109,15 @@
 
     async def handle_request(self) -> List[bytes]:
         _logger.debug(f"Headers: {self.headers}")
         if self.command == "GET" and "Upgrade" in self.headers and self.headers["Upgrade"] == "websocket":
             self.send_error(501)
             self.start_response(self.status, self.response_headers)
         else:
-            handler = HTTPRequestHandler(self, environment=self.env)
+            handler = HttpRequestHandler(self, environment=self.env)
             await handler.handle_request()
             self.start_response(self.status, self.response_headers)
         return self.body
 
     def send_header(self, key, val):
         if key not in self.__res_headers:
             self.__res_headers[key] = [val]
```

### Comparing `naja-atra-wsgi-1.0.0/naja_atra_wsgi.egg-info/PKG-INFO` & `naja-atra-wsgi-1.0.1/naja_atra_wsgi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naja-atra-wsgi
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is a simple http server, use MVC like design.
 Author-email: keijack <keijack.wu@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Keijack Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naja-atra-wsgi-1.0.0/pyproject.toml` & `naja-atra-wsgi-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naja-atra-wsgi-1.0.0/tests/test_all_ctrls_wsgi.py` & `naja-atra-wsgi-1.0.1/tests/test_all_ctrls_wsgi.py`

 * *Files identical despite different names*

