# Comparing `tmp/memory_graph-0.2.2.tar.gz` & `tmp/memory_graph-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.2.2.tar", last modified: Tue Apr  9 12:29:15 2024, max compression
+gzip compressed data, was "memory_graph-0.2.3.tar", last modified: Thu Apr 11 18:23:20 2024, max compression
```

## Comparing `memory_graph-0.2.2.tar` & `memory_graph-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-09 12:29:15.150614 memory_graph-0.2.2/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2024-02-16 13:16:53.000000 memory_graph-0.2.2/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2024-02-16 13:16:53.000000 memory_graph-0.2.2/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21286 2024-04-09 12:29:15.150614 memory_graph-0.2.2/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20639 2024-04-09 12:27:53.000000 memory_graph-0.2.2/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-09 12:29:15.150614 memory_graph-0.2.2/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5038 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/HTML_Table.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/Memory_Graph.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-08 20:46:55.000000 memory_graph-0.2.2/memory_graph/Memory_Visitor.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3168 2024-04-08 20:45:29.000000 memory_graph-0.2.2/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      847 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/Node_Hidden.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3968 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/Node_Key_Value.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2520 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/Node_Linear.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3287 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/Node_Table.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3949 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/Sliced.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6586 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/Slicer.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6542 2024-04-09 12:28:27.000000 memory_graph-0.2.2/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      327 2024-04-08 20:50:18.000000 memory_graph-0.2.2/memory_graph/config.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3231 2024-04-08 21:10:10.000000 memory_graph-0.2.2/memory_graph/config_default.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2400 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/config_helpers.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1340 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/extension_numpy.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      660 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/extension_pandas.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       24 2024-04-08 20:16:22.000000 memory_graph-0.2.2/memory_graph/special_types.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4909 2024-04-08 21:05:52.000000 memory_graph-0.2.2/memory_graph/test.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      536 2024-04-08 19:52:20.000000 memory_graph-0.2.2/memory_graph/test_memory_graph.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      286 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/test_memory_visitor.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1944 2024-04-07 17:46:45.000000 memory_graph-0.2.2/memory_graph/utils.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-09 12:29:15.150614 memory_graph-0.2.2/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21286 2024-04-09 12:29:15.000000 memory_graph-0.2.2/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      807 2024-04-09 12:29:15.000000 memory_graph-0.2.2/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2024-04-09 12:29:15.000000 memory_graph-0.2.2/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2024-04-09 12:29:15.000000 memory_graph-0.2.2/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2024-04-09 12:29:15.000000 memory_graph-0.2.2/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2024-04-09 12:29:15.150614 memory_graph-0.2.2/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1037 2024-04-09 12:28:33.000000 memory_graph-0.2.2/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-11 18:23:20.819594 memory_graph-0.2.3/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2024-02-16 13:16:53.000000 memory_graph-0.2.3/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2024-02-16 13:16:53.000000 memory_graph-0.2.3/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21333 2024-04-11 18:23:20.819594 memory_graph-0.2.3/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20686 2024-04-11 00:46:48.000000 memory_graph-0.2.3/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-11 18:23:20.815594 memory_graph-0.2.3/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5038 2024-04-07 17:46:45.000000 memory_graph-0.2.3/memory_graph/HTML_Table.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-07 17:46:45.000000 memory_graph-0.2.3/memory_graph/Memory_Graph.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-08 20:46:55.000000 memory_graph-0.2.3/memory_graph/Memory_Visitor.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3131 2024-04-11 17:51:04.000000 memory_graph-0.2.3/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      847 2024-04-11 17:52:51.000000 memory_graph-0.2.3/memory_graph/Node_Hidden.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4254 2024-04-11 18:14:00.000000 memory_graph-0.2.3/memory_graph/Node_Key_Value.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2481 2024-04-11 17:52:34.000000 memory_graph-0.2.3/memory_graph/Node_Linear.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3462 2024-04-11 17:53:02.000000 memory_graph-0.2.3/memory_graph/Node_Table.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4134 2024-04-11 18:12:31.000000 memory_graph-0.2.3/memory_graph/Sliced.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6586 2024-04-07 17:46:45.000000 memory_graph-0.2.3/memory_graph/Slicer.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6542 2024-04-11 18:21:41.000000 memory_graph-0.2.3/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      327 2024-04-08 20:50:18.000000 memory_graph-0.2.3/memory_graph/config.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3231 2024-04-08 21:10:10.000000 memory_graph-0.2.3/memory_graph/config_default.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2400 2024-04-07 17:46:45.000000 memory_graph-0.2.3/memory_graph/config_helpers.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1340 2024-04-07 17:46:45.000000 memory_graph-0.2.3/memory_graph/extension_numpy.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      660 2024-04-07 17:46:45.000000 memory_graph-0.2.3/memory_graph/extension_pandas.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       24 2024-04-08 20:16:22.000000 memory_graph-0.2.3/memory_graph/special_types.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4909 2024-04-08 21:05:52.000000 memory_graph-0.2.3/memory_graph/test.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      536 2024-04-08 19:52:20.000000 memory_graph-0.2.3/memory_graph/test_memory_graph.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      286 2024-04-07 17:46:45.000000 memory_graph-0.2.3/memory_graph/test_memory_visitor.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1944 2024-04-07 17:46:45.000000 memory_graph-0.2.3/memory_graph/utils.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-11 18:23:20.815594 memory_graph-0.2.3/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21333 2024-04-11 18:23:20.000000 memory_graph-0.2.3/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      807 2024-04-11 18:23:20.000000 memory_graph-0.2.3/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2024-04-11 18:23:20.000000 memory_graph-0.2.3/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2024-04-11 18:23:20.000000 memory_graph-0.2.3/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2024-04-11 18:23:20.000000 memory_graph-0.2.3/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2024-04-11 18:23:20.819594 memory_graph-0.2.3/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1037 2024-04-11 18:21:46.000000 memory_graph-0.2.3/setup.py
```

### Comparing `memory_graph-0.2.2/LICENSE.txt` & `memory_graph-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/PKG-INFO` & `memory_graph-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_graph
-Version: 0.2.2
+Version: 0.2.3
 Summary: Draws a graph of your data to analyze its structure.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -63,15 +63,15 @@
 a: 4, 3, 2, 1
 b: 4, 3, 2, 1
 ids: 126432214913216 126432214913216
 identical?: True
 ```
 A better way to understand what data is shared is to draw a graph of the data using the [memory_graph](https://pypi.org/project/memory-graph/) package.
 
-# Memory Graph Packge #
+# Memory Graph #
 The [memory_graph](https://pypi.org/project/memory-graph/) package can graph many different data types.
 
 ```python
 import memory_graph
 
 class MyClass:
 
@@ -283,15 +283,15 @@
 add_one(a, b, c.copy())
 print(f"a:{a} b:{b} c:{c}")
 ```
 ![add_one.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/add_one.png)
 
 As `a` is of immutable type 'int' and as we call the function with a copy of `c`, only `b` is shared so only `b` is changed in the calling stack frame as reflected in the printed output:
 ```
-a:0 b:[4, 3, 2, 1] c:[4, 3, 2]
+a:10 b:[4, 3, 2, 1] c:[4, 3, 2]
 ```
 
 ### Recursion ###
 The call stack also helps to visualize how recursion works. Here we show each step of how recursively ```factorial(3)``` is computed:
 
 ```python
 import memory_graph
@@ -511,14 +511,15 @@
 ### Numpy ###
 Numpy types `arrray` and `matrix` and `ndarray` can be graphed with the "memory_graph.extension_numpy" extension:
 
 ```python
 from memory_graph import d
 import numpy as np
 import memory_graph.extension_numpy
+np.random.seed(0) # use same random numbers each run
 
 array = np.array([1.1, 2, 3, 4, 5])
 matrix = np.matrix([[i*20+j for j in range(20)] for i in range(20)])
 ndarray = np.random.rand(20,20)
 d()
 ```
 ![extension_numpy.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/extension_numpy.png)
```

### Comparing `memory_graph-0.2.2/README.md` & `memory_graph-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 a: 4, 3, 2, 1
 b: 4, 3, 2, 1
 ids: 126432214913216 126432214913216
 identical?: True
 ```
 A better way to understand what data is shared is to draw a graph of the data using the [memory_graph](https://pypi.org/project/memory-graph/) package.
 
-# Memory Graph Packge #
+# Memory Graph #
 The [memory_graph](https://pypi.org/project/memory-graph/) package can graph many different data types.
 
 ```python
 import memory_graph
 
 class MyClass:
 
@@ -264,15 +264,15 @@
 add_one(a, b, c.copy())
 print(f"a:{a} b:{b} c:{c}")
 ```
 ![add_one.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/add_one.png)
 
 As `a` is of immutable type 'int' and as we call the function with a copy of `c`, only `b` is shared so only `b` is changed in the calling stack frame as reflected in the printed output:
 ```
-a:0 b:[4, 3, 2, 1] c:[4, 3, 2]
+a:10 b:[4, 3, 2, 1] c:[4, 3, 2]
 ```
 
 ### Recursion ###
 The call stack also helps to visualize how recursion works. Here we show each step of how recursively ```factorial(3)``` is computed:
 
 ```python
 import memory_graph
@@ -492,14 +492,15 @@
 ### Numpy ###
 Numpy types `arrray` and `matrix` and `ndarray` can be graphed with the "memory_graph.extension_numpy" extension:
 
 ```python
 from memory_graph import d
 import numpy as np
 import memory_graph.extension_numpy
+np.random.seed(0) # use same random numbers each run
 
 array = np.array([1.1, 2, 3, 4, 5])
 matrix = np.matrix([[i*20+j for j in range(20)] for i in range(20)])
 ndarray = np.random.rand(20,20)
 d()
 ```
 ![extension_numpy.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/extension_numpy.png)
```

### Comparing `memory_graph-0.2.2/memory_graph/HTML_Table.py` & `memory_graph-0.2.3/memory_graph/HTML_Table.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/Memory_Graph.py` & `memory_graph-0.2.3/memory_graph/Memory_Graph.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/Memory_Visitor.py` & `memory_graph-0.2.3/memory_graph/Memory_Visitor.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/Node.py` & `memory_graph-0.2.3/memory_graph/Node.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,52 +11,57 @@
     Create a Node object.
 
     Args:
         data (object): The data represented by the node.
         children (list): The children of the node.
         size (string): The size of the node to be shown in the graph.
     """
-    def __init__(self, data, children=None, size=None):
+    def __init__(self, data, children=None):
         self.node_id = Node.node_id
         Node.node_id += 1
         self.data = data
-        self.size = size
         self.parent = None
         self.children = children
 
     def __repr__(self):
         """
         Return a string representation of the node showing the original data represented by the node.
         """
         return f'Node({self.data})'
 
     def get_data(self):
         """
         Return the original data represented by the node.
         """
         return self.data
+    
+    def get_type(self):
+        """
+        Return the type of the data represented by the node.
+        """
+        return type(self.data)
+    
+    def get_type_name(self):
+        """
+        Return the name of the type of the data represented by the node.
+        """
+        return utils.get_type_name(self.data)
 
     def set_parent(self, parent):
         """
         Set the parent of the node.
         """
         self.parent = parent
 
     def get_parent(self):
         """
         Return the parent of the node.
         """    
         return self.parent
 
-    def get_size(self):
-        """
-        Return the size of the node to be shown in the graph.
-        """
-        return self.size
-
     def get_children(self):
         """
         Return the children of the node. Initially the children are raw data, but 
         later they too are converted to Node by the Memory_visitor using the Node 'transform' method.
         """
         return self.children
     
@@ -74,25 +79,14 @@
         html_table = HTML_Table()
         if self.children is None:
             html_table.add_string(f'{self.data}')
         elif self.children.has_data():
             self.fill_html_table(html_table)
         return html_table
     
-    def get_label(self):
-        """
-        Return a label for the node to be shown in the graph next to the HTML table, the size 
-        is included in the label if available.
-        """
-        label = utils.get_type_name(self.data)
-        size = self.get_size()
-        if not size is None:
-            label +=f' ({size})'
-        return label
-    
     # -------------------- Node interface, overriden by subclasses --------------------
 
     def do_backtrack_callback(self):
         """
         Returns if the callback function is called for this Node type. 
         """
         return True
@@ -105,7 +99,13 @@
         pass
         
     def fill_html_table(self, html_table):
         """
         Fill the HTML_Table object with each child of the node.
         """
         pass
+
+    def get_label(self):
+        """
+        Return a label for the node to be shown in the graph next to the HTML table.
+        """
+        return self.get_type_name()
```

### Comparing `memory_graph-0.2.2/memory_graph/Node_Hidden.py` & `memory_graph-0.2.3/memory_graph/Node_Hidden.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/Node_Key_Value.py` & `memory_graph-0.2.3/memory_graph/Node_Key_Value.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,18 @@
     def __init__(self, data, children):
         """
         Create a Node_Key_Value object. Use a Slicer to slice the children so the
         Node will not get too big or have too many childeren in the graph.
         """
         #print('Node_Key_Value children:', children)
         hidden_children = [ Node_Hidden(i,list(i)) for i in children ]
+        self.size = len(hidden_children)
         slicer = config_helpers.get_slicer_1d(self, data)
         sliced_children = slicer.slice(hidden_children)
-        super().__init__(data, sliced_children, sliced_children.get_original_length())
+        super().__init__(data, sliced_children)
         
     def transform(self, fun):
         """
         Transform the children of the Node using the 'fun' function and the 
         'transform_node_hidden' helper to function transform each key and value instead of each tuple.
         """
         self.children.transform(lambda node_hidden: transform_node_hidden(node_hidden, fun) )
@@ -87,7 +88,16 @@
         html_table.add_new_line()
         for index, jump, value in self.children:
             if jump:
                 html_table.add_dots()
             if value is not None:
                 key_value = value.get_children() # add the key-value pair of Hidden_Node, not the tuple
                 html_table.add_entry(self, key_value[1])
+
+    def get_label(self):
+        """
+        Return a label for the node to be shown in the graph next to the HTML table.
+        """
+        if self.get_children().has_all_data():
+            return f'{self.get_type_name()}'
+        return f'{self.get_type_name()} {self.size}'
+
```

### Comparing `memory_graph-0.2.2/memory_graph/Node_Linear.py` & `memory_graph-0.2.3/memory_graph/Node_Linear.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(self, data, children=None):
         """
         Create a Node_Linear object. Use a Slicer to slice the children so the 
         Node will not get to big or have too many childeren in the graph.
         """
         slicer = config_helpers.get_slicer_1d(self, data)
         sliced_children = slicer.slice(children)
-        super().__init__(data, sliced_children, sliced_children.get_original_length())
+        super().__init__(data, sliced_children)
 
     def transform(self, fun):
         """
         Transform the children of the Node using the 'fun' function.
         """
         self.children.transform(fun)
```

### Comparing `memory_graph-0.2.2/memory_graph/Node_Table.py` & `memory_graph-0.2.3/memory_graph/Node_Table.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             sliced_children = slicer_height.slice(children)
             self.data_width = len(children[0])
         sliced_children.transform(lambda c: slicer_width.slice(c) )
         self.data_height = sliced_children.get_original_length()
 
         self.row_names = row_names
         self.column_names = column_names
-        super().__init__(data, sliced_children, f'{self.data_height}⨯{self.data_width}')
+        super().__init__(data, sliced_children)
 
     def transform(self, fun):
         """
         Transform the children of the Node using the 'fun' function.
         """
         self.children.transform(lambda s: s.transform(fun))
 
@@ -78,7 +78,13 @@
                     #print('  index2:',index2,'jump2:',jump2,'value:',value)
                     if jump2:
                         html_table.add_dots()
                     if value is not None:
                         html_table.add_entry(self, value)
                 html_table.add_new_line()
 
+    def get_label(self):
+        """
+        Return a label for the node to be shown in the graph next to the HTML table.
+        """
+        return f'{self.get_type_name()} {self.data_height}⨯{self.data_width}'
+
```

### Comparing `memory_graph-0.2.2/memory_graph/Sliced.py` & `memory_graph-0.2.3/memory_graph/Sliced.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,8 +104,11 @@
     def has_data(self):
         """ Return True if the Sliced object has any data. """
         return len(self.slices) > 1 or (len(self.slices) == 1 and len(self.slices[0].data) > 0)
     
     def last_slice_empty(self):
         """ Return True if the last slice of the Sliced object is empty. """
         return len(self.slices) > 0 and len(self.slices[-1].data) == 0
-    
+    
+    def has_all_data(self):
+        """ Return True if the Sliced object has all the data. """
+        return len(self.slices) == 1 and len(self.slices[0].data) == self.original_length
```

### Comparing `memory_graph-0.2.2/memory_graph/Slicer.py` & `memory_graph-0.2.3/memory_graph/Slicer.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/__init__.py` & `memory_graph-0.2.3/memory_graph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import memory_graph.config_default as config_default
 import memory_graph.utils as utils
 
 import inspect
 import sys
 
-__version__ = "0.2.02"
+__version__ = "0.2.03"
 __author__ = 'Bas Terwijn'
 
 log_file=sys.stdout
 press_enter_text="press <ENTER> to continue..."
 
 def get_source_location(stack_index):
     """ Helper function to get the source location of the stack with 'stack_index' of the call stack. """
```

### Comparing `memory_graph-0.2.2/memory_graph/config_default.py` & `memory_graph-0.2.3/memory_graph/config_default.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/config_helpers.py` & `memory_graph-0.2.3/memory_graph/config_helpers.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/extension_numpy.py` & `memory_graph-0.2.3/memory_graph/extension_numpy.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/extension_pandas.py` & `memory_graph-0.2.3/memory_graph/extension_pandas.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/test.py` & `memory_graph-0.2.3/memory_graph/test.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/test_memory_graph.py` & `memory_graph-0.2.3/memory_graph/test_memory_graph.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph/utils.py` & `memory_graph-0.2.3/memory_graph/utils.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.2.3/memory_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-graph
-Version: 0.2.2
+Version: 0.2.3
 Summary: Draws a graph of your data to analyze its structure.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -63,15 +63,15 @@
 a: 4, 3, 2, 1
 b: 4, 3, 2, 1
 ids: 126432214913216 126432214913216
 identical?: True
 ```
 A better way to understand what data is shared is to draw a graph of the data using the [memory_graph](https://pypi.org/project/memory-graph/) package.
 
-# Memory Graph Packge #
+# Memory Graph #
 The [memory_graph](https://pypi.org/project/memory-graph/) package can graph many different data types.
 
 ```python
 import memory_graph
 
 class MyClass:
 
@@ -283,15 +283,15 @@
 add_one(a, b, c.copy())
 print(f"a:{a} b:{b} c:{c}")
 ```
 ![add_one.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/add_one.png)
 
 As `a` is of immutable type 'int' and as we call the function with a copy of `c`, only `b` is shared so only `b` is changed in the calling stack frame as reflected in the printed output:
 ```
-a:0 b:[4, 3, 2, 1] c:[4, 3, 2]
+a:10 b:[4, 3, 2, 1] c:[4, 3, 2]
 ```
 
 ### Recursion ###
 The call stack also helps to visualize how recursion works. Here we show each step of how recursively ```factorial(3)``` is computed:
 
 ```python
 import memory_graph
@@ -511,14 +511,15 @@
 ### Numpy ###
 Numpy types `arrray` and `matrix` and `ndarray` can be graphed with the "memory_graph.extension_numpy" extension:
 
 ```python
 from memory_graph import d
 import numpy as np
 import memory_graph.extension_numpy
+np.random.seed(0) # use same random numbers each run
 
 array = np.array([1.1, 2, 3, 4, 5])
 matrix = np.matrix([[i*20+j for j in range(20)] for i in range(20)])
 ndarray = np.random.rand(20,20)
 d()
 ```
 ![extension_numpy.png](https://raw.githubusercontent.com/bterwijn/memory_graph/main/images/extension_numpy.png)
```

### Comparing `memory_graph-0.2.2/memory_graph.egg-info/SOURCES.txt` & `memory_graph-0.2.3/memory_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.2/setup.py` & `memory_graph-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.2.02',
+    version = '0.2.03',
     description = 'Draws a graph of your data to analyze its structure.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
```

