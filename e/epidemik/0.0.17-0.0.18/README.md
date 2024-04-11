# Comparing `tmp/epidemik-0.0.17.tar.gz` & `tmp/epidemik-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.17.tar", last modified: Thu Apr 11 14:05:51 2024, max compression
+gzip compressed data, was "epidemik-0.0.18.tar", last modified: Thu Apr 11 18:43:33 2024, max compression
```

## Comparing `epidemik-0.0.17.tar` & `epidemik-0.0.18.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:05:51.592472 epidemik-0.0.17/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.17/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5355 2024-04-11 14:05:51.592255 epidemik-0.0.17/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)     4677 2024-04-08 18:37:11.000000 epidemik-0.0.17/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      782 2024-04-08 18:36:54.000000 epidemik-0.0.17/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-11 14:05:51.592515 epidemik-0.0.17/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:05:51.590010 epidemik-0.0.17/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:05:51.591085 epidemik-0.0.17/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    17939 2024-04-11 14:01:24.000000 epidemik-0.0.17/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)    11396 2024-04-11 14:03:39.000000 epidemik-0.0.17/src/epidemik/MetaEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     4729 2024-04-11 14:03:53.000000 epidemik-0.0.17/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      329 2024-04-11 14:05:42.000000 epidemik-0.0.17/src/epidemik/__init__.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)       41 2024-04-11 14:01:09.000000 epidemik-0.0.17/src/epidemik/utils.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:05:51.592045 epidemik-0.0.17/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5355 2024-04-11 14:05:51.000000 epidemik-0.0.17/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      368 2024-04-11 14:05:51.000000 epidemik-0.0.17/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-11 14:05:51.000000 epidemik-0.0.17/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)       64 2024-04-11 14:05:51.000000 epidemik-0.0.17/src/epidemik.egg-info/requires.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-11 14:05:51.000000 epidemik-0.0.17/src/epidemik.egg-info/top_level.txt
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 14:05:51.591886 epidemik-0.0.17/tests/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      797 2024-04-08 21:04:05.000000 epidemik-0.0.17/tests/tests_EpiModel.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.726635 epidemik-0.0.18/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.18/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5384 2024-04-11 18:43:33.726454 epidemik-0.0.18/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)     4683 2024-04-11 18:19:19.000000 epidemik-0.0.18/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      852 2024-04-11 18:43:24.000000 epidemik-0.0.18/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-11 18:43:33.726678 epidemik-0.0.18/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.724152 epidemik-0.0.18/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.725265 epidemik-0.0.18/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    18065 2024-04-11 18:03:03.000000 epidemik-0.0.18/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)    11348 2024-04-11 17:58:26.000000 epidemik-0.0.18/src/epidemik/MetaEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     4729 2024-04-11 14:03:53.000000 epidemik-0.0.18/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      329 2024-04-11 18:43:28.000000 epidemik-0.0.18/src/epidemik/__init__.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       41 2024-04-11 14:01:09.000000 epidemik-0.0.18/src/epidemik/utils.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.726229 epidemik-0.0.18/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5384 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      368 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       72 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/requires.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-11 18:43:33.000000 epidemik-0.0.18/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-11 18:43:33.726064 epidemik-0.0.18/tests/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      797 2024-04-08 21:04:05.000000 epidemik-0.0.18/tests/tests_EpiModel.py
```

### Comparing `epidemik-0.0.17/LICENSE` & `epidemik-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.17/PKG-INFO` & `epidemik-0.0.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.17
+Version: 0.0.18
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: networkx>=3
 Requires-Dist: numpy>=1.20
 Requires-Dist: pandas>=2.0
 Requires-Dist: scipy>=1.10
+Requires-Dist: tqdm>=4
 
 # epidemik
 
 Compartmental Epidemic Models in Python
 
 
 ---
@@ -136,15 +137,15 @@
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 Join our project and provide assistance by:
-* Checking out the list of [open issues](https://github.com/aregtech/areg-sdk/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help.
+* Checking out the list of [open issues](https://github.com/DataForScience/epidemik/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help.
 * If you need new features, please open a [new issue](https://github.com/DataForScience/epidemik/issues) or start a [discussion](https://github.com/DataForScience/epidemik/discussions).
 
  Contact us for the feedback or new ideas.
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.17 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.18 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
-Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10 #
-epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
-(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
-pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
-(#usage) - [Contributing](#contributing) - [License](#license) --- ##
-Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
-main/images/pin.svg)](#installation) Use the package manager [pip](https://
-pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
+Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10
+Requires-Dist: tqdm>=4 # epidemik Compartmental Epidemic Models in Python --
+- ## Table of contents[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#toc) - [Installation](#installation) - [Tech
+Stack](#tech) - [Usage](#usage) - [Contributing](#contributing) - [License]
+(#license) --- ## Installation[![](https://raw.githubusercontent.com/
+DataForScience/epidemik/main/images/pin.svg)](#installation) Use the package
+manager [pip](https://pip.pypa.io/en/stable/) to install epidemik. ```bash pip
+install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
 directed multigraph using [networkx](https://networkx.org/) - Ordinary
 Differential Equations are numerically integrated using [scipy](https://
 scipy.org/) - Random numbers are generated by[numpy](https://numpy.org/) -
@@ -44,15 +45,15 @@
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
 major changes, please open an issue first to discuss what you would like to
 change. Please make sure to update tests as appropriate. Join our project and
 provide assistance by: * Checking out the list of [open issues](https://
-github.com/aregtech/areg-sdk/
+github.com/DataForScience/epidemik/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help. *
 If you need new features, please open a [new issue](https://github.com/
 DataForScience/epidemik/issues) or start a [discussion](https://github.com/
 DataForScience/epidemik/discussions). Contact us for the feedback or new ideas.
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Spread The Word[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#spread) If you want to say thank you and/or
```

### Comparing `epidemik-0.0.17/README.md` & `epidemik-0.0.18/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 Join our project and provide assistance by:
-* Checking out the list of [open issues](https://github.com/aregtech/areg-sdk/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help.
+* Checking out the list of [open issues](https://github.com/DataForScience/epidemik/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help.
 * If you need new features, please open a [new issue](https://github.com/DataForScience/epidemik/issues) or start a [discussion](https://github.com/DataForScience/epidemik/discussions).
 
  Contact us for the feedback or new ideas.
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
```

#### html2text {}

```diff
@@ -35,15 +35,15 @@
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
 major changes, please open an issue first to discuss what you would like to
 change. Please make sure to update tests as appropriate. Join our project and
 provide assistance by: * Checking out the list of [open issues](https://
-github.com/aregtech/areg-sdk/
+github.com/DataForScience/epidemik/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help. *
 If you need new features, please open a [new issue](https://github.com/
 DataForScience/epidemik/issues) or start a [discussion](https://github.com/
 DataForScience/epidemik/discussions). Contact us for the feedback or new ideas.
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Spread The Word[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#spread) If you want to say thank you and/or
```

### Comparing `epidemik-0.0.17/pyproject.toml` & `epidemik-0.0.18/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,25 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
  "matplotlib>=3.8",
  "networkx>=3",
  "numpy>=1.20",
  "pandas>=2.0",
- "scipy>=1.10"
+ "scipy>=1.10",
+ "tqdm>=4"
 ]
 [project.urls]
 Homepage = "https://github.com/DataForScience/epidemik"
 Issues = "https://github.com/DataForScience/epidemik/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 version = {attr = "epidemik.__version__"}
+
+[tool.pytest.ini_options]
+pythonpath = [
+  ".", "src",
+]
```

### Comparing `epidemik-0.0.17/src/epidemik/EpiModel.py` & `epidemik-0.0.18/src/epidemik/EpiModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                     rate *= season
                 
             diff[pos[source]] -= rate
             diff[pos[target]] += rate
             
         return diff
     
-    def plot(self, title=None, normed=True, **kwargs):
+    def plot(self, title=None, normed=True, show=True, **kwargs):
         """
         Convenience function for plotting
         
         Parameters:
         - title: string, optional
             Title of the plot
         - normed: bool, optional
@@ -213,14 +213,17 @@
                 
             ax.set_xlabel('Time')
             ax.set_ylabel('Population')
             
             if title is not None:
                 ax.set_title(title)
             
+            if show:
+                plt.show()
+
             return ax
         except:
             raise NotInitialized('You must call integrate() or simulate() first')
     
     def __getattr__(self, name):
         """
         Dynamic method to return the individual compartment values
@@ -454,20 +457,20 @@
                     inf[agent][node_i] = {}
 
                 inf[agent][node_i]['target'] = node_j
                 inf[agent][node_i]['rate'] = data['rate']
 
         return inf
 
-    def draw_model(self, ax=None):
+    def draw_model(self, ax=None, show=True):
         try:
             from networkx.drawing.nx_agraph import graphviz_layout
             pos=graphviz_layout(self.transitions, prog='dot', args='-Grankdir="LR"')
         except:
-            pos=nx.layout.spectral_layout(G)
+            pos=nx.layout.spectral_layout(self.transitions)
 
         colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
 
         S_color = colors[0]
         E_color = colors[4]
         I_color = colors[1]
         R_color = colors[2]
@@ -507,14 +510,16 @@
         if ax is None:
             fig, ax = plt.subplots(1)
 
         nx.draw(self.transitions, pos, with_labels=True, arrows=True, node_shape='H', 
         font_color='k', node_color=node_colors, node_size=1000, ax=ax)
         nx.draw_networkx_edge_labels(self.transitions, pos, edge_labels=edge_labels, ax=ax)
 
+        if show:
+            plt.show()
 
     def R0(self):
         infected = set()
 
         susceptible = self._get_susceptible()
 
         for node_i, node_j, data in self.transitions.edges(data=True):
```

### Comparing `epidemik-0.0.17/src/epidemik/MetaEpiModel.py` & `epidemik-0.0.18/src/epidemik/MetaEpiModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ### −∗− mode : python ; −∗−
-# @file EpiModel.py
+# @file MetaEpiModel.py
 # @author Bruno Goncalves
 ######################################################
 
 import networkx as nx
 import numpy as np
 from numpy import linalg
 from numpy import random
-import scipy.integrate
 import pandas as pd
 import matplotlib.pyplot as plt
-import string
+import matplotlib.patches as mpatches
+from matplotlib.collections import PatchCollection
 
 from .EpiModel import *
 
 from tqdm import tqdm
 tqdm.pandas()
 
 class MetaEpiModel:
@@ -199,16 +199,15 @@
         ax.invert_yaxis()
 
         patches = []
         color_list = []
         colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
         x = np.linspace(0., 0.75, self.models['NY'].values_.shape[0])
 
-        import matplotlib.patches as mpatches
-        from matplotlib.collections import PatchCollection
+
 
         for state in self.models:
             daily = self.models[state]['I'].values
             
             timeline = (daily/daily.max())
             color = colors[3]
```

### Comparing `epidemik-0.0.17/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.18/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.17/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.18/src/epidemik.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.17
+Version: 0.0.18
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: networkx>=3
 Requires-Dist: numpy>=1.20
 Requires-Dist: pandas>=2.0
 Requires-Dist: scipy>=1.10
+Requires-Dist: tqdm>=4
 
 # epidemik
 
 Compartmental Epidemic Models in Python
 
 
 ---
@@ -136,15 +137,15 @@
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 Join our project and provide assistance by:
-* Checking out the list of [open issues](https://github.com/aregtech/areg-sdk/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help.
+* Checking out the list of [open issues](https://github.com/DataForScience/epidemik/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help.
 * If you need new features, please open a [new issue](https://github.com/DataForScience/epidemik/issues) or start a [discussion](https://github.com/DataForScience/epidemik/discussions).
 
  Contact us for the feedback or new ideas.
 
 <div align="right">[ <a href="#table-of-contents">↑ Back to top ↑</a> ]</div>
 
 ---
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: epidemik Version: 0.0.17 Summary: A pakage to
+Metadata-Version: 2.1 Name: epidemik Version: 0.0.18 Summary: A pakage to
 simulate compartmental epidemic models Author-email: Bruno GonÃ§alves
 data4sci.com> Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: matplotlib>=3.8 Requires-Dist: networkx>=3 Requires-
-Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10 #
-epidemik Compartmental Epidemic Models in Python --- ## Table of contents[![]
-(https://raw.githubusercontent.com/DataForScience/epidemik/main/images/
-pin.svg)](#toc) - [Installation](#installation) - [Tech Stack](#tech) - [Usage]
-(#usage) - [Contributing](#contributing) - [License](#license) --- ##
-Installation[![](https://raw.githubusercontent.com/DataForScience/epidemik/
-main/images/pin.svg)](#installation) Use the package manager [pip](https://
-pip.pypa.io/en/stable/) to install epidemik. ```bash pip install epidemik ```
+Dist: numpy>=1.20 Requires-Dist: pandas>=2.0 Requires-Dist: scipy>=1.10
+Requires-Dist: tqdm>=4 # epidemik Compartmental Epidemic Models in Python --
+- ## Table of contents[![](https://raw.githubusercontent.com/DataForScience/
+epidemik/main/images/pin.svg)](#toc) - [Installation](#installation) - [Tech
+Stack](#tech) - [Usage](#usage) - [Contributing](#contributing) - [License]
+(#license) --- ## Installation[![](https://raw.githubusercontent.com/
+DataForScience/epidemik/main/images/pin.svg)](#installation) Use the package
+manager [pip](https://pip.pypa.io/en/stable/) to install epidemik. ```bash pip
+install epidemik ```
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Tech Stack[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#tech) Here's a brief high-level overview of the
 tech stack the `epidemik` package uses: - The model is implemented as a
 directed multigraph using [networkx](https://networkx.org/) - Ordinary
 Differential Equations are numerically integrated using [scipy](https://
 scipy.org/) - Random numbers are generated by[numpy](https://numpy.org/) -
@@ -44,15 +45,15 @@
 raw.githubusercontent.com/DataForScience/epidemik/main/images/SIR_results.png]
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Contributing[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#contributing) Pull requests are welcome. For
 major changes, please open an issue first to discuss what you would like to
 change. Please make sure to update tests as appropriate. Join our project and
 provide assistance by: * Checking out the list of [open issues](https://
-github.com/aregtech/areg-sdk/
+github.com/DataForScience/epidemik/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) where we need help. *
 If you need new features, please open a [new issue](https://github.com/
 DataForScience/epidemik/issues) or start a [discussion](https://github.com/
 DataForScience/epidemik/discussions). Contact us for the feedback or new ideas.
                                                         [ _â___ _B_a_c_k_ _t_o_ _t_o_p_ _â__ ]
 --- ## Spread The Word[![](https://raw.githubusercontent.com/DataForScience/
 epidemik/main/images/pin.svg)](#spread) If you want to say thank you and/or
```

### Comparing `epidemik-0.0.17/tests/tests_EpiModel.py` & `epidemik-0.0.18/tests/tests_EpiModel.py`

 * *Files identical despite different names*

