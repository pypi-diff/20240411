# Comparing `tmp/ofdcomparer-1.5.39.tar.gz` & `tmp/ofdcomparer-1.5.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofdcomparer-1.5.39.tar", last modified: Sat Apr  6 09:32:38 2024, max compression
+gzip compressed data, was "ofdcomparer-1.5.40.tar", last modified: Thu Apr 11 05:15:50 2024, max compression
```

## Comparing `ofdcomparer-1.5.39.tar` & `ofdcomparer-1.5.40.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 09:32:38.009008 ofdcomparer-1.5.39/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 13:19:58.000000 ofdcomparer-1.5.39/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-06 09:32:38.009008 ofdcomparer-1.5.39/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-01 17:56:55.000000 ofdcomparer-1.5.39/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 09:32:38.008008 ofdcomparer-1.5.39/ofdcomparer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 13:19:58.000000 ofdcomparer-1.5.39/ofdcomparer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-12 13:37:12.000000 ofdcomparer-1.5.39/ofdcomparer/allure_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    21525 2024-04-06 09:21:48.000000 ofdcomparer-1.5.39/ofdcomparer/compare_ffd.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-06 09:21:48.000000 ofdcomparer-1.5.39/ofdcomparer/configs.py
--rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-06 09:21:48.000000 ofdcomparer-1.5.39/ofdcomparer/convert.py
--rw-rw-rw-   0 root         (0) root         (0)    39765 2024-04-06 09:21:48.000000 ofdcomparer-1.5.39/ofdcomparer/dto10.py
--rw-rw-rw-   0 root         (0) root         (0)    38192 2024-04-06 09:32:23.000000 ofdcomparer-1.5.39/ofdcomparer/dto_error_descriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8301 2024-01-23 20:47:59.000000 ofdcomparer-1.5.39/ofdcomparer/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1563 2024-01-12 13:37:12.000000 ofdcomparer-1.5.39/ofdcomparer/ofd_cri_atol.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-12 14:45:58.000000 ofdcomparer-1.5.39/ofdcomparer/ofd_taxcom.py
--rw-rw-rw-   0 root         (0) root         (0)    39179 2024-01-23 20:47:59.000000 ofdcomparer-1.5.39/ofdcomparer/tags_fn.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2024-03-09 15:40:06.000000 ofdcomparer-1.5.39/ofdcomparer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 09:32:38.009008 ofdcomparer-1.5.39/ofdcomparer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-06 09:32:37.000000 ofdcomparer-1.5.39/ofdcomparer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2024-04-06 09:32:37.000000 ofdcomparer-1.5.39/ofdcomparer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 09:32:37.000000 ofdcomparer-1.5.39/ofdcomparer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-06 09:32:37.000000 ofdcomparer-1.5.39/ofdcomparer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 09:32:37.000000 ofdcomparer-1.5.39/ofdcomparer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-06 09:32:38.010007 ofdcomparer-1.5.39/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-06 09:32:23.000000 ofdcomparer-1.5.39/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:15:50.710245 ofdcomparer-1.5.40/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-20 08:16:51.000000 ofdcomparer-1.5.40/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-11 05:15:50.711245 ofdcomparer-1.5.40/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-06 21:06:45.000000 ofdcomparer-1.5.40/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:15:50.709245 ofdcomparer-1.5.40/ofdcomparer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-20 08:16:51.000000 ofdcomparer-1.5.40/ofdcomparer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-12 07:39:03.000000 ofdcomparer-1.5.40/ofdcomparer/allure_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    21525 2024-04-11 05:15:32.000000 ofdcomparer-1.5.40/ofdcomparer/compare_ffd.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-11 05:15:32.000000 ofdcomparer-1.5.40/ofdcomparer/configs.py
+-rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-11 05:15:32.000000 ofdcomparer-1.5.40/ofdcomparer/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    39765 2024-04-11 05:15:32.000000 ofdcomparer-1.5.40/ofdcomparer/dto10.py
+-rw-rw-rw-   0 root         (0) root         (0)    38192 2024-04-11 05:15:32.000000 ofdcomparer-1.5.40/ofdcomparer/dto_error_descriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8301 2024-01-25 10:39:56.000000 ofdcomparer-1.5.40/ofdcomparer/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2024-01-12 13:52:59.000000 ofdcomparer-1.5.40/ofdcomparer/ofd_cri_atol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-12 14:13:15.000000 ofdcomparer-1.5.40/ofdcomparer/ofd_taxcom.py
+-rw-rw-rw-   0 root         (0) root         (0)    40219 2024-04-11 05:15:32.000000 ofdcomparer-1.5.40/ofdcomparer/tags_fn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-11 05:15:32.000000 ofdcomparer-1.5.40/ofdcomparer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 05:15:50.710245 ofdcomparer-1.5.40/ofdcomparer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-11 05:15:50.000000 ofdcomparer-1.5.40/ofdcomparer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2024-04-11 05:15:50.000000 ofdcomparer-1.5.40/ofdcomparer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 05:15:50.000000 ofdcomparer-1.5.40/ofdcomparer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-11 05:15:50.000000 ofdcomparer-1.5.40/ofdcomparer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-11 05:15:50.000000 ofdcomparer-1.5.40/ofdcomparer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-11 05:15:50.711245 ofdcomparer-1.5.40/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-11 05:15:32.000000 ofdcomparer-1.5.40/setup.py
```

### Comparing `ofdcomparer-1.5.39/PKG-INFO` & `ofdcomparer-1.5.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.39
+Version: 1.5.40
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.39/README.md` & `ofdcomparer-1.5.40/README.md`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer/compare_ffd.py` & `ofdcomparer-1.5.40/ofdcomparer/compare_ffd.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer/convert.py` & `ofdcomparer-1.5.40/ofdcomparer/convert.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer/dto10.py` & `ofdcomparer-1.5.40/ofdcomparer/dto10.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer/dto_error_descriptions.py` & `ofdcomparer-1.5.40/ofdcomparer/dto_error_descriptions.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer/helpers.py` & `ofdcomparer-1.5.40/ofdcomparer/helpers.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer/ofd_cri_atol.py` & `ofdcomparer-1.5.40/ofdcomparer/ofd_cri_atol.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer/ofd_taxcom.py` & `ofdcomparer-1.5.40/ofdcomparer/ofd_taxcom.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer/tags_fn.py` & `ofdcomparer-1.5.40/ofdcomparer/tags_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -872,14 +872,28 @@
         "Name": "мера количества предмета расчета",
     },
     "2110": {
         "Type": BYTE,
         "Head": "",
         "Name": "присвоенный статус товара",
     },
+    "2112": {
+        "Type": BITS,
+        "Head": "",
+        "Name": "признак некорректных кодов маркировки",
+        "BIT1": "в течение смены или между сменами поступил ответ на запрос, содержащий сведения о некорректном КМ",
+        "BIT2": "в течение смены или между сменами поступила квитанция на уведомление, содержащая сведения о некорректном КМ"
+    },
+    "2113": {
+        "Type": BITS,
+        "Head": "",
+        "Name": "признак некорректных запросов и уведомлений",
+        "BIT0": "отрицательный результат обработки запроса о коде маркировки",
+        "BIT1": "отрицательный результат обработки уведомления о реализации маркированного товара"
+    },
     "2115": {
         "Type": STRING,
         "Head": "",
         "Name": "код идентификации вида товара",
     },
     "2117": {
         "Type": COINS,
```

### Comparing `ofdcomparer-1.5.39/ofdcomparer/utils.py` & `ofdcomparer-1.5.40/ofdcomparer/utils.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/ofdcomparer.egg-info/PKG-INFO` & `ofdcomparer-1.5.40/ofdcomparer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.39
+Version: 1.5.40
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.39/ofdcomparer.egg-info/SOURCES.txt` & `ofdcomparer-1.5.40/ofdcomparer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.39/setup.py` & `ofdcomparer-1.5.40/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ofdcomparer",
-    version="1.5.39",
+    version="1.5.40",
     long_description=long_description,
     description="Библиотека для сравнивания ФД из ФН и ОФД",
     packages=["ofdcomparer"],
     author_email="k.kabisova@atol.ru",
     install_requires=[
         "requests==2.31.0",
         "requests-toolbelt==1.0.0",
```

