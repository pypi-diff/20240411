# Comparing `tmp/nnsom-1.5.3.tar.gz` & `tmp/nnsom-1.5.4.tar.gz`

## Comparing `nnsom-1.5.3.tar` & `nnsom-1.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    77087 2020-02-02 00:00:00.000000 nnsom-1.5.3/src/NNSOM/plots.py
--rw-r--r--   0        0        0    13419 2020-02-02 00:00:00.000000 nnsom-1.5.3/src/NNSOM/som.py
--rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.3/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.3/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.3/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0    77087 2020-02-02 00:00:00.000000 nnsom-1.5.4/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 nnsom-1.5.4/src/NNSOM/som.py
+-rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.4/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.4/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.4/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.4/PKG-INFO
```

### Comparing `nnsom-1.5.3/src/NNSOM/plots.py` & `nnsom-1.5.4/src/NNSOM/plots.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.3/src/NNSOM/som.py` & `nnsom-1.5.4/src/NNSOM/som.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .utils import *
 import numpy as np
 from tensorflow.keras.utils import to_categorical
 from datetime import datetime
 from scipy.spatial.distance import cdist
 import pickle
+import warnings
 
 class SOM():
     """
-    A class     to represent a Self-Organizing Map (SOM), a type of artificial neural network
+    A class to represent a Self-Organizing Map (SOM), a type of artificial neural network
     trained using unsupervised learning to produce a two-dimensional, discretized representation
     of the input space of the training samples.
 
     Attributes
     ----------
     dimensions : tuple, list, or array-like
         The dimensions of the SOM grid. Determines the layout and number of neurons in the map.
@@ -52,39 +53,61 @@
     save_pickle(self, filename, path, data_format='pkl'):
         Saves the SOM object to a file using the pickle format.
 
     load_pickle(self, filename, path, data_format='pkl'):
         Loads a SOM object from a file using the pickle format.
     """
     def __init__(self, dimensions):
+        """
+        Initializes the SOM with the specified dimensions and calculates the positions and distances between neurons in the SOM grid.
+
+        Parameters
+        ----------
+        dimensions : tuple, list, or np.ndarray
+                    The dimensions (shape) of the SOM grid.
+        """
 
         self.dimensions = dimensions
         self.numNeurons = np.prod(dimensions)
         # Calculate positions of neurons
         self.pos = calculate_positions(dimensions)
         # Calculate distances between neurons
         self.neuron_dist = distances(self.pos)
         # Initialize the weight matrix with empty list
         self.w = []
         # Set simulation flag to True,  needs to do simulation
         self.sim_flag = True
+        # Initialize the output of simulation
+        self.output = None
+        # Initialize a normalize() function
+        self.norm_func = None
 
         # Initialize the dictionary of sub-cluster. {neuron_number(int): sub-clustering SOM obj}
         self.sub_som = {}
 
+    def init_w(self, x, norm_func=None):
+        """
+        Initializes the weights of the SOM using principal components analysis (PCA) on the input data x.
 
-    def init_w(self, x):
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data used for weight initialization.
+        """
         # Initialize SOM weights using principal components
 
         # Print Beginning time for initialization
         print('Beginning Initialization')
         now = datetime.now()
         current_time = now.strftime("%H:%M:%S")
         print("Current Time =", current_time)
 
+        # Normalize the input data
+        x = self.normalize(x, norm_func)
+
         sz = x.shape
 
         posMean = np.mean(x, axis=1)
         posMean = np.expand_dims(posMean, axis=1)
 
         xc = x - posMean
 
@@ -127,14 +150,28 @@
         # Print Ending time for initialization
         print('Ending Initialization')
         now = datetime.now()
         current_time = now.strftime("%H:%M:%S")
         print("Current Time =", current_time)
 
     def sim_som(self, x):
+        """
+        Simulates the SOM with x as the input, determining which neurons are activated by the input vectors.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data to simulate the SOM with.
+
+        Returns
+        -------
+        np.ndarray
+            The simulated output of the SOM.
+        """
+
         # Simulate the SOM, with x as the input
         shapx = x.shape   # shapes of the input x
         shapw = self.w.shape # weights of the SOM
 
         # Compute the negative distance from the inputs to each center
         n = -cdist(self.w, np.transpose(x), 'euclidean')
         # n = np.empty((shapw[0], shapx[1]))
@@ -148,15 +185,36 @@
 
         # Find out which center was closest to the input
         maxRows = np.argmax(n, axis=0)
         a = to_categorical(maxRows, num_classes=n.shape[0]) #made correction-added number of class
         # a = tf.constant(a, shape=[np.transpose(n).shape[0],np.transpose(n).shape[1]])  # made change
         return np.transpose(a)
 
-    def train(self, x, init_neighborhood=3, epochs=200, steps=100):
+    def train(self, x, init_neighborhood=3, epochs=200, steps=100, norm_func=None):
+        """
+        Trains the SOM using the batch SOM algorithm on the input data x.
+
+        Parameters
+        ----------
+        x : np.ndarray
+            The input data to train the SOM with.
+        init_neighborhood : int, optional
+            The initial neighborhood size.
+        epochs : int, optional
+            The number of epochs to train for.
+        steps : int, optional
+            The number of steps for training.
+
+        Returns
+        -------
+        None
+        """
+        # Normalize the input data
+        x = self.normalize(x, norm_func)
+
         # Train the SOM using the batch SOM algorithm
 
         w = self.w
         shapw = w.shape
         S = shapw[0]
         shapx = x.shape
         Q = shapx[1]
@@ -251,17 +309,20 @@
         ValueError
             If the number of features in the input data and the SOM weights do not match.
         """
 
         if self.sim_flag:
             raise ValueError("SOM has not been trained.")
 
-        if x.shape[0] != self.w.shape[1]:
+        if x.shape[1] != self.w.shape[1]:
             raise ValueError('The number of features in the input data and the SOM weights do not match.')
 
+        # Normalize the input data
+        x = self.normalize(x, self.norm_func)
+
         w = self.w
         shapw = w.shape
         S = shapw[0]
 
         x_w_dist = cdist(w, np.transpose(x), 'euclidean')
         ind1 = np.argmin(x_w_dist, axis=0)
 
@@ -292,14 +353,81 @@
 
             # Save the maximum distance to any input in the cluster from cluster center
             if num > 0:
                 max_cluster_distances[i] = tempdist[-1]
 
         return clusters, cluster_distances, max_cluster_distances, cluster_sizes
 
+    def normalize(self, x, norm_func=None):
+        """
+        Normalize the input data using a custom function.
+
+        Parameters
+        ----------
+        x: array-like
+            The input data to be normalized.
+        norm_func: callable, optional
+            A custom normalization or standardization function to be applied to the input data.
+            If provided, it should take the input data as its argument and return the preprocessed data.
+            Default is None, in which case the input data is returned as-is.
+
+        Returns
+        -------
+        x_preprocessed: array-like
+            The preprocessed input data.
+
+        Raises
+        ------
+        Warning
+            If `norm_func` is None, a warning is raised to indicate the potential inefficiency in SOM training.
+
+        Examples
+        --------
+        >>> import numpy as np
+        >>> from sklearn.datasets import load_iris
+        >>> from sklearn.feature_extraction.text import TfidfVectorizer
+        >>> from sklearn.preprocessing import StandardScaler
+
+        >>> # Case 1: Tabular data (without normalization)
+        >>> iris = load_iris()
+        >>> X = iris.data
+        >>> som = SOM(dimensions=(5, 5))
+        >>> X_norm = som.normalize(X)
+        >>> print(np.allclose(np.transpose(X_norm), X))
+        True
+
+        >>> # Case 2: Image data (using custom normalization)
+        >>> image_data = np.random.randint(0, 256, size=(28, 28))
+        >>> som = SOM(dimensions=(10, 10))
+        >>> custom_norm_func = lambda x: x / 255  # Custom normalization function
+        >>> image_data_norm = som.normalize(image_data, norm_func=custom_norm_func)
+        >>> print(image_data_norm.min(), image_data_norm.max())
+        0.0 1.0
+
+        >>> # Case 3: Text data (without normalization)
+        >>> text_data = ["This is a sample text.", "Another example sentence."]
+        >>> vectorizer = TfidfVectorizer()
+        >>> tfidf_matrix = vectorizer.fit_transform(text_data)
+        >>> som = SOM(dimensions=(8, 8))
+        >>> text_data_norm = som.normalize(tfidf_matrix.toarray())
+        >>> print(np.allclose(np.transpose(text_data_norm), tfidf_matrix.toarray()))
+        True
+        """
+
+        if norm_func is not None:
+            x_norm = norm_func(x)  # Use the provided custom normalization function
+            self.norm_func = norm_func
+        else:
+            warnings.warn(
+                "Without normalization function: SOM training may be inefficient if you are not normalized.",
+                UserWarning, stacklevel=2)
+            x_norm = x  # Return the input data as-is
+
+        return np.transpose(x_norm)
+
     def quantization_error(self, dist):
         """
         Calculate quantization error
         """
         quant_err = np.array([0 if len(item) == 0 else np.mean(item) for item in dist]).mean()
 
         return quant_err
@@ -393,8 +521,7 @@
             raise ValueError('data_format must be one of: pkl')
 
         if data_format == 'pkl':
             with open(path + filename, 'rb') as f:
                 som = pickle.load(f)
 
         return som
-
```

### Comparing `nnsom-1.5.3/src/NNSOM/utils.py` & `nnsom-1.5.4/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.3/.gitignore` & `nnsom-1.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.3/pyproject.toml` & `nnsom-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.5.3"
+version = "1.5.4"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.5.3/PKG-INFO` & `nnsom-1.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.5.3
+Version: 1.5.4
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

