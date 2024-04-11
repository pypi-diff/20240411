# Comparing `tmp/telegram_collector-0.2.0.tar.gz` & `tmp/telegram_collector-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.2.0.tar", last modified: Thu Apr 11 13:58:24 2024, max compression
+gzip compressed data, was "telegram_collector-0.2.1.tar", last modified: Thu Apr 11 14:24:27 2024, max compression
```

## Comparing `telegram_collector-0.2.0.tar` & `telegram_collector-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 13:58:24.054205 telegram_collector-0.2.0/
--rw-rw-rw-   0        0        0      287 2024-04-11 13:58:24.052765 telegram_collector-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-10 05:47:49.000000 telegram_collector-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 13:58:24.054205 telegram_collector-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-11 13:58:19.000000 telegram_collector-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:58:24.041620 telegram_collector-0.2.0/telegram_collector/
--rw-rw-rw-   0        0        0     4705 2024-04-10 06:24:09.000000 telegram_collector-0.2.0/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0     1982 2024-04-10 06:24:09.000000 telegram_collector-0.2.0/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2542 2024-04-10 05:53:36.000000 telegram_collector-0.2.0/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:58:24.051661 telegram_collector-0.2.0/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-11 13:58:23.000000 telegram_collector-0.2.0/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:24:27.570630 telegram_collector-0.2.1/
+-rw-rw-rw-   0        0        0      287 2024-04-11 14:24:27.569201 telegram_collector-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-11 14:11:58.000000 telegram_collector-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:24:27.570630 telegram_collector-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-11 14:24:01.000000 telegram_collector-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:24:27.559224 telegram_collector-0.2.1/telegram_collector/
+-rw-rw-rw-   0        0        0     4771 2024-04-11 14:24:01.000000 telegram_collector-0.2.1/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0     1961 2024-04-11 14:22:26.000000 telegram_collector-0.2.1/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2542 2024-04-10 05:53:36.000000 telegram_collector-0.2.1/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:24:27.569201 telegram_collector-0.2.1/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-11 14:24:27.000000 telegram_collector-0.2.1/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-11 14:24:27.000000 telegram_collector-0.2.1/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:24:27.000000 telegram_collector-0.2.1/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-11 14:24:27.000000 telegram_collector-0.2.1/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-11 14:24:27.000000 telegram_collector-0.2.1/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-11 14:24:27.000000 telegram_collector-0.2.1/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.2.0/setup.py` & `telegram_collector-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.2.0',
+    version='0.2.1',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks'],
     entry_points={
```

### Comparing `telegram_collector-0.2.0/telegram_collector/__init__.py` & `telegram_collector-0.2.1/telegram_collector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,8 +126,11 @@
     def send_new_message_src_to_dest(self):
         asyncio.run(self.__do_after_init(self.__send_new_message_src_to_dest))
 
     def send_history_message_src_to_dest(self):
         asyncio.run(self.__do_after_init(self.__send_history_message_src_to_dest))
 
     def print_my_dialogs(self):
-        asyncio.run(self.__do_after_init(print_dialogs))
+        def wrapper():
+            print_dialogs(self.my_dialogs)
+
+        asyncio.run(self.__do_after_init(wrapper()))
```

### Comparing `telegram_collector-0.2.0/telegram_collector/__main__.py` & `telegram_collector-0.2.1/telegram_collector/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import getopt
 import sys
 
 from .__init__ import *
 import configparser
-import python_socks
 
 
 def new_telegram_collector():
     tc = TelegramCollector()
     config_file = 'tg.ini'
     parser = configparser.ConfigParser()
     parser.read(config_file)
```

### Comparing `telegram_collector-0.2.0/telegram_collector/util.py` & `telegram_collector-0.2.1/telegram_collector/util.py`

 * *Files identical despite different names*

