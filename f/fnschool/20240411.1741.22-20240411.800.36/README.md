# Comparing `tmp/fnschool-20240411.1741.22.tar.gz` & `tmp/fnschool-20240411.800.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240411.1741.22.tar", last modified: Thu Apr 11 09:41:27 2024, max compression
+gzip compressed data, was "fnschool-20240411.800.36.tar", last modified: Thu Apr 11 00:00:41 2024, max compression
```

## Comparing `fnschool-20240411.1741.22.tar` & `fnschool-20240411.800.36.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.498694 fnschool-20240411.1741.22/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240411.1741.22/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)     9964 2024-04-11 09:41:27.497694 fnschool-20240411.1741.22/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240411.1741.22/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240411.1741.22/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-11 09:41:27.498694 fnschool-20240411.1741.22/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.479694 fnschool-20240411.1741.22/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.486694 fnschool-20240411.1741.22/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-11 09:41:22.000000 fnschool-20240411.1741.22/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.491694 fnschool-20240411.1741.22/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13523 2024-04-11 09:33:22.000000 fnschool-20240411.1741.22/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240411.1741.22/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/canteen/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.494694 fnschool-20240411.1741.22/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   872266 2024-04-10 23:56:57.000000 fnschool-20240411.1741.22/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240411.1741.22/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14625 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/canteen/profile.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3121 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    95794 2024-04-11 09:38:58.000000 fnschool-20240411.1741.22/src/fnschool/canteen/workbook.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.495694 fnschool-20240411.1741.22/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240411.1741.22/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1088 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      845 2024-04-11 09:33:21.000000 fnschool-20240411.1741.22/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      828 2024-04-11 09:33:21.000000 fnschool-20240411.1741.22/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.482694 fnschool-20240411.1741.22/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.481694 fnschool-20240411.1741.22/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.495694 fnschool-20240411.1741.22/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-11 09:41:22.000000 fnschool-20240411.1741.22/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.481694 fnschool-20240411.1741.22/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.495694 fnschool-20240411.1741.22/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    11306 2024-04-11 09:41:22.000000 fnschool-20240411.1741.22/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.481694 fnschool-20240411.1741.22/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.496694 fnschool-20240411.1741.22/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 09:41:22.000000 fnschool-20240411.1741.22/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.482694 fnschool-20240411.1741.22/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.496694 fnschool-20240411.1741.22/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 09:41:22.000000 fnschool-20240411.1741.22/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.482694 fnschool-20240411.1741.22/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.496694 fnschool-20240411.1741.22/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-11 09:41:22.000000 fnschool-20240411.1741.22/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1200 2024-04-11 09:33:21.000000 fnschool-20240411.1741.22/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-04-11 08:56:17.000000 fnschool-20240411.1741.22/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-11 09:41:27.497694 fnschool-20240411.1741.22/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)     9964 2024-04-11 09:41:27.000000 fnschool-20240411.1741.22/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-11 09:41:27.000000 fnschool-20240411.1741.22/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-11 09:41:27.000000 fnschool-20240411.1741.22/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-11 09:41:27.000000 fnschool-20240411.1741.22/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-11 09:41:27.000000 fnschool-20240411.1741.22/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-11 09:41:27.000000 fnschool-20240411.1741.22/src/fnschool.egg-info/top_level.txt
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

### Comparing `fnschool-20240411.1741.22/LICENSE` & `fnschool-20240411.800.36/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/PKG-INFO` & `fnschool-20240411.800.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240411.1741.22
+Version: 20240411.800.36
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240411.1741.22/pyproject.toml` & `fnschool-20240411.800.36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/bill.py` & `fnschool-20240411.800.36/src/fnschool/canteen/bill.py`

 * *Files 6% similar despite different names*

```diff
@@ -241,41 +241,28 @@
 
     @property
     def is_changsheng(self):
         return "昌盛" in self.profile.suppliers
 
     def show_msg(self):
         has_tip = False
-        print_info(
-            _("The configuration directory is: {0}").format(
-                canteen_config_fpath.parent
-            )
-        )
         if any([self.is_changsheng, self.is_xuelan]):
             has_tip = True
             print_warning(_("Hello! helping information is here for you:"))
         if self.is_changsheng:
             print_info(
                 _(
                     "Tips for Changsheng files:\n"
                     + "You need to add the residue of last year "
                     + "or last semester: Open the first "
                     + "spreadsheet you got from Changsheng, "
                     + "and add the 'residue' column, then "
                     + "insert the 'residue' foods after the end "
                     + "of entered data, the 'residue' column names "
-                    + "you could set are:\n\t{0}\n"
-                    + "The columns need to be updated are:"
-                    + "\n\t1. Inventory time: The time of residue "
-                    + "foods inventorying."
-                    + "\n\t2. The organization name or school name."
-                    + "\n\t3. The food name."
-                    + "\n\t4. The food count, fill in all count related columns if "
-                    + "there are many 'food count columns'."
-                    + "\n\t5. The total price."
+                    + "you could set are:\n\t{0}"
                 ).format(" | ".join(self.workbook.residue_col_names))
             )
 
         if self.is_xuelan:
             print_info(
                 _(
                     "If new Xuelan milks is purchased. you have to "
```

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/canteen.toml` & `fnschool-20240411.800.36/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/config.py` & `fnschool-20240411.800.36/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240411.800.36/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240411.800.36/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/food.py` & `fnschool-20240411.800.36/src/fnschool/canteen/food.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,19 +369,14 @@
             )
 
         return self.bill._foods
 
     def get_foods(self):
         if not self.bill._foods:
             self.get_purchased_foods()
-            print_info(
-                _("The directory of consuming files is: {0}").format(
-                    self.workbook.get_profile_copy_data_dpath()
-                )
-            )
             self.set_consumption_of_foods()
         return self.bill._foods
 
     def set_consumption_of_foods(self):
         self.workbook.read_consumptions_from_pre_consuming_workbooks()
         print_info(_("Consumptions were read."))
```

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/path.py` & `fnschool-20240411.800.36/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/profile.py` & `fnschool-20240411.800.36/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/test.py` & `fnschool-20240411.800.36/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool/canteen/workbook.py` & `fnschool-20240411.800.36/src/fnschool/canteen/workbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1198,14 +1198,15 @@
                     )
                     open_file_via_app0(wb_fpath)
                     _org_name_col_index = input()
                     if not _org_name_col_index.isnumeric():
                         continue
                     _org_name_col_index = int(_org_name_col_index)
 
+                print(wb_fpath)
                 _org_names = list(
                     set(
                         [
                             str(sheet.cell(ri, _org_name_col_index + 1).value)
                             for ri in range(
                                 header_row_index + 1, sheet.max_row + 1
                             )
@@ -1214,23 +1215,26 @@
                     )
                 )
 
                 if not any(
                     [o == self.bill.profile.org_name for o in _org_names]
                 ):
                     print_warning(
-                        (
-                            _('Organization name read from {0} are "{1}",')
-                            if len(_org_names) > 1
-                            else _('Organization name read from {0} is "{1}",')
-                        ).format(wb_fpath, " | ".join(_org_names))
-                        + _('But organization name of {0} is "{1}".').format(
-                            f"{self.profile.label}({self.profile.name})",
-                            self.profile.org_name,
+                        _("Organization name read from {wb_fpath}:").format(
+                            wb_fpath=wb_fpath
+                        )
+                        + " "
+                        + " | ".join(_org_names)
+                    )
+                    print_warning(
+                        _("Organization name of {profile_name}:").format(
+                            profile_name=self.profile.name
                         )
+                        + " "
+                        + self.profile.org_name
                     )
                     print_error(
                         _("'{wb_fpath}' was discarded.").format(
                             wb_fpath=wb_fpath
                         )
                     )
                     if not wb_fpath in self.excluded_purchase_sheets:
@@ -1748,37 +1752,35 @@
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
@@ -2360,30 +2362,30 @@
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

### Comparing `fnschool-20240411.1741.22/src/fnschool/entry.py` & `fnschool-20240411.800.36/src/fnschool/entry.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from fnschool import *
 
 
 def set_canteen(args):
     from fnschool.canteen.bill import Bill
 
     bill = Bill()
-    if args.action in "mk_bill":
+    if args.action in "mk_tspreadsheet":
         bill.make_spreadsheets()
     elif args.action in "help_friends":
         bill.help_friends_via_email()
 
     else:
         print_info(_("Function is not found."))
 
@@ -30,15 +30,15 @@
     )
     subparsers = parser.add_subparsers(help=_("The modules to run."))
     parser_canteen = subparsers.add_parser(
         "canteen", help=_("Canteen related functions.")
     )
     parser_canteen.add_argument(
         "action",
-        choices=["mk_bill", "help_friends"],
+        choices=["mk_tspreadsheet", "help_friends"],
         help=_("The functions of canteen."),
     )
     parser_canteen.set_defaults(func=set_canteen)
 
     args = parser.parse_args()
 
     if hasattr(args, "func"):
```

### Comparing `fnschool-20240411.1741.22/src/fnschool/external.py` & `fnschool-20240411.800.36/src/fnschool/external.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,19 +24,17 @@
         "https://gitee.com/larryw3i/funingschool/issues"
         if language_code_is_zh_CN
         else "https://github.com/larryw3i/funingschool/issues/new"
     )
 
 
 def open_file_via_app0(file_path):
-    file_path = '"' + str(file_path) + '"'
+    file_path = str(file_path)
     bin_name = (
         "xdg-open"
         if sys_is_linux()
         else "open" if sys_is_darwin() else "start"
     )
-    if sys_is_win() and file_path.endswith(".toml"):
-        bin_name = "notepad"
     os.system(bin_name + " " + file_path)
 
 
 # The end.
```

### Comparing `fnschool-20240411.1741.22/src/fnschool/language.py` & `fnschool-20240411.800.36/src/fnschool/language.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,19 +24,15 @@
     return language_code
 
 
 app_language_code = get_language_code()
 
 language_code_is_zh_CN = "zh_CN" in app_language_code
 
-T = gettext.translation(
+translations = gettext.translation(
     app_name, locale_dir, fallback=True, languages=[app_language_code]
 )
-T.install()
 
-t = T.gettext
-_ = t
-N_ = T.ngettext
-n_ = N_
-ngettext = N_
 
-# The end.
+T = translations.install()
+t = T
+_ = T
```

### Comparing `fnschool-20240411.1741.22/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240411.800.36/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-11 17:39+0800\n"
-"PO-Revision-Date: 2024-04-11 17:39+0800\n"
+"POT-Creation-Date: 2024-04-10 22:27+0800\n"
+"PO-Revision-Date: 2024-04-10 04:15+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_Hans_CN <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -18,17 +18,14 @@
 
 msgid "'{wb_fpath}' was discarded."
 msgstr "“{wb_fpath}” 已被舍去。"
 
 msgid "All food sheets have their tab colors reset."
 msgstr "所有食材台账表标签颜色已被重置。"
 
-msgid "But organization name of {0} is \"{1}\"."
-msgstr "但是 “{0}” 的 机构名（学校名）是 “{1}”。"
-
 msgid "Canteen related functions."
 msgstr "Cateen 的相关函数。"
 
 msgid "Command line interface of fnschool."
 msgstr "“fnschool“ 的命令行接口。"
 
 msgid "Configuration file '%s' was copied to '%s'."
@@ -177,22 +174,22 @@
 
 msgid "Operator name"
 msgstr "操作员姓名"
 
 msgid "Organization Name:"
 msgstr "机构名："
 
+msgid "Organization name of {profile_name}:"
+msgstr "{profile_name} 的组织名（学校名）："
+
 msgid "Organization name or school name"
 msgstr "组织名 或 学校名"
 
-msgid "Organization name read from {0} are \"{1}\","
-msgstr "从 “{0}” 中读取到的 机构名（学校名）是 “{1}”，"
-
-msgid "Organization name read from {0} is \"{1}\","
-msgstr "从 “{0}” 中读取到的 机构名（学校名）是 “{1}”，"
+msgid "Organization name read from {wb_fpath}:"
+msgstr "从 “{wb_fpath}” 中得到的 机构名（学校名）："
 
 msgid "Please add codes to get foods from your suppliers."
 msgstr "没有与这个供应商相关的解析代码，你可以添加代码。"
 
 msgid "Please design the consumptions of spreadsheet '{0}' ."
 msgstr "请给工作簿 “{0}” 设计每天的消耗。"
 
@@ -262,20 +259,14 @@
 
 msgid "Suppliers:"
 msgstr "供应商："
 
 msgid "The column names of 'negligible' mark are following:"
 msgstr "“非入库”食材的列名有以下可供选择（随意选择一个都可以被识别）："
 
-msgid "The configuration directory is: {0}"
-msgstr "配置文件所在的目录是：{0}"
-
-msgid "The directory of consuming files is: {0}"
-msgstr "出库设计文件所在的目录是：{0}"
-
 msgid "The end."
 msgstr "配置结束。"
 
 msgid "The food purchasing times of preadsheet {0} is {1} ."
 msgstr "工作簿 {0} 的食材购入时间集是 {1} 。"
 
 msgid "The functions of canteen."
@@ -298,34 +289,21 @@
 
 msgid ""
 "Tips for Changsheng files:\n"
 "You need to add the residue of last year or last semester: Open the first "
 "spreadsheet you got from Changsheng, and add the 'residue' column, then "
 "insert the 'residue' foods after the end of entered data, the 'residue' "
 "column names you could set are:\n"
-"\t{0}\n"
-"The columns need to be updated are:\n"
-"\t1. Inventory time: The time of residue foods inventorying.\n"
-"\t2. The organization name or school name.\n"
-"\t3. The food name.\n"
-"\t4. The food count, fill in all count related columns if there are many "
-"'food count columns'.\n"
-"\t5. The total price."
+"\t{0}"
 msgstr ""
 "关于 昌盛 提供的文件的小提示：\n"
 "你要把 去年 或 上个学期 的结余添加到昌盛提供的这个学期的第一个工作簿里面：打"
 "开工作簿，给工作簿添加“结余”列，然后在已有数据的后行中添加结余的所有食材，你"
 "可以输入以下之一作为列名:\n"
-"\t{0}\n"
-"盘存食材的以下信息需要被添加：\n"
-"\t1、盘存时间：食材的盘存时间。\n"
-"\t2、组织名 或 学校名。\n"
-"\t3、食材名。\n"
-"\t4、食材数量，如果您的表格有多个数量列，把所有数量列都填上。\n"
-"\t5、食材总价。"
+"\t{0}"
 
 msgid ""
 "Unable to find {0} from {1}, You can input it (1 base) directly or give "
 "feedback to the maintainers --> {2} ."
 msgstr ""
 "从 {1} 中未找到 {0} ，你可以直接输入它（以1开始）或这给项目维护人员反馈 —> "
 "{2} 。"
```

### Comparing `fnschool-20240411.1741.22/src/fnschool/path.py` & `fnschool-20240411.800.36/src/fnschool/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 
 user_name = getpass.getuser()
 
 dirs = AppDirs(app_name, app_author)
 
 app_dpath = Path(__file__).parent
 data_dpath = app_dpath / "data"
+config0_fpath = data_dpath / "config0.toml"
 user_config_dir = Path(dirs.user_config_dir)
 user_data_dir = Path(dirs.user_data_dir)
 user0_data_dir = user_data_dir / user_name
-config0_fpath = data_dpath / "config0.toml"
 config_fpath = user_config_dir / "config.toml"
 
-
 for d in [
     user_config_dir,
     user_data_dir,
     user0_data_dir,
 ]:
     if not d.exists():
         os.makedirs(d)
```

### Comparing `fnschool-20240411.1741.22/src/fnschool/test.py` & `fnschool-20240411.800.36/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240411.1741.22/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240411.800.36/src/fnschool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240411.1741.22
+Version: 20240411.800.36
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240411.1741.22/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240411.800.36/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

