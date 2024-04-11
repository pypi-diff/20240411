# Comparing `tmp/SAMMEC2-0.0.2.tar.gz` & `tmp/SAMMEC2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMMEC2-0.0.2.tar", last modified: Thu Apr 11 14:10:29 2024, max compression
+gzip compressed data, was "SAMMEC2-0.0.3.tar", last modified: Thu Apr 11 14:32:29 2024, max compression
```

## Comparing `SAMMEC2-0.0.2.tar` & `SAMMEC2-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:10:29.716555 SAMMEC2-0.0.2/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:10:29.715872 SAMMEC2-0.0.2/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.2/README
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:10:29.706426 SAMMEC2-0.0.2/SAMMEC2/
--rw-r--r--   0 bso2     (1724916894) 285334988     3806 2024-04-11 05:26:25.000000 SAMMEC2-0.0.2/SAMMEC2/SAMMEC2.py
--rw-r--r--   0 bso2     (1724916894) 285334988        0 2024-04-11 14:08:10.000000 SAMMEC2-0.0.2/SAMMEC2/__init__.py
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:10:29.715107 SAMMEC2-0.0.2/SAMMEC2.egg-info/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:10:29.000000 SAMMEC2-0.0.2/SAMMEC2.egg-info/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988      206 2024-04-11 14:10:29.000000 SAMMEC2-0.0.2/SAMMEC2.egg-info/SOURCES.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-11 14:10:29.000000 SAMMEC2-0.0.2/SAMMEC2.egg-info/dependency_links.txt
--rw-r--r--   0 bso2     (1724916894) 285334988      659 2024-04-11 13:24:26.000000 SAMMEC2-0.0.2/SAMMEC2.egg-info/example.py
--rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-11 14:10:29.000000 SAMMEC2-0.0.2/SAMMEC2.egg-info/top_level.txt
--rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-11 14:10:29.716719 SAMMEC2-0.0.2/setup.cfg
--rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-11 14:08:10.000000 SAMMEC2-0.0.2/setup.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:32:29.902526 SAMMEC2-0.0.3/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:32:29.901742 SAMMEC2-0.0.3/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.3/README
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:32:29.895791 SAMMEC2-0.0.3/SAMMEC2/
+-rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.3/SAMMEC2/SAMMEC2.py
+-rw-r--r--   0 bso2     (1724916894) 285334988        0 2024-04-11 14:08:10.000000 SAMMEC2-0.0.3/SAMMEC2/__init__.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:32:29.900934 SAMMEC2-0.0.3/SAMMEC2.egg-info/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:32:29.000000 SAMMEC2-0.0.3/SAMMEC2.egg-info/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988      178 2024-04-11 14:32:29.000000 SAMMEC2-0.0.3/SAMMEC2.egg-info/SOURCES.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-11 14:32:29.000000 SAMMEC2-0.0.3/SAMMEC2.egg-info/dependency_links.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-11 14:32:29.000000 SAMMEC2-0.0.3/SAMMEC2.egg-info/top_level.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-11 14:32:29.902723 SAMMEC2-0.0.3/setup.cfg
+-rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-11 14:32:13.000000 SAMMEC2-0.0.3/setup.py
```

### Comparing `SAMMEC2-0.0.2/SAMMEC2/SAMMEC2.py` & `SAMMEC2-0.0.3/SAMMEC2/SAMMEC2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,9 @@
-import pandas as pd
 import numpy as np
 from sklearn.ensemble import AdaBoostClassifier
-from sklearn.metrics import accuracy_score
-from sklearn.tree import DecisionTreeClassifier
-from pandas.api.types import CategoricalDtype
-from sklearn.metrics import confusion_matrix, f1_score, classification_report
-from imblearn.metrics import geometric_mean_score
-import matplotlib.pyplot as plt
 
 
 class AdaBoostClassifier_C2V2(AdaBoostClassifier):
     """algorithm: default=SAMME
     """
     def __init__(self,
                  estimator=None,
@@ -95,8 +88,9 @@
                                                               (estimator_weight < 0))))
             # for i in range(len(y)):
             #    if sample_weight[i]<0.00000005:
             #        sample_weight[i]=0.00000005
             #    else:
             #        sample_weight[i]=sample_weight[i]
 
-        return sample_weight, estimator_weight, estimator_error
+        return sample_weight, estimator_weight, estimator_error
+
```

### Comparing `SAMMEC2-0.0.2/setup.py` & `SAMMEC2-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SAMMEC2", # Replace with your own PyPI username(id)
-    version="0.0.2",
+    version="0.0.3",
     author="Banghee So",
     author_email="bso@towson.edu",
     description="SAMMEC2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bheeso/SAMME.C2",
     packages=setuptools.find_packages(),
```

