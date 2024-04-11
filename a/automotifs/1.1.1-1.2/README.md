# Comparing `tmp/automotifs-1.1.1.tar.gz` & `tmp/automotifs-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automotifs-1.1.1.tar", last modified: Tue Apr  9 14:52:53 2024, max compression
+gzip compressed data, was "automotifs-1.2.tar", last modified: Thu Apr 11 14:05:39 2024, max compression
```

## Comparing `automotifs-1.1.1.tar` & `automotifs-1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:52:53.306534 automotifs-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 14:52:29.000000 automotifs-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-09 14:52:53.306534 automotifs-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-09 14:52:29.000000 automotifs-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:52:53.306534 automotifs-1.1.1/automotif/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 14:52:29.000000 automotifs-1.1.1/automotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-09 14:52:29.000000 automotifs-1.1.1/automotif/automotif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:52:53.306534 automotifs-1.1.1/automotifs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-09 14:52:53.000000 automotifs-1.1.1/automotifs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 14:52:53.000000 automotifs-1.1.1/automotifs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:52:53.000000 automotifs-1.1.1/automotifs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 14:52:53.000000 automotifs-1.1.1/automotifs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 14:52:53.000000 automotifs-1.1.1/automotifs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:52:53.306534 automotifs-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-09 14:52:29.000000 automotifs-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:52:53.306534 automotifs-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-09 14:52:29.000000 automotifs-1.1.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:05:39.288104 automotifs-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 14:05:11.000000 automotifs-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-11 14:05:39.288104 automotifs-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-11 14:05:11.000000 automotifs-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:05:39.284104 automotifs-1.2/automotif/
+-rw-r--r--   0 runner    (1001) docker     (127)    19087 2024-04-11 14:05:11.000000 automotifs-1.2/automotif/Neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 14:05:11.000000 automotifs-1.2/automotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17518 2024-04-11 14:05:11.000000 automotifs-1.2/automotif/automotif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:05:39.288104 automotifs-1.2/automotifs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 14:05:39.000000 automotifs-1.2/automotifs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:05:39.288104 automotifs-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-11 14:05:11.000000 automotifs-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:05:39.288104 automotifs-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-11 14:05:11.000000 automotifs-1.2/tests/test.py
```

### Comparing `automotifs-1.1.1/LICENSE` & `automotifs-1.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
```

### Comparing `automotifs-1.1.1/PKG-INFO` & `automotifs-1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.1.1
+Version: 1.2
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.1.5
 Requires-Dist: pylint>=2.6.0
 Requires-Dist: numpy>=1.23
 Requires-Dist: dotmotif>=0.14.0
 Requires-Dist: networkx>=3.2.1
+Requires-Dist: tamarind>=0.2.1
+Requires-Dist: py2neo>=2021.2.4
 
 # AutoMotif: Automated Motif Detection in Network Graphs
 ## What is it?
 AutoMotif streamlines the identification and cataloging of motifs within network graphs. Utilizing NetworkX for graph manipulation, dotmotif for detecting motifs, and pandas for data management, it simplifies the process of uncovering patterns across both directed and undirected networks. Users can customize searches based on motif size, directionality, executors and the treatment of automorphisms, as well as even having the option to save the results for further analysis.
 
 ## Installation
 
@@ -27,28 +29,31 @@
 ```python
 from automotif import AutoMotif
 from dotmotif import executors
 import networkx as nx
 # Example: A random directed graph
 G = nx.gnp_random_graph(100, 0.5, directed=True)
 # Set up AutoMotif
-motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True, use_GrandISO = True)
+motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True, use_GrandISO=True)
 # Start finding motifs
 motifs = motif_finder.find_all_motifs()
 # Calculate the Z-Score for the motifs
 z_scores = motif_finder.calculate_zscore(num_random_graphs = 30, Executor = executors.NetworkXExecutor)
+# Display the motifs found
+motif_finder.display_all_motifs()
 ```
 ## Features
-- **Automated Detection**: AutoMotif automates the detection of motifs, eliminating the need for manual parameter adjustments. It's designed to be efficient and user-friendly, allowing researchers to focus more on analysis and less on setup.
+- **Automated Detection**: AutoMotif automates the detection of motifs, eliminating the need for manual parameter adjustments. It's designed to be efficient and user-friendly, allowing users to focus more on analysis and less on setup.
 - **Flexible and Powerful**: Capable of handling both directed and undirected graphs, AutoMotif provides flexibility in defining motifs, including size and whether to consider automorphisms, ensuring a broad applicability across different types of network analyses.
 - **Data Organization and Export**: Directly save your motifs to CSV files for easy access, further analysis, or sharing with your team or research community.
 - **Z-Score Calculation**: Assess the statistical significance of detected motifs by calculating their Z-scores, providing insights into the rarity or commonality of patterns within your network compared to random expectations.
+- **Visual Representation**: AutoMotif includes features for visualizing network motifs, allowing users to display them as graphs within the application. This aids in the qualitative analysis of motifs, offering a graphical representation of network patterns and their connections for easier interpretation and presentation.
 ## Contributions
 We encourage contributions to AutoMotif! If you have ideas for improvements or new features, don't hesitate to open an issue or submit a pull request on our repository.
 ## License
 AutoMotif is made available under the MIT License. See the LICENSE file for more details.
 ***
 ## Who made this? 
 AutoMotif was developed by Giorgio Micaletto under the guidance of Professor Marta Zava at Bocconi University. This tool is designed to simplify and facilitate the complex process of network motif analysis.
 Contacts:
 - giorgio.micaletto@studbocconi.it
-- [linkedin](linkedin.com/in/giorgio-micaletto/)
+- [LinkedIn](linkedin.com/in/giorgio-micaletto/)
```

### Comparing `automotifs-1.1.1/README.md` & `automotifs-1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,28 +11,31 @@
 ```python
 from automotif import AutoMotif
 from dotmotif import executors
 import networkx as nx
 # Example: A random directed graph
 G = nx.gnp_random_graph(100, 0.5, directed=True)
 # Set up AutoMotif
-motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True, use_GrandISO = True)
+motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True, use_GrandISO=True)
 # Start finding motifs
 motifs = motif_finder.find_all_motifs()
 # Calculate the Z-Score for the motifs
 z_scores = motif_finder.calculate_zscore(num_random_graphs = 30, Executor = executors.NetworkXExecutor)
+# Display the motifs found
+motif_finder.display_all_motifs()
 ```
 ## Features
-- **Automated Detection**: AutoMotif automates the detection of motifs, eliminating the need for manual parameter adjustments. It's designed to be efficient and user-friendly, allowing researchers to focus more on analysis and less on setup.
+- **Automated Detection**: AutoMotif automates the detection of motifs, eliminating the need for manual parameter adjustments. It's designed to be efficient and user-friendly, allowing users to focus more on analysis and less on setup.
 - **Flexible and Powerful**: Capable of handling both directed and undirected graphs, AutoMotif provides flexibility in defining motifs, including size and whether to consider automorphisms, ensuring a broad applicability across different types of network analyses.
 - **Data Organization and Export**: Directly save your motifs to CSV files for easy access, further analysis, or sharing with your team or research community.
 - **Z-Score Calculation**: Assess the statistical significance of detected motifs by calculating their Z-scores, providing insights into the rarity or commonality of patterns within your network compared to random expectations.
+- **Visual Representation**: AutoMotif includes features for visualizing network motifs, allowing users to display them as graphs within the application. This aids in the qualitative analysis of motifs, offering a graphical representation of network patterns and their connections for easier interpretation and presentation.
 ## Contributions
 We encourage contributions to AutoMotif! If you have ideas for improvements or new features, don't hesitate to open an issue or submit a pull request on our repository.
 ## License
 AutoMotif is made available under the MIT License. See the LICENSE file for more details.
 ***
 ## Who made this? 
 AutoMotif was developed by Giorgio Micaletto under the guidance of Professor Marta Zava at Bocconi University. This tool is designed to simplify and facilitate the complex process of network motif analysis.
 Contacts:
 - giorgio.micaletto@studbocconi.it
-- [linkedin](linkedin.com/in/giorgio-micaletto/)
+- [LinkedIn](linkedin.com/in/giorgio-micaletto/)
```

### Comparing `automotifs-1.1.1/automotif/automotif.py` & `automotifs-1.2/automotif/automotif.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 Developed by Giorgio Micaletto under the supervision of Professor Marta Zava at Bocconi University,
 this tool aims to facilitate the systematic study of network motifs.
 """
 import random
 import pandas as pd 
 import networkx as nx
+from .Neo4j import Neo4jExecutor
 import os
 from dotmotif import Motif
 from itertools import product
 import dotmotif.executors as executors
 from typing import Union
 import numpy as np
 import matplotlib.pyplot as plt
@@ -52,14 +53,15 @@
                  upto: bool = False,
                  lower: int = 3, 
                  save: bool = False, 
                  path: str = None,
                  find: bool = False, 
                  verbose: bool = False,
                  use_GrandISO: bool = False,
+                 use_Neo4j: bool = False,
                  personal_executor: executors.Executor = None):
         if not hasattr(Graph, "nodes") or not callable(getattr(Graph, "nodes")):
             raise ValueError("Graph should be a NetworkX graph")
         elif type(size) != int:
             raise ValueError("Size should be an integer")
         elif type(upto) != bool:
             raise ValueError("Upto should be a boolean")
@@ -84,14 +86,18 @@
         self.lower = lower
         if personal_executor is not None:
             self.Ex = personal_executor
         if use_GrandISO == True:
             self.Ex = executors.GrandIsoExecutor(graph = self.Graph)
             if personal_executor is not None:
                 print("Warning: The Executor provided will be ignored in favor of GrandIsoExecutor as use_GrandISO is set to True")
+        elif use_Neo4j == True:
+            self.Ex = Neo4jExecutor(graph = self.Graph)
+            if personal_executor is not None:
+                print("Warning: The Executor provided will be ignored in favor of Neo4jExecutor as use_Neo4j is set to True")
         else:
             self.Ex = executors.NetworkXExecutor(graph = self.Graph)
         self.motifs = None
         self.generate_required_motifs()
         self.motifs_found = None
         if find == True:
             self.find_all_motifs()
```

### Comparing `automotifs-1.1.1/automotifs.egg-info/PKG-INFO` & `automotifs-1.2/automotifs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.1.1
+Version: 1.2
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.1.5
 Requires-Dist: pylint>=2.6.0
 Requires-Dist: numpy>=1.23
 Requires-Dist: dotmotif>=0.14.0
 Requires-Dist: networkx>=3.2.1
+Requires-Dist: tamarind>=0.2.1
+Requires-Dist: py2neo>=2021.2.4
 
 # AutoMotif: Automated Motif Detection in Network Graphs
 ## What is it?
 AutoMotif streamlines the identification and cataloging of motifs within network graphs. Utilizing NetworkX for graph manipulation, dotmotif for detecting motifs, and pandas for data management, it simplifies the process of uncovering patterns across both directed and undirected networks. Users can customize searches based on motif size, directionality, executors and the treatment of automorphisms, as well as even having the option to save the results for further analysis.
 
 ## Installation
 
@@ -27,28 +29,31 @@
 ```python
 from automotif import AutoMotif
 from dotmotif import executors
 import networkx as nx
 # Example: A random directed graph
 G = nx.gnp_random_graph(100, 0.5, directed=True)
 # Set up AutoMotif
-motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True, use_GrandISO = True)
+motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True, use_GrandISO=True)
 # Start finding motifs
 motifs = motif_finder.find_all_motifs()
 # Calculate the Z-Score for the motifs
 z_scores = motif_finder.calculate_zscore(num_random_graphs = 30, Executor = executors.NetworkXExecutor)
+# Display the motifs found
+motif_finder.display_all_motifs()
 ```
 ## Features
-- **Automated Detection**: AutoMotif automates the detection of motifs, eliminating the need for manual parameter adjustments. It's designed to be efficient and user-friendly, allowing researchers to focus more on analysis and less on setup.
+- **Automated Detection**: AutoMotif automates the detection of motifs, eliminating the need for manual parameter adjustments. It's designed to be efficient and user-friendly, allowing users to focus more on analysis and less on setup.
 - **Flexible and Powerful**: Capable of handling both directed and undirected graphs, AutoMotif provides flexibility in defining motifs, including size and whether to consider automorphisms, ensuring a broad applicability across different types of network analyses.
 - **Data Organization and Export**: Directly save your motifs to CSV files for easy access, further analysis, or sharing with your team or research community.
 - **Z-Score Calculation**: Assess the statistical significance of detected motifs by calculating their Z-scores, providing insights into the rarity or commonality of patterns within your network compared to random expectations.
+- **Visual Representation**: AutoMotif includes features for visualizing network motifs, allowing users to display them as graphs within the application. This aids in the qualitative analysis of motifs, offering a graphical representation of network patterns and their connections for easier interpretation and presentation.
 ## Contributions
 We encourage contributions to AutoMotif! If you have ideas for improvements or new features, don't hesitate to open an issue or submit a pull request on our repository.
 ## License
 AutoMotif is made available under the MIT License. See the LICENSE file for more details.
 ***
 ## Who made this? 
 AutoMotif was developed by Giorgio Micaletto under the guidance of Professor Marta Zava at Bocconi University. This tool is designed to simplify and facilitate the complex process of network motif analysis.
 Contacts:
 - giorgio.micaletto@studbocconi.it
-- [linkedin](linkedin.com/in/giorgio-micaletto/)
+- [LinkedIn](linkedin.com/in/giorgio-micaletto/)
```

### Comparing `automotifs-1.1.1/setup.py` & `automotifs-1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """This module sets up the package for distribution."""
 from setuptools import setup, find_packages
 setup(
     name='automotifs',
-    version='1.1.1',
+    version='1.2',
     packages=find_packages(),
     description='A wrapper for automatic Motif Detection',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/auto_dotmotif/',
     install_requires=[
         'pandas>=1.1.5',
         'pylint>=2.6.0',
         'numpy>=1.23',
         'dotmotif>=0.14.0',
-        'networkx>=3.2.1'
+        'networkx>=3.2.1',
+        'tamarind>=0.2.1',
+        'py2neo>=2021.2.4',
     ],
     python_requires='>=3.6',
 )
```

### Comparing `automotifs-1.1.1/tests/test.py` & `automotifs-1.2/tests/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Module containing test cases for the package."""
 import unittest
 import networkx as nx
 from automotif import AutoMotif
 class TestAutoMotif(unittest.TestCase):
-
     def setUp(self):
         self.graph = nx.DiGraph()
         self.graph.add_edges_from([(1, 2), (2, 3), (3, 1)])
 
     def test_initialization(self):
         """Test whether the AutoMotif class initializes correctly with basic parameters."""
         automotif = AutoMotif(Graph=self.graph, size=3)
```

