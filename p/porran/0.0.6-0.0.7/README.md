# Comparing `tmp/porran-0.0.6.tar.gz` & `tmp/porran-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porran-0.0.6.tar", last modified: Thu Apr  4 12:27:49 2024, max compression
+gzip compressed data, was "porran-0.0.7.tar", last modified: Thu Apr 11 14:55:00 2024, max compression
```

## Comparing `porran-0.0.6.tar` & `porran-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 12:27:49.925570 porran-0.0.6/
--rw-rw-rw-   0        0        0     1090 2024-03-19 11:55:51.000000 porran-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1807 2024-04-04 12:27:49.923569 porran-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2024-04-04 09:21:13.000000 porran-0.0.6/README.md
--rw-rw-rw-   0        0        0      695 2024-04-04 12:26:17.000000 porran-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 12:27:49.926568 porran-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 12:27:49.817525 porran-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 12:27:49.883177 porran-0.0.6/src/porran/
--rw-rw-rw-   0        0        0       53 2024-04-04 09:21:13.000000 porran-0.0.6/src/porran/__init__.py
--rw-rw-rw-   0        0        0     4297 2024-04-04 09:21:13.000000 porran-0.0.6/src/porran/create_structure.py
--rw-rw-rw-   0        0        0     3125 2024-04-04 09:24:44.000000 porran-0.0.6/src/porran/get_zeolite.py
--rw-rw-rw-   0        0        0     3075 2024-03-20 15:16:29.000000 porran-0.0.6/src/porran/graph_creation.py
--rw-rw-rw-   0        0        0     4812 2024-04-04 09:21:13.000000 porran-0.0.6/src/porran/mask_method.py
--rw-rw-rw-   0        0        0    14187 2024-04-04 09:27:29.000000 porran-0.0.6/src/porran/porran.py
--rw-rw-rw-   0        0        0     6548 2024-03-20 15:16:29.000000 porran-0.0.6/src/porran/replacement_algorithms.py
--rw-rw-rw-   0        0        0     7163 2024-04-04 09:21:13.000000 porran-0.0.6/src/porran/transformations.py
--rw-rw-rw-   0        0        0     3503 2024-04-04 12:23:09.000000 porran-0.0.6/src/porran/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:27:49.920569 porran-0.0.6/src/porran.egg-info/
--rw-rw-rw-   0        0        0     1807 2024-04-04 12:27:49.000000 porran-0.0.6/src/porran.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2024-04-04 12:27:49.000000 porran-0.0.6/src/porran.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 12:27:49.000000 porran-0.0.6/src/porran.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-04 12:27:49.000000 porran-0.0.6/src/porran.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-04 12:27:49.000000 porran-0.0.6/src/porran.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:55:00.904414 porran-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2024-03-19 11:55:51.000000 porran-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1807 2024-04-11 14:55:00.901416 porran-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2024-04-04 09:21:13.000000 porran-0.0.7/README.md
+-rw-rw-rw-   0        0        0      695 2024-04-11 14:48:15.000000 porran-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:55:00.905418 porran-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 14:55:00.738840 porran-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:55:00.857762 porran-0.0.7/src/porran/
+-rw-rw-rw-   0        0        0       53 2024-04-11 14:48:18.000000 porran-0.0.7/src/porran/__init__.py
+-rw-rw-rw-   0        0        0     5725 2024-04-11 14:32:04.000000 porran-0.0.7/src/porran/create_structure.py
+-rw-rw-rw-   0        0        0     3125 2024-04-04 09:24:44.000000 porran-0.0.7/src/porran/get_zeolite.py
+-rw-rw-rw-   0        0        0     3075 2024-03-20 15:16:29.000000 porran-0.0.7/src/porran/graph_creation.py
+-rw-rw-rw-   0        0        0     4812 2024-04-04 09:21:13.000000 porran-0.0.7/src/porran/mask_method.py
+-rw-rw-rw-   0        0        0    14612 2024-04-11 14:39:12.000000 porran-0.0.7/src/porran/porran.py
+-rw-rw-rw-   0        0        0     8849 2024-04-11 14:42:02.000000 porran-0.0.7/src/porran/replacement_algorithms.py
+-rw-rw-rw-   0        0        0     7163 2024-04-04 09:21:13.000000 porran-0.0.7/src/porran/transformations.py
+-rw-rw-rw-   0        0        0     3503 2024-04-04 12:23:09.000000 porran-0.0.7/src/porran/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:55:00.899879 porran-0.0.7/src/porran.egg-info/
+-rw-rw-rw-   0        0        0     1807 2024-04-11 14:55:00.000000 porran-0.0.7/src/porran.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2024-04-11 14:55:00.000000 porran-0.0.7/src/porran.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:55:00.000000 porran-0.0.7/src/porran.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-11 14:55:00.000000 porran-0.0.7/src/porran.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 14:55:00.000000 porran-0.0.7/src/porran.egg-info/top_level.txt
```

### Comparing `porran-0.0.6/LICENSE` & `porran-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `porran-0.0.6/PKG-INFO` & `porran-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porran
-Version: 0.0.6
+Version: 0.0.7
 Summary: PORous RANdom crystal structure generation
 Author-email: Marko Petkovic <m.petkovic1@tue.nl>, Koen Wortelboer <k.a.wortelboer1@tue.nl>
 Project-URL: Home-page, https://github.com/marko-petkovic/porran
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `porran-0.0.6/README.md` & `porran-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `porran-0.0.6/pyproject.toml` & `porran-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "porran"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   {name="Marko Petkovic", email="m.petkovic1@tue.nl" },
   {name="Koen Wortelboer", email="k.a.wortelboer1@tue.nl"}
 ]
 description = "PORous RANdom crystal structure generation"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `porran-0.0.6/src/porran/create_structure.py` & `porran-0.0.7/src/porran/create_structure.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import List, Optional
 
 import numpy as np
 from pymatgen.core import Molecule, Structure
+from scipy import spatial
 
 from .transformations import rotation_axis_angle
 
 logger = logging.getLogger(__name__)
 
 
 def create_zeo(structure: Structure, mask, replacement_inds, *args, **kwargs):
@@ -51,17 +52,29 @@
     """Create a MOF with added functional groups.
 
     Parameters
     ----------
     structure : Structure
         The MOF to add functional groups to.
     mask : np.ndarray
-        _description_
+        Mask to select atoms to be replaced
     replacement_inds : np.ndarray
-        _description_
+        Indices to replace within the structure graph.
+    dopants: Molecule | List[Molecule]
+        Molecule(s) representing the functional groups to add. If a
+        single Molecule is provided, then that is used for all
+        replacements. If a List, it must have the same length as
+        replacement_inds.
+    max_attempts: int
+        A random rotation is applied to the dopant to avoid overlap with
+        existing sites at most max_attempts times. If there is still
+        overlap after that, the dopant is not placed and a warning is
+        logged.
+    rng: np.random.Generator, optional
+        Generator for random rotations.
     """
     if rng is None:
         rng = np.random.default_rng()
 
     max_ch_bond_length: float = 1.15  # Angstrom
 
     # if dopants is a single Molecule, copy it replacement_inds times
@@ -96,29 +109,45 @@
         structure_copy.remove_sites([h_i])
 
         # try to add the dopant to the structure
         for _ in range(max_attempts):
             dopant.rotate_sites(
                 theta=rng.uniform(0, 2 * np.pi), axis=direction, anchor=location
             )
-            try:
-                for site in dopant:
-                    structure_copy.append(
-                        species=site.species,
-                        coords=site.coords,
-                        coords_are_cartesian=True,
-                        validate_proximity=True,
-                        properties=site.properties,
-                    )
-                break
-            except ValueError as e:
-                # only catch the error if it is about proximity
-                if e.args[0] == "New site is too close to an existing site!":
-                    continue
-                raise e
+
+            # check for overlap with existing atoms
+            # get the fractional coordinates of the dopants.
+            d_frac = structure_copy.lattice.get_fractional_coords(
+                cart_coords=dopant.cart_coords
+            )
+            # calculate the distances between dopant and structure atoms
+            # along the lattice dimensions, taking periodic boundaries
+            # into account
+            frac_dists = np.abs(structure_copy.frac_coords[:, None] - d_frac)
+            frac_dists = np.where(frac_dists > 0.5, np.abs(1 - frac_dists), frac_dists)
+            # convert to cartesian distances
+            cart_dists = structure_copy.lattice.get_cartesian_coords(
+                fractional_coords=frac_dists
+            )
+            # calculate square of norm and compare to tolerance
+            if np.any(
+                np.sum(np.square(cart_dists), -1) < structure_copy.DISTANCE_TOLERANCE**2
+            ):
+                continue
+
+            # no overlap, add the dopant
+            for site in dopant:
+                structure_copy.append(
+                    species=site.species,
+                    coords=site.coords,
+                    coords_are_cartesian=True,
+                    validate_proximity=False,
+                    properties=site.properties,
+                )
+            break
         else:
             logger.warning(
                 "Could not add dopant %s to the structure at index %d",
                 dopant.reduced_formula,
                 c_i,
             )
```

### Comparing `porran-0.0.6/src/porran/get_zeolite.py` & `porran-0.0.7/src/porran/get_zeolite.py`

 * *Files identical despite different names*

### Comparing `porran-0.0.6/src/porran/graph_creation.py` & `porran-0.0.7/src/porran/graph_creation.py`

 * *Files identical despite different names*

### Comparing `porran-0.0.6/src/porran/mask_method.py` & `porran-0.0.7/src/porran/mask_method.py`

 * *Files identical despite different names*

### Comparing `porran-0.0.6/src/porran/porran.py` & `porran-0.0.7/src/porran/porran.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     mask_array,
     mask_box,
     mask_combination,
     mask_h_on_c,
     mask_species,
     mask_zeo,
 )
-from .replacement_algorithms import chains, clusters, maximize_entropy, random
+from .replacement_algorithms import multi_clusters, chains, clusters, maximize_entropy, random, random_lowenstein
 from .utils import is_atom, write_cif
 
 
 class PORRAN:
 
     def __init__(
         self,
@@ -151,26 +151,27 @@
         create_algo: Union[str, Callable],
         n_subs: int,
         max_tries: int = 100,
         post_algo: Optional[Callable] = None,
         write: bool = False, overwrite_ok = False,
         writepath: Optional[str] = "structures",
         verbose: bool = True,
+        print_error : bool = False,
         *args,
         **kwargs,
     ) -> List[Structure]:
         """
         Generate structures by replacing nodes in the graph
 
         Parameters
         ----------
         n_structures : int
             Number of structures to generate
         replace_algo : Union[str, Callable]
-            Algorithm to select nodes to replace. If str, it can be 'random', 'clusters', 'chains' or 'maximize_entropy'
+            Algorithm to select nodes to replace. If str, it can be 'random', 'random_lowenstein', 'clusters', 'multi_clusters','chains' or 'maximize_entropy'
         create_algo : Union[str, Callable]
             Algorithm to create the new structure. If str, it can be 'zeolite'
         n_subs : int
             Number of nodes to replace
         max_tries : int, optional
             Maximum number of tries to replace nodes, default is 100
         post_algo : Callable, optional
@@ -212,17 +213,20 @@
         for i in range(n_structures):
 
             # for each structure, try to replace nodes max_tries times
             for j in range(max_tries):
                 try:
                     sub_array = self._replace(n_subs, *args, **kwargs)
                     break
-                except:
+                except Exception as e:
                     sub_array = None
                     total_failed += 1
+                    if print_error:
+                        print(f"Failed to generate new structure: {e}")
+
 
             # if the maximum number of tries is reached, skip the structure
             if sub_array is None:
                 failed += 1
                 continue
 
             new_structure = self.create_algo(
@@ -278,16 +282,20 @@
         else:
             raise ValueError("Unknown mask method")
 
     def _get_replace_algo(self, replace_algo: Union[str, Callable]):
         if isinstance(replace_algo, str):
             if replace_algo == "random":
                 return random
+            elif replace_algo == "random_lowenstein":
+                return random_lowenstein
             elif replace_algo == "clusters":
                 return clusters
+            elif replace_algo == "multi_clusters":
+                return multi_clusters
             elif replace_algo == "chains":
                 return chains
             elif replace_algo == "maximize_entropy":
                 return maximize_entropy
             else:
                 raise ValueError(f"Unknown replace algorithm: {replace_algo}")
         else:
```

### Comparing `porran-0.0.6/src/porran/replacement_algorithms.py` & `porran-0.0.7/src/porran/replacement_algorithms.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,47 @@
     -------
     np.array
         Array of selected nodes
     '''	
     n_nodes = len(G.nodes)
     return np.random.choice(np.arange(n_nodes), n_subs, replace=False)
 
+
+def random_lowenstein(G : nx.Graph, n_subs : int, *args, **kwargs):
+    '''
+    Randomly select n_subs nodes from the graph while obeying the Lowenstein constraint
+    
+    Parameters
+    ----------
+    G : nx.Graph
+        Graph to select nodes from
+    n_subs : int
+        Number of nodes to select
+
+    Returns
+    -------
+    np.array
+        Array of selected nodes
+    '''
+    G = deepcopy(G)
+
+    selected_nodes = set()
+    for i in range(n_subs):
+
+        # Select a random node
+        node = np.random.choice(list(G.nodes))
+        selected_nodes.add(node)
+
+        # Remove the node and its neighbours from the graph
+        G.remove_nodes_from(list(G.neighbors(node)))
+        G.remove_node(node)
+
+    return np.array(list(selected_nodes))
+
+
 def clusters(G : nx.Graph, n_subs : int, node_idx : Optional[int] = None, *args, **kwargs):
     '''
     Selects n_subs nodes around a random node
 
     Parameters
     ----------
     G : nx.Graph
@@ -144,15 +177,68 @@
         
         # remove neighbours of the last node from the graph
         
         neighbours = set(G.neighbors(node_idx))
         G.remove_nodes_from(neighbours)
     
     return np.array(al_subs)
+
+
+def multi_clusters(G : nx.Graph, n_subs : int, cluster_sizes : List[int], make_space : bool = False, *args, **kwargs):
+    '''
+    Selects nodes in multiple clusters of specified sizes
+
+    Parameters
+    ----------
+    G : nx.Graph
+        Graph to select nodes from
+    n_subs : int
+        Number of nodes to select
+    cluster_sizes : List[int]
+        List of cluster sizes to select
+        Sum of cluster sizes should be equal to n_subs
+    make_space : bool, optional
+        If True, clusters cannot be connected, default is False    
+    
+    Returns
+    -------
+    np.array
+        Array of selected nodes
+    '''
+        
+    G = deepcopy(G)
+
+    if n_subs != sum(cluster_sizes):
+        raise ValueError('Sum of cluster sizes should be equal to n_subs')
+    
+    al_subs = []
+
+    for cluster in cluster_sizes:
+        
+        new_al_subs = clusters(G, cluster, *args, **kwargs)
+        
+        if make_space:
+            to_be_removed = set()
+            # remove remaining neighbours of the selected nodes
+            for node in new_al_subs:
+                neighbours = set(G.neighbors(node))
+                to_be_removed = to_be_removed.union(neighbours)
+        
+            to_be_removed = to_be_removed.difference(new_al_subs)
+            G.remove_nodes_from(to_be_removed)
+
+        # remove selected nodes from the graph
+        G.remove_nodes_from(new_al_subs)
+
+        al_subs.extend(new_al_subs)
+
+    return np.array(al_subs)
         
+
+
 def maximize_entropy(G : nx.Graph, n_subs : int, stochastic : bool = False, scaling : float = 1.0, *args, **kwargs):	
     '''
     Selects nodes to maximize the entropy of the selected nodes
 
     Parameters
     ----------
     G : nx.Graph
```

### Comparing `porran-0.0.6/src/porran/transformations.py` & `porran-0.0.7/src/porran/transformations.py`

 * *Files identical despite different names*

### Comparing `porran-0.0.6/src/porran/utils.py` & `porran-0.0.7/src/porran/utils.py`

 * *Files identical despite different names*

### Comparing `porran-0.0.6/src/porran.egg-info/PKG-INFO` & `porran-0.0.7/src/porran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porran
-Version: 0.0.6
+Version: 0.0.7
 Summary: PORous RANdom crystal structure generation
 Author-email: Marko Petkovic <m.petkovic1@tue.nl>, Koen Wortelboer <k.a.wortelboer1@tue.nl>
 Project-URL: Home-page, https://github.com/marko-petkovic/porran
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

