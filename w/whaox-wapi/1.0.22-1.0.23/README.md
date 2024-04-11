# Comparing `tmp/whaox-wapi-1.0.22.tar.gz` & `tmp/whaox-wapi-1.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whaox-wapi-1.0.22.tar", last modified: Thu Apr 11 20:26:38 2024, max compression
+gzip compressed data, was "whaox-wapi-1.0.23.tar", last modified: Thu Apr 11 20:46:15 2024, max compression
```

## Comparing `whaox-wapi-1.0.22.tar` & `whaox-wapi-1.0.23.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 20:26:38.052855 whaox-wapi-1.0.22/
--rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.22/LICENSE
--rw-rw-rw-   0        0        0     2790 2024-04-11 20:26:38.051533 whaox-wapi-1.0.22/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2024-04-11 20:10:04.000000 whaox-wapi-1.0.22/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 20:26:38.052855 whaox-wapi-1.0.22/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-04-11 20:26:11.000000 whaox-wapi-1.0.22/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 20:26:38.042550 whaox-wapi-1.0.22/wapi/
--rw-rw-rw-   0        0        0       43 2024-04-11 20:25:15.000000 whaox-wapi-1.0.22/wapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 20:26:38.051533 whaox-wapi-1.0.22/whaox_wapi.egg-info/
--rw-rw-rw-   0        0        0     2790 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-11 20:26:37.000000 whaox-wapi-1.0.22/whaox_wapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 20:46:15.376806 whaox-wapi-1.0.23/
+-rw-rw-rw-   0        0        0     1083 2024-04-11 20:02:10.000000 whaox-wapi-1.0.23/LICENSE
+-rw-rw-rw-   0        0        0     2790 2024-04-11 20:46:15.375669 whaox-wapi-1.0.23/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2024-04-11 20:10:04.000000 whaox-wapi-1.0.23/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 20:46:15.376806 whaox-wapi-1.0.23/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-04-11 20:44:58.000000 whaox-wapi-1.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:46:15.348636 whaox-wapi-1.0.23/wapi/
+-rw-rw-rw-   0        0        0       48 2024-04-11 20:44:58.000000 whaox-wapi-1.0.23/wapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:46:15.374354 whaox-wapi-1.0.23/whaox_wapi.egg-info/
+-rw-rw-rw-   0        0        0     2790 2024-04-11 20:46:15.000000 whaox-wapi-1.0.23/whaox_wapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-04-11 20:46:15.000000 whaox-wapi-1.0.23/whaox_wapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 20:46:15.000000 whaox-wapi-1.0.23/whaox_wapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 20:46:15.000000 whaox-wapi-1.0.23/whaox_wapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-11 20:46:15.000000 whaox-wapi-1.0.23/whaox_wapi.egg-info/top_level.txt
```

### Comparing `whaox-wapi-1.0.22/LICENSE` & `whaox-wapi-1.0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.22/PKG-INFO` & `whaox-wapi-1.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.22
+Version: 1.0.23
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whaox-wapi-1.0.22/README.md` & `whaox-wapi-1.0.23/README.md`

 * *Files identical despite different names*

### Comparing `whaox-wapi-1.0.22/setup.py` & `whaox-wapi-1.0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 :authors: WHAOX
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 WHAOX
 """
 
-version = '1.0.22'
+version = '1.0.23'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='whaox-wapi',
     version=version,
```

### Comparing `whaox-wapi-1.0.22/whaox_wapi.egg-info/PKG-INFO` & `whaox-wapi-1.0.23/whaox_wapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whaox-wapi
-Version: 1.0.22
+Version: 1.0.23
 Summary: Web-Library for Python
 Home-page: https://github.com/topanim/WApi
 Author: WHAOX
 Author-email: gorogannisan641@gmail.com
 License: MIT LICENSE, see LICENSE file
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

