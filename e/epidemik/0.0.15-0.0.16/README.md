# Comparing `tmp/epidemik-0.0.15.tar.gz` & `tmp/epidemik-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.15.tar", last modified: Thu Apr 11 14:02:49 2024, max compression
+gzip compressed data, was "epidemik-0.0.16.tar", last modified: Thu Apr 11 14:04:25 2024, max compression
```

## Comparing `epidemik-0.0.15.tar` & `epidemik-0.0.16.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.900515 epidemik-0.0.15/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.15/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5355 2024-04-11 14:02:49.900291 epidemik-0.0.15/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)     4677 2024-04-08 18:37:11.000000 epidemik-0.0.15/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      782 2024-04-08 18:36:54.000000 epidemik-0.0.15/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-11 14:02:49.900563 epidemik-0.0.15/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.898083 epidemik-0.0.15/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.899130 epidemik-0.0.15/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    17939 2024-04-11 14:01:24.000000 epidemik-0.0.15/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)    11395 2024-04-11 14:02:05.000000 epidemik-0.0.15/src/epidemik/MetaEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     4721 2024-04-11 14:01:17.000000 epidemik-0.0.15/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      290 2024-04-11 14:02:46.000000 epidemik-0.0.15/src/epidemik/__init__.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)       41 2024-04-11 14:01:09.000000 epidemik-0.0.15/src/epidemik/utils.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.900080 epidemik-0.0.15/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5355 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      368 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)       64 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/requires.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/top_level.txt
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.899916 epidemik-0.0.15/tests/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      797 2024-04-08 21:04:05.000000 epidemik-0.0.15/tests/tests_EpiModel.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:04:25.721941 epidemik-0.0.16/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.16/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5355 2024-04-11 14:04:25.721743 epidemik-0.0.16/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)     4677 2024-04-08 18:37:11.000000 epidemik-0.0.16/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      782 2024-04-08 18:36:54.000000 epidemik-0.0.16/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-11 14:04:25.721980 epidemik-0.0.16/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:04:25.719592 epidemik-0.0.16/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:04:25.720637 epidemik-0.0.16/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    17939 2024-04-11 14:01:24.000000 epidemik-0.0.16/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)    11396 2024-04-11 14:03:39.000000 epidemik-0.0.16/src/epidemik/MetaEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     4729 2024-04-11 14:03:53.000000 epidemik-0.0.16/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      290 2024-04-11 14:04:08.000000 epidemik-0.0.16/src/epidemik/__init__.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       41 2024-04-11 14:01:09.000000 epidemik-0.0.16/src/epidemik/utils.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:04:25.721544 epidemik-0.0.16/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5355 2024-04-11 14:04:25.000000 epidemik-0.0.16/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      368 2024-04-11 14:04:25.000000 epidemik-0.0.16/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-11 14:04:25.000000 epidemik-0.0.16/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       64 2024-04-11 14:04:25.000000 epidemik-0.0.16/src/epidemik.egg-info/requires.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-11 14:04:25.000000 epidemik-0.0.16/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:04:25.721399 epidemik-0.0.16/tests/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      797 2024-04-08 21:04:05.000000 epidemik-0.0.16/tests/tests_EpiModel.py
```

### Comparing `epidemik-0.0.15/LICENSE` & `epidemik-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.15/PKG-INFO` & `epidemik-0.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.15
+Version: 0.0.16
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.15 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.16 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
```

### Comparing `epidemik-0.0.15/README.md` & `epidemik-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.15/pyproject.toml` & `epidemik-0.0.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.15/src/epidemik/EpiModel.py` & `epidemik-0.0.16/src/epidemik/EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.15/src/epidemik/MetaEpiModel.py` & `epidemik-0.0.16/src/epidemik/MetaEpiModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from numpy import linalg
 from numpy import random
 import scipy.integrate
 import pandas as pd
 import matplotlib.pyplot as plt
 import string
 
-from EpiModel import *
+from .EpiModel import *
 
 from tqdm import tqdm
 tqdm.pandas()
 
 class MetaEpiModel:
     """Simple Epidemic Model Implementation
```

### Comparing `epidemik-0.0.15/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.16/src/epidemik/NetworkEpiModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import networkx as nx
 import numpy as np
 from numpy import linalg
 from numpy import random
 import pandas as pd
 import matplotlib.pyplot as plt
-from . import EpiModel
+from .EpiModel import EpiModel
 from collections import Counter
 from .utils import *
 
 class NetworkEpiModel(EpiModel):
     def __init__(self, network, compartments=None):
         super(NetworkEpiModel, self).__init__(compartments)
         self.network = network
```

### Comparing `epidemik-0.0.15/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.16/src/epidemik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.15
+Version: 0.0.16
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.15 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.16 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
```

### Comparing `epidemik-0.0.15/tests/tests_EpiModel.py` & `epidemik-0.0.16/tests/tests_EpiModel.py`

 * *Files identical despite different names*

