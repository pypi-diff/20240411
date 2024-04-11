# Comparing `tmp/whaox-wapi-1.0.21.tar.gz` & `tmp/whaox-wapi-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.0.21.tar", last modified: Thu Apr 11 20:07:51 2024, max compression
+gzip compressed data, was "whaox-wapi-1.0.22.tar", last modified: Thu Apr 11 20:26:38 2024, max compression
```

## Comparing `whaox-wapi-1.0.21.tar` & `whaox-wapi-1.0.22.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 20:07:51.727604 whaox-wapi-1.0.21/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.21/LICENSE
--rw-rw-rw-   0        0        0     2791 2024-04-11 20:07:51.725654 whaox-wapi-1.0.21/PKG-INFO
--rw-rw-rw-   0        0        0     2447 2024-04-11 20:02:05.000000 whaox-wapi-1.0.21/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 20:07:51.727604 whaox-wapi-1.0.21/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-04-11 20:07:25.000000 whaox-wapi-1.0.21/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 20:07:51.716416 whaox-wapi-1.0.21/wapi/
--rw-rw-rw-   0        0        0       26 2024-04-11 20:01:35.000000 whaox-wapi-1.0.21/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 20:07:51.725654 whaox-wapi-1.0.21/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     2791 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-11 20:07:51.000000 whaox-wapi-1.0.21/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 20:26:38.052855 whaox-wapi-1.0.22/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.22/LICENSE
+-rw-rw-rw-   0        0        0     2790 2024-04-11 20:26:38.051533 whaox-wapi-1.0.22/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2024-04-11 20:10:04.000000 whaox-wapi-1.0.22/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 20:26:38.052855 whaox-wapi-1.0.22/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-04-11 20:26:11.000000 whaox-wapi-1.0.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:26:38.042550 whaox-wapi-1.0.22/wapi/
+-rw-rw-rw-   0        0        0       43 2024-04-11 20:25:15.000000 whaox-wapi-1.0.22/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:26:38.051533 whaox-wapi-1.0.22/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     2790 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.0.21/LICENSE` & `whaox-wapi-1.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.21/PKG-INFO` & `whaox-wapi-1.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.21
+Version: 1.0.22
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 # WApi: Web-Library for Python
 
 
- ## Libraries used:
+## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
 
 ## Installation
 
  You can install the latest version with the command:
```

### Comparing `whaox-wapi-1.0.21/README.md` & `whaox-wapi-1.0.22/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # WApi: Web-Library for Python
 
 
- ## Libraries used:
+## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
 
 ## Installation
 
  You can install the latest version with the command:
```

### Comparing `whaox-wapi-1.0.21/setup.py` & `whaox-wapi-1.0.22/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.21'
+version = '1.0.22'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
```

### Comparing `whaox-wapi-1.0.21/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.0.22/whaox_wapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.21
+Version: 1.0.22
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jsons
 Requires-Dist: requests
 
 # WApi: Web-Library for Python
 
 
- ## Libraries used:
+## Libraries used:
 * [jsons](https://github.com/ramonhagenaars/jsons)
 * [requests]() 
 
 
 ## Installation
 
  You can install the latest version with the command:
```

