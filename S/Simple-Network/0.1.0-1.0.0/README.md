# Comparing `tmp/Simple-Network-0.1.0.tar.gz` & `tmp/Simple-Network-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Simple-Network-0.1.0.tar", last modified: Tue Apr  9 18:18:43 2024, max compression
+gzip compressed data, was "Simple-Network-1.0.0.tar", last modified: Thu Apr 11 02:19:13 2024, max compression
```

## Comparing `Simple-Network-0.1.0.tar` & `Simple-Network-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-09 18:18:43.638439 Simple-Network-0.1.0/
--rw-r--r--   0 admin     (1001) root         (0)     1065 2024-04-09 17:32:21.000000 Simple-Network-0.1.0/LICENSE
--rw-r--r--   0 admin     (1001) root         (0)     6390 2024-04-09 18:18:43.638439 Simple-Network-0.1.0/PKG-INFO
--rw-r--r--   0 admin     (1001) root         (0)     5282 2024-04-09 18:09:56.000000 Simple-Network-0.1.0/README.md
-drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-09 18:18:43.638439 Simple-Network-0.1.0/Simple_Network.egg-info/
--rw-r--r--   0 admin     (1001) root         (0)     6390 2024-04-09 18:18:43.000000 Simple-Network-0.1.0/Simple_Network.egg-info/PKG-INFO
--rw-r--r--   0 admin     (1001) root         (0)      283 2024-04-09 18:18:43.000000 Simple-Network-0.1.0/Simple_Network.egg-info/SOURCES.txt
--rw-r--r--   0 admin     (1001) root         (0)        1 2024-04-09 18:18:43.000000 Simple-Network-0.1.0/Simple_Network.egg-info/dependency_links.txt
--rw-r--r--   0 admin     (1001) root         (0)       13 2024-04-09 18:18:43.000000 Simple-Network-0.1.0/Simple_Network.egg-info/requires.txt
--rw-r--r--   0 admin     (1001) root         (0)        8 2024-04-09 18:18:43.000000 Simple-Network-0.1.0/Simple_Network.egg-info/top_level.txt
--rw-r--r--   0 admin     (1001) root         (0)     1068 2024-04-09 18:09:31.000000 Simple-Network-0.1.0/pyproject.toml
--rw-r--r--   0 admin     (1001) root         (0)       38 2024-04-09 18:18:43.638439 Simple-Network-0.1.0/setup.cfg
--rw-r--r--   0 admin     (1001) root         (0)      667 2024-04-09 18:17:42.000000 Simple-Network-0.1.0/setup.py
-drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-09 18:18:43.638439 Simple-Network-0.1.0/simpleN/
--rw-r--r--   0 admin     (1001) root         (0)       64 2024-04-09 17:44:08.000000 Simple-Network-0.1.0/simpleN/__init__.py
--rw-r--r--   0 admin     (1001) root         (0)     5693 2024-04-09 17:39:55.000000 Simple-Network-0.1.0/simpleN/net.py
--rw-r--r--   0 admin     (1001) root         (0)     3461 2024-04-09 17:39:31.000000 Simple-Network-0.1.0/simpleN/visual.py
+drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/
+-rw-r--r--   0 admin     (1001) root         (0)     1065 2024-04-09 17:32:21.000000 Simple-Network-1.0.0/LICENSE
+-rw-r--r--   0 admin     (1001) root         (0)    12679 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/PKG-INFO
+-rw-r--r--   0 admin     (1001) root         (0)    11615 2024-04-11 01:42:55.000000 Simple-Network-1.0.0/README.md
+drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/Simple_Network.egg-info/
+-rw-r--r--   0 admin     (1001) root         (0)    12679 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/PKG-INFO
+-rw-r--r--   0 admin     (1001) root         (0)      331 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/SOURCES.txt
+-rw-r--r--   0 admin     (1001) root         (0)        1 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/dependency_links.txt
+-rw-r--r--   0 admin     (1001) root         (0)       28 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/requires.txt
+-rw-r--r--   0 admin     (1001) root         (0)        8 2024-04-11 02:19:13.000000 Simple-Network-1.0.0/Simple_Network.egg-info/top_level.txt
+-rw-r--r--   0 admin     (1001) root         (0)     1097 2024-04-11 01:14:06.000000 Simple-Network-1.0.0/pyproject.toml
+-rw-r--r--   0 admin     (1001) root         (0)       38 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/setup.cfg
+-rw-r--r--   0 admin     (1001) root         (0)      668 2024-04-11 01:14:26.000000 Simple-Network-1.0.0/setup.py
+drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/simpleN/
+-rw-r--r--   0 admin     (1001) root         (0)       97 2024-04-11 02:18:15.000000 Simple-Network-1.0.0/simpleN/__init__.py
+-rw-r--r--   0 admin     (1001) root         (0)     8094 2024-04-11 02:12:20.000000 Simple-Network-1.0.0/simpleN/analyze.py
+-rw-r--r--   0 admin     (1001) root         (0)    10959 2024-04-11 01:20:00.000000 Simple-Network-1.0.0/simpleN/net.py
+-rw-r--r--   0 admin     (1001) root         (0)     3466 2024-04-11 01:20:24.000000 Simple-Network-1.0.0/simpleN/visual.py
+drwxr-xr-x   0 admin     (1001) root         (0)        0 2024-04-11 02:19:13.754350 Simple-Network-1.0.0/tests/
+-rw-r--r--   0 admin     (1001) root         (0)     2227 2024-04-11 01:17:15.000000 Simple-Network-1.0.0/tests/test.py
+-rw-r--r--   0 admin     (1001) root         (0)     2205 2024-04-11 01:18:27.000000 Simple-Network-1.0.0/tests/test2.py
```

### Comparing `Simple-Network-0.1.0/LICENSE` & `Simple-Network-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Simple-Network-0.1.0/pyproject.toml` & `Simple-Network-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Network"
-version = "0.1.0"
+version = "1.0.0"
 description = "A basic tool designed for the construction and visualization of complex, multilayer networks."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
@@ -19,14 +19,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'plotly',
-    'numpy'
+    'numpy',
+    'scipy',
+    'nbformat'
 ]
 [project.urls]
 Homepage = "https://github.com/cloner174/Simple-Network"
 Documentation = "https://github.com/cloner174/Simple-Network#readme"
 Repository = "https://github.com/cloner174/Simple-Network"
 Issues = "https://github.com/cloner174/Simple-Network/issues"
```

### Comparing `Simple-Network-0.1.0/setup.py` & `Simple-Network-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Simple-Network',
-    version='0.1.0',
+    version='1.0.0',
     packages=find_packages(),
     author="Hamed Hajipour",
     author_email="cloner174.org@gmail.com",
     description="A basic tool designed for the construction and visualization of complex, multilayer networks.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/cloner174/Simple-Network",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-)
+)
```

### Comparing `Simple-Network-0.1.0/simpleN/visual.py` & `Simple-Network-1.0.0/simpleN/visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                             x_i, y_i, z_i = node_positions[layer_name][node_i]
                             x_j, y_j, z_j = node_positions[layer_name][node_j]
                             edge_x.extend([x_i, x_j, None])  # None will create a gap between the edges, necessary for Plotly
                             edge_y.extend([y_i, y_j, None])
                             edge_z.extend([z_i, z_j, None])
         # Inter-layer edges
         for edge in self.network.inter_layer_edges:
-            node1, layer1, node2, layer2, weight = edge
+            (node1, layer1), (node2, layer2), weight = edge
             if weight < edge_visibility_threshold:
                 continue
             x1, y1, z1 = node_positions[layer1][node1]
             x2, y2, z2 = node_positions[layer2][node2]
             edge_x.extend([x1, x2, None])
             edge_y.extend([y1, y2, None])
             edge_z.extend([z1, z2, None])
@@ -73,8 +73,8 @@
             )
         )
         # Create the figure
         fig = go.Figure(data=[edge_trace, node_trace], layout=layout)
         # Render the figure
         fig.show()
 
-#end#
+#end#
```

