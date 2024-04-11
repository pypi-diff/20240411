# Comparing `tmp/codeplot-ipython-1.9.2.tar.gz` & `tmp/codeplot-ipython-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeplot-ipython-1.9.2.tar", last modified: Wed Mar  6 20:52:58 2024, max compression
+gzip compressed data, was "codeplot-ipython-1.9.3.tar", last modified: Wed Mar  6 21:02:43 2024, max compression
```

## Comparing `codeplot-ipython-1.9.2.tar` & `codeplot-ipython-1.9.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-03-06 20:52:58.821789 codeplot-ipython-1.9.2/
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     4974 2024-03-06 20:52:58.821789 codeplot-ipython-1.9.2/PKG-INFO
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     4504 2024-02-28 23:22:26.000000 codeplot-ipython-1.9.2/README.md
-drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-03-06 20:52:58.821789 codeplot-ipython-1.9.2/codeplot-ipython/
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     3912 2024-03-06 20:48:23.000000 codeplot-ipython-1.9.2/codeplot-ipython/__init__.py
-drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-03-06 20:52:58.821789 codeplot-ipython-1.9.2/codeplot_ipython.egg-info/
--rw-r--r--   0 antl3x    (1000) antl3x    (1000)     4974 2024-03-06 20:52:58.000000 codeplot-ipython-1.9.2/codeplot_ipython.egg-info/PKG-INFO
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      246 2024-03-06 20:52:58.000000 codeplot-ipython-1.9.2/codeplot_ipython.egg-info/SOURCES.txt
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)        1 2024-03-06 20:52:58.000000 codeplot-ipython-1.9.2/codeplot_ipython.egg-info/dependency_links.txt
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)       31 2024-03-06 20:52:58.000000 codeplot-ipython-1.9.2/codeplot_ipython.egg-info/requires.txt
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)       17 2024-03-06 20:52:58.000000 codeplot-ipython-1.9.2/codeplot_ipython.egg-info/top_level.txt
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)       38 2024-03-06 20:52:58.821789 codeplot-ipython-1.9.2/setup.cfg
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      798 2024-03-06 20:52:57.000000 codeplot-ipython-1.9.2/setup.py
+drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-03-06 21:02:43.745088 codeplot-ipython-1.9.3/
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     4974 2024-03-06 21:02:43.745088 codeplot-ipython-1.9.3/PKG-INFO
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     4504 2024-02-28 23:22:26.000000 codeplot-ipython-1.9.3/README.md
+drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-03-06 21:02:43.745088 codeplot-ipython-1.9.3/codeplot-ipython/
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     4012 2024-03-06 21:02:35.000000 codeplot-ipython-1.9.3/codeplot-ipython/__init__.py
+drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-03-06 21:02:43.745088 codeplot-ipython-1.9.3/codeplot_ipython.egg-info/
+-rw-r--r--   0 antl3x    (1000) antl3x    (1000)     4974 2024-03-06 21:02:43.000000 codeplot-ipython-1.9.3/codeplot_ipython.egg-info/PKG-INFO
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      246 2024-03-06 21:02:43.000000 codeplot-ipython-1.9.3/codeplot_ipython.egg-info/SOURCES.txt
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)        1 2024-03-06 21:02:43.000000 codeplot-ipython-1.9.3/codeplot_ipython.egg-info/dependency_links.txt
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)       31 2024-03-06 21:02:43.000000 codeplot-ipython-1.9.3/codeplot_ipython.egg-info/requires.txt
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)       17 2024-03-06 21:02:43.000000 codeplot-ipython-1.9.3/codeplot_ipython.egg-info/top_level.txt
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)       38 2024-03-06 21:02:43.745088 codeplot-ipython-1.9.3/setup.cfg
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      798 2024-03-06 21:02:39.000000 codeplot-ipython-1.9.3/setup.py
```

### Comparing `codeplot-ipython-1.9.2/PKG-INFO` & `codeplot-ipython-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeplot-ipython
-Version: 1.9.2
+Version: 1.9.3
 Summary: codeplot is a canvas designed for code-driven data exploration where you can plot graphs, data frames, markdown and much more using plain Python
 Home-page: https://github.com/codeplot-co/codeplot
 Author: Antonio Moura (@antl3x)
 Author-email: antonio@codeplot.co
 License: AGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codeplot-ipython Version: 1.9.2 Summary: codeplot
+Metadata-Version: 2.1 Name: codeplot-ipython Version: 1.9.3 Summary: codeplot
 is a canvas designed for code-driven data exploration where you can plot
 graphs, data frames, markdown and much more using plain Python Home-page:
 https://github.com/codeplot-co/codeplot Author: Antonio Moura (@antl3x) Author-
 email: antonio@codeplot.co License: AGPL-3.0-or-later Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/
 markdown ![codeplot-readme](https://github.com/codeplot-co/codeplot/assets/
 26308297/e1212d25-a731-4755-875d-e988848f6d87)
```

### Comparing `codeplot-ipython-1.9.2/README.md` & `codeplot-ipython-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `codeplot-ipython-1.9.2/codeplot-ipython/__init__.py` & `codeplot-ipython-1.9.3/codeplot-ipython/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,25 +79,27 @@
     def post_run_cell(self, result):
         if not self.connection_established:
             # The connection is now established using the %connect magic, so this may not be needed
             pass
         if result.result is not None and self.cP is not None:
             asyncio.create_task(self.cP.plot(result.result, **self._plot_magic_args))
         
-        if self._supress_output is True and self.connection_established is True:
-            # Clean the output
-            self.ipython.display_pub.clear_output()
-        
         # Clean up the current cell id
         self._magic_current_cell_id = None
         self._plot_magic_args = {}
+    
+    def post_execute(self):
+        if self._supress_output is True and self.connection_established is True:
+            # Clean the output
+            self.ipython.display_pub.clear_output()
            
 
 def load_ipython_extension(ipython):
     
         ipython.register_magics(Magics(ipython))
         _cP_extension = IPythonExtension(ipython)
         # Store the extension instance in the IPython user namespace for access from magics
         ipython.user_ns['_cP_extension'] = _cP_extension
         ipython.events.register('pre_run_cell', _cP_extension.pre_run_cell)
         ipython.events.register('post_run_cell', _cP_extension.post_run_cell)
+        ipython.events.register('post_execute', _cP_extension.post_execute)
```

### Comparing `codeplot-ipython-1.9.2/codeplot_ipython.egg-info/PKG-INFO` & `codeplot-ipython-1.9.3/codeplot_ipython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeplot-ipython
-Version: 1.9.2
+Version: 1.9.3
 Summary: codeplot is a canvas designed for code-driven data exploration where you can plot graphs, data frames, markdown and much more using plain Python
 Home-page: https://github.com/codeplot-co/codeplot
 Author: Antonio Moura (@antl3x)
 Author-email: antonio@codeplot.co
 License: AGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: codeplot-ipython Version: 1.9.2 Summary: codeplot
+Metadata-Version: 2.1 Name: codeplot-ipython Version: 1.9.3 Summary: codeplot
 is a canvas designed for code-driven data exploration where you can plot
 graphs, data frames, markdown and much more using plain Python Home-page:
 https://github.com/codeplot-co/codeplot Author: Antonio Moura (@antl3x) Author-
 email: antonio@codeplot.co License: AGPL-3.0-or-later Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/
 markdown ![codeplot-readme](https://github.com/codeplot-co/codeplot/assets/
 26308297/e1212d25-a731-4755-875d-e988848f6d87)
```

### Comparing `codeplot-ipython-1.9.2/setup.py` & `codeplot-ipython-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='codeplot-ipython',
-    version='1.9.2',
+    version='1.9.3',
     packages=find_packages(),
     install_requires=[
         'codeplot >= 1.2.0',
         'asyncio >= 3.4.2',
     ],
     author='Antonio Moura (@antl3x)',
     author_email='antonio@codeplot.co',
```

