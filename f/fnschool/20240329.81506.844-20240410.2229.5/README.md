# Comparing `tmp/fnschool-20240329.81506.844.tar.gz` & `tmp/fnschool-20240410.2229.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240329.81506.844.tar", last modified: Fri Mar 29 07:06:48 2024, max compression
+gzip compressed data, was "fnschool-20240410.2229.5.tar", last modified: Wed Apr 10 14:29:09 2024, max compression
```

## Comparing `fnschool-20240329.81506.844.tar` & `fnschool-20240410.2229.5.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240329.81506.844/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)     9966 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240329.81506.844/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240329.81506.844/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.932251 fnschool-20240329.81506.844/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.936251 fnschool-20240329.81506.844/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      235 2024-03-29 07:06:44.000000 fnschool-20240329.81506.844/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/__main__.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.944251 fnschool-20240329.81506.844/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    12592 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240329.81506.844/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/canteen/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.944251 fnschool-20240329.81506.844/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   872376 2024-03-13 06:03:46.000000 fnschool-20240329.81506.844/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240329.81506.844/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14422 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/canteen/profile.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3121 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    91431 2024-03-29 07:02:16.000000 fnschool-20240329.81506.844/src/fnschool/canteen/workbook.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240329.81506.844/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1104 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      767 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      919 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.932251 fnschool-20240329.81506.844/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.932251 fnschool-20240329.81506.844/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-03-29 07:06:44.000000 fnschool-20240329.81506.844/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.932251 fnschool-20240329.81506.844/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)     9882 2024-03-29 07:06:44.000000 fnschool-20240329.81506.844/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.932251 fnschool-20240329.81506.844/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-03-29 07:06:44.000000 fnschool-20240329.81506.844/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.932251 fnschool-20240329.81506.844/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-03-29 07:06:44.000000 fnschool-20240329.81506.844/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.932251 fnschool-20240329.81506.844/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-03-29 07:06:44.000000 fnschool-20240329.81506.844/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1361 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-03-29 06:17:35.000000 fnschool-20240329.81506.844/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-03-29 07:06:48.948251 fnschool-20240329.81506.844/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)     9966 2024-03-29 07:06:48.000000 fnschool-20240329.81506.844/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     1109 2024-03-29 07:06:48.000000 fnschool-20240329.81506.844/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-03-29 07:06:48.000000 fnschool-20240329.81506.844/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-03-29 07:06:48.000000 fnschool-20240329.81506.844/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-03-29 07:06:48.000000 fnschool-20240329.81506.844/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-03-29 07:06:48.000000 fnschool-20240329.81506.844/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.586207 fnschool-20240410.2229.5/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240410.2229.5/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)     9963 2024-04-10 14:29:09.586207 fnschool-20240410.2229.5/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240410.2229.5/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240410.2229.5/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-10 14:29:09.587207 fnschool-20240410.2229.5/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.570207 fnschool-20240410.2229.5/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.576207 fnschool-20240410.2229.5/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-10 14:29:05.000000 fnschool-20240410.2229.5/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-09 16:59:34.000000 fnschool-20240410.2229.5/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.581207 fnschool-20240410.2229.5/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    12592 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240410.2229.5/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/canteen/config.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.583207 fnschool-20240410.2229.5/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   872376 2024-03-13 06:03:46.000000 fnschool-20240410.2229.5/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240410.2229.5/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14422 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/canteen/profile.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3121 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    94307 2024-04-10 14:20:58.000000 fnschool-20240410.2229.5/src/fnschool/canteen/workbook.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.583207 fnschool-20240410.2229.5/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240410.2229.5/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1104 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      767 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      797 2024-04-09 16:57:51.000000 fnschool-20240410.2229.5/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.573207 fnschool-20240410.2229.5/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.571207 fnschool-20240410.2229.5/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.584207 fnschool-20240410.2229.5/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-10 14:29:04.000000 fnschool-20240410.2229.5/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.572207 fnschool-20240410.2229.5/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.584207 fnschool-20240410.2229.5/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10434 2024-04-10 14:29:04.000000 fnschool-20240410.2229.5/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.572207 fnschool-20240410.2229.5/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.584207 fnschool-20240410.2229.5/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-10 14:29:04.000000 fnschool-20240410.2229.5/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.572207 fnschool-20240410.2229.5/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.585207 fnschool-20240410.2229.5/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-10 14:29:04.000000 fnschool-20240410.2229.5/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.573207 fnschool-20240410.2229.5/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.585207 fnschool-20240410.2229.5/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-10 14:29:04.000000 fnschool-20240410.2229.5/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1215 2024-04-09 16:55:08.000000 fnschool-20240410.2229.5/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-03-29 06:17:35.000000 fnschool-20240410.2229.5/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-10 14:29:09.585207 fnschool-20240410.2229.5/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)     9963 2024-04-10 14:29:09.000000 fnschool-20240410.2229.5/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-10 14:29:09.000000 fnschool-20240410.2229.5/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-10 14:29:09.000000 fnschool-20240410.2229.5/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-10 14:29:09.000000 fnschool-20240410.2229.5/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-10 14:29:09.000000 fnschool-20240410.2229.5/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-10 14:29:09.000000 fnschool-20240410.2229.5/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240329.81506.844/LICENSE` & `fnschool-20240410.2229.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/PKG-INFO` & `fnschool-20240410.2229.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240329.81506.844
+Version: 20240410.2229.5
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240329.81506.844/pyproject.toml` & `fnschool-20240410.2229.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/bill.py` & `fnschool-20240410.2229.5/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/canteen.toml` & `fnschool-20240410.2229.5/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/config.py` & `fnschool-20240410.2229.5/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240410.2229.5/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240410.2229.5/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/food.py` & `fnschool-20240410.2229.5/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/path.py` & `fnschool-20240410.2229.5/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/profile.py` & `fnschool-20240410.2229.5/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/test.py` & `fnschool-20240410.2229.5/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/canteen/workbook.py` & `fnschool-20240410.2229.5/src/fnschool/canteen/workbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.pre_consuming_sheet0_name = "出库计划表"
         self._recounts = None
         self.food_name_col_names = ["商品名称", "食材名称", "商品名", "食材名"]
         self.purchase_sheet_names = ["客户商品销售报表", "客户送货明细报表"]
         self.negligible_col_names = ["忽略", "不计", "非入库", "可忽略", "非盘点"]
         self.residue_col_names = ["上季结余", "是剩余", "是结余", "上年结余", "剩余", "结余"]
         self.org_col_names = ["客户名称"]
-        self.total_price_col_names = ["金额", "折前金额", "总价"]
+        self.total_price_col_names = ["金额", "折前金额", "总价", "折后金额"]
         self.count_col_names = ["数量", "记账数量", "订货数量", "订货总量", "订货总数量"]
         self.unit_name_col_names = ["单位", "订货单位"]
         self.check_date_col_names = ["送货日期", "送货时间"]
         self.warehousing_form_index_offset = 0
         self.inventory_form_index_offset = 1
         self.bill_workbook = None
         self.pre_consuming_workbook0 = None
@@ -1022,15 +1022,15 @@
                     and not f.is_negligible
                 )
             ]
             if len(_foods) < 1:
                 print_warning(
                     _(
                         "There is not food of time node %s ,skip workbook designing."
-                    )
+                    ) % (t0.strftime("%Y.%m.%d")+t1.strftime("%Y.%m.%d"))
                 )
                 continue
 
             if not sheet.cell(1, col_index_offset).value:
                 for i, t in enumerate(
                     [
                         t0 + timedelta(days=a)
@@ -1128,30 +1128,92 @@
 
             self.purchase_workbook_fdpath = dpath
         print_info(_("Entered directory: %s") % dpath)
 
         for file in os.listdir(dpath):
             if file.split(".")[-1] in self.spreadsheet_ext_names:
                 wb_fpath = (Path(dpath) / file).as_posix()
+                if wb_fpath in self.excluded_purchase_sheets:
+                    continue
                 wb = load_workbook(wb_fpath, read_only=True)
                 sheetnames = [
                     n for n in wb.sheetnames if n in self.purchase_sheet_names
                 ]
                 if len(sheetnames) < 1:
+                    if not wb_fpath in self.excluded_purchase_sheets:
+                        self.excluded_purchase_sheets.append(wb_fpath)
                     continue
                 sheet = wb[sheetnames[0]]
 
+                header_row_index = 1
+                header_names = [
+                    str(sheet.cell(header_row_index, ci).value)
+                    for ci in range(1, sheet.max_column + 1)
+                ]
+
+                _org_name_col_index = -1
+
+                for hn in header_names:
+                    if hn in self.org_col_names:
+                        _org_name_col_index = header_names.index(hn)
+
+                if _org_name_col_index < 0:
+                    print_warning(
+                        _(
+                            "{app_name} desn't pick the index of organization name"
+                            + " column, input it (0 base) or '{wb_fpath}' will be ignored."
+                        ).format(app_name=app_name, wb_fpath=wb_fpath)
+                    )
+                    open_file_via_app0(wb_fpath)
+                    _org_name_col_index = input()
+                    if not _org_name_col_index.isnumeric():
+                        continue
+                    _org_name_col_index = int(_org_name_col_index)
+                
+                print(wb_fpath)
+                _org_names = list(
+                    set(
+                        [
+                            str(sheet.cell(ri, _org_name_col_index + 1).value)
+                            for ri in range(
+                                header_row_index + 1, sheet.max_row + 1
+                            )
+                            if sheet.cell(ri, _org_name_col_index + 1).value
+                        ]
+                    )
+                )
+
                 if not any(
-                    [
-                        (
-                            str(sheet.cell(1, ci).value)
-                            in self.negligible_col_names
+                    [o == self.bill.profile.org_name for o in _org_names]
+                ):
+                    print_warning(
+                        _("Organization name read from {wb_fpath}:").format(
+                            wb_fpath=wb_fpath
                         )
-                        for ci in range(1, sheet.max_column + 1)
-                    ]
+                        + " "
+                        + " | ".join(_org_names)
+                    )
+                    print_warning(
+                        _("Organization name of {profile_name}:").format(
+                            profile_name=self.profile.name
+                        )
+                        + " "
+                        + self.profile.org_name
+                    )
+                    print_error(
+                        _("'{wb_fpath}' was discarded.").format(
+                            wb_fpath=wb_fpath
+                        )
+                    )
+                    if not wb_fpath in self.excluded_purchase_sheets:
+                        self.excluded_purchase_sheets.append(wb_fpath)
+                    continue
+
+                if not any(
+                    [(h in self.negligible_col_names) for h in header_names]
                 ):
                     print_info(
                         _(
                             "It seems you didn't set the 'negligible' mark "
                             + "for workbook '{0}' , update this workbook "
                             + "and press ANY key to continue. (Add the "
                             + "'negligible' column name even though there "
@@ -1198,14 +1260,16 @@
                             datetime.strptime(check_date, "%Y-%m-%d")
                             if "-" in check_date
                             else datetime.strptime(check_date, "%Y%d%m")
                         )
                         org_name = row[food_org_name_index].value
 
                         if org_name != self.bill.profile.org_name:
+                            if not wb_fpath in self.excluded_purchase_sheets:
+                                self.excluded_purchase_sheets.append(wb_fpath)
                             continue
 
                         name = row[food_name_index].value
                         count = row[food_count_index].value
                         if isinstance(count, str):
                             count = float(self.clean_quotation_marks(count))
                         unit = row[food_unit_index].value
```

### Comparing `fnschool-20240329.81506.844/src/fnschool/entry.py` & `fnschool-20240410.2229.5/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/external.py` & `fnschool-20240410.2229.5/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool/language.py` & `fnschool-20240410.2229.5/src/fnschool/language.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import os
 import sys
 import gettext
 import locale
 from pathlib import Path
+from fnschool.app import *
 
-app_name = Path(__file__).parent.as_posix()
-app_name = (
-    app_name.split(os.sep)[-1]
-    if os.sep in app_name
-    else app_name.split("/")[-1]
-)
 locale_dir = (Path(__file__).parent / "locales").as_posix()
 
 
 def get_language_code():
     locale.setlocale(locale.LC_ALL, "")
     language_code = (
         locale.getdefaultlocale()[0]
```

### Comparing `fnschool-20240329.81506.844/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240410.2229.5/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,25 +1,28 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-03-29 11:41+0800\n"
-"PO-Revision-Date: 2024-03-29 11:49+0800\n"
+"POT-Creation-Date: 2024-04-10 22:27+0800\n"
+"PO-Revision-Date: 2024-04-10 04:15+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_Hans_CN <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.14.0\n"
 
 msgid "%s can't change."
 msgstr "%s 无法转换。"
 
+msgid "'{wb_fpath}' was discarded."
+msgstr "“{wb_fpath}” 已被舍去。"
+
 msgid "All food sheets have their tab colors reset."
 msgstr "所有食材台账表标签颜色已被重置。"
 
 msgid "Canteen related functions."
 msgstr "Cateen 的相关函数。"
 
 msgid "Command line interface of fnschool."
@@ -171,17 +174,23 @@
 
 msgid "Operator name"
 msgstr "操作员姓名"
 
 msgid "Organization Name:"
 msgstr "机构名："
 
+msgid "Organization name of {profile_name}:"
+msgstr "{profile_name} 的组织名（学校名）："
+
 msgid "Organization name or school name"
 msgstr "组织名 或 学校名"
 
+msgid "Organization name read from {wb_fpath}:"
+msgstr "从 “{wb_fpath}” 中得到的 机构名（学校名）："
+
 msgid "Please add codes to get foods from your suppliers."
 msgstr "没有与这个供应商相关的解析代码，你可以添加代码。"
 
 msgid "Please design the consumptions of spreadsheet '{0}' ."
 msgstr "请给工作簿 “{0}” 设计每天的消耗。"
 
 msgid ""
@@ -335,7 +344,14 @@
 msgstr "行 “%s” 被舍去。"
 
 msgid "values length is less than %s."
 msgstr "值的长度小于 %s 。"
 
 msgid "{0}.{1}.{2}--{3}.{4}.{5}"
 msgstr "{0}年{1}月{2}日——{3}年{4}月{5}日"
+
+msgid ""
+"{app_name} desn't pick the index of organization name column, input it (0 "
+"base) or '{wb_fpath}' will be ignored."
+msgstr ""
+"{app_name} 找不到机构名（学校名）列的索引，您可以直接输入索引，否则 "
+"“{wb_fpath}” 会被忽略。"
```

### Comparing `fnschool-20240329.81506.844/src/fnschool/path.py` & `fnschool-20240410.2229.5/src/fnschool/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,17 @@
 import shutil
 import getpass
 import platform
 import subprocess
 
 from appdirs import AppDirs
 from fnschool.log import *
+from fnschool.app import *
 
-app_name = Path(__file__).parent.as_posix()
-app_name = (
-    app_name.split(os.sep)[-1]
-    if os.sep in app_name
-    else app_name.split("/")[-1]
-)
 
-app_author = "larryw3i"
 user_name = getpass.getuser()
 
 dirs = AppDirs(app_name, app_author)
 
 app_dpath = Path(__file__).parent
 data_dpath = app_dpath / "data"
 config0_fpath = data_dpath / "config0.toml"
```

### Comparing `fnschool-20240329.81506.844/src/fnschool/test.py` & `fnschool-20240410.2229.5/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240329.81506.844/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240410.2229.5/src/fnschool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240329.81506.844
+Version: 20240410.2229.5
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240329.81506.844/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240410.2229.5/src/fnschool.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 src/fnschool/__init__.py
 src/fnschool/__main__.py
+src/fnschool/app.py
 src/fnschool/entry.py
 src/fnschool/external.py
 src/fnschool/language.py
 src/fnschool/log.py
 src/fnschool/path.py
 src/fnschool/test.py
 src/fnschool.egg-info/PKG-INFO
```

