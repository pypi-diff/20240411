# Comparing `tmp/whaox-wapi-1.0.2.tar.gz` & `tmp/whaox-wapi-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.0.2.tar", last modified: Thu Apr 11 19:53:50 2024, max compression
+gzip compressed data, was "whaox-wapi-1.0.21.tar", last modified: Thu Apr 11 20:07:51 2024, max compression
```

## Comparing `whaox-wapi-1.0.2.tar` & `whaox-wapi-1.0.21.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 19:53:50.521374 whaox-wapi-1.0.2/
--rw-rw-rw-   0        0        0     2647 2024-04-11 19:53:50.521374 whaox-wapi-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2327 2024-04-11 17:27:02.000000 whaox-wapi-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 19:53:50.521374 whaox-wapi-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-04-11 19:53:45.000000 whaox-wapi-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:53:50.496287 whaox-wapi-1.0.2/wapi/
--rw-rw-rw-   0        0        0       26 2024-04-08 16:26:36.000000 whaox-wapi-1.0.2/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:53:50.520369 whaox-wapi-1.0.2/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     2647 2024-04-11 19:53:50.000000 whaox-wapi-1.0.2/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-04-11 19:53:50.000000 whaox-wapi-1.0.2/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 19:53:50.000000 whaox-wapi-1.0.2/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-11 19:53:50.000000 whaox-wapi-1.0.2/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-11 19:53:50.000000 whaox-wapi-1.0.2/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 20:07:51.727604 whaox-wapi-1.0.21/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.21/LICENSE
+-rw-rw-rw-   0        0        0     2791 2024-04-11 20:07:51.725654 whaox-wapi-1.0.21/PKG-INFO
+-rw-rw-rw-   0        0        0     2447 2024-04-11 20:02:05.000000 whaox-wapi-1.0.21/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 20:07:51.727604 whaox-wapi-1.0.21/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-04-11 20:07:25.000000 whaox-wapi-1.0.21/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:07:51.716416 whaox-wapi-1.0.21/wapi/
+-rw-rw-rw-   0        0        0       26 2024-04-11 20:01:35.000000 whaox-wapi-1.0.21/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:07:51.725654 whaox-wapi-1.0.21/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     2791 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.0.2/PKG-INFO` & `whaox-wapi-1.0.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.2
+Version: 1.0.21
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 # WApi: Web-Library for Python
 
 
-> ### Libraries used:
- >* [jsons](https://github.com/ramonhagenaars/jsons)
- >* [requests]() 
+ ## Libraries used:
+* [jsons](https://github.com/ramonhagenaars/jsons)
+* [requests]() 
+
+
+## Installation
+
+ You can install the latest version with the command:
+ 
+```commandline
+pip install whaox-wapi
+```
 
 ## • Routes 
 
 > You can create paths as you like, splitting your client into modules
 
 ```python
```

### Comparing `whaox-wapi-1.0.2/README.md` & `whaox-wapi-1.0.21/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # WApi: Web-Library for Python
 
 
-> ### Libraries used:
- >* [jsons](https://github.com/ramonhagenaars/jsons)
- >* [requests]() 
+ ## Libraries used:
+* [jsons](https://github.com/ramonhagenaars/jsons)
+* [requests]() 
+
+
+## Installation
+
+ You can install the latest version with the command:
+ 
+```commandline
+pip install whaox-wapi
+```
 
 ## • Routes 
 
 > You can create paths as you like, splitting your client into modules
 
 ```python
```

### Comparing `whaox-wapi-1.0.2/setup.py` & `whaox-wapi-1.0.21/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.2'
+version = '1.0.21'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
```

### Comparing `whaox-wapi-1.0.2/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.0.21/whaox_wapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.2
+Version: 1.0.21
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 # WApi: Web-Library for Python
 
 
-> ### Libraries used:
- >* [jsons](https://github.com/ramonhagenaars/jsons)
- >* [requests]() 
+ ## Libraries used:
+* [jsons](https://github.com/ramonhagenaars/jsons)
+* [requests]() 
+
+
+## Installation
+
+ You can install the latest version with the command:
+ 
+```commandline
+pip install whaox-wapi
+```
 
 ## • Routes 
 
 > You can create paths as you like, splitting your client into modules
 
 ```python
```

