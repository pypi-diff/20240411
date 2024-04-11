# Comparing `tmp/htag-0.91.0.tar.gz` & `tmp/htag-0.91.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htag-0.91.0.tar", max compression
+gzip compressed data, was "htag-0.91.1.tar", max compression
```

## Comparing `htag-0.91.0.tar` & `htag-0.91.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2024-03-14 07:20:48.786023 htag-0.91.0/LICENSE
--rw-r--r--   0        0        0     5356 2024-03-14 07:20:48.786023 htag-0.91.0/README.md
--rw-r--r--   0        0        0      419 2024-03-14 07:20:49.050022 htag-0.91.0/htag/__init__.py
--rw-r--r--   0        0        0     2740 2024-03-14 07:20:48.790023 htag-0.91.0/htag/__main__.py
--rw-r--r--   0        0        0     3358 2024-03-14 07:20:48.790023 htag-0.91.0/htag/attrs.py
--rw-r--r--   0        0        0    14712 2024-03-14 07:20:48.790023 htag-0.91.0/htag/render.py
--rw-r--r--   0        0        0     5737 2024-03-14 07:20:48.790023 htag-0.91.0/htag/runners/__init__.py
--rw-r--r--   0        0        0     5331 2024-03-14 07:20:48.790023 htag-0.91.0/htag/runners/chromeappmode.py
--rw-r--r--   0        0        0     2779 2024-03-14 07:20:48.790023 htag-0.91.0/htag/runners/commons/__init__.py
--rw-r--r--   0        0        0     2550 2024-03-14 07:20:48.790023 htag-0.91.0/htag/runners/pyscript.py
--rw-r--r--   0        0        0     1694 2024-03-14 07:20:48.790023 htag-0.91.0/htag/runners/pywebview.py
--rw-r--r--   0        0        0    15834 2024-03-14 07:20:48.790023 htag-0.91.0/htag/runners/runner.py
--rw-r--r--   0        0        0    23436 2024-03-14 07:20:48.790023 htag-0.91.0/htag/runners/server/__init__.py
--rw-r--r--   0        0        0    24144 2024-03-14 07:20:48.790023 htag-0.91.0/htag/tag.py
--rw-r--r--   0        0        0     1147 2024-03-14 07:20:49.050022 htag-0.91.0/pyproject.toml
--rw-r--r--   0        0        0     6622 1970-01-01 00:00:00.000000 htag-0.91.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-14 12:41:20.003000 htag-0.91.1/LICENSE
+-rw-r--r--   0        0        0     5356 2024-03-14 12:41:20.003000 htag-0.91.1/README.md
+-rw-r--r--   0        0        0      419 2024-03-14 12:41:20.475002 htag-0.91.1/htag/__init__.py
+-rw-r--r--   0        0        0     2740 2024-03-14 12:41:20.007000 htag-0.91.1/htag/__main__.py
+-rw-r--r--   0        0        0     3358 2024-03-14 12:41:20.007000 htag-0.91.1/htag/attrs.py
+-rw-r--r--   0        0        0    14712 2024-03-14 12:41:20.007000 htag-0.91.1/htag/render.py
+-rw-r--r--   0        0        0     5737 2024-03-14 12:41:20.007000 htag-0.91.1/htag/runners/__init__.py
+-rw-r--r--   0        0        0     5331 2024-03-14 12:41:20.007000 htag-0.91.1/htag/runners/chromeappmode.py
+-rw-r--r--   0        0        0     2779 2024-03-14 12:41:20.007000 htag-0.91.1/htag/runners/commons/__init__.py
+-rw-r--r--   0        0        0     2550 2024-03-14 12:41:20.007000 htag-0.91.1/htag/runners/pyscript.py
+-rw-r--r--   0        0        0     1694 2024-03-14 12:41:20.007000 htag-0.91.1/htag/runners/pywebview.py
+-rw-r--r--   0        0        0    15834 2024-03-14 12:41:20.007000 htag-0.91.1/htag/runners/runner.py
+-rw-r--r--   0        0        0    23436 2024-03-14 12:41:20.007000 htag-0.91.1/htag/runners/server/__init__.py
+-rw-r--r--   0        0        0    24146 2024-03-14 12:41:20.007000 htag-0.91.1/htag/tag.py
+-rw-r--r--   0        0        0     1147 2024-03-14 12:41:20.475002 htag-0.91.1/pyproject.toml
+-rw-r--r--   0        0        0     6622 1970-01-01 00:00:00.000000 htag-0.91.1/PKG-INFO
```

### Comparing `htag-0.91.0/LICENSE` & `htag-0.91.1/LICENSE`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/README.md` & `htag-0.91.1/README.md`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/__main__.py` & `htag-0.91.1/htag/__main__.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/attrs.py` & `htag-0.91.1/htag/attrs.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/render.py` & `htag-0.91.1/htag/render.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/runners/__init__.py` & `htag-0.91.1/htag/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/runners/chromeappmode.py` & `htag-0.91.1/htag/runners/chromeappmode.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/runners/commons/__init__.py` & `htag-0.91.1/htag/runners/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/runners/pyscript.py` & `htag-0.91.1/htag/runners/pyscript.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/runners/pywebview.py` & `htag-0.91.1/htag/runners/pywebview.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/runners/runner.py` & `htag-0.91.1/htag/runners/runner.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/runners/server/__init__.py` & `htag-0.91.1/htag/runners/server/__init__.py`

 * *Files identical despite different names*

### Comparing `htag-0.91.0/htag/tag.py` & `htag-0.91.1/htag/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
         Tag.__instances__[id(self)]=self
 
         # compute an hash at creation time (used in hrender to identify doubles)
         self._hash_ = md5( str(self._attrs.items())+str(self.childs) )
 
 
     def __declareArgsKargs(self, content:AnyTags=None,**_attrs):
-        self.set(content)
+        self.clear(content)
 
         for k,v in _attrs.items():
             if k.startswith("_"):
                 self[ k[1:].replace("_","-") ] = v
             else:
                 raise HTagException(f"Can't set attributs without underscore ('{k}' should be '_{k}')") # for convention only ;-( (not possible to get it)
```

### Comparing `htag-0.91.0/pyproject.toml` & `htag-0.91.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htag"
-version = "0.91.0" # auto-updated
+version = "0.91.1" # auto-updated
 description = "GUI toolkit for building GUI toolkits (and create beautiful applications for mobile, web, and desktop from a single python3 codebase)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['gui', 'electron', "cef", "pywebview", "starlette", "uvicorn", "tornado", "asyncio", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript", "android", "kivy", "apk"]
 homepage = "https://github.com/manatlan/htag"
 repository = "https://github.com/manatlan/htag"
```

### Comparing `htag-0.91.0/PKG-INFO` & `htag-0.91.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htag
-Version: 0.91.0
+Version: 0.91.1
 Summary: GUI toolkit for building GUI toolkits (and create beautiful applications for mobile, web, and desktop from a single python3 codebase)
 Home-page: https://github.com/manatlan/htag
 License: MIT
 Keywords: gui,electron,cef,pywebview,starlette,uvicorn,tornado,asyncio,desktop,web,mobile,http,websocket,html,pyscript,android,kivy,apk
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: htag Version: 0.91.0 Summary: GUI toolkit for
+Metadata-Version: 2.1 Name: htag Version: 0.91.1 Summary: GUI toolkit for
 building GUI toolkits (and create beautiful applications for mobile, web, and
 desktop from a single python3 codebase) Home-page: https://github.com/manatlan/
 htag License: MIT Keywords:
 gui,electron,cef,pywebview,starlette,uvicorn,tornado,asyncio,desktop,web,mobile,http,websocket,html,pyscript,android,kivy,apk
 Author: manatlan Author-email: manatlan@gmail.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

