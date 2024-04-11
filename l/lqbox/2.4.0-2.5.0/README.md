# Comparing `tmp/lqbox-2.4.0.tar.gz` & `tmp/lqbox-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqbox-2.4.0.tar", max compression
+gzip compressed data, was "lqbox-2.5.0.tar", max compression
```

## Comparing `lqbox-2.4.0.tar` & `lqbox-2.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1091 2024-03-20 09:46:12.799882 lqbox-2.4.0/LICENSE
--rw-r--r--   0        0        0      322 2024-04-09 01:54:42.172904 lqbox-2.4.0/pyproject.toml
--rw-r--r--   0        0        0       30 2024-03-20 09:46:12.799882 lqbox-2.4.0/README.md
--rw-r--r--   0        0        0      143 2024-03-20 09:46:12.801882 lqbox-2.4.0/src/lqbox/__init__.py
--rw-r--r--   0        0        0     2705 2024-04-09 01:53:28.324154 lqbox-2.4.0/src/lqbox/ali/__init__.py
--rw-r--r--   0        0        0     1289 2024-03-20 09:46:12.801882 lqbox-2.4.0/src/lqbox/base/__init__.py
--rw-r--r--   0        0        0      255 2024-03-20 09:46:12.802882 lqbox-2.4.0/src/lqbox/bidp/__init__.py
--rw-r--r--   0        0        0     2975 2024-03-20 09:46:12.802882 lqbox-2.4.0/src/lqbox/elihu/__init__.py
--rw-r--r--   0        0        0     1834 2024-03-20 09:46:12.802882 lqbox-2.4.0/src/lqbox/mc/__init__.py
--rw-r--r--   0        0        0     1955 2024-03-21 07:02:22.124270 lqbox-2.4.0/src/lqbox/oc/__init__.py
--rw-r--r--   0        0        0     2324 2024-03-20 09:46:12.803882 lqbox-2.4.0/src/lqbox/open_bidp/__init__.py
--rw-r--r--   0        0        0     3803 2024-03-20 09:46:12.803882 lqbox-2.4.0/src/lqbox/open_elihu/__init__.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lqbox-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-03-20 09:46:12.799882 lqbox-2.5.0/LICENSE
+-rw-r--r--   0        0        0      322 2024-04-10 08:12:57.279115 lqbox-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2024-03-20 09:46:12.799882 lqbox-2.5.0/README.md
+-rw-r--r--   0        0        0      143 2024-03-20 09:46:12.801882 lqbox-2.5.0/src/lqbox/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-09 01:53:28.324154 lqbox-2.5.0/src/lqbox/ali/__init__.py
+-rw-r--r--   0        0        0     1289 2024-03-20 09:46:12.801882 lqbox-2.5.0/src/lqbox/base/__init__.py
+-rw-r--r--   0        0        0     2970 2024-04-10 08:12:43.668992 lqbox-2.5.0/src/lqbox/bidp/__init__.py
+-rw-r--r--   0        0        0     2975 2024-03-20 09:46:12.802882 lqbox-2.5.0/src/lqbox/elihu/__init__.py
+-rw-r--r--   0        0        0     1834 2024-03-20 09:46:12.802882 lqbox-2.5.0/src/lqbox/mc/__init__.py
+-rw-r--r--   0        0        0     1955 2024-03-21 07:02:22.124270 lqbox-2.5.0/src/lqbox/oc/__init__.py
+-rw-r--r--   0        0        0     2324 2024-03-20 09:46:12.803882 lqbox-2.5.0/src/lqbox/open_bidp/__init__.py
+-rw-r--r--   0        0        0     3803 2024-03-20 09:46:12.803882 lqbox-2.5.0/src/lqbox/open_elihu/__init__.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lqbox-2.5.0/PKG-INFO
```

### Comparing `lqbox-2.4.0/LICENSE` & `lqbox-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lqbox-2.4.0/src/lqbox/ali/__init__.py` & `lqbox-2.5.0/src/lqbox/ali/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.4.0/src/lqbox/base/__init__.py` & `lqbox-2.5.0/src/lqbox/base/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.4.0/src/lqbox/elihu/__init__.py` & `lqbox-2.5.0/src/lqbox/elihu/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.4.0/src/lqbox/mc/__init__.py` & `lqbox-2.5.0/src/lqbox/mc/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.4.0/src/lqbox/oc/__init__.py` & `lqbox-2.5.0/src/lqbox/oc/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.4.0/src/lqbox/open_bidp/__init__.py` & `lqbox-2.5.0/src/lqbox/open_bidp/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.4.0/src/lqbox/open_elihu/__init__.py` & `lqbox-2.5.0/src/lqbox/open_elihu/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.4.0/PKG-INFO` & `lqbox-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqbox
-Version: 2.4.0
+Version: 2.5.0
 Summary: lqbox
 License: MIT
 Author: luke9012
 Author-email: luke781520097@163.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

