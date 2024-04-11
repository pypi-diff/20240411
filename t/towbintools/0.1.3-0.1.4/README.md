# Comparing `tmp/towbintools-0.1.3.tar.gz` & `tmp/towbintools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "towbintools-0.1.3.tar", last modified: Fri Mar  8 15:35:58 2024, max compression
+gzip compressed data, was "towbintools-0.1.4.tar", last modified: Thu Apr 11 13:41:38 2024, max compression
```

## Comparing `towbintools-0.1.3.tar` & `towbintools-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.376248 towbintools-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-08 15:35:48.000000 towbintools-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-03-08 15:35:58.376248 towbintools-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-08 15:35:48.000000 towbintools-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-08 15:35:48.000000 towbintools-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 15:35:58.376248 towbintools-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.372248 towbintools-0.1.3/towbintools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.372248 towbintools-0.1.3/towbintools/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/classification/classification_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.372248 towbintools-0.1.3/towbintools/deep_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.372248 towbintools-0.1.3/towbintools/deep_learning/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/architectures/archs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/architectures/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/deep_learning_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.372248 towbintools-0.1.3/towbintools/deep_learning/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/deep_learning/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.376248 towbintools-0.1.3/towbintools/foundation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/binary_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    16291 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/detect_molts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/image_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/image_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/worm_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/foundation/zstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.376248 towbintools-0.1.3/towbintools/legacy_straightening/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/legacy_straightening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/legacy_straightening/straightening_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.376248 towbintools-0.1.3/towbintools/quantification/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/quantification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/quantification/quantification_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.376248 towbintools-0.1.3/towbintools/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/segmentation/segmentation_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.376248 towbintools-0.1.3/towbintools/straightening/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/straightening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-03-08 15:35:48.000000 towbintools-0.1.3/towbintools/straightening/straightening_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:35:58.376248 towbintools-0.1.3/towbintools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-03-08 15:35:58.000000 towbintools-0.1.3/towbintools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-08 15:35:58.000000 towbintools-0.1.3/towbintools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 15:35:58.000000 towbintools-0.1.3/towbintools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-08 15:35:58.000000 towbintools-0.1.3/towbintools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-08 15:35:58.000000 towbintools-0.1.3/towbintools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 13:41:34.000000 towbintools-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-11 13:41:38.878879 towbintools-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-11 13:41:34.000000 towbintools-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-11 13:41:34.000000 towbintools-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:41:38.878879 towbintools-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.870879 towbintools-0.1.4/towbintools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/classification/classification_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/data_analysis/growth_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/deep_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/deep_learning/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/architectures/archs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/architectures/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/deep_learning_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.874879 towbintools-0.1.4/towbintools/deep_learning/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/deep_learning/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/foundation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/binary_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/detect_molts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/image_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/image_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/worm_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/foundation/zstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/legacy_straightening/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/legacy_straightening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/legacy_straightening/straightening_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/quantification/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/quantification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/quantification/quantification_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/segmentation/segmentation_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools/straightening/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/straightening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35283 2024-04-11 13:41:34.000000 towbintools-0.1.4/towbintools/straightening/straightening_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:41:38.878879 towbintools-0.1.4/towbintools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 13:41:38.000000 towbintools-0.1.4/towbintools.egg-info/top_level.txt
```

### Comparing `towbintools-0.1.3/LICENSE` & `towbintools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/PKG-INFO` & `towbintools-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towbintools
-Version: 0.1.3
+Version: 0.1.4
 Summary: All the tools used by the Towbin Lab !
 Author-email: Sacha Psalmon <sacha.psalmon@unibe.ch>, Boris Gusev <boris.gusev@unibe.ch>
 Maintainer-email: Sacha Psalmon <sacha.psalmon@unibe.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.22.4
```

### Comparing `towbintools-0.1.3/README.md` & `towbintools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/pyproject.toml` & `towbintools-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "towbintools"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Sacha Psalmon", email="sacha.psalmon@unibe.ch" },
   {name="Boris Gusev", email="boris.gusev@unibe.ch" }
 ]
 maintainers = [
     {name = "Sacha Psalmon", email="sacha.psalmon@unibe.ch"},
 ]
```

### Comparing `towbintools-0.1.3/towbintools/classification/classification_tools.py` & `towbintools-0.1.4/towbintools/classification/classification_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/deep_learning/architectures/archs.py` & `towbintools-0.1.4/towbintools/deep_learning/architectures/archs.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/deep_learning/architectures/models.py` & `towbintools-0.1.4/towbintools/deep_learning/architectures/models.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/deep_learning/deep_learning_tools.py` & `towbintools-0.1.4/towbintools/deep_learning/deep_learning_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/deep_learning/utils/augmentation.py` & `towbintools-0.1.4/towbintools/deep_learning/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/deep_learning/utils/dataset.py` & `towbintools-0.1.4/towbintools/deep_learning/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/deep_learning/utils/loss.py` & `towbintools-0.1.4/towbintools/deep_learning/utils/loss.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/foundation/backbone.py` & `towbintools-0.1.4/towbintools/foundation/backbone.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/foundation/binary_image.py` & `towbintools-0.1.4/towbintools/foundation/binary_image.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/foundation/detect_molts.py` & `towbintools-0.1.4/towbintools/foundation/detect_molts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,15 @@
 from typing import Tuple
 
 import numpy as np
 from scipy.ndimage import uniform_filter1d
 from scipy.signal import find_peaks, medfilt, savgol_filter
 from scipy.stats import linregress
 
-from .utils import nan_helper
-
-
-def interpolate_nans(
-    signal: np.ndarray,
-) -> np.ndarray:
-    """
-    Interpolate NaN values in a given signal.
-
-    Uses linear interpolation to estimate and replace NaN values in the provided
-    signal based on the values of non-NaN neighbors.
-
-    Parameters:
-        signal (np.ndarray): The input signal array, which might contain NaN values.
-
-    Returns:
-        np.ndarray: The signal array with NaN values interpolated.
-    """
-
-    nans, x = nan_helper(signal)
-    signal[nans] = np.interp(x(nans), x(~nans), signal[~nans])
-    return signal
-
+from .utils import interpolate_nans
 
 def interpolate_peaks(
     signal: np.ndarray,
 ) -> np.ndarray:
     """
     Interpolate over prominent peaks in a given signal.
```

### Comparing `towbintools-0.1.3/towbintools/foundation/file_handling.py` & `towbintools-0.1.4/towbintools/foundation/file_handling.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/foundation/image_handling.py` & `towbintools-0.1.4/towbintools/foundation/image_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Optional
+from typing import List, Tuple, Optional
 
 import cv2
 import numpy as np
 import skimage.metrics
 from tifffile import imread
 from tifffile import tiffcomment
 import ome_types
@@ -210,28 +210,29 @@
     clahe = cv2.createCLAHE(clipLimit=clip_limit, tileGridSize=(tile_size, tile_size))
     image = clahe.apply(image).astype(np.uint16)
     return image
 
 
 def read_tiff_file(
     file_path: str,
-    channels_to_keep: list = [],
+    channels_to_keep: Optional[List[int]] = None,
 ) -> np.ndarray:
     """
     Read a TIFF file and optionally select specific channels from the image.
 
     Parameters:
             file_path (str): Path to the TIFF image file.
-            channels_to_keep (list): List of channel indices to keep. If empty, all channels are kept.
+            channels_to_keep (list): List of channel indices to keep. If empty or None, all channels are kept.
 
     Returns:
             np.ndarray: The image data as a NumPy array. The number of dimensions may vary depending on the input and selected channels.
     """
     image = imread(file_path)
 
+    # If no channels are specified, return the image as is.
     if image.ndim == 2 or not channels_to_keep:
         return image
 
     if image.ndim == 3:
         return image[channels_to_keep, ...].squeeze()  # type: ignore
     else:
         return image[:, channels_to_keep, ...].squeeze()  # type: ignore
```

### Comparing `towbintools-0.1.3/towbintools/foundation/image_quality.py` & `towbintools-0.1.4/towbintools/foundation/image_quality.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/foundation/worm_features.py` & `towbintools-0.1.4/towbintools/foundation/worm_features.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/foundation/zstack.py` & `towbintools-0.1.4/towbintools/foundation/zstack.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/legacy_straightening/straightening_tools.py` & `towbintools-0.1.4/towbintools/legacy_straightening/straightening_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/quantification/quantification_tools.py` & `towbintools-0.1.4/towbintools/quantification/quantification_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools/straightening/straightening_tools.py` & `towbintools-0.1.4/towbintools/straightening/straightening_tools.py`

 * *Files identical despite different names*

### Comparing `towbintools-0.1.3/towbintools.egg-info/PKG-INFO` & `towbintools-0.1.4/towbintools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: towbintools
-Version: 0.1.3
+Version: 0.1.4
 Summary: All the tools used by the Towbin Lab !
 Author-email: Sacha Psalmon <sacha.psalmon@unibe.ch>, Boris Gusev <boris.gusev@unibe.ch>
 Maintainer-email: Sacha Psalmon <sacha.psalmon@unibe.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.22.4
```

### Comparing `towbintools-0.1.3/towbintools.egg-info/SOURCES.txt` & `towbintools-0.1.4/towbintools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 towbintools.egg-info/PKG-INFO
 towbintools.egg-info/SOURCES.txt
 towbintools.egg-info/dependency_links.txt
 towbintools.egg-info/requires.txt
 towbintools.egg-info/top_level.txt
 towbintools/classification/__init__.py
 towbintools/classification/classification_tools.py
+towbintools/data_analysis/__init__.py
+towbintools/data_analysis/growth_rate.py
 towbintools/deep_learning/__init__.py
 towbintools/deep_learning/deep_learning_tools.py
 towbintools/deep_learning/architectures/__init__.py
 towbintools/deep_learning/architectures/archs.py
 towbintools/deep_learning/architectures/models.py
 towbintools/deep_learning/utils/__init__.py
 towbintools/deep_learning/utils/augmentation.py
```

