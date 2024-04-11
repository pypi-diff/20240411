# Comparing `tmp/draggable-line-chart-0.3.tar.gz` & `tmp/draggable-line-chart-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draggable-line-chart-0.3.tar", last modified: Wed Apr 10 23:41:11 2024, max compression
+gzip compressed data, was "draggable-line-chart-0.3.1.tar", last modified: Thu Apr 11 00:49:53 2024, max compression
```

## Comparing `draggable-line-chart-0.3.tar` & `draggable-line-chart-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 23:41:11.120622 draggable-line-chart-0.3/
--rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 draggable-line-chart-0.3/LICENSE
--rw-rw-rw-   0        0        0       57 2024-04-06 22:46:10.000000 draggable-line-chart-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3252 2024-04-10 23:41:11.110246 draggable-line-chart-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2799 2024-04-10 23:33:09.000000 draggable-line-chart-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 23:41:10.805579 draggable-line-chart-0.3/draggable_line_chart/
--rw-rw-rw-   0        0        0     4355 2024-04-10 23:38:03.000000 draggable-line-chart-0.3/draggable_line_chart/__init__.py
--rw-rw-rw-   0        0        0      831 2024-04-10 23:29:20.000000 draggable-line-chart-0.3/draggable_line_chart/example.py
-drwxrwxrwx   0        0        0        0 2024-04-10 23:41:10.736810 draggable-line-chart-0.3/draggable_line_chart/frontend/
-drwxrwxrwx   0        0        0        0 2024-04-10 23:41:10.892268 draggable-line-chart-0.3/draggable_line_chart/frontend/build/
--rw-rw-rw-   0        0        0      221 2024-04-10 23:40:06.000000 draggable-line-chart-0.3/draggable_line_chart/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2024-04-05 22:58:35.000000 draggable-line-chart-0.3/draggable_line_chart/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      492 2024-04-10 23:40:06.000000 draggable-line-chart-0.3/draggable_line_chart/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2024-04-10 23:41:10.740645 draggable-line-chart-0.3/draggable_line_chart/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2024-04-10 23:41:11.006327 draggable-line-chart-0.3/draggable_line_chart/frontend/build/static/js/
--rw-rw-rw-   0        0        0   560985 2024-04-10 23:40:06.000000 draggable-line-chart-0.3/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js
--rw-rw-rw-   0        0        0     1831 2024-04-10 23:40:06.000000 draggable-line-chart-0.3/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2402037 2024-04-10 23:40:06.000000 draggable-line-chart-0.3/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js.map
-drwxrwxrwx   0        0        0        0 2024-04-10 23:41:10.856856 draggable-line-chart-0.3/draggable_line_chart.egg-info/
--rw-rw-rw-   0        0        0     3252 2024-04-10 23:41:10.000000 draggable-line-chart-0.3/draggable_line_chart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2024-04-10 23:41:10.000000 draggable-line-chart-0.3/draggable_line_chart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 23:41:10.000000 draggable-line-chart-0.3/draggable_line_chart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-04-10 23:41:10.000000 draggable-line-chart-0.3/draggable_line_chart.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-10 23:41:10.000000 draggable-line-chart-0.3/draggable_line_chart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 23:41:11.124457 draggable-line-chart-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1075 2024-04-10 23:37:18.000000 draggable-line-chart-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 00:49:52.991624 draggable-line-chart-0.3.1/
+-rw-rw-rw-   0        0        0     1082 2024-04-05 22:58:34.000000 draggable-line-chart-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       57 2024-04-06 22:46:10.000000 draggable-line-chart-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3360 2024-04-11 00:49:52.986637 draggable-line-chart-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2905 2024-04-11 00:41:05.000000 draggable-line-chart-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 00:49:52.793617 draggable-line-chart-0.3.1/draggable_line_chart/
+-rw-rw-rw-   0        0        0     4534 2024-04-11 00:40:43.000000 draggable-line-chart-0.3.1/draggable_line_chart/__init__.py
+-rw-rw-rw-   0        0        0      833 2024-04-11 00:40:30.000000 draggable-line-chart-0.3.1/draggable_line_chart/example.py
+drwxrwxrwx   0        0        0        0 2024-04-11 00:49:52.709559 draggable-line-chart-0.3.1/draggable_line_chart/frontend/
+drwxrwxrwx   0        0        0        0 2024-04-11 00:49:52.901215 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/
+-rw-rw-rw-   0        0        0      221 2024-04-11 00:49:42.000000 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2024-04-05 22:58:35.000000 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      492 2024-04-11 00:49:42.000000 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2024-04-11 00:49:52.715290 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2024-04-11 00:49:52.948923 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   560985 2024-04-11 00:49:42.000000 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js
+-rw-rw-rw-   0        0        0     1831 2024-04-11 00:49:42.000000 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2402037 2024-04-11 00:49:42.000000 draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js.map
+drwxrwxrwx   0        0        0        0 2024-04-11 00:49:52.851771 draggable-line-chart-0.3.1/draggable_line_chart.egg-info/
+-rw-rw-rw-   0        0        0     3360 2024-04-11 00:49:52.000000 draggable-line-chart-0.3.1/draggable_line_chart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2024-04-11 00:49:52.000000 draggable-line-chart-0.3.1/draggable_line_chart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 00:49:52.000000 draggable-line-chart-0.3.1/draggable_line_chart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-04-11 00:49:52.000000 draggable-line-chart-0.3.1/draggable_line_chart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-11 00:49:52.000000 draggable-line-chart-0.3.1/draggable_line_chart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 00:49:52.993619 draggable-line-chart-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1077 2024-04-11 00:48:17.000000 draggable-line-chart-0.3.1/setup.py
```

### Comparing `draggable-line-chart-0.3/LICENSE` & `draggable-line-chart-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.3/PKG-INFO` & `draggable-line-chart-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-line-chart
-Version: 0.3
+Version: 0.3.1
 Summary: A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 Home-page: 
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -46,14 +46,19 @@
 #### Raises
 
 - `ValueError`: If the data is not a pandas Series or DataFrame or if the DataFrame does not have only numeric columns.
 
 ## Example
 
 ```python
+import pandas as pd
+import streamlit as st
+
+from draggable_line_chart import draggable_line_chart
+
 st.header("Draggable Plot 1!")
 initial_data = pd.DataFrame({
     "Col1": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
     "Col2": [1, 4, 9, 16, 25, 36, 49, 64, 81, 200],
     "Col3": [-1, -2, -3, -4, -5, -6, -7, -8, -50, -100]
 })
 
@@ -70,8 +75,9 @@
 new_data = draggable_line_chart(data=initial_data, options=plot_options)
 new_data
 
 st.header("Draggable Plot 2!")
 series_data = pd.Series([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 new_series_data = draggable_line_chart(data=series_data)
 new_series_data
+
 ```
```

### Comparing `draggable-line-chart-0.3/README.md` & `draggable-line-chart-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,19 @@
 #### Raises
 
 - `ValueError`: If the data is not a pandas Series or DataFrame or if the DataFrame does not have only numeric columns.
 
 ## Example
 
 ```python
+import pandas as pd
+import streamlit as st
+
+from draggable_line_chart import draggable_line_chart
+
 st.header("Draggable Plot 1!")
 initial_data = pd.DataFrame({
     "Col1": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
     "Col2": [1, 4, 9, 16, 25, 36, 49, 64, 81, 200],
     "Col3": [-1, -2, -3, -4, -5, -6, -7, -8, -50, -100]
 })
 
@@ -58,8 +63,9 @@
 new_data = draggable_line_chart(data=initial_data, options=plot_options)
 new_data
 
 st.header("Draggable Plot 2!")
 series_data = pd.Series([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 new_series_data = draggable_line_chart(data=series_data)
 new_series_data
+
 ```
```

### Comparing `draggable-line-chart-0.3/draggable_line_chart/__init__.py` & `draggable-line-chart-0.3.1/draggable_line_chart/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,22 +73,27 @@
     """
     if not options:
         options = {
             "x_grid": True,
             "y_grid": True
         }
     if isinstance(data, pd.Series):
-        if data.name is None:
+        if not data.name:
             data.name = "data"
         dict_data = {data.name: data.to_dict()}
     elif isinstance(data, pd.DataFrame):
         if not data.apply(lambda s: pd.to_numeric(s, errors='coerce').notnull().all()).all():
             raise ValueError("The DataFrame must have only numeric columns.")
         dict_data = data.to_dict()
     else:
         raise ValueError("The data must be a pandas Series or DataFrame.")
-        
-    new_data = _draggable_line_chart(data=dict_data, options=options, key=key, default=data)
-    if isinstance(data, pd.Series):
-        return pd.Series(new_data[data.name])
+
+    new_data = _draggable_line_chart(
+        data=dict_data, options=options, key=key, default=data)
+    if isinstance(data, pd.Series) and isinstance(new_data, pd.Series):
+        return pd.Series(new_data)
+    elif isinstance(data, pd.Series):
+        new_series = pd.Series(new_data[data.name])
+        new_series.name = data.name
+        return new_series
     elif isinstance(data, pd.DataFrame):
         return pd.DataFrame(new_data)
```

### Comparing `draggable-line-chart-0.3/draggable_line_chart/example.py` & `draggable-line-chart-0.3.1/draggable_line_chart/example.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 }
 new_data = draggable_line_chart(data=initial_data, options=plot_options)
 new_data
 
 st.header("Draggable Plot 2!")
 series_data = pd.Series([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 new_series_data = draggable_line_chart(data=series_data)
-new_series_data
+new_series_data
```

### Comparing `draggable-line-chart-0.3/draggable_line_chart/frontend/build/bootstrap.min.css` & `draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.3/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js` & `draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.3/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js.LICENSE.txt` & `draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.3/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js.map` & `draggable-line-chart-0.3.1/draggable_line_chart/frontend/build/static/js/main.7210bbf2.js.map`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.3/draggable_line_chart.egg-info/PKG-INFO` & `draggable-line-chart-0.3.1/draggable_line_chart.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draggable-line-chart
-Version: 0.3
+Version: 0.3.1
 Summary: A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.
 Home-page: 
 Author: Brayan Munoz
 Author-email: balexander.munoz@udea.edu.co
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: devel
@@ -46,14 +46,19 @@
 #### Raises
 
 - `ValueError`: If the data is not a pandas Series or DataFrame or if the DataFrame does not have only numeric columns.
 
 ## Example
 
 ```python
+import pandas as pd
+import streamlit as st
+
+from draggable_line_chart import draggable_line_chart
+
 st.header("Draggable Plot 1!")
 initial_data = pd.DataFrame({
     "Col1": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
     "Col2": [1, 4, 9, 16, 25, 36, 49, 64, 81, 200],
     "Col3": [-1, -2, -3, -4, -5, -6, -7, -8, -50, -100]
 })
 
@@ -70,8 +75,9 @@
 new_data = draggable_line_chart(data=initial_data, options=plot_options)
 new_data
 
 st.header("Draggable Plot 2!")
 series_data = pd.Series([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
 new_series_data = draggable_line_chart(data=series_data)
 new_series_data
+
 ```
```

### Comparing `draggable-line-chart-0.3/draggable_line_chart.egg-info/SOURCES.txt` & `draggable-line-chart-0.3.1/draggable_line_chart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draggable-line-chart-0.3/setup.py` & `draggable-line-chart-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="draggable-line-chart",
-    version="0.3",
+    version="0.3.1",
     author="Brayan Munoz",
     author_email="balexander.munoz@udea.edu.co",
     description="A Streamlit component that displays a line chart with draggable points. Users can click and drag points on the chart to adjust their values. The updated data of the chart is returned.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

