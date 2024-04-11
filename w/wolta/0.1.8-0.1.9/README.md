# Comparing `tmp/wolta-0.1.8.tar.gz` & `tmp/wolta-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.1.8.tar", last modified: Wed Apr 10 00:51:45 2024, max compression
+gzip compressed data, was "wolta-0.1.9.tar", last modified: Thu Apr 11 11:06:16 2024, max compression
```

## Comparing `wolta-0.1.8.tar` & `wolta-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 00:51:45.072917 wolta-0.1.8/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0    17575 2024-04-10 00:51:45.072917 wolta-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    16268 2024-04-10 00:49:00.000000 wolta-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 00:51:45.073954 wolta-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1209 2024-04-10 00:51:27.000000 wolta-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 00:51:45.022791 wolta-0.1.8/wolta/
--rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.8/wolta/__init__.py
--rw-rw-rw-   0        0        0    11272 2024-04-10 00:37:03.000000 wolta-0.1.8/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.8/wolta/feature_tools.py
--rw-rw-rw-   0        0        0    18051 2024-04-06 14:08:07.000000 wolta-0.1.8/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.8/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-10 00:51:45.071893 wolta-0.1.8/wolta.egg-info/
--rw-rw-rw-   0        0        0    17575 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-04-10 00:51:44.000000 wolta-0.1.8/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 11:06:16.837572 wolta-0.1.9/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    17575 2024-04-11 11:06:16.836547 wolta-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    16268 2024-04-10 00:49:00.000000 wolta-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 11:06:16.837572 wolta-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2024-04-11 11:06:12.000000 wolta-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:06:16.796640 wolta-0.1.9/wolta/
+-rw-rw-rw-   0        0        0      113 2024-03-31 11:58:39.000000 wolta-0.1.9/wolta/__init__.py
+-rw-rw-rw-   0        0        0    11388 2024-04-11 11:06:12.000000 wolta-0.1.9/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.1.9/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0    18051 2024-04-06 14:08:07.000000 wolta-0.1.9/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.1.9/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:06:16.835392 wolta-0.1.9/wolta.egg-info/
+-rw-rw-rw-   0        0        0    17575 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-04-11 11:06:16.000000 wolta-0.1.9/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.1.8/LICENSE.txt` & `wolta-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.1.8/PKG-INFO` & `wolta-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.8
+Version: 0.1.9
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wolta-0.1.8/README.md` & `wolta-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wolta-0.1.8/setup.py` & `wolta-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
```

### Comparing `wolta-0.1.8/wolta/data_tools.py` & `wolta-0.1.9/wolta/data_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -296,72 +296,74 @@
 
         return X, y
 
     elif strategy == 'log-m':
         amin_x = numpy.amin(X)
         amin_y = numpy.amin(y)
 
-        X = np.log(X + amin_x + 1)
-        y = np.log(y + amin_y + 1)
+        X = np.log(X + np.abs(amin_x) + 1)
+        y = np.log(y + np.abs(amin_y) + 1)
 
         return X, y, amin_x, amin_y
 
     elif strategy == 'log2':
         X = np.log2(X)
         y = np.log2(y)
 
         return X, y
 
     elif strategy == 'log2-m':
         amin_x = numpy.amin(X)
         amin_y = numpy.amin(y)
 
-        X = np.log2(X + amin_x + 1)
-        y = np.log2(y + amin_y + 1)
+        X = np.log2(X + np.abs(amin_x) + 1)
+        y = np.log2(y + np.abs(amin_y) + 1)
 
         return X, y, amin_x, amin_y
 
     elif strategy == 'log10':
         X = np.log10(X)
         y = np.log10(y)
 
         return X, y
 
     elif strategy == 'log10-m':
         amin_x = numpy.amin(X)
         amin_y = numpy.amin(y)
 
-        X = np.log10(X + amin_x + 1)
-        y = np.log10(y + amin_y + 1)
+        X = np.log10(X + np.abs(amin_x) + 1)
+        y = np.log10(y + np.abs(amin_y) + 1)
 
         return X, y, amin_x, amin_y
 
     elif strategy == 'sqrt':
         X = np.sqrt(X)
         y = np.sqrt(y)
 
         return X, y
 
     elif strategy == 'sqrt-m':
         amin_x = numpy.amin(X)
         amin_y = numpy.amin(y)
 
-        X = np.sqrt(X + amin_x + 1)
-        y = np.sqrt(y + amin_y + 1)
+        X = np.sqrt(X + np.abs(amin_x) + 1)
+        y = np.sqrt(y + np.abs(amin_y) + 1)
 
         return X, y, amin_x, amin_y
 
     elif strategy == 'cbrt':
         X = np.cbrt(X)
         y = np.cbrt(y)
 
         return X, y
 
 
 def transform_pred(y_pred, strategy='log-m', amin_y=0):
+    amin_y = np.abs(amin_y)
+
     if strategy == 'log':
         y_pred = np.exp(y_pred)
 
     elif strategy == 'log-m':
         y_pred = np.exp(y_pred) - amin_y - 1
 
     elif strategy == 'log2':
@@ -384,14 +386,16 @@
 
     elif strategy == 'cbrt':
         y_pred = np.power(y_pred, 3)
 
     elif strategy == 'cbrt-m':
         y_pred = np.power(y_pred, 3) - amin_y - 1
 
+    return y_pred
+
 
 def make_categorical(y, strategy='normal'):
     import numpy as np
 
     if strategy == 'normal' or strategy == 'normal-extra':
         amin = np.amin(y)
         amax = np.amax(y)
```

### Comparing `wolta-0.1.8/wolta/feature_tools.py` & `wolta-0.1.9/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.8/wolta/model_tools.py` & `wolta-0.1.9/wolta/model_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.8/wolta/progressive_tools.py` & `wolta-0.1.9/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.1.8/wolta.egg-info/PKG-INFO` & `wolta-0.1.9/wolta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.1.8
+Version: 0.1.9
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

