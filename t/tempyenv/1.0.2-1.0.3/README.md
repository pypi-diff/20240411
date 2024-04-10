# Comparing `tmp/tempyenv-1.0.2.tar.gz` & `tmp/tempyenv-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempyenv-1.0.2.tar", last modified: Tue Apr  9 00:12:42 2024, max compression
+gzip compressed data, was "tempyenv-1.0.3.tar", last modified: Wed Apr 10 23:34:15 2024, max compression
```

## Comparing `tempyenv-1.0.2.tar` & `tempyenv-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-09 00:12:42.054628 tempyenv-1.0.2/
--rw-r--r--   0 starboarder2001   (501) staff       (20)     1063 2024-04-07 13:44:24.000000 tempyenv-1.0.2/LICENSE
--rw-r--r--   0 starboarder2001   (501) staff       (20)     3234 2024-04-09 00:12:42.053361 tempyenv-1.0.2/PKG-INFO
--rw-r--r--   0 starboarder2001   (501) staff       (20)     1379 2024-04-07 21:56:28.000000 tempyenv-1.0.2/README.md
--rw-r--r--   0 starboarder2001   (501) staff       (20)      859 2024-04-09 00:11:34.000000 tempyenv-1.0.2/pyproject.toml
--rw-r--r--   0 starboarder2001   (501) staff       (20)       79 2024-04-09 00:12:42.057416 tempyenv-1.0.2/setup.cfg
--rw-r--r--   0 starboarder2001   (501) staff       (20)     2158 2024-04-09 00:11:34.000000 tempyenv-1.0.2/setup.py
-drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-09 00:12:42.039352 tempyenv-1.0.2/src/
-drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-09 00:12:42.046301 tempyenv-1.0.2/src/tempyenv/
--rw-r--r--   0 starboarder2001   (501) staff       (20)       53 2024-04-09 00:11:34.000000 tempyenv-1.0.2/src/tempyenv/__init__.py
--rw-r--r--   0 starboarder2001   (501) staff       (20)     1661 2024-04-09 00:11:34.000000 tempyenv-1.0.2/src/tempyenv/cli.py
-drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-09 00:12:42.051573 tempyenv-1.0.2/src/tempyenv.egg-info/
--rw-r--r--   0 starboarder2001   (501) staff       (20)     3234 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/PKG-INFO
--rw-r--r--   0 starboarder2001   (501) staff       (20)      279 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/SOURCES.txt
--rw-r--r--   0 starboarder2001   (501) staff       (20)        1 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/dependency_links.txt
--rw-r--r--   0 starboarder2001   (501) staff       (20)       75 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/entry_points.txt
--rw-r--r--   0 starboarder2001   (501) staff       (20)        9 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/top_level.txt
+drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-10 23:34:15.859089 tempyenv-1.0.3/
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     1063 2024-04-07 13:44:24.000000 tempyenv-1.0.3/LICENSE
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     3267 2024-04-10 23:34:15.858734 tempyenv-1.0.3/PKG-INFO
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     1412 2024-04-10 23:31:17.000000 tempyenv-1.0.3/README.md
+-rw-r--r--   0 starboarder2001   (501) staff       (20)      859 2024-04-10 23:33:32.000000 tempyenv-1.0.3/pyproject.toml
+-rw-r--r--   0 starboarder2001   (501) staff       (20)       79 2024-04-10 23:34:15.860750 tempyenv-1.0.3/setup.cfg
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     2158 2024-04-10 23:31:11.000000 tempyenv-1.0.3/setup.py
+drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-10 23:34:15.842872 tempyenv-1.0.3/src/
+drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-10 23:34:15.850858 tempyenv-1.0.3/src/tempyenv/
+-rw-r--r--   0 starboarder2001   (501) staff       (20)       53 2024-04-10 23:33:32.000000 tempyenv-1.0.3/src/tempyenv/__init__.py
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     1661 2024-04-10 23:31:11.000000 tempyenv-1.0.3/src/tempyenv/cli.py
+drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-10 23:34:15.857691 tempyenv-1.0.3/src/tempyenv.egg-info/
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     3267 2024-04-10 23:34:15.000000 tempyenv-1.0.3/src/tempyenv.egg-info/PKG-INFO
+-rw-r--r--   0 starboarder2001   (501) staff       (20)      279 2024-04-10 23:34:15.000000 tempyenv-1.0.3/src/tempyenv.egg-info/SOURCES.txt
+-rw-r--r--   0 starboarder2001   (501) staff       (20)        1 2024-04-10 23:34:15.000000 tempyenv-1.0.3/src/tempyenv.egg-info/dependency_links.txt
+-rw-r--r--   0 starboarder2001   (501) staff       (20)       75 2024-04-10 23:34:15.000000 tempyenv-1.0.3/src/tempyenv.egg-info/entry_points.txt
+-rw-r--r--   0 starboarder2001   (501) staff       (20)        9 2024-04-10 23:34:15.000000 tempyenv-1.0.3/src/tempyenv.egg-info/top_level.txt
```

### Comparing `tempyenv-1.0.2/LICENSE` & `tempyenv-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tempyenv-1.0.2/PKG-INFO` & `tempyenv-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempyenv
-Version: 1.0.2
+Version: 1.0.3
 Summary: Easiest and quickest way to setup a temporary python virtual environment
 Home-page: https://github.com/outbit/tempyenv
 Author: David Whiteside
 Author-email: David Whiteside <david@davidwhiteside.com>
 License: MIT License
         
         Copyright (c) 2024 Outbit
@@ -45,28 +45,34 @@
 The easiest and quickest way to create a temp/tmp/temporary python virtual environment.
 
 tempyenv sets up a python environment in a temporary path.  Quick way to create a throw away python environment.
 
 [![Build Status](https://app.travis-ci.com/outbit/tempyenv.svg?branch=develop "ansible-docs latest build")](http://travis-ci.org/outbit/tempyenv)
 [![PIP Version](https://img.shields.io/pypi/v/tempyenv.svg "tempyenv PyPI version")](https://pypi.python.org/pypi/tempyenv)
 [![Coverage Status](https://coveralls.io/repos/outbit/tempyenv/badge.svg?branch=develop&service=github)](https://coveralls.io/github/outbit/tempyenv?branch=develop)
-[![Gitter IM](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/outbit/tempyenv)
+[![Gitter IM](https://badges.gitter.im/Join%20Chat.svg)](https://matrix.to/#/#tempyenv:gitter.im)
 
 
 Installation
 ===========
 
 ```shell
 $ python -m pip install tempyenv
 ```
 
 Usage
 ===========
 
-```shell
+```bash
+$ tmpyenv
+```
+
+or
+
+```bash
 $ tempyenv
 (tempyenv) is setting up your virtual environment...hold tight
 Virtual environment created at /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
 Virtual environment loading from /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
 (tempyenv)(venv) $ echo "now you can pip install in your virtual environment"
 ```
 
@@ -75,7 +81,8 @@
 
 tempyenv is released under the [MIT License](LICENSE.md).
 
 Author
 ======
 
 David Whiteside (<david@davidwhiteside.com>)
+
```

### Comparing `tempyenv-1.0.2/README.md` & `tempyenv-1.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,28 +7,34 @@
 The easiest and quickest way to create a temp/tmp/temporary python virtual environment.
 
 tempyenv sets up a python environment in a temporary path.  Quick way to create a throw away python environment.
 
 [![Build Status](https://app.travis-ci.com/outbit/tempyenv.svg?branch=develop "ansible-docs latest build")](http://travis-ci.org/outbit/tempyenv)
 [![PIP Version](https://img.shields.io/pypi/v/tempyenv.svg "tempyenv PyPI version")](https://pypi.python.org/pypi/tempyenv)
 [![Coverage Status](https://coveralls.io/repos/outbit/tempyenv/badge.svg?branch=develop&service=github)](https://coveralls.io/github/outbit/tempyenv?branch=develop)
-[![Gitter IM](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/outbit/tempyenv)
+[![Gitter IM](https://badges.gitter.im/Join%20Chat.svg)](https://matrix.to/#/#tempyenv:gitter.im)
 
 
 Installation
 ===========
 
 ```shell
 $ python -m pip install tempyenv
 ```
 
 Usage
 ===========
 
-```shell
+```bash
+$ tmpyenv
+```
+
+or
+
+```bash
 $ tempyenv
 (tempyenv) is setting up your virtual environment...hold tight
 Virtual environment created at /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
 Virtual environment loading from /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
 (tempyenv)(venv) $ echo "now you can pip install in your virtual environment"
 ```
 
@@ -37,7 +43,8 @@
 
 tempyenv is released under the [MIT License](LICENSE.md).
 
 Author
 ======
 
 David Whiteside (<david@davidwhiteside.com>)
+
```

### Comparing `tempyenv-1.0.2/pyproject.toml` & `tempyenv-1.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tempyenv"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="David Whiteside", email="david@davidwhiteside.com" },
 ]
 description = "Easiest and quickest way to setup a temporary python virtual environment"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `tempyenv-1.0.2/setup.py` & `tempyenv-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `tempyenv-1.0.2/src/tempyenv/cli.py` & `tempyenv-1.0.3/src/tempyenv/cli.py`

 * *Files identical despite different names*

### Comparing `tempyenv-1.0.2/src/tempyenv.egg-info/PKG-INFO` & `tempyenv-1.0.3/src/tempyenv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempyenv
-Version: 1.0.2
+Version: 1.0.3
 Summary: Easiest and quickest way to setup a temporary python virtual environment
 Home-page: https://github.com/outbit/tempyenv
 Author: David Whiteside
 Author-email: David Whiteside <david@davidwhiteside.com>
 License: MIT License
         
         Copyright (c) 2024 Outbit
@@ -45,28 +45,34 @@
 The easiest and quickest way to create a temp/tmp/temporary python virtual environment.
 
 tempyenv sets up a python environment in a temporary path.  Quick way to create a throw away python environment.
 
 [![Build Status](https://app.travis-ci.com/outbit/tempyenv.svg?branch=develop "ansible-docs latest build")](http://travis-ci.org/outbit/tempyenv)
 [![PIP Version](https://img.shields.io/pypi/v/tempyenv.svg "tempyenv PyPI version")](https://pypi.python.org/pypi/tempyenv)
 [![Coverage Status](https://coveralls.io/repos/outbit/tempyenv/badge.svg?branch=develop&service=github)](https://coveralls.io/github/outbit/tempyenv?branch=develop)
-[![Gitter IM](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/outbit/tempyenv)
+[![Gitter IM](https://badges.gitter.im/Join%20Chat.svg)](https://matrix.to/#/#tempyenv:gitter.im)
 
 
 Installation
 ===========
 
 ```shell
 $ python -m pip install tempyenv
 ```
 
 Usage
 ===========
 
-```shell
+```bash
+$ tmpyenv
+```
+
+or
+
+```bash
 $ tempyenv
 (tempyenv) is setting up your virtual environment...hold tight
 Virtual environment created at /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
 Virtual environment loading from /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
 (tempyenv)(venv) $ echo "now you can pip install in your virtual environment"
 ```
 
@@ -75,7 +81,8 @@
 
 tempyenv is released under the [MIT License](LICENSE.md).
 
 Author
 ======
 
 David Whiteside (<david@davidwhiteside.com>)
+
```

