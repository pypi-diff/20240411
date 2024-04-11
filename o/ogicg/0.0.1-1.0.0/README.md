# Comparing `tmp/ogicg-0.0.1.tar.gz` & `tmp/ogicg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogicg-0.0.1.tar", last modified: Thu Apr 11 00:47:07 2024, max compression
+gzip compressed data, was "ogicg-1.0.0.tar", last modified: Thu Apr 11 01:47:48 2024, max compression
```

## Comparing `ogicg-0.0.1.tar` & `ogicg-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 00:47:07.936569 ogicg-0.0.1/
--rw-rw-rw-   0        0        0     1141 2024-04-11 00:47:07.933575 ogicg-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 00:47:07.800521 ogicg-0.0.1/library/
--rw-rw-rw-   0        0        0        0 2024-04-10 21:50:52.000000 ogicg-0.0.1/library/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:47:07.805632 ogicg-0.0.1/library/app/
--rw-rw-rw-   0        0        0        0 2024-03-20 22:29:43.000000 ogicg-0.0.1/library/app/__init__.py
--rw-rw-rw-   0        0        0     5505 2024-04-10 22:40:56.000000 ogicg-0.0.1/library/app/image_processor.py
--rw-rw-rw-   0        0        0     2639 2024-04-10 22:40:56.000000 ogicg-0.0.1/library/app/input_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:47:07.830006 ogicg-0.0.1/library/models/
--rw-rw-rw-   0        0        0        0 2024-03-20 20:39:04.000000 ogicg-0.0.1/library/models/__init__.py
--rw-rw-rw-   0        0        0     1088 2024-04-06 18:59:12.000000 ogicg-0.0.1/library/models/blip_image.py
--rw-rw-rw-   0        0        0      641 2024-04-06 18:59:12.000000 ogicg-0.0.1/library/models/cohere.py
--rw-rw-rw-   0        0        0     2022 2024-04-08 21:51:30.000000 ogicg-0.0.1/library/models/easy_ocr.py
--rw-rw-rw-   0        0        0      486 2024-04-10 23:03:44.000000 ogicg-0.0.1/library/runner.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:47:07.850178 ogicg-0.0.1/library/testing/
--rw-rw-rw-   0        0        0        0 2024-02-21 18:21:23.000000 ogicg-0.0.1/library/testing/__init__.py
--rw-rw-rw-   0        0        0      620 2024-02-21 18:29:23.000000 ogicg-0.0.1/library/testing/runner.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:47:07.880611 ogicg-0.0.1/library/testing/tests/
--rw-rw-rw-   0        0        0        0 2024-02-21 18:21:32.000000 ogicg-0.0.1/library/testing/tests/__init__.py
--rw-rw-rw-   0        0        0      799 2024-04-10 22:40:56.000000 ogicg-0.0.1/library/testing/tests/test_singleton.py
--rw-rw-rw-   0        0        0      110 2024-04-10 21:51:40.000000 ogicg-0.0.1/library/testing/tests/test_user_input.py
--rw-rw-rw-   0        0        0     1687 2024-04-10 22:40:56.000000 ogicg-0.0.1/library/testing/tests/utils_test.py
--rw-rw-rw-   0        0        0     5391 2024-04-02 08:55:00.000000 ogicg-0.0.1/library/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:47:07.928566 ogicg-0.0.1/ogicg.egg-info/
--rw-rw-rw-   0        0        0     1141 2024-04-11 00:47:07.000000 ogicg-0.0.1/ogicg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      604 2024-04-11 00:47:07.000000 ogicg-0.0.1/ogicg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 00:47:07.000000 ogicg-0.0.1/ogicg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2024-04-11 00:47:07.000000 ogicg-0.0.1/ogicg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 00:47:07.000000 ogicg-0.0.1/ogicg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 00:47:07.937574 ogicg-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1416 2024-04-11 00:47:06.000000 ogicg-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:47:48.255724 ogicg-1.0.0/
+-rw-rw-rw-   0        0        0     1141 2024-04-11 01:47:48.253722 ogicg-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 01:47:48.095427 ogicg-1.0.0/library/
+-rw-rw-rw-   0        0        0        0 2024-04-10 21:50:52.000000 ogicg-1.0.0/library/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:47:48.102433 ogicg-1.0.0/library/app/
+-rw-rw-rw-   0        0        0        0 2024-03-20 22:29:43.000000 ogicg-1.0.0/library/app/__init__.py
+-rw-rw-rw-   0        0        0     5505 2024-04-10 22:40:56.000000 ogicg-1.0.0/library/app/image_processor.py
+-rw-rw-rw-   0        0        0     2639 2024-04-10 22:40:56.000000 ogicg-1.0.0/library/app/input_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:47:48.150949 ogicg-1.0.0/library/models/
+-rw-rw-rw-   0        0        0        0 2024-03-20 20:39:04.000000 ogicg-1.0.0/library/models/__init__.py
+-rw-rw-rw-   0        0        0     1088 2024-04-06 18:59:12.000000 ogicg-1.0.0/library/models/blip_image.py
+-rw-rw-rw-   0        0        0      641 2024-04-06 18:59:12.000000 ogicg-1.0.0/library/models/cohere.py
+-rw-rw-rw-   0        0        0     2022 2024-04-08 21:51:30.000000 ogicg-1.0.0/library/models/easy_ocr.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:47:48.159102 ogicg-1.0.0/library/testing/
+-rw-rw-rw-   0        0        0        0 2024-02-21 18:21:23.000000 ogicg-1.0.0/library/testing/__init__.py
+-rw-rw-rw-   0        0        0      620 2024-02-21 18:29:23.000000 ogicg-1.0.0/library/testing/runner.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:47:48.192831 ogicg-1.0.0/library/testing/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-21 18:21:32.000000 ogicg-1.0.0/library/testing/tests/__init__.py
+-rw-rw-rw-   0        0        0      799 2024-04-10 22:40:56.000000 ogicg-1.0.0/library/testing/tests/test_singleton.py
+-rw-rw-rw-   0        0        0      110 2024-04-10 21:51:40.000000 ogicg-1.0.0/library/testing/tests/test_user_input.py
+-rw-rw-rw-   0        0        0     1687 2024-04-10 22:40:56.000000 ogicg-1.0.0/library/testing/tests/utils_test.py
+-rw-rw-rw-   0        0        0     5391 2024-04-02 08:55:00.000000 ogicg-1.0.0/library/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 01:47:48.250723 ogicg-1.0.0/ogicg.egg-info/
+-rw-rw-rw-   0        0        0     1141 2024-04-11 01:47:47.000000 ogicg-1.0.0/ogicg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2024-04-11 01:47:47.000000 ogicg-1.0.0/ogicg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 01:47:47.000000 ogicg-1.0.0/ogicg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2024-04-11 01:47:47.000000 ogicg-1.0.0/ogicg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 01:47:47.000000 ogicg-1.0.0/ogicg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 01:47:48.256719 ogicg-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1416 2024-04-11 01:16:29.000000 ogicg-1.0.0/setup.py
```

### Comparing `ogicg-0.0.1/PKG-INFO` & `ogicg-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogicg
-Version: 0.0.1
+Version: 1.0.0
 Summary: An image caption generator for advertisements.
 Author: Ian King, Mason Myles, Omar Elsegeiny, Emily Anderson, & Bohdan Ivanyshyn
 Author-email: kingian404@gmail.com
 Keywords: python,image,caption,generator,image caption generator,OCR,optical character recognition,ad,ads,advertisement,advertisements,ogicg,Ovative,Ovative Group,Ovative Group Image Caption Generator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ogicg-0.0.1/library/app/image_processor.py` & `ogicg-1.0.0/library/app/image_processor.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/library/app/input_manager.py` & `ogicg-1.0.0/library/app/input_manager.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/library/models/blip_image.py` & `ogicg-1.0.0/library/models/blip_image.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/library/models/cohere.py` & `ogicg-1.0.0/library/models/cohere.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/library/models/easy_ocr.py` & `ogicg-1.0.0/library/models/easy_ocr.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/library/testing/runner.py` & `ogicg-1.0.0/library/testing/runner.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/library/testing/tests/test_singleton.py` & `ogicg-1.0.0/library/testing/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/library/testing/tests/utils_test.py` & `ogicg-1.0.0/library/testing/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/library/utils.py` & `ogicg-1.0.0/library/utils.py`

 * *Files identical despite different names*

### Comparing `ogicg-0.0.1/ogicg.egg-info/PKG-INFO` & `ogicg-1.0.0/ogicg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogicg
-Version: 0.0.1
+Version: 1.0.0
 Summary: An image caption generator for advertisements.
 Author: Ian King, Mason Myles, Omar Elsegeiny, Emily Anderson, & Bohdan Ivanyshyn
 Author-email: kingian404@gmail.com
 Keywords: python,image,caption,generator,image caption generator,OCR,optical character recognition,ad,ads,advertisement,advertisements,ogicg,Ovative,Ovative Group,Ovative Group Image Caption Generator
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ogicg-0.0.1/ogicg.egg-info/SOURCES.txt` & `ogicg-1.0.0/ogicg.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 setup.py
 library/__init__.py
-library/runner.py
 library/utils.py
 library/app/__init__.py
 library/app/image_processor.py
 library/app/input_manager.py
 library/models/__init__.py
 library/models/blip_image.py
 library/models/cohere.py
```

### Comparing `ogicg-0.0.1/setup.py` & `ogicg-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '1.0.0'
 DESCRIPTION = 'An image caption generator for advertisements.'
 LONG_DESCRIPTION = ('A package that generates captions, collects text, and saves it to a .csv file after being given '
                     'an image of an advertisement.')
 
 # Setting up
 setup(
     name='ogicg',
```

