# Comparing `tmp/htagui-0.0.2.tar.gz` & `tmp/htagui-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.0.2.tar", max compression
+gzip compressed data, was "htagui-0.0.3.tar", max compression
```

## Comparing `htagui-0.0.2.tar` & `htagui-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-04-11 11:46:06.340489 htagui-0.0.2/LICENSE
--rw-r--r--   0        0        0     6371 2024-04-11 11:46:06.340489 htagui-0.0.2/README.md
--rw-r--r--   0        0        0     1106 2024-04-11 11:46:06.596492 htagui-0.0.2/htagui/__init__.py
--rw-r--r--   0        0        0     3549 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/basics/__init__.py
--rw-r--r--   0        0        0     3215 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/common.py
--rw-r--r--   0        0        0     5335 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/flex.py
--rw-r--r--   0        0        0      758 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/form.py
--rw-r--r--   0        0        0     2075 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/splitters.py
--rw-r--r--   0        0        0     2023 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-11 11:46:06.596492 htagui-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 htagui-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-11 17:50:46.027510 htagui-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6371 2024-04-11 17:50:46.027510 htagui-0.0.3/README.md
+-rw-r--r--   0        0        0     1113 2024-04-11 17:50:46.267511 htagui-0.0.3/htagui/__init__.py
+-rw-r--r--   0        0        0     3549 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/basics/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/common.py
+-rw-r--r--   0        0        0     5335 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/flex.py
+-rw-r--r--   0        0        0      758 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/form.py
+-rw-r--r--   0        0        0     2075 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/splitters.py
+-rw-r--r--   0        0        0     2023 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-11 17:50:46.267511 htagui-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 htagui-0.0.3/PKG-INFO
```

### Comparing `htagui-0.0.2/LICENSE` & `htagui-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/README.md` & `htagui-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/htagui/__init__.py` & `htagui-0.0.3/htagui/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2024 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.0.2" # auto updated
+__version__ = "0.0.3" # auto updated
 
 from htag import Tag
 ########################################################################################
 from .basics import Button,Input,Menu,Spinner,Select
 ########################################################################################
 from .form import Form
 from .tabs import Tabs
@@ -25,8 +25,8 @@
     @property
     def ui(self):
         if self._ui is None:
             self._ui = Dialog(self)
         return self._ui
 
 ALL=[App,Button,Input,Select,Menu,Spinner,Form,Tabs,Dialog,HSplit]
-__all__=["App","Button","Input","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",      "hflex","vflex"]
+__all__=["App","Button","Input","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",      "hflex","vflex", "ALL"]
```

### Comparing `htagui-0.0.2/htagui/basics/__init__.py` & `htagui-0.0.3/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/htagui/common.py` & `htagui-0.0.3/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/htagui/dialog.py` & `htagui-0.0.3/htagui/dialog.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/htagui/flex.py` & `htagui-0.0.3/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/htagui/form.py` & `htagui-0.0.3/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/htagui/splitters.py` & `htagui-0.0.3/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/htagui/tabs.py` & `htagui-0.0.3/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.2/pyproject.toml` & `htagui-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.0.2" # auto-updated
+version = "0.0.3" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
@@ -15,15 +15,15 @@
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
 ]
 
 [tool.poetry.dependencies]
 # https://python-poetry.org/docs/dependency-specification/
 python = "^3.7"
-htag = ">= 0.101"
+htag = ">= 0.102"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6"
 pytest-cov = "^2.6"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `htagui-0.0.2/PKG-INFO` & `htagui-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.0.2
+Version: 0.0.3
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: htag (>=0.101)
+Requires-Dist: htag (>=0.102)
 Project-URL: Documentation, https://github.com/manatlan/htagui
 Project-URL: Repository, https://github.com/manatlan/htagui
 Description-Content-Type: text/markdown
 
 # htagUI
 
 This is a (basic) UI toolkit for [htag](https://github.com/manatlan/htag) apps. Contrario to [htbulma](https://github.com/manatlan/htbulma), this one is a minimal toolkit, providing only useful and solid widgets, and will be maintained (you can use it ;-)).
```

