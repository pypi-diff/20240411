# Comparing `tmp/pibe-0.8.tar.gz` & `tmp/pibe-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibe-0.8.tar", last modified: Mon Oct  9 11:03:26 2023, max compression
+gzip compressed data, was "pibe-0.9.tar", last modified: Mon Nov  6 16:09:25 2023, max compression
```

## Comparing `pibe-0.8.tar` & `pibe-0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxr-x   0 mendonca  (1000) mendonca  (1000)        0 2023-10-09 11:03:26.289774 pibe-0.8/
--rw-rw-r--   0 mendonca  (1000) mendonca  (1000)     1147 2023-10-09 11:03:26.289774 pibe-0.8/PKG-INFO
--rw-rw-r--   0 mendonca  (1000) mendonca  (1000)     6204 2023-10-09 10:56:53.008421 pibe-0.8/pibe.py
--rw-rw-r--   0 mendonca  (1000) mendonca  (1000)      170 2023-10-09 10:56:53.008421 pibe-0.8/setup.cfg
--rw-rw-r--   0 mendonca  (1000) mendonca  (1000)     1386 2023-10-09 11:02:12.817254 pibe-0.8/setup.py
+drwxrwxr-x   0 mendonca  (1000) mendonca  (1000)        0 2023-11-06 16:09:25.651394 pibe-0.9/
+-rw-rw-r--   0 mendonca  (1000) mendonca  (1000)     1147 2023-11-06 16:09:25.651394 pibe-0.9/PKG-INFO
+-rw-rw-r--   0 mendonca  (1000) mendonca  (1000)     6633 2023-11-06 15:55:53.800383 pibe-0.9/pibe.py
+-rw-rw-r--   0 mendonca  (1000) mendonca  (1000)      170 2023-10-09 10:56:53.008421 pibe-0.9/setup.cfg
+-rw-rw-r--   0 mendonca  (1000) mendonca  (1000)     1386 2023-11-06 16:03:03.620800 pibe-0.9/setup.py
```

### Comparing `pibe-0.8/PKG-INFO` & `pibe-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pibe
-Version: 0.8
+Version: 0.9
 Summary: pibe is a webob router.
 Home-page: https://github.com/luismsmendonca/pibe
 Author: Luis Mendonca
 Author-email: luismsmendonca@gmail.com
 License: MIT
 Download-URL: https://github.com/luismsmendonca/pibe/archive/refs/tags/v0.6.tar.gz
 Description: UNKNOWN
```

### Comparing `pibe-0.8/pibe.py` & `pibe-0.9/pibe.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,15 @@
             return func
         return func_decorator
 
 
 class Router(list):
     def __init__(self, middleware=None):
         self.names = dict()
+        self.error_handlers = list()
         self.middleware = Middleware(middleware)
         super().__init__()
 
     def resolve(self, req):
         uri_matched = False
         for (regex, resource, methods, opts) in self:
             match = regex.match(req.path_info)
@@ -122,14 +123,24 @@
         if uri_matched:
             raise exc.HTTPMethodNotAllowed
         raise exc.HTTPNotFound
 
     def response_wrapper(self, resp, **opts):
         return resp
 
+    def error_handler(self):
+        def wrapper(func):
+            self.error_handlers.append(func)
+            return func
+        return wrapper
+
+    def exec_error_handlers(self, *args, **kwargs):
+        for func in self.error_handlers:
+            func(*args, **kwargs)
+
     @wsgify
     def application(self, req):
         (func, kwargs, opts) = self.resolve(req)
 
         # build the middleware
         gen_mw = [mw(req, **opts) for mw in self.middleware if inspect.isgeneratorfunction(mw)]
         func_mw = [mw for mw in self.middleware if not inspect.isgeneratorfunction(mw)]
@@ -138,15 +149,19 @@
         for mw in func_mw:
             mw(req, **opts)
 
         for mw in gen_mw:
             next(mw)
 
         # call the function
-        resp = func(req, **kwargs)
+        try:
+            resp = func(req, **kwargs)
+        except Exception as err:
+            self.exec_error_handlers(req, err)
+            raise
 
         # reverse the middleware
         gen_mw.reverse()
 
         # call the second leg of the middleware
         for mw in gen_mw:
             mw.send(resp)
```

### Comparing `pibe-0.8/setup.py` & `pibe-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "coverage",
     "pytest-cov",
 ]
 
 setup(
     name="pibe",
     py_modules=['pibe'],
-    version="0.8",
+    version="0.9",
     license="MIT",
     description="pibe is a webob router.",
     author="Luis Mendonca",
     author_email="luismsmendonca@gmail.com",
     url="https://github.com/luismsmendonca/pibe",
     download_url="https://github.com/luismsmendonca/pibe/archive/refs/tags/v0.6.tar.gz",
     keywords=["webob", "router"],
```

