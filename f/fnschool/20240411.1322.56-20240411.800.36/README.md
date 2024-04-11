# Comparing `tmp/fnschool-20240411.1322.56.tar.gz` & `tmp/fnschool-20240411.800.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240411.1322.56.tar", last modified: Thu Apr 11 05:23:01 2024, max compression
+gzip compressed data, was "fnschool-20240411.800.36.tar", last modified: Thu Apr 11 00:00:41 2024, max compression
```

## Comparing `fnschool-20240411.1322.56.tar` & `fnschool-20240411.800.36.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.421732 fnschool-20240411.1322.56/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240411.1322.56/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)     9964 2024-04-11 05:23:01.421732 fnschool-20240411.1322.56/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240411.1322.56/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240411.1322.56/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-11 05:23:01.421732 fnschool-20240411.1322.56/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.405732 fnschool-20240411.1322.56/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.411732 fnschool-20240411.1322.56/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-11 05:22:56.000000 fnschool-20240411.1322.56/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-09 16:59:34.000000 fnschool-20240411.1322.56/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.415732 fnschool-20240411.1322.56/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    12891 2024-04-10 23:46:22.000000 fnschool-20240411.1322.56/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240411.1322.56/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/canteen/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.418732 fnschool-20240411.1322.56/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   872266 2024-04-10 23:56:57.000000 fnschool-20240411.1322.56/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240411.1322.56/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14435 2024-04-10 23:58:08.000000 fnschool-20240411.1322.56/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/canteen/profile.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3121 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    95819 2024-04-11 02:59:51.000000 fnschool-20240411.1322.56/src/fnschool/canteen/workbook.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.418732 fnschool-20240411.1322.56/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240411.1322.56/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1104 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      751 2024-04-10 23:46:21.000000 fnschool-20240411.1322.56/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      797 2024-04-09 16:57:51.000000 fnschool-20240411.1322.56/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.407732 fnschool-20240411.1322.56/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.406732 fnschool-20240411.1322.56/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.418732 fnschool-20240411.1322.56/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-11 05:22:56.000000 fnschool-20240411.1322.56/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.406732 fnschool-20240411.1322.56/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.419732 fnschool-20240411.1322.56/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    10434 2024-04-11 05:22:56.000000 fnschool-20240411.1322.56/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.407732 fnschool-20240411.1322.56/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.419732 fnschool-20240411.1322.56/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 05:22:56.000000 fnschool-20240411.1322.56/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.407732 fnschool-20240411.1322.56/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.419732 fnschool-20240411.1322.56/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 05:22:56.000000 fnschool-20240411.1322.56/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.407732 fnschool-20240411.1322.56/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.420732 fnschool-20240411.1322.56/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 05:22:56.000000 fnschool-20240411.1322.56/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1199 2024-04-10 23:46:22.000000 fnschool-20240411.1322.56/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-03-29 06:17:35.000000 fnschool-20240411.1322.56/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 05:23:01.420732 fnschool-20240411.1322.56/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)     9964 2024-04-11 05:23:01.000000 fnschool-20240411.1322.56/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-11 05:23:01.000000 fnschool-20240411.1322.56/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-11 05:23:01.000000 fnschool-20240411.1322.56/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-11 05:23:01.000000 fnschool-20240411.1322.56/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-11 05:23:01.000000 fnschool-20240411.1322.56/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-11 05:23:01.000000 fnschool-20240411.1322.56/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.492302 fnschool-20240411.800.36/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240411.800.36/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)     9963 2024-04-11 00:00:41.492302 fnschool-20240411.800.36/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240411.800.36/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240411.800.36/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-11 00:00:41.492302 fnschool-20240411.800.36/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.474308 fnschool-20240411.800.36/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.480306 fnschool-20240411.800.36/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-11 00:00:36.000000 fnschool-20240411.800.36/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-09 16:59:34.000000 fnschool-20240411.800.36/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.485304 fnschool-20240411.800.36/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    12891 2024-04-10 23:46:22.000000 fnschool-20240411.800.36/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240411.800.36/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/canteen/config.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.487304 fnschool-20240411.800.36/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   872266 2024-04-10 23:56:57.000000 fnschool-20240411.800.36/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240411.800.36/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14435 2024-04-10 23:58:08.000000 fnschool-20240411.800.36/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/canteen/profile.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3121 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    95812 2024-04-10 23:57:41.000000 fnschool-20240411.800.36/src/fnschool/canteen/workbook.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.489303 fnschool-20240411.800.36/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240411.800.36/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1104 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      751 2024-04-10 23:46:21.000000 fnschool-20240411.800.36/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      797 2024-04-09 16:57:51.000000 fnschool-20240411.800.36/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.477307 fnschool-20240411.800.36/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.475308 fnschool-20240411.800.36/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.489303 fnschool-20240411.800.36/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-11 00:00:36.000000 fnschool-20240411.800.36/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.476307 fnschool-20240411.800.36/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.490303 fnschool-20240411.800.36/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10434 2024-04-11 00:00:36.000000 fnschool-20240411.800.36/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.476307 fnschool-20240411.800.36/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.490303 fnschool-20240411.800.36/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 00:00:36.000000 fnschool-20240411.800.36/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.476307 fnschool-20240411.800.36/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.490303 fnschool-20240411.800.36/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 00:00:36.000000 fnschool-20240411.800.36/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.477307 fnschool-20240411.800.36/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.491302 fnschool-20240411.800.36/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 00:00:36.000000 fnschool-20240411.800.36/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1199 2024-04-10 23:46:22.000000 fnschool-20240411.800.36/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-03-29 06:17:35.000000 fnschool-20240411.800.36/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 00:00:41.491302 fnschool-20240411.800.36/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)     9963 2024-04-11 00:00:41.000000 fnschool-20240411.800.36/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-11 00:00:41.000000 fnschool-20240411.800.36/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-11 00:00:41.000000 fnschool-20240411.800.36/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-11 00:00:41.000000 fnschool-20240411.800.36/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-11 00:00:41.000000 fnschool-20240411.800.36/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-11 00:00:41.000000 fnschool-20240411.800.36/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240411.1322.56/LICENSE` & `fnschool-20240411.800.36/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/PKG-INFO` & `fnschool-20240411.800.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240411.1322.56
+Version: 20240411.800.36
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240411.1322.56/pyproject.toml` & `fnschool-20240411.800.36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/bill.py` & `fnschool-20240411.800.36/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/canteen.toml` & `fnschool-20240411.800.36/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/config.py` & `fnschool-20240411.800.36/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240411.800.36/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240411.800.36/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/food.py` & `fnschool-20240411.800.36/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/path.py` & `fnschool-20240411.800.36/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/profile.py` & `fnschool-20240411.800.36/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/test.py` & `fnschool-20240411.800.36/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/canteen/workbook.py` & `fnschool-20240411.800.36/src/fnschool/canteen/workbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1752,37 +1752,35 @@
             tfoods_len = len(tfoods)
             consuming_n = day_index + 1
             csheet.cell(form_index0, 2, self.bill.profile.org_name)
             csheet.cell(
                 form_index0,
                 4,
                 f"{day.year}年 {day.month} 月 {day.day} 日  " + f"单位：元",
-            )
 
             csheet.cell(
                 form_index0,
                 7,
                 f"编号：C{day.month:0>2}{consuming_n:0>2}",
             )
-
             csheet.cell(
-                form_index1 + 2,
+                form_index1+2,
                 1,
                 (
                     "   "
                     + "审核人："
                     + "        "
                     + "经办人："
-                    + "　    "
+                    + "　    " 
                     + "过称人："
                     + self.bill.profile.name
                     + "      "
                     + "仓管人："
                     + " 　"
-                ),
+                )
             )
 
             row_difference = (
                 tfoods_len + len(classes_without_food) - food_index_len
             )
 
             if row_difference > 0:
@@ -2364,30 +2362,30 @@
                 + f"{time_point.day} 日  单位：元",
             )
             wsheet.cell(
                 form_index0,
                 7,
                 f"编号：R{time_point.month:0>2}{warehousing_n:0>2}",
             )
-
+            
             wsheet.cell(
-                form_index1 + 1,
+                form_index1+1,
                 1,
                 (
                     "   "
-                    + "审核人："
+                    + "审核人：" 
                     + "        "
                     + "经办人："
                     + self.bill.profile.name
                     + " 　    "
-                    + "过称人："
+                    + "过称人：" 
                     + "        "
-                    + "仓管人："
+                    + "仓管人：
                     + " 　"
-                ),
+                )
             )
 
             for class_name in class_names:
                 cfoods = [f for f in wfoods if f.class_name == class_name]
                 cfoods_total_price = sum([f.total_price for f in cfoods])
 
                 wsheet.cell(entry_index, 1, class_name)
```

### Comparing `fnschool-20240411.1322.56/src/fnschool/entry.py` & `fnschool-20240411.800.36/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/external.py` & `fnschool-20240411.800.36/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/language.py` & `fnschool-20240411.800.36/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240411.800.36/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/path.py` & `fnschool-20240411.800.36/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool/test.py` & `fnschool-20240411.800.36/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1322.56/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240411.800.36/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240411.1322.56
+Version: 20240411.800.36
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240411.1322.56/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240411.800.36/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

