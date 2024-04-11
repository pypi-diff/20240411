# Comparing `tmp/python-flux-0.8.4.tar.gz` & `tmp/python_flux-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-flux-0.8.4.tar", max compression
+gzip compressed data, was "python_flux-0.9.0.tar", max compression
```

## Comparing `python-flux-0.8.4.tar` & `python_flux-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      696 2022-09-13 18:12:45.757783 python-flux-0.8.4/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.854791 python-flux-0.8.4/python_flux/__init__.py
--rw-r--r--   0        0        0     6492 2022-09-13 18:07:36.742067 python-flux-0.8.4/python_flux/flux.py
--rw-r--r--   0        0        0     1182 2022-08-03 05:02:04.955464 python-flux-0.8.4/python_flux/producers.py
--rw-r--r--   0        0        0      858 2022-08-04 02:39:35.852762 python-flux-0.8.4/python_flux/subscribers.py
--rw-r--r--   0        0        0      686 2022-09-13 18:12:45.900666 python-flux-0.8.4/setup.py
--rw-r--r--   0        0        0      594 2022-09-13 18:12:45.901039 python-flux-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      719 2024-04-11 04:42:26.800886 python_flux-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-0.9.0/python_flux/__init__.py
+-rw-r--r--   0        0        0     7123 2024-04-11 02:03:51.782589 python_flux-0.9.0/python_flux/flux.py
+-rw-r--r--   0        0        0     1182 2022-12-06 14:51:39.000000 python_flux-0.9.0/python_flux/producers.py
+-rw-r--r--   0        0        0      858 2022-09-13 18:15:28.000000 python_flux-0.9.0/python_flux/subscribers.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-0.9.0/PKG-INFO
```

### Comparing `python-flux-0.8.4/pyproject.toml` & `python_flux-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "python-flux"
-version = "0.8.4"
+version = "0.9.0"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
-authors = ["Juan Pablo Bochard <jbochard@despegar.com>"]
+authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 jsonmerge = "^1.8"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 
 [tool.poetry-dynamic-versioning]
-enable = false
-pattern = '(?P<base>\d+\.\d+\.\d+)'
+enable = true
+vcs = "git"
+style = "semver"
 
 [build-system]
-requires = ["poetry>=1.1.0", "poetry-dynamic-versioning"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `python-flux-0.8.4/python_flux/flux.py` & `python_flux-0.9.0/python_flux/flux.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import datetime
 import time
 import traceback
 import logging
+import types
 from datetime import timedelta
 
 from jsonmerge import merge
 
 from python_flux.subscribers import SSubscribe, SForeach
 
 
 class Flux(object):
 
+    def __default_action_with_context(value, context):
+        pass
+
+    def __default_action(value):
+        pass
+
     def __default_success(value):
         pass
 
     def __default_error(e):
         if not isinstance(e, StopIteration):
             traceback.print_exception(type(e), e, e.__traceback__)
 
-    def filter(self, predicate):
-        return FFilter(predicate, self)
+    def filter(self, predicate, on_mismatch=__default_action):
+        return FFilter(predicate, on_mismatch, self)
 
-    def filter_with_context(self, predicate_with_context):
-        return FFilterWithContext(predicate_with_context, self)
+    def filter_with_context(self, predicate_with_context, on_mismatch=__default_action_with_context):
+        return FFilterWithContext(predicate_with_context, on_mismatch, self)
 
     def map(self, f):
         return FMap(f, self)
 
     def map_context(self, f):
         return FMapContext(f, self)
 
@@ -71,34 +78,38 @@
         value, ctx = self.upstream.next(context)
         while value is None:
             value, ctx = self.upstream.next(context)
         return value, ctx
 
 
 class FFilter(Stream):
-    def __init__(self, p, flux):
+    def __init__(self, p, m, flux):
         super().__init__(flux)
         self.predicate = p
+        self.on_mismatch = m
 
     def next(self, context):
         value, ctx = super(FFilter, self).next(context)
         while not self.predicate(value):
+            self.on_mismatch(value)
             value, ctx = super(FFilter, self).next(context)
         return value, ctx
 
 
 class FFilterWithContext(Stream):
-    def __init__(self, p, flux):
+    def __init__(self, p, m, flux):
         super().__init__(flux)
         self.predicate = p
+        self.on_mismatch = m
 
     def next(self, context):
         value, ctx = super(FFilterWithContext, self).next(context)
         ctx_bkp = ctx.copy()
         while not self.predicate(value, ctx_bkp):
+            self.on_mismatch(value, ctx_bkp)
             value, ctx = super(FFilterWithContext, self).next(context)
         return value, ctx
 
 
 class FTake(Stream):
     def __init__(self, count, flux):
         super().__init__(flux)
@@ -209,15 +220,22 @@
 
     def next(self, context):
         ctx = context
         while True:
             while self.current is None:
                 value, ctx = super(FFlatMap, self).next(ctx)
                 ctx_bkp = ctx.copy()
-                self.current = self.function(value, ctx_bkp).subscribe(ctx)
+                func = self.function(value, ctx_bkp)
+
+                if isinstance(func, types.GeneratorType):
+                    from python_flux.producers import PFromGenerator
+                    fgen = PFromGenerator(func)
+                else:
+                    fgen = func
+                self.current = fgen.subscribe(ctx)
             try:
                 v, c = next(self.current)
                 while v is None:
                     v, c = next(self.current)
                 ctx = merge(ctx, c)
                 return v, ctx
             except StopIteration:
```

### Comparing `python-flux-0.8.4/python_flux/producers.py` & `python_flux-0.9.0/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python-flux-0.8.4/python_flux/subscribers.py` & `python_flux-0.9.0/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python-flux-0.8.4/PKG-INFO` & `python_flux-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 0.8.4
+Version: 0.9.0
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
-Author-email: jbochard@despegar.com
+Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: jsonmerge (>=1.8,<2.0)
```

