# Comparing `tmp/quantminer-0.3.0.tar.gz` & `tmp/quantminer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantminer-0.3.0.tar", last modified: Wed Apr 10 21:11:22 2024, max compression
+gzip compressed data, was "quantminer-0.3.1.tar", last modified: Wed Apr 10 21:17:35 2024, max compression
```

## Comparing `quantminer-0.3.0.tar` & `quantminer-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:11:22.601206 quantminer-0.3.0/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 21:11:22.601090 quantminer-0.3.0/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.3.0/pyproject.toml
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:11:22.599569 quantminer-0.3.0/quantminer/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.3.0/quantminer/__init__.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:11:22.600711 quantminer-0.3.0/quantminer/classes/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.3.0/quantminer/classes/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.3.0/quantminer/classes/pivot_pip.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.3.0/quantminer/classes/seqkmeans.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    18829 2024-04-10 21:09:44.000000 quantminer-0.3.0/quantminer/pipminer.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:11:22.600079 quantminer-0.3.0/quantminer.egg-info/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/SOURCES.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/dependency_links.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/requires.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-10 21:11:22.000000 quantminer-0.3.0/quantminer.egg-info/top_level.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-10 21:11:22.601247 quantminer-0.3.0/setup.cfg
--rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-10 21:10:56.000000 quantminer-0.3.0/setup.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:17:35.655459 quantminer-0.3.1/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 21:17:35.655284 quantminer-0.3.1/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.3.1/pyproject.toml
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:17:35.649689 quantminer-0.3.1/quantminer/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.3.1/quantminer/__init__.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:17:35.654357 quantminer-0.3.1/quantminer/classes/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.3.1/quantminer/classes/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.3.1/quantminer/classes/pivot_pip.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.3.1/quantminer/classes/seqkmeans.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    18877 2024-04-10 21:16:30.000000 quantminer-0.3.1/quantminer/pipminer.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-10 21:17:35.650722 quantminer-0.3.1/quantminer.egg-info/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/requires.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-10 21:17:35.000000 quantminer-0.3.1/quantminer.egg-info/top_level.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-10 21:17:35.655677 quantminer-0.3.1/setup.cfg
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-10 21:16:43.000000 quantminer-0.3.1/setup.py
```

### Comparing `quantminer-0.3.0/quantminer/classes/pivot_pip.py` & `quantminer-0.3.1/quantminer/classes/pivot_pip.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.3.0/quantminer/classes/seqkmeans.py` & `quantminer-0.3.1/quantminer/classes/seqkmeans.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.3.0/quantminer/pipminer.py` & `quantminer-0.3.1/quantminer/pipminer.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,21 @@
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 
 
 class Miner:
     def __init__(self, 
                  n_lookback: int, 
                  n_pivots: int, 
-                 hold_period: int = 6, 
+                 n_clusters: int = 8,
+                 hold_period: int = 6,
                  model_type:Literal['standard', 'ts', 'sequential']='standard') -> None:
         self.n_lookback = n_lookback
         self.n_pivots = n_pivots
         self.hold_period = hold_period
+        self.n_cluster = n_clusters
 
         self._model_type = model_type
 
         # Store Training Data
         self._data: List = []
         self._data_train_X: Union[List, np.ndarray] = []
         self._data_train_y: Union[List, np.ndarray] = []
@@ -46,15 +48,15 @@
         # Store the dimensionality reduction agent
         self._agent_reduce: PIP = None
 
         # Store the clustering agent
         self._agent_cluster = None
 
         # Preset attributes
-        self._n_cluster = 8
+        
         self._random_state = 0
 
 
     def fit(self, data: np.ndarray):
         # Set the random state
         np.random.seed(self._random_state)
 
@@ -151,15 +153,14 @@
         _l = self._agent_cluster.predict(_pivots)
         indices = _unique_indices + self.n_lookback - 1
         _labels = self._assign_cluster_labels(data, _l, indices)
 
         return _labels
         
 
-
     def generate_signal(self, data: List[np.ndarray]):
         """
         This generates signal for one data window.
 
         Return:
             signal, pivots : Tuple containing the predicted signal, and the list of pivots points.
         """
@@ -331,34 +332,34 @@
 
 
     def _generate_clusters(self):
         """
         Cluster the training data. Default n_clusters
         """
         
-        # self._n_cluster = self.__find_n_clusters()
+        # self.n_cluster = self.__find_n_clusters()
         
         # SKTime (TSLearn) Kmeans
         if self._model_type == 'ts':
-            self._agent_cluster = TimeSeriesKMeansTslearn(n_clusters=self._n_cluster,
+            self._agent_cluster = TimeSeriesKMeansTslearn(n_clusters=self.n_cluster,
                                     metric='euclidean',
                                     n_jobs=-1,
                                     random_state=self._random_state,
                                     )
 
         elif self._model_type == 'standard':
             self._agent_cluster = KMeans(
-                n_clusters=self._n_cluster,
+                n_clusters=self.n_cluster,
                 n_init="auto",
                 random_state=self._random_state,
                 )
 
         elif self._model_type == "sequential":
             self._agent_cluster = SeqKMeans(
-                n_clusters=self._n_cluster, 
+                n_clusters=self.n_cluster, 
                 learning_rate=0.5, 
                 centroid_update_threshold_std=3, 
                 verbose=False,
                 fit_method='sequential',
                 random_state=self._random_state,
                 )
 
@@ -418,15 +419,15 @@
         # Compute the returns
         _returns = np.diff(self._data, prepend=self._data[0])
 
         # Get the cluster labels
         _labels = self._cluster_labels
 
         # Iterate through each cluster label
-        for _label in range(self._n_cluster):
+        for _label in range(self.n_cluster):
             # Create a mask for the label in the labels; everything else should be zero
             mask_label: np.ndarray = _labels == _label
 
             # Filter the labels
             _signals = mask_label.astype(int)
 
             # Implement Holding Period
```

### Comparing `quantminer-0.3.0/setup.py` & `quantminer-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='quantminer',
-    version='0.3.0', 
+    version='0.3.1', 
     description='Data/Pattern Mining Algorithms for Financial Data',
     author='Jerry Inyang',
     author_email='jerprog0@gmail.com',
     packages=find_packages(),  # Automatically finds your package
     install_requires=[  # List any dependencies here
         "kneed",
         "quantstats",
```

