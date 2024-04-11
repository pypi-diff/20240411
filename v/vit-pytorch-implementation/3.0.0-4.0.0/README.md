# Comparing `tmp/vit-pytorch-implementation-3.0.0.tar.gz` & `tmp/vit-pytorch-implementation-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-pytorch-implementation-3.0.0.tar", last modified: Thu Apr 11 04:58:19 2024, max compression
+gzip compressed data, was "vit-pytorch-implementation-4.0.0.tar", last modified: Thu Apr 11 05:48:18 2024, max compression
```

## Comparing `vit-pytorch-implementation-3.0.0.tar` & `vit-pytorch-implementation-4.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:58:19.679649 vit-pytorch-implementation-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-11 04:58:19.679649 vit-pytorch-implementation-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 04:58:13.000000 vit-pytorch-implementation-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 04:58:19.679649 vit-pytorch-implementation-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-11 04:58:13.000000 vit-pytorch-implementation-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:58:19.679649 vit-pytorch-implementation-3.0.0/vit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 04:58:13.000000 vit-pytorch-implementation-3.0.0/vit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-11 04:58:13.000000 vit-pytorch-implementation-3.0.0/vit_pytorch/lilvit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 04:58:19.679649 vit-pytorch-implementation-3.0.0/vit_pytorch_implementation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-11 04:58:19.000000 vit-pytorch-implementation-3.0.0/vit_pytorch_implementation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-11 04:58:19.000000 vit-pytorch-implementation-3.0.0/vit_pytorch_implementation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 04:58:19.000000 vit-pytorch-implementation-3.0.0/vit_pytorch_implementation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 04:58:19.000000 vit-pytorch-implementation-3.0.0/vit_pytorch_implementation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 04:58:19.000000 vit-pytorch-implementation-3.0.0/vit_pytorch_implementation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:48:18.492636 vit-pytorch-implementation-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-11 05:48:18.492636 vit-pytorch-implementation-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-11 05:48:14.000000 vit-pytorch-implementation-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:48:18.492636 vit-pytorch-implementation-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-11 05:48:14.000000 vit-pytorch-implementation-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:48:18.488636 vit-pytorch-implementation-4.0.0/vit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:48:14.000000 vit-pytorch-implementation-4.0.0/vit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-11 05:48:14.000000 vit-pytorch-implementation-4.0.0/vit_pytorch/lilvit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:48:18.492636 vit-pytorch-implementation-4.0.0/vit_pytorch_implementation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-11 05:48:18.000000 vit-pytorch-implementation-4.0.0/vit_pytorch_implementation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-11 05:48:18.000000 vit-pytorch-implementation-4.0.0/vit_pytorch_implementation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 05:48:18.000000 vit-pytorch-implementation-4.0.0/vit_pytorch_implementation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:48:18.000000 vit-pytorch-implementation-4.0.0/vit_pytorch_implementation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 05:48:18.000000 vit-pytorch-implementation-4.0.0/vit_pytorch_implementation.egg-info/top_level.txt
```

### Comparing `vit-pytorch-implementation-3.0.0/PKG-INFO` & `vit-pytorch-implementation-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch-implementation
-Version: 3.0.0
+Version: 4.0.0
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/soumya1729/vit-pytorch-implementation/
 Author: SM
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `vit-pytorch-implementation-3.0.0/setup.py` & `vit-pytorch-implementation-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vit-pytorch-implementation',
-  version = '3.0.0',
+  version = '4.0.0',
   license='MIT',
   description = 'Vision Transformer (ViT) - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'SM',
   url = 'https://github.com/soumya1729/vit-pytorch-implementation/',
   keywords = [
     'artificial intelligence',
```

### Comparing `vit-pytorch-implementation-3.0.0/vit_pytorch/lilvit.py` & `vit-pytorch-implementation-4.0.0/vit_pytorch/lilvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-implementation-3.0.0/vit_pytorch_implementation.egg-info/PKG-INFO` & `vit-pytorch-implementation-4.0.0/vit_pytorch_implementation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vit-pytorch-implementation
-Version: 3.0.0
+Version: 4.0.0
 Summary: Vision Transformer (ViT) - Pytorch
 Home-page: https://github.com/soumya1729/vit-pytorch-implementation/
 Author: SM
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

