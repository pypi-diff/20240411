# Comparing `tmp/staticjinjaplus-1.1.0.tar.gz` & `tmp/staticjinjaplus-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticjinjaplus-1.1.0.tar", last modified: Thu Apr 11 08:45:33 2024, max compression
+gzip compressed data, was "staticjinjaplus-1.1.1.tar", last modified: Thu Apr 11 14:50:34 2024, max compression
```

## Comparing `staticjinjaplus-1.1.0.tar` & `staticjinjaplus-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 08:45:33.370458 staticjinjaplus-1.1.0/
--rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.1.0/LICENSE.md
--rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    20489 2024-04-11 08:45:33.369458 staticjinjaplus-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    18804 2024-04-11 08:36:27.000000 staticjinjaplus-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 08:45:33.370458 staticjinjaplus-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4098 2024-04-11 08:37:09.000000 staticjinjaplus-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:45:33.348457 staticjinjaplus-1.1.0/staticjinjaplus/
--rw-rw-rw-   0        0        0     6415 2024-04-11 08:42:19.000000 staticjinjaplus-1.1.0/staticjinjaplus/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-11 08:29:30.000000 staticjinjaplus-1.1.0/staticjinjaplus/__version__.py
--rw-rw-rw-   0        0        0     1289 2024-04-08 22:09:51.000000 staticjinjaplus-1.1.0/staticjinjaplus/cli.py
--rw-rw-rw-   0        0        0     2942 2024-04-11 08:42:04.000000 staticjinjaplus-1.1.0/staticjinjaplus/http.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 14:40:43.000000 staticjinjaplus-1.1.0/staticjinjaplus/jinja_helpers.py
--rw-rw-rw-   0        0        0     1174 2024-04-09 21:15:15.000000 staticjinjaplus-1.1.0/staticjinjaplus/staticjinja_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-11 08:45:33.368458 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/
--rw-rw-rw-   0        0        0    20489 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      115 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:50:34.680072 staticjinjaplus-1.1.1/
+-rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    20476 2024-04-11 14:50:34.679072 staticjinjaplus-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    18742 2024-04-11 13:59:07.000000 staticjinjaplus-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:50:34.680072 staticjinjaplus-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     4142 2024-04-11 13:54:01.000000 staticjinjaplus-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:50:34.670072 staticjinjaplus-1.1.1/staticjinjaplus/
+-rw-rw-rw-   0        0        0     6415 2024-04-11 08:42:19.000000 staticjinjaplus-1.1.1/staticjinjaplus/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-11 14:49:29.000000 staticjinjaplus-1.1.1/staticjinjaplus/__version__.py
+-rw-rw-rw-   0        0        0     1289 2024-04-08 22:09:51.000000 staticjinjaplus-1.1.1/staticjinjaplus/cli.py
+-rw-rw-rw-   0        0        0     2942 2024-04-11 08:42:04.000000 staticjinjaplus-1.1.1/staticjinjaplus/http.py
+-rw-rw-rw-   0        0        0     1284 2024-04-11 12:23:18.000000 staticjinjaplus-1.1.1/staticjinjaplus/jinja_helpers.py
+-rw-rw-rw-   0        0        0     1174 2024-04-09 21:15:15.000000 staticjinjaplus-1.1.1/staticjinjaplus/staticjinja_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:50:34.677072 staticjinjaplus-1.1.1/staticjinjaplus.egg-info/
+-rw-rw-rw-   0        0        0    20476 2024-04-11 14:50:34.000000 staticjinjaplus-1.1.1/staticjinjaplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2024-04-11 14:50:34.000000 staticjinjaplus-1.1.1/staticjinjaplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:50:34.000000 staticjinjaplus-1.1.1/staticjinjaplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-11 14:50:34.000000 staticjinjaplus-1.1.1/staticjinjaplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      115 2024-04-11 14:50:34.000000 staticjinjaplus-1.1.1/staticjinjaplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-11 14:50:34.000000 staticjinjaplus-1.1.1/staticjinjaplus.egg-info/top_level.txt
```

### Comparing `staticjinjaplus-1.1.0/LICENSE.md` & `staticjinjaplus-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.1.0/PKG-INFO` & `staticjinjaplus-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: staticjinjaplus
-Version: 1.1.0
-Summary: An opinionated sweet spot between staticjinja and a full-blown static site generator.
+Version: 1.1.1
+Summary: A sweet spot between staticjinja and a full-blown static site generator.
 Home-page: https://github.com/EpocDotFr/staticjinjaplus
 Author: Maxime "Epoc" Gross
 Author-email: contact.nospam@epoc.nospam.fr
 License: DBAD
 Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme
 Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
 Project-URL: Tracker, https://github.com/EpocDotFr/staticjinjaplus/issues
 Project-URL: Changelog, https://github.com/EpocDotFr/staticjinjaplus/releases
 Keywords: static,website,site,generator,staticjinja,jinja,jinja2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -35,28 +36,27 @@
 Provides-Extra: dev
 Requires-Dist: build~=1.2; extra == "dev"
 Requires-Dist: twine~=5.0; extra == "dev"
 
 
 # staticjinjaplus
 
-An opinionated sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static
-site generator.
+A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
 
 ![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
 
 [PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
 
 Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
 I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
 order to be able to generate a static website that will actually be ready for real world usage.
 
 staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
-That's also why "opinionated" is an important keyword in this project's description: choices have been made to cover some
-use cases, but not all. This is not your average static site generator.
+Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
+static site generator.
 
 ## Features
 
 All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
 
   - Simple, file-based configuration to centralize *a handful* of configuration values
   - Build improvements
@@ -75,15 +75,15 @@
 
 **Planned:**
 
   - Generic support of Markdown-formatted templates collections (forget about the usual "pages" or "articles/blog posts" feature)
 
 ## Prerequisites
 
-  - Python >= 3.12
+  - Python >= 3.9
 
 ## Installation
 
 From PyPI:
 
 ```bash
 $ pip install staticjinjaplus
```

### Comparing `staticjinjaplus-1.1.0/README.md` & `staticjinjaplus-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # staticjinjaplus
 
-An opinionated sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static
-site generator.
+A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
 
 ![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
 
 [PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
 
 Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
 I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
 order to be able to generate a static website that will actually be ready for real world usage.
 
 staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
-That's also why "opinionated" is an important keyword in this project's description: choices have been made to cover some
-use cases, but not all. This is not your average static site generator.
+Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
+static site generator.
 
 ## Features
 
 All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
 
   - Simple, file-based configuration to centralize *a handful* of configuration values
   - Build improvements
@@ -36,15 +35,15 @@
 
 **Planned:**
 
   - Generic support of Markdown-formatted templates collections (forget about the usual "pages" or "articles/blog posts" feature)
 
 ## Prerequisites
 
-  - Python >= 3.12
+  - Python >= 3.9
 
 ## Installation
 
 From PyPI:
 
 ```bash
 $ pip install staticjinjaplus
```

### Comparing `staticjinjaplus-1.1.0/setup.py` & `staticjinjaplus-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from importlib import util as importlib_util
 from subprocess import call
 from shutil import rmtree
 from os import path
 import sys
 
 NAME = 'staticjinjaplus'
-DESCRIPTION = 'An opinionated sweet spot between staticjinja and a full-blown static site generator.'
+DESCRIPTION = 'A sweet spot between staticjinja and a full-blown static site generator.'
 URL = 'https://github.com/EpocDotFr/staticjinjaplus'
 EMAIL = 'contact.nospam@epoc.nospam.fr'
 AUTHOR = 'Maxime "Epoc" Gross'
 REQUIRES_PYTHON = '>=3.9'
 VERSION = None  # Pulled from staticjinjaplus/__version__.py
 
 REQUIRED = [
@@ -32,14 +32,15 @@
 }
 
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Operating System :: OS Independent',
     'Environment :: Console',
     'Environment :: Web Environment',
+    'Topic :: Internet :: WWW/HTTP :: Site Management',
     'Topic :: Text Processing :: Markup :: XML',
     'Topic :: Text Processing :: Markup :: HTML',
     'Topic :: Text Processing :: Markup :: Markdown',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
```

### Comparing `staticjinjaplus-1.1.0/staticjinjaplus/__init__.py` & `staticjinjaplus-1.1.1/staticjinjaplus/__init__.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.1.0/staticjinjaplus/cli.py` & `staticjinjaplus-1.1.1/staticjinjaplus/cli.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.1.0/staticjinjaplus/http.py` & `staticjinjaplus-1.1.1/staticjinjaplus/http.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.1.0/staticjinjaplus/jinja_helpers.py` & `staticjinjaplus-1.1.1/staticjinjaplus/jinja_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import Dict, Callable
 from markupsafe import Markup
 from os import path
 
 
 def url(config: Dict) -> Callable:
     """Build a relative or absolute URL to a file relative to the output dir"""
-    def inner(path: str, absolute: bool = False) -> str:
+    def inner(p: str, absolute: bool = False) -> str:
         ret = config['BASE_URL'].rstrip('/') + '/' if absolute else '/'
-        ret += path.lstrip('/')
+        ret += p.lstrip('/')
 
         return ret
 
     return inner
 
 
 def icon(config: Dict) -> Callable:
```

### Comparing `staticjinjaplus-1.1.0/staticjinjaplus/staticjinja_helpers.py` & `staticjinjaplus-1.1.1/staticjinjaplus/staticjinja_helpers.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.1.0/staticjinjaplus.egg-info/PKG-INFO` & `staticjinjaplus-1.1.1/staticjinjaplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: staticjinjaplus
-Version: 1.1.0
-Summary: An opinionated sweet spot between staticjinja and a full-blown static site generator.
+Version: 1.1.1
+Summary: A sweet spot between staticjinja and a full-blown static site generator.
 Home-page: https://github.com/EpocDotFr/staticjinjaplus
 Author: Maxime "Epoc" Gross
 Author-email: contact.nospam@epoc.nospam.fr
 License: DBAD
 Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme
 Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
 Project-URL: Tracker, https://github.com/EpocDotFr/staticjinjaplus/issues
 Project-URL: Changelog, https://github.com/EpocDotFr/staticjinjaplus/releases
 Keywords: static,website,site,generator,staticjinja,jinja,jinja2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -35,28 +36,27 @@
 Provides-Extra: dev
 Requires-Dist: build~=1.2; extra == "dev"
 Requires-Dist: twine~=5.0; extra == "dev"
 
 
 # staticjinjaplus
 
-An opinionated sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static
-site generator.
+A sweet spot between [staticjinja](https://staticjinja.readthedocs.io/en/latest/) and a full-blown static  site generator.
 
 ![Python versions](https://img.shields.io/pypi/pyversions/staticjinjaplus.svg) ![Version](https://img.shields.io/pypi/v/staticjinjaplus.svg) ![License](https://img.shields.io/pypi/l/staticjinjaplus.svg)
 
 [PyPI](https://pypi.org/project/staticjinjaplus/) - [Documentation](https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme) - [Source Code](https://github.com/EpocDotFr/staticjinjaplus) - [Issue Tracker](https://github.com/EpocDotFr/staticjinjaplus/issues) - [Changelog](https://github.com/EpocDotFr/staticjinjaplus/releases)
 
 Citing staticjinja's documentation, "most static site generators are cumbersome to use". While I fully agree, and while
 I find staticjinja to be an awesome piece of software, there's still some gaps here and there that needs to be filled in
 order to be able to generate a static website that will actually be ready for real world usage.
 
 staticjinjaplus try to fill these gaps, while still being built on staticjinja and its philosophy: keep it simple, stupid.
-That's also why "opinionated" is an important keyword in this project's description: choices have been made to cover some
-use cases, but not all. This is not your average static site generator.
+Note staticjinjaplus is opinionated: choices have been made to cover some use cases, but not all. This is not your average
+static site generator.
 
 ## Features
 
 All of [staticjinja](https://staticjinja.readthedocs.io/en/latest/)'s features, plus:
 
   - Simple, file-based configuration to centralize *a handful* of configuration values
   - Build improvements
@@ -75,15 +75,15 @@
 
 **Planned:**
 
   - Generic support of Markdown-formatted templates collections (forget about the usual "pages" or "articles/blog posts" feature)
 
 ## Prerequisites
 
-  - Python >= 3.12
+  - Python >= 3.9
 
 ## Installation
 
 From PyPI:
 
 ```bash
 $ pip install staticjinjaplus
```

