# Comparing `tmp/codeplot-1.2.0.tar.gz` & `tmp/codeplot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeplot-1.2.0.tar", last modified: Thu Feb 29 19:13:26 2024, max compression
+gzip compressed data, was "codeplot-1.3.0.tar", last modified: Thu Apr 11 02:39:17 2024, max compression
```

## Comparing `codeplot-1.2.0.tar` & `codeplot-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-02-29 19:13:26.629730 codeplot-1.2.0/
--rw-r--r--   0 antl3x    (1000) antl3x    (1000)     5159 2024-02-29 19:13:26.629730 codeplot-1.2.0/PKG-INFO
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     4504 2024-02-28 23:22:30.000000 codeplot-1.2.0/README.md
-drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-02-29 19:13:26.629730 codeplot-1.2.0/codeplot/
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      331 2024-02-14 02:06:49.000000 codeplot-1.2.0/codeplot/__init__.py
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     8614 2024-02-29 18:54:04.000000 codeplot-1.2.0/codeplot/main.py
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     1862 2024-02-28 22:58:03.000000 codeplot-1.2.0/codeplot/yutils.py
-drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-02-29 19:13:26.629730 codeplot-1.2.0/codeplot.egg-info/
--rw-r--r--   0 antl3x    (1000) antl3x    (1000)     5159 2024-02-29 19:13:26.000000 codeplot-1.2.0/codeplot.egg-info/PKG-INFO
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      234 2024-02-29 19:13:26.000000 codeplot-1.2.0/codeplot.egg-info/SOURCES.txt
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)        1 2024-02-29 19:13:26.000000 codeplot-1.2.0/codeplot.egg-info/dependency_links.txt
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      103 2024-02-29 19:13:26.000000 codeplot-1.2.0/codeplot.egg-info/requires.txt
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)        9 2024-02-29 19:13:26.000000 codeplot-1.2.0/codeplot.egg-info/top_level.txt
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)       38 2024-02-29 19:13:26.629730 codeplot-1.2.0/setup.cfg
--rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      914 2024-02-29 19:13:11.000000 codeplot-1.2.0/setup.py
+drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-04-11 02:39:17.942628 codeplot-1.3.0/
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     4966 2024-04-11 02:39:17.942628 codeplot-1.3.0/PKG-INFO
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     4504 2024-02-28 23:22:30.000000 codeplot-1.3.0/README.md
+drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-04-11 02:39:17.942628 codeplot-1.3.0/codeplot/
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      331 2024-02-14 02:06:49.000000 codeplot-1.3.0/codeplot/__init__.py
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     8555 2024-04-11 02:23:56.000000 codeplot-1.3.0/codeplot/main.py
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)     1862 2024-02-28 22:58:03.000000 codeplot-1.3.0/codeplot/yutils.py
+drwxrwxr-x   0 antl3x    (1000) antl3x    (1000)        0 2024-04-11 02:39:17.942628 codeplot-1.3.0/codeplot.egg-info/
+-rw-r--r--   0 antl3x    (1000) antl3x    (1000)     4966 2024-04-11 02:39:17.000000 codeplot-1.3.0/codeplot.egg-info/PKG-INFO
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      234 2024-04-11 02:39:17.000000 codeplot-1.3.0/codeplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)        1 2024-04-11 02:39:17.000000 codeplot-1.3.0/codeplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      103 2024-04-11 02:39:17.000000 codeplot-1.3.0/codeplot.egg-info/requires.txt
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)        9 2024-04-11 02:39:17.000000 codeplot-1.3.0/codeplot.egg-info/top_level.txt
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)       38 2024-04-11 02:39:17.942628 codeplot-1.3.0/setup.cfg
+-rw-rw-r--   0 antl3x    (1000) antl3x    (1000)      914 2024-04-11 02:39:03.000000 codeplot-1.3.0/setup.py
```

### Comparing `codeplot-1.2.0/PKG-INFO` & `codeplot-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 Metadata-Version: 2.1
 Name: codeplot
-Version: 1.2.0
+Version: 1.3.0
 Summary: codeplot is a canvas designed for code-driven data exploration where you can plot graphs, data frames, markdown and much more using plain Python
 Home-page: https://github.com/codeplot-co/codeplot
 Author: Antonio Moura (@antl3x)
 Author-email: antonio@codeplot.co
 License: AGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: watchdog>=3.0.0
-Requires-Dist: typeid-python>=0.2.2
-Requires-Dist: ypy-websocket>=0.12.4
-Requires-Dist: asyncio>=3.4.3
-Requires-Dist: websockets>=11.0
-Requires-Dist: y-py>=0.6.2
 
 ![codeplot-readme](https://github.com/codeplot-co/codeplot/assets/26308297/e1212d25-a731-4755-875d-e988848f6d87)
 <div align="center">
 <a href="https://codeplot.co">Demo</a> 
 <span> · </span>
 <a href="https://codeplot.co/discord">Discord</a>
 </div>
```

#### html2text {}

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 2.1 Name: codeplot Version: 1.2.0 Summary: codeplot is a
+Metadata-Version: 2.1 Name: codeplot Version: 1.3.0 Summary: codeplot is a
 canvas designed for code-driven data exploration where you can plot graphs,
 data frames, markdown and much more using plain Python Home-page: https://
 github.com/codeplot-co/codeplot Author: Antonio Moura (@antl3x) Author-email:
 antonio@codeplot.co License: AGPL-3.0-or-later Classifier: Programming Language
-:: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Requires-Dist: watchdog>=3.0.0 Requires-Dist: typeid-python>=0.2.2 Requires-
-Dist: ypy-websocket>=0.12.4 Requires-Dist: asyncio>=3.4.3 Requires-Dist:
-websockets>=11.0 Requires-Dist: y-py>=0.6.2 ![codeplot-readme](https://
-github.com/codeplot-co/codeplot/assets/26308297/e1212d25-a731-4755-875d-
-e988848f6d87)
+:: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown !
+[codeplot-readme](https://github.com/codeplot-co/codeplot/assets/26308297/
+e1212d25-a731-4755-875d-e988848f6d87)
                                 _D_e_m_o Â· _D_i_s_c_o_r_d
 --- codeplot is a dynamic spatial canvas for data exploration, offering an
 interactive environment for graphing and visualizing data with Python. Created
 by [@antl3x](https://github.com/antl3x), [read more](https://antl3x.co/posts/
 2024-01-25-today-i-decided-to-create-a-tool-that-i-always-wanted/) about its
 inception. # Video Demo [![Watch the video](https://img.youtube.com/vi/
 nu5pY9nxXsA/maxresdefault.jpg)](https://youtu.be/nu5pY9nxXsA) **Why Choose
```

### Comparing `codeplot-1.2.0/README.md` & `codeplot-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `codeplot-1.2.0/codeplot/main.py` & `codeplot-1.3.0/codeplot/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,16 +109,16 @@
             kwargs.setdefault("id", str(TypeID(prefix="plot")))
             kwargs.setdefault("title", "Untitled"),
             kwargs.setdefault("width", shape['props']['w'] if shape else 500) 
             kwargs.setdefault("height",  shape['props']['h'] if shape else 250)
             kwargs.setdefault("rotation",shape['rotation'] if shape else 0)
             kwargs.setdefault("opacity", shape['opacity'] if shape else 1)
             kwargs.setdefault("is_locked", shape['isLocked'] if shape else False)
-            kwargs.setdefault("x_pos", shape['x'] if shape else -camera["x"] + 100)
-            kwargs.setdefault("y_pos", shape['y'] if shape else -camera["y"] + 100)
+            kwargs.setdefault("x_pos", shape['x'] if shape else 0)
+            kwargs.setdefault("y_pos", shape['y'] if shape else 0)
             kwargs.setdefault("page_id", instance["currentPageId"])
             kwargs.setdefault("ipythonRawCell", None)
             kwargs.setdefault("ipythonCellId", None)
             kwargs.setdefault("id", str(TypeID(prefix="plot")))
 
 
             shape = {
@@ -133,15 +133,15 @@
                         "h": kwargs["height"],
                         "id": "shape:"+kwargs["id"],
                         "title": kwargs["title"],
                         "type": str(type(data)),
                         "renderWith": "default",
                         "mime": _get_mime_representations(data),
                         "metadata": {
-                            "isPinned": False,
+                            "isPinned": True,
                             "pythonCallerFrameCodeContext": metacode_line,
                             "ipythonRawCell": kwargs["ipythonRawCell"],
                             "ipythonCellId": kwargs["ipythonCellId"],
                         },
                         "createdAt": datetime.datetime.utcnow().isoformat() + "Z"
                     },
                     "meta": {},
@@ -194,15 +194,15 @@
         '_repr_markdown_': 'text/markdown',
         # Add more as needed
     }
 
     representations = {}
 
     # Here we check if obj is a representation itself
-    if isinstance(obj, dict) and 'text/plain' in obj:
+    if isinstance(obj, dict):
         return obj
 
     for method_name, mime_type in mime_types.items():
         if hasattr(obj, method_name):
             method = getattr(obj, method_name)
             try:
                 content = method()
```

### Comparing `codeplot-1.2.0/codeplot/yutils.py` & `codeplot-1.3.0/codeplot/yutils.py`

 * *Files identical despite different names*

### Comparing `codeplot-1.2.0/codeplot.egg-info/PKG-INFO` & `codeplot-1.3.0/codeplot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 Metadata-Version: 2.1
 Name: codeplot
-Version: 1.2.0
+Version: 1.3.0
 Summary: codeplot is a canvas designed for code-driven data exploration where you can plot graphs, data frames, markdown and much more using plain Python
 Home-page: https://github.com/codeplot-co/codeplot
 Author: Antonio Moura (@antl3x)
 Author-email: antonio@codeplot.co
 License: AGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: watchdog>=3.0.0
-Requires-Dist: typeid-python>=0.2.2
-Requires-Dist: ypy-websocket>=0.12.4
-Requires-Dist: asyncio>=3.4.3
-Requires-Dist: websockets>=11.0
-Requires-Dist: y-py>=0.6.2
 
 ![codeplot-readme](https://github.com/codeplot-co/codeplot/assets/26308297/e1212d25-a731-4755-875d-e988848f6d87)
 <div align="center">
 <a href="https://codeplot.co">Demo</a> 
 <span> · </span>
 <a href="https://codeplot.co/discord">Discord</a>
 </div>
```

#### html2text {}

```diff
@@ -1,18 +1,15 @@
-Metadata-Version: 2.1 Name: codeplot Version: 1.2.0 Summary: codeplot is a
+Metadata-Version: 2.1 Name: codeplot Version: 1.3.0 Summary: codeplot is a
 canvas designed for code-driven data exploration where you can plot graphs,
 data frames, markdown and much more using plain Python Home-page: https://
 github.com/codeplot-co/codeplot Author: Antonio Moura (@antl3x) Author-email:
 antonio@codeplot.co License: AGPL-3.0-or-later Classifier: Programming Language
-:: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown
-Requires-Dist: watchdog>=3.0.0 Requires-Dist: typeid-python>=0.2.2 Requires-
-Dist: ypy-websocket>=0.12.4 Requires-Dist: asyncio>=3.4.3 Requires-Dist:
-websockets>=11.0 Requires-Dist: y-py>=0.6.2 ![codeplot-readme](https://
-github.com/codeplot-co/codeplot/assets/26308297/e1212d25-a731-4755-875d-
-e988848f6d87)
+:: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown !
+[codeplot-readme](https://github.com/codeplot-co/codeplot/assets/26308297/
+e1212d25-a731-4755-875d-e988848f6d87)
                                 _D_e_m_o Â· _D_i_s_c_o_r_d
 --- codeplot is a dynamic spatial canvas for data exploration, offering an
 interactive environment for graphing and visualizing data with Python. Created
 by [@antl3x](https://github.com/antl3x), [read more](https://antl3x.co/posts/
 2024-01-25-today-i-decided-to-create-a-tool-that-i-always-wanted/) about its
 inception. # Video Demo [![Watch the video](https://img.youtube.com/vi/
 nu5pY9nxXsA/maxresdefault.jpg)](https://youtu.be/nu5pY9nxXsA) **Why Choose
```

### Comparing `codeplot-1.2.0/setup.py` & `codeplot-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='codeplot',
-    version='1.2.0',
+    version='1.3.0',
     packages=find_packages(),
     install_requires=[
         'watchdog >= 3.0.0',
         'typeid-python >= 0.2.2',
         'ypy-websocket >= 0.12.4',
         'asyncio >= 3.4.3',
         'websockets >= 11.0',
```

