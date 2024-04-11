# Comparing `tmp/epidemik-0.0.14.tar.gz` & `tmp/epidemik-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.14.tar", last modified: Mon Apr  8 18:34:49 2024, max compression
+gzip compressed data, was "epidemik-0.0.15.tar", last modified: Thu Apr 11 14:02:49 2024, max compression
```

## Comparing `epidemik-0.0.14.tar` & `epidemik-0.0.15.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-08 18:34:49.701127 epidemik-0.0.14/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.14/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5356 2024-04-08 18:34:49.700935 epidemik-0.0.14/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)     4678 2024-04-08 18:32:00.000000 epidemik-0.0.14/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      782 2024-04-08 18:30:25.000000 epidemik-0.0.14/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-08 18:34:49.701172 epidemik-0.0.14/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-08 18:34:49.698891 epidemik-0.0.14/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-08 18:34:49.699922 epidemik-0.0.14/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    17904 2024-04-06 19:09:23.000000 epidemik-0.0.14/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     4701 2024-04-06 18:54:54.000000 epidemik-0.0.14/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      290 2024-04-08 18:34:20.000000 epidemik-0.0.14/src/epidemik/__init__.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-08 18:34:49.700743 epidemik-0.0.14/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5356 2024-04-08 18:34:49.000000 epidemik-0.0.14/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      293 2024-04-08 18:34:49.000000 epidemik-0.0.14/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-08 18:34:49.000000 epidemik-0.0.14/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)       64 2024-04-08 18:34:49.000000 epidemik-0.0.14/src/epidemik.egg-info/requires.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-08 18:34:49.000000 epidemik-0.0.14/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.900515 epidemik-0.0.15/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.15/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5355 2024-04-11 14:02:49.900291 epidemik-0.0.15/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)     4677 2024-04-08 18:37:11.000000 epidemik-0.0.15/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      782 2024-04-08 18:36:54.000000 epidemik-0.0.15/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-11 14:02:49.900563 epidemik-0.0.15/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.898083 epidemik-0.0.15/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.899130 epidemik-0.0.15/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    17939 2024-04-11 14:01:24.000000 epidemik-0.0.15/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)    11395 2024-04-11 14:02:05.000000 epidemik-0.0.15/src/epidemik/MetaEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     4721 2024-04-11 14:01:17.000000 epidemik-0.0.15/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      290 2024-04-11 14:02:46.000000 epidemik-0.0.15/src/epidemik/__init__.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       41 2024-04-11 14:01:09.000000 epidemik-0.0.15/src/epidemik/utils.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.900080 epidemik-0.0.15/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5355 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      368 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       64 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/requires.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-11 14:02:49.000000 epidemik-0.0.15/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:02:49.899916 epidemik-0.0.15/tests/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      797 2024-04-08 21:04:05.000000 epidemik-0.0.15/tests/tests_EpiModel.py
```

### Comparing `epidemik-0.0.14/LICENSE` & `epidemik-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.14/PKG-INFO` & `epidemik-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.14
+Version: 0.0.15
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -107,15 +107,15 @@
 ```python
 SIR.R0()
 ```
 
 
 
 ```python
-N = 100_000
+N = 10_000
 I0 = 10
 
 SIR.integrate(365, S=N-I0, I=I0, R=0)
 ```
 
 The results of the integration are stored in the `values_` field. A quick visualization of the results can be obtained using:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.14 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.15 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
@@ -33,15 +33,15 @@
 'R', mu) ``` This fully defines the model. We can get a textual representation
 of the model using ```python print(SIR) ``` resulting in a simple description
 of hte model structure. Epidemic Model with 3 compartments and 2 transitions: S
 + I = I 0.200000 I -> R 0.100000 R0=2.00 or a graphical representation by
 calling `draw_model`: ```python SIR.draw_model() ``` [https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR.png]The
 models value of the Basic Reproductive Number (R~0~) can be determined using
-the `R0()` function: ```python SIR.R0() ``` ```python N = 100_000 I0 = 10
+the `R0()` function: ```python SIR.R0() ``` ```python N = 10_000 I0 = 10
 SIR.integrate(365, S=N-I0, I=I0, R=0) ``` The results of the integration are
 stored in the `values_` field. A quick visualization of the results can be
 obtained using: ```python SIR.plot() ``` which produces:[https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
```

### Comparing `epidemik-0.0.14/README.md` & `epidemik-0.0.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 ```python
 SIR.R0()
 ```
 
 
 
 ```python
-N = 100_000
+N = 10_000
 I0 = 10
 
 SIR.integrate(365, S=N-I0, I=I0, R=0)
 ```
 
 The results of the integration are stored in the `values_` field. A quick visualization of the results can be obtained using:
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 'R', mu) ``` This fully defines the model. We can get a textual representation
 of the model using ```python print(SIR) ``` resulting in a simple description
 of hte model structure. Epidemic Model with 3 compartments and 2 transitions: S
 + I = I 0.200000 I -> R 0.100000 R0=2.00 or a graphical representation by
 calling `draw_model`: ```python SIR.draw_model() ``` [https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR.png]The
 models value of the Basic Reproductive Number (R~0~) can be determined using
-the `R0()` function: ```python SIR.R0() ``` ```python N = 100_000 I0 = 10
+the `R0()` function: ```python SIR.R0() ``` ```python N = 10_000 I0 = 10
 SIR.integrate(365, S=N-I0, I=I0, R=0) ``` The results of the integration are
 stored in the `values_` field. A quick visualization of the results can be
 obtained using: ```python SIR.plot() ``` which produces:[https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
```

### Comparing `epidemik-0.0.14/pyproject.toml` & `epidemik-0.0.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.14/src/epidemik/EpiModel.py` & `epidemik-0.0.15/src/epidemik/EpiModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 from numpy import linalg
 from numpy import random
 import scipy.integrate
 import pandas as pd
 import matplotlib.pyplot as plt
 import string
+from .utils import *
 
 class EpiModel(object):
     """Simple Epidemic Model Implementation
     
         Provides a way to implement and numerically integrate 
     """
     def __init__(self, compartments=None):
@@ -214,15 +215,15 @@
             ax.set_ylabel('Population')
             
             if title is not None:
                 ax.set_title(title)
             
             return ax
         except:
-            raise NotInitialized('You must call integrate() first')
+            raise NotInitialized('You must call integrate() or simulate() first')
     
     def __getattr__(self, name):
         """
         Dynamic method to return the individual compartment values
         
         Parameters:
         - name: string
```

### Comparing `epidemik-0.0.14/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.15/src/epidemik/NetworkEpiModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 from numpy import linalg
 from numpy import random
 import pandas as pd
 import matplotlib.pyplot as plt
 from . import EpiModel
 from collections import Counter
-
+from .utils import *
 
 class NetworkEpiModel(EpiModel):
     def __init__(self, network, compartments=None):
         super(NetworkEpiModel, self).__init__(compartments)
         self.network = network
         self.kavg_ = 2*network.number_of_edges()/network.number_of_nodes() 
         self.spontaneous = {}
```

### Comparing `epidemik-0.0.14/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.15/src/epidemik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.14
+Version: 0.0.15
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -107,15 +107,15 @@
 ```python
 SIR.R0()
 ```
 
 
 
 ```python
-N = 100_000
+N = 10_000
 I0 = 10
 
 SIR.integrate(365, S=N-I0, I=I0, R=0)
 ```
 
 The results of the integration are stored in the `values_` field. A quick visualization of the results can be obtained using:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.14 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.15 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
@@ -33,15 +33,15 @@
 'R', mu) ``` This fully defines the model. We can get a textual representation
 of the model using ```python print(SIR) ``` resulting in a simple description
 of hte model structure. Epidemic Model with 3 compartments and 2 transitions: S
 + I = I 0.200000 I -> R 0.100000 R0=2.00 or a graphical representation by
 calling `draw_model`: ```python SIR.draw_model() ``` [https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR.png]The
 models value of the Basic Reproductive Number (R~0~) can be determined using
-the `R0()` function: ```python SIR.R0() ``` ```python N = 100_000 I0 = 10
+the `R0()` function: ```python SIR.R0() ``` ```python N = 10_000 I0 = 10
 SIR.integrate(365, S=N-I0, I=I0, R=0) ``` The results of the integration are
 stored in the `values_` field. A quick visualization of the results can be
 obtained using: ```python SIR.plot() ``` which produces:[https://
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
```

