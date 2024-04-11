# Comparing `tmp/S_Taper-0.8.3.6.tar.gz` & `tmp/S_Taper-0.8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "S_Taper-0.8.3.6.tar", last modified: Fri Mar 29 21:33:01 2024, max compression
+gzip compressed data, was "S_Taper-0.8.4.0.tar", last modified: Thu Apr 11 09:18:52 2024, max compression
```

## Comparing `S_Taper-0.8.3.6.tar` & `S_Taper-0.8.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 21:33:01.257654 S_Taper-0.8.3.6/
--rw-rw-rw-   0        0        0      663 2024-03-29 21:33:01.256654 S_Taper-0.8.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-03-29 21:32:09.000000 S_Taper-0.8.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 21:33:01.253655 S_Taper-0.8.3.6/S_Taper.egg-info/
--rw-rw-rw-   0        0        0      663 2024-03-29 21:33:01.000000 S_Taper-0.8.3.6/S_Taper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-03-29 21:33:01.000000 S_Taper-0.8.3.6/S_Taper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 21:33:01.000000 S_Taper-0.8.3.6/S_Taper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-29 21:33:01.000000 S_Taper-0.8.3.6/S_Taper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-29 21:33:01.000000 S_Taper-0.8.3.6/S_Taper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-29 21:33:01.246654 S_Taper-0.8.3.6/s_taper/
--rw-rw-rw-   0        0        0    15532 2024-03-29 21:04:31.000000 S_Taper-0.8.3.6/s_taper/__init__.py
--rw-rw-rw-   0        0        0     8706 2024-01-31 04:33:07.000000 S_Taper-0.8.3.6/s_taper/aio.py
--rw-rw-rw-   0        0        0       80 2023-08-11 19:52:02.000000 S_Taper-0.8.3.6/s_taper/consts.py
--rw-rw-rw-   0        0        0       42 2024-03-29 21:33:01.259653 S_Taper-0.8.3.6/setup.cfg
--rw-rw-rw-   0        0        0      654 2024-03-29 21:32:26.000000 S_Taper-0.8.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 21:33:01.249654 S_Taper-0.8.3.6/tests/
--rw-rw-rw-   0        0        0     5059 2024-03-29 20:18:51.000000 S_Taper-0.8.3.6/tests/test_init.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:52.473028 S_Taper-0.8.4.0/
+-rw-rw-rw-   0        0        0     3753 2024-04-11 09:18:52.473028 S_Taper-0.8.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3381 2024-04-11 09:17:33.000000 S_Taper-0.8.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:52.471026 S_Taper-0.8.4.0/S_Taper.egg-info/
+-rw-rw-rw-   0        0        0     3753 2024-04-11 09:18:52.000000 S_Taper-0.8.4.0/S_Taper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-11 09:18:52.000000 S_Taper-0.8.4.0/S_Taper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:18:52.000000 S_Taper-0.8.4.0/S_Taper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 09:18:52.000000 S_Taper-0.8.4.0/S_Taper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 09:18:52.000000 S_Taper-0.8.4.0/S_Taper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:52.469026 S_Taper-0.8.4.0/s_taper/
+-rw-rw-rw-   0        0        0    15531 2024-04-11 08:39:19.000000 S_Taper-0.8.4.0/s_taper/__init__.py
+-rw-rw-rw-   0        0        0    15857 2024-04-10 13:07:24.000000 S_Taper-0.8.4.0/s_taper/aio.py
+-rw-rw-rw-   0        0        0       80 2023-08-11 19:52:02.000000 S_Taper-0.8.4.0/s_taper/consts.py
+-rw-rw-rw-   0        0        0       42 2024-04-11 09:18:52.474027 S_Taper-0.8.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      654 2024-04-11 09:18:24.000000 S_Taper-0.8.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:18:52.470027 S_Taper-0.8.4.0/tests/
+-rw-rw-rw-   0        0        0     5059 2024-03-29 20:18:51.000000 S_Taper-0.8.4.0/tests/test_init.py
```

### Comparing `S_Taper-0.8.3.6/s_taper/__init__.py` & `S_Taper-0.8.4.0/s_taper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pickle
 import sqlite3
 import s_taper.consts
 import s_taper.aio
 
-
 class Taper:
     """
     Класс для работы с таблицами в базе данных SQLite.
 
     :param str table_name: Название таблицы.
     :param str file_name: Название файла базы данных SQLite.
     """
```

### Comparing `S_Taper-0.8.3.6/setup.py` & `S_Taper-0.8.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt', encoding='utf-8') as f:
 	required = f.read().splitlines()
 
 
 setuptools.setup(
 	name='S_Taper',
-	version="0.8.3.6",
+	version="0.8.4.0",
 	author="STaper_Admin",
 	description="Simple write-read add-on to SQLite3",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	install_requires=required,
 	classifiers=[
 		"Programming Language :: Python :: 3.10",
```

### Comparing `S_Taper-0.8.3.6/tests/test_init.py` & `S_Taper-0.8.4.0/tests/test_init.py`

 * *Files identical despite different names*

