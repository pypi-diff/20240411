# Comparing `tmp/nnsom-1.5.4.tar.gz` & `tmp/nnsom-1.5.5.tar.gz`

## Comparing `nnsom-1.5.4.tar` & `nnsom-1.5.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    77087 2020-02-02 00:00:00.000000 nnsom-1.5.4/src/NNSOM/plots.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 nnsom-1.5.4/src/NNSOM/som.py
--rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.4/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.4/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.4/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0    80117 2020-02-02 00:00:00.000000 nnsom-1.5.5/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 nnsom-1.5.5/src/NNSOM/som.py
+-rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.5/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.5/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.5/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.5/PKG-INFO
```

### Comparing `nnsom-1.5.4/src/NNSOM/plots.py` & `nnsom-1.5.5/src/NNSOM/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1300,14 +1300,81 @@
                     color = plt.cm.viridis(norm(feature_weights[j]))  # Choose colormap as viridis
                     inverted_color = tuple(
                         1 - np.array(color[:3]))  # Invert the color to make darker colors represent larger weights
                     ax.fill(pos[0, j] + shapex, pos[1, j] + shapey, facecolor=inverted_color, edgecolor=(0.8, 0.8, 0.8))
 
         plt.show()
 
+    def weight_as_image(self, mouse_click=False, connect_pick_event=True, **kwargs):
+        w = self.w  # Weight matrix
+        pos = self.pos  # Positions of the neurons
+        numNeurons = self.numNeurons  # Number of neurons
+
+        # Get the shape of a single hexagon
+        shapex, shapey = get_hexagon_shape()
+
+        # Create the figure and axis with a larger size to accommodate the decorations
+        fig, ax = plt.subplots(figsize=(8, 6))
+
+        # Set the aspect of the plot to be equal
+        plt.axis('equal')
+
+        # List to keep track of the hexagon patches
+        patches = []
+
+        for i in range(numNeurons):
+            hex_center_x = pos[0, i]  # x coordinate of the ith position
+            hex_center_y = pos[1, i]  # y coordinate of the ith position
+
+            # Draw the hexagon
+            temp, = ax.fill(hex_center_x + shapex, hex_center_y + shapey, facecolor='none', edgecolor='k', picker=True)
+            patches.append(temp)
+
+            # Assign the cluster number for each hexagon
+            hexagon_to_neuron = {hex: neuron for neuron, hex in enumerate(patches)}
+
+            # Transform the row of weights into a matrix if necessary
+            weight_matrix = w[i].reshape((int(np.sqrt(w.shape[1])), -1))  # Assuming square matrix for simplicity
+
+            # Calculate the size and position for the imshow plot
+            # Find the radius of the hexagon, accounting for the scaling of the shape
+            hex_radius = (np.max(shapex) - np.min(shapex)) / 2
+
+            # Calculate the side length of the hexagon for a regular hexagon
+            side_length = hex_radius * np.sqrt(3) / 2
+
+            # Offset the inset_axes to be centered within the hexagon
+            # The factor of sqrt(3)/2 is because in a regular hexagon, the distance from the center to a side is sqrt(3)/2 times the side length
+            axins = ax.inset_axes([hex_center_x - side_length / 2,
+                                   hex_center_y - side_length * (np.sqrt(3) / 2) / 2,
+                                   side_length,
+                                   side_length * (np.sqrt(3) / 2)], transform=ax.transData)
+
+            # Ensure the imshow plot takes up the correct amount of space
+            # Adjust aspect ratio if necessary, depending on the weight matrix shape
+            aspect_ratio = weight_matrix.shape[0] / weight_matrix.shape[1]
+            axins.imshow(weight_matrix, aspect='equal')
+            axins.set_aspect(aspect_ratio * (side_length / (side_length * (np.sqrt(3) / 2))))
+
+            # Turn off the axis
+            axins.axis('off')
+
+        # Connect the pick event for interactivity if required
+        if mouse_click and connect_pick_event:
+            fig.canvas.mpl_connect('pick_event', lambda event: self.onpick(event, patches,hexagon_to_neuron, **kwargs))
+
+        # Adjust the layout to fit everything
+        plt.tight_layout()
+
+        # Display the plot
+        plt.show()
+
+        # Return the figure components
+        return fig, ax, patches
+
     # Generic Plot Function
     def plot(self, plot_type, data_dict=None, ind=None, target_class=None, use_add_1darray=False,
              use_add_2darray=False, **kwargs):
         """ Generic Plot Function.
         It generates a plot based on the plot type and data provides.
 
         Parameters
```

### Comparing `nnsom-1.5.4/src/NNSOM/som.py` & `nnsom-1.5.5/src/NNSOM/som.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,43 +428,49 @@
         """
         Calculate quantization error
         """
         quant_err = np.array([0 if len(item) == 0 else np.mean(item) for item in dist]).mean()
 
         return quant_err
 
-    def topological_error(self, data):
+    def topological_error(self, x):
         """
         Calculate topological error
         """
         w = self.w
         ndist = self.neuron_dist
 
+        # Normalize Input
+        x = self.normalize(x, self.norm_func)
+
         # Calculate the distance between item vs. cluster center
-        x_w_dist = cdist(w, np.transpose(data), 'euclidean')
+        x_w_dist = cdist(w, np.transpose(x), 'euclidean')
 
         sort_dist = np.argsort(x_w_dist, axis=0)
         top_dist = [ndist[sort_dist[0, ii], sort_dist[1, ii]] for ii in range(sort_dist.shape[1])]
         neighbors = np.where(np.array(top_dist) > 1.1)
         top_error_1st = 100 * len(neighbors[0]) / x_w_dist.shape[1]
         neighbors = np.where(np.array(top_dist) > 2.1)
         top_error_1st_and_2nd = 100 * len(neighbors[0]) / x_w_dist.shape[1]
 
         return top_error_1st, top_error_1st_and_2nd
 
-    def distortion_error(self, data):
+    def distortion_error(self, x):
         """
         Calculate distortion
         """
-        shapx = data.shape
+        # Normalize input data
+        x = self.normalize(x, self.norm_func)
+
+        shapx = x.shape
         Q = shapx[1]  # Number of samples
 
         ww = self.w
         ndist = self.neuron_dist
-        x_w_dist = cdist(ww, np.transpose(data), 'euclidean')
+        x_w_dist = cdist(ww, np.transpose(x), 'euclidean')
         ind1 = np.argmin(x_w_dist, axis=0)
 
         dd = [1, 2, 3]  # neighborhood distances
         wwdist = cdist(ww, ww, 'euclidean')
         sst = ndist[:, ind1]
 
         for d in dd:
```

### Comparing `nnsom-1.5.4/src/NNSOM/utils.py` & `nnsom-1.5.5/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.4/.gitignore` & `nnsom-1.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.4/pyproject.toml` & `nnsom-1.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.5.4"
+version = "1.5.5"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.5.4/PKG-INFO` & `nnsom-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.5.4
+Version: 1.5.5
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

