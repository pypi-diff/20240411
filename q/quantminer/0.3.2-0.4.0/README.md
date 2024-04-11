# Comparing `tmp/quantminer-0.3.2.tar.gz` & `tmp/quantminer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantminer-0.3.2.tar", last modified: Thu Apr 11 02:05:26 2024, max compression
+gzip compressed data, was "quantminer-0.4.0.tar", last modified: Thu Apr 11 15:25:44 2024, max compression
```

## Comparing `quantminer-0.3.2.tar` & `quantminer-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 02:05:26.517655 quantminer-0.3.2/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 02:05:26.517538 quantminer-0.3.2/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.3.2/pyproject.toml
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 02:05:26.515715 quantminer-0.3.2/quantminer/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.3.2/quantminer/__init__.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 02:05:26.517215 quantminer-0.3.2/quantminer/classes/
--rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.3.2/quantminer/classes/__init__.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.3.2/quantminer/classes/pivot_pip.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.3.2/quantminer/classes/seqkmeans.py
--rw-r--r--   0 jerryinyang   (501) staff       (20)    18864 2024-04-11 02:04:50.000000 quantminer-0.3.2/quantminer/pipminer.py
-drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 02:05:26.516620 quantminer-0.3.2/quantminer.egg-info/
--rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/PKG-INFO
--rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/SOURCES.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/dependency_links.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/requires.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-11 02:05:26.000000 quantminer-0.3.2/quantminer.egg-info/top_level.txt
--rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-11 02:05:26.517699 quantminer-0.3.2/setup.cfg
--rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-11 02:04:39.000000 quantminer-0.3.2/setup.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 15:25:44.546450 quantminer-0.4.0/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 15:25:44.546335 quantminer-0.4.0/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      258 2024-04-10 10:17:30.000000 quantminer-0.4.0/pyproject.toml
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 15:25:44.544686 quantminer-0.4.0/quantminer/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       34 2024-04-10 11:41:22.000000 quantminer-0.4.0/quantminer/__init__.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 15:25:44.545817 quantminer-0.4.0/quantminer/classes/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       73 2024-04-10 11:38:53.000000 quantminer-0.4.0/quantminer/classes/__init__.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)     2718 2024-04-10 11:32:09.000000 quantminer-0.4.0/quantminer/classes/pivot_pip.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    13017 2024-04-10 04:48:20.000000 quantminer-0.4.0/quantminer/classes/seqkmeans.py
+-rw-r--r--   0 jerryinyang   (501) staff       (20)    21815 2024-04-11 15:25:32.000000 quantminer-0.4.0/quantminer/pipminer.py
+drwxr-xr-x   0 jerryinyang   (501) staff       (20)        0 2024-04-11 15:25:44.545210 quantminer-0.4.0/quantminer.egg-info/
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      167 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/PKG-INFO
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      333 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)        1 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       89 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/requires.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       11 2024-04-11 15:25:44.000000 quantminer-0.4.0/quantminer.egg-info/top_level.txt
+-rw-r--r--   0 jerryinyang   (501) staff       (20)       38 2024-04-11 15:25:44.546486 quantminer-0.4.0/setup.cfg
+-rw-r--r--   0 jerryinyang   (501) staff       (20)      600 2024-04-11 15:23:37.000000 quantminer-0.4.0/setup.py
```

### Comparing `quantminer-0.3.2/quantminer/classes/pivot_pip.py` & `quantminer-0.4.0/quantminer/classes/pivot_pip.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.3.2/quantminer/classes/seqkmeans.py` & `quantminer-0.4.0/quantminer/classes/seqkmeans.py`

 * *Files identical despite different names*

### Comparing `quantminer-0.3.2/quantminer/pipminer.py` & `quantminer-0.4.0/quantminer/pipminer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pickle  # noqa
 import warnings
 
 from pathlib import Path
-from typing import List, Literal, Union
+from typing import List, Literal, Optional, Union
 
 import matplotlib.pyplot as plt 
 import numpy as np
 import pandas as pd
 import quantstats as qt
 from kneed import KneeLocator
 from sklearn.cluster import Birch, KMeans
@@ -215,14 +215,62 @@
                 print(f'Model Loaded from : {path}')
             except Exception as e:
                 raise e
         
         return miner 
 
 
+    def apply_holding_period(self, labels, hold_period:Optional[int]=-1, selected_labels:Optional[List]=None):
+        """
+        Applies a holding period to selected cluster labels, ensuring that consecutive occurrences of the same label are separated by the specified time.
+
+        Args:
+            labels (numpy.ndarray): An array of cluster labels representing the labeling sequence.
+            hold_period (int, optional): The minimum number of time steps required between consecutive 
+                                        occurrences of the same label. If -1, uses the value stored in  
+                                        `self.hold_period`. Defaults to -1.
+            selected_labels (List, optional):  A list of specific cluster labels to apply the holding 
+                                            period to. If None, applies to all cluster labels. 
+                                            Defaults to None.
+
+        Returns:
+            numpy.ndarray: A new array of labels with the holding period applied. Unmodified labels are
+                        assigned a value of -1.
+        """
+        n_clusters = self.n_cluster
+
+        # If no holding period is passed, use self.hold_period
+        if hold_period <= 0:
+            hold_period = self.hold_period
+
+        # If no specific labels are passed, apply the holding period to all cluster labels
+        if (selected_labels is None) or (len(selected_labels) == 0):
+            selected_labels = list(range(n_clusters))
+
+        labels = np.array(labels)
+
+        valid_indices = np.where(np.isin(labels, selected_labels))[0]
+        new_labels = np.ones_like(labels) * -1
+
+        prev_index = -hold_period - 1
+        for index in valid_indices:
+            label = labels[index]
+            
+            # Ensure no overlapping labels
+            if (index > prev_index + hold_period):
+                prev_index = index
+
+                start_index = index + 1
+                end_index = min(index + hold_period + 1, len(labels))
+
+                new_labels[start_index:end_index] = label
+
+        return new_labels
+
+
     def _preprocess_data(self, data, **kwargs):
         """
         Perform series-level data transformations. These can include detrending, denoising/filtering, domain transformations.
         The parameters of these transformations are saved, to be used for new data.
         """
 
         if kwargs.get("test_mode", False):
@@ -481,24 +529,49 @@
 
         # Clear Clusters Assignments
         self._unique_pip_indices = []
         self._cluster_labels = []
 
 
     def __apply_holding_period(self, signals):
-        """Apply holding period logic to signals."""
-        prev = 0
+        """
+        Applies a holding period to a set of trading signals, enforcing a delay between 
+        consecutive non-zero signals.
+
+        This function is likely used in trading strategies to prevent overly frequent 
+        trades, potentially reducing transaction costs and mitigating the effects of 
+        temporary market noise.
+
+        Args:
+            signals (numpy.ndarray): An array containing trading signals (e.g., buy/sell). 
+
+        Returns:
+            numpy.ndarray: An array of signals with the holding period applied. 
+                        Non-zero signals will be followed by a specified number of
+                        zero signals.  
+        """
+        
+        signals = np.array(signals)
+
+        nonzero = np.where(signals != 0)[0]
+        new_signals = np.zeros_like(signals)
+
+        prev_index = -self.hold_period - 1
+        for index in nonzero:
+            signal = signals[index]
+            
+            if (index > prev_index + self.hold_period):
+                prev_index = index
 
-        for index, signal in enumerate(signals):
-            if (signal != 0) and (index > (prev + self.hold_period)):
-                prev = index
+                start_index = index + 1
                 end_index = min(index + self.hold_period + 1, len(signals))
-                signals[index + 1 : end_index] = signal
-                signals[index] = 0
-        return signals
+
+                new_signals[start_index:end_index] = signal
+
+        return new_signals
 
 
     def __compute_martin(self, rets: np.array):
     
         rsum = np.sum(rets)
         short = False
         if rsum < 0.0:
@@ -618,11 +691,11 @@
     # miner = Miner(25, 5)
     # miner.fit(train_data)
 
     # miner.save_model(parent_path / 'pipminer.pkl')
 
     miner : Miner = Miner.load_model(parent_path / 'pipminer.pkl')
 
-    print(miner.transform(test_data))
+    # print(miner.transform(test_data))
 
-    # miner.test(test_data)
+    miner.test(test_data)
     print('Successful')
```

### Comparing `quantminer-0.3.2/setup.py` & `quantminer-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='quantminer',
-    version='0.3.2', 
+    version='0.4.0', 
     description='Data/Pattern Mining Algorithms for Financial Data',
     author='Jerry Inyang',
     author_email='jerprog0@gmail.com',
     packages=find_packages(),  # Automatically finds your package
     install_requires=[  # List any dependencies here
         "kneed",
         "quantstats",
```

