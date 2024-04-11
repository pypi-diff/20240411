# Comparing `tmp/Velkoz-0.0.42.tar.gz` & `tmp/Velkoz-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Velkoz-0.0.42.tar", last modified: Wed Apr 10 19:51:13 2024, max compression
+gzip compressed data, was "Velkoz-0.0.43.tar", last modified: Wed Apr 10 19:55:27 2024, max compression
```

## Comparing `Velkoz-0.0.42.tar` & `Velkoz-0.0.43.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 19:51:13.670784 Velkoz-0.0.42/
--rw-rw-rw-   0        0        0      671 2024-04-10 19:51:13.670268 Velkoz-0.0.42/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 19:51:13.634340 Velkoz-0.0.42/Velkoz/
--rw-rw-rw-   0        0        0      346 2024-03-21 19:18:50.000000 Velkoz-0.0.42/Velkoz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:51:13.660038 Velkoz-0.0.42/Velkoz/eye/
--rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.42/Velkoz/eye/__init__.py
--rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.42/Velkoz/eye/account.py
--rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.42/Velkoz/eye/champion_mastery.py
--rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.42/Velkoz/eye/common.py
--rw-rw-rw-   0        0        0     7581 2024-04-06 09:20:19.000000 Velkoz-0.0.42/Velkoz/eye/match.py
--rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.42/Velkoz/eye/summoner.py
--rw-rw-rw-   0        0        0     1160 2024-04-10 19:50:55.000000 Velkoz-0.0.42/Velkoz/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:51:13.662763 Velkoz-0.0.42/Velkoz/supp/
--rw-rw-rw-   0        0        0      129 2024-04-05 19:15:06.000000 Velkoz-0.0.42/Velkoz/supp/__init__.py
--rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.42/Velkoz/supp/account.py
--rw-rw-rw-   0        0        0     1147 2024-04-10 19:50:28.000000 Velkoz-0.0.42/Velkoz/supp/champion_mastery.py
--rw-rw-rw-   0        0        0      272 2024-04-10 19:50:21.000000 Velkoz-0.0.42/Velkoz/supp/match.py
--rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.42/Velkoz/supp/summoner.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:51:13.668764 Velkoz-0.0.42/Velkoz/tentacles/
--rw-rw-rw-   0        0        0      213 2024-03-18 23:45:33.000000 Velkoz-0.0.42/Velkoz/tentacles/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.42/Velkoz/tentacles/account.py
--rw-rw-rw-   0        0        0     3340 2024-04-10 19:40:42.000000 Velkoz-0.0.42/Velkoz/tentacles/champion_mastery.py
--rw-rw-rw-   0        0        0     4505 2024-04-06 09:36:14.000000 Velkoz-0.0.42/Velkoz/tentacles/common.py
--rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.42/Velkoz/tentacles/config.py
--rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.42/Velkoz/tentacles/match.py
--rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.42/Velkoz/tentacles/summoner.py
--rw-rw-rw-   0        0        0     5364 2024-04-10 19:40:41.000000 Velkoz-0.0.42/Velkoz/velkoz.py
-drwxrwxrwx   0        0        0        0 2024-04-10 19:51:13.668764 Velkoz-0.0.42/Velkoz.egg-info/
--rw-rw-rw-   0        0        0      671 2024-04-10 19:51:13.000000 Velkoz-0.0.42/Velkoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2024-04-10 19:51:13.000000 Velkoz-0.0.42/Velkoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 19:51:13.000000 Velkoz-0.0.42/Velkoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-10 19:51:13.000000 Velkoz-0.0.42/Velkoz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 19:51:13.000000 Velkoz-0.0.42/Velkoz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 19:51:13.671342 Velkoz-0.0.42/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 19:55:27.429477 Velkoz-0.0.43/
+-rw-rw-rw-   0        0        0      671 2024-04-10 19:55:27.428480 Velkoz-0.0.43/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 19:55:27.391271 Velkoz-0.0.43/Velkoz/
+-rw-rw-rw-   0        0        0      549 2024-04-10 19:54:57.000000 Velkoz-0.0.43/Velkoz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:55:27.416961 Velkoz-0.0.43/Velkoz/eye/
+-rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.43/Velkoz/eye/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.43/Velkoz/eye/account.py
+-rw-rw-rw-   0        0        0      591 2024-04-09 19:37:05.000000 Velkoz-0.0.43/Velkoz/eye/champion_mastery.py
+-rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.43/Velkoz/eye/common.py
+-rw-rw-rw-   0        0        0     7581 2024-04-06 09:20:19.000000 Velkoz-0.0.43/Velkoz/eye/match.py
+-rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.43/Velkoz/eye/summoner.py
+-rw-rw-rw-   0        0        0     1160 2024-04-10 19:55:13.000000 Velkoz-0.0.43/Velkoz/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:55:27.421478 Velkoz-0.0.43/Velkoz/supp/
+-rw-rw-rw-   0        0        0      129 2024-04-05 19:15:06.000000 Velkoz-0.0.43/Velkoz/supp/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.43/Velkoz/supp/account.py
+-rw-rw-rw-   0        0        0     1147 2024-04-10 19:50:28.000000 Velkoz-0.0.43/Velkoz/supp/champion_mastery.py
+-rw-rw-rw-   0        0        0      272 2024-04-10 19:50:21.000000 Velkoz-0.0.43/Velkoz/supp/match.py
+-rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.43/Velkoz/supp/summoner.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:55:27.425480 Velkoz-0.0.43/Velkoz/tentacles/
+-rw-rw-rw-   0        0        0      213 2024-03-18 23:45:33.000000 Velkoz-0.0.43/Velkoz/tentacles/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.43/Velkoz/tentacles/account.py
+-rw-rw-rw-   0        0        0     3340 2024-04-10 19:40:42.000000 Velkoz-0.0.43/Velkoz/tentacles/champion_mastery.py
+-rw-rw-rw-   0        0        0     4505 2024-04-06 09:36:14.000000 Velkoz-0.0.43/Velkoz/tentacles/common.py
+-rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.43/Velkoz/tentacles/config.py
+-rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.43/Velkoz/tentacles/match.py
+-rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.43/Velkoz/tentacles/summoner.py
+-rw-rw-rw-   0        0        0     5364 2024-04-10 19:40:41.000000 Velkoz-0.0.43/Velkoz/velkoz.py
+drwxrwxrwx   0        0        0        0 2024-04-10 19:55:27.427479 Velkoz-0.0.43/Velkoz.egg-info/
+-rw-rw-rw-   0        0        0      671 2024-04-10 19:55:27.000000 Velkoz-0.0.43/Velkoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2024-04-10 19:55:27.000000 Velkoz-0.0.43/Velkoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 19:55:27.000000 Velkoz-0.0.43/Velkoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-10 19:55:27.000000 Velkoz-0.0.43/Velkoz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 19:55:27.000000 Velkoz-0.0.43/Velkoz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 19:55:27.429477 Velkoz-0.0.43/setup.cfg
```

### Comparing `Velkoz-0.0.42/PKG-INFO` & `Velkoz-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.42
+Version: 0.0.43
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `Velkoz-0.0.42/Velkoz/eye/account.py` & `Velkoz-0.0.43/Velkoz/eye/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/eye/champion_mastery.py` & `Velkoz-0.0.43/Velkoz/eye/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/eye/match.py` & `Velkoz-0.0.43/Velkoz/eye/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/eye/summoner.py` & `Velkoz-0.0.43/Velkoz/eye/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/setup.py` & `Velkoz-0.0.43/Velkoz/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
  #python setup.py sdist bdist_wheel
-VERSION = '0.0.42' 
+VERSION = '0.0.43' 
 DESCRIPTION = 'Velkoz Riot Api package'
 LONG_DESCRIPTION = 'Package that uses RiotApi to get information.\n Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.'
 
 # Setting up
 setup(
         name="Velkoz", 
         version=VERSION,
```

### Comparing `Velkoz-0.0.42/Velkoz/supp/account.py` & `Velkoz-0.0.43/Velkoz/supp/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/supp/champion_mastery.py` & `Velkoz-0.0.43/Velkoz/supp/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/supp/summoner.py` & `Velkoz-0.0.43/Velkoz/supp/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/tentacles/account.py` & `Velkoz-0.0.43/Velkoz/tentacles/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/tentacles/champion_mastery.py` & `Velkoz-0.0.43/Velkoz/tentacles/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/tentacles/common.py` & `Velkoz-0.0.43/Velkoz/tentacles/common.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/tentacles/match.py` & `Velkoz-0.0.43/Velkoz/tentacles/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/tentacles/summoner.py` & `Velkoz-0.0.43/Velkoz/tentacles/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz/velkoz.py` & `Velkoz-0.0.43/Velkoz/velkoz.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.42/Velkoz.egg-info/PKG-INFO` & `Velkoz-0.0.43/Velkoz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.42
+Version: 0.0.43
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `Velkoz-0.0.42/Velkoz.egg-info/SOURCES.txt` & `Velkoz-0.0.43/Velkoz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

