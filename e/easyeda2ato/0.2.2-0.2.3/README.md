# Comparing `tmp/easyeda2ato-0.2.2.tar.gz` & `tmp/easyeda2ato-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyeda2ato-0.2.2.tar", last modified: Thu Apr 11 00:45:14 2024, max compression
+gzip compressed data, was "easyeda2ato-0.2.3.tar", last modified: Thu Apr 11 01:19:01 2024, max compression
```

## Comparing `easyeda2ato-0.2.2.tar` & `easyeda2ato-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 00:45:14.943288 easyeda2ato-0.2.2/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    34523 2023-11-20 17:47:17.000000 easyeda2ato-0.2.2/LICENSE
--rw-r--r--   0 narayanpowderly   (501) staff       (20)      283 2024-04-11 00:42:55.000000 easyeda2ato-0.2.2/MANIFEST.in
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     6141 2024-04-11 00:45:14.943507 easyeda2ato-0.2.2/PKG-INFO
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     5351 2024-03-15 22:17:17.000000 easyeda2ato-0.2.2/README.md
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 00:45:14.938905 easyeda2ato-0.2.2/easyeda2ato.egg-info/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     6141 2024-04-11 00:45:14.000000 easyeda2ato-0.2.2/easyeda2ato.egg-info/PKG-INFO
--rw-r--r--   0 narayanpowderly   (501) staff       (20)      883 2024-04-11 00:45:14.000000 easyeda2ato-0.2.2/easyeda2ato.egg-info/SOURCES.txt
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        1 2024-04-11 00:45:14.000000 easyeda2ato-0.2.2/easyeda2ato.egg-info/dependency_links.txt
--rw-r--r--   0 narayanpowderly   (501) staff       (20)       62 2024-04-11 00:45:14.000000 easyeda2ato-0.2.2/easyeda2ato.egg-info/entry_points.txt
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        1 2023-12-11 17:48:19.000000 easyeda2ato-0.2.2/easyeda2ato.egg-info/not-zip-safe
--rw-r--r--   0 narayanpowderly   (501) staff       (20)       57 2024-04-11 00:45:14.000000 easyeda2ato-0.2.2/easyeda2ato.egg-info/requires.txt
--rw-r--r--   0 narayanpowderly   (501) staff       (20)       14 2024-04-11 00:45:14.000000 easyeda2ato-0.2.2/easyeda2ato.egg-info/top_level.txt
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 00:45:14.939341 easyeda2ato-0.2.2/easyeda2kicad/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)       75 2024-03-23 03:05:51.000000 easyeda2ato-0.2.2/easyeda2kicad/__init__.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    14054 2024-04-11 00:34:56.000000 easyeda2ato-0.2.2/easyeda2kicad/__main__.py
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 00:45:14.939848 easyeda2ato-0.2.2/easyeda2kicad/atopile/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     3920 2024-03-23 03:04:45.000000 easyeda2ato-0.2.2/easyeda2kicad/atopile/export_ato.py
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 00:45:14.941450 easyeda2ato-0.2.2/easyeda2kicad/easyeda/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        0 2023-12-11 18:29:50.000000 easyeda2ato-0.2.2/easyeda2kicad/easyeda/__init__.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     2307 2024-03-15 22:15:55.000000 easyeda2ato-0.2.2/easyeda2kicad/easyeda/easyeda_api.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     9743 2024-03-15 22:15:55.000000 easyeda2ato-0.2.2/easyeda2kicad/easyeda/easyeda_importer.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    14438 2024-03-15 22:15:55.000000 easyeda2ato-0.2.2/easyeda2kicad/easyeda/parameters_easyeda.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     1833 2023-12-11 18:29:50.000000 easyeda2ato-0.2.2/easyeda2kicad/easyeda/svg_path_parser.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     5263 2023-12-11 18:29:50.000000 easyeda2ato-0.2.2/easyeda2kicad/helpers.py
-drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 00:45:14.943120 easyeda2ato-0.2.2/easyeda2kicad/kicad/
--rw-r--r--   0 narayanpowderly   (501) staff       (20)        0 2023-12-11 18:29:50.000000 easyeda2ato-0.2.2/easyeda2kicad/kicad/__init__.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     4737 2024-03-15 22:15:55.000000 easyeda2ato-0.2.2/easyeda2kicad/kicad/export_kicad_3d_model.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    18012 2023-12-11 18:29:50.000000 easyeda2ato-0.2.2/easyeda2kicad/kicad/export_kicad_footprint.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    12792 2023-12-11 18:29:50.000000 easyeda2ato-0.2.2/easyeda2kicad/kicad/export_kicad_symbol.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     7207 2023-12-11 18:29:50.000000 easyeda2ato-0.2.2/easyeda2kicad/kicad/parameters_kicad_footprint.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)    22150 2023-12-11 18:29:50.000000 easyeda2ato-0.2.2/easyeda2kicad/kicad/parameters_kicad_symbol.py
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     1244 2023-12-11 18:09:41.000000 easyeda2ato-0.2.2/pyproject.toml
--rw-r--r--   0 narayanpowderly   (501) staff       (20)      446 2024-04-11 00:45:14.943862 easyeda2ato-0.2.2/setup.cfg
--rw-r--r--   0 narayanpowderly   (501) staff       (20)     1716 2024-04-11 00:45:12.000000 easyeda2ato-0.2.2/setup.py
+drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 01:19:01.414296 easyeda2ato-0.2.3/
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)    34523 2023-11-20 17:47:17.000000 easyeda2ato-0.2.3/LICENSE
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)      283 2024-04-11 00:42:55.000000 easyeda2ato-0.2.3/MANIFEST.in
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     6141 2024-04-11 01:19:01.414490 easyeda2ato-0.2.3/PKG-INFO
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     5351 2024-03-15 22:17:17.000000 easyeda2ato-0.2.3/README.md
+drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 01:19:01.409558 easyeda2ato-0.2.3/easyeda2ato.egg-info/
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     6141 2024-04-11 01:19:01.000000 easyeda2ato-0.2.3/easyeda2ato.egg-info/PKG-INFO
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)      917 2024-04-11 01:19:01.000000 easyeda2ato-0.2.3/easyeda2ato.egg-info/SOURCES.txt
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)        1 2024-04-11 01:19:01.000000 easyeda2ato-0.2.3/easyeda2ato.egg-info/dependency_links.txt
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)       62 2024-04-11 01:19:01.000000 easyeda2ato-0.2.3/easyeda2ato.egg-info/entry_points.txt
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)        1 2024-04-11 01:14:44.000000 easyeda2ato-0.2.3/easyeda2ato.egg-info/not-zip-safe
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)       57 2024-04-11 01:19:01.000000 easyeda2ato-0.2.3/easyeda2ato.egg-info/requires.txt
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)       14 2024-04-11 01:19:01.000000 easyeda2ato-0.2.3/easyeda2ato.egg-info/top_level.txt
+drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 01:19:01.410965 easyeda2ato-0.2.3/easyeda2kicad/
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)       75 2024-04-11 01:15:17.000000 easyeda2ato-0.2.3/easyeda2kicad/__init__.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)    14054 2024-04-11 00:34:56.000000 easyeda2ato-0.2.3/easyeda2kicad/__main__.py
+drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 01:19:01.411397 easyeda2ato-0.2.3/easyeda2kicad/atopile/
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 01:17:18.000000 easyeda2ato-0.2.3/easyeda2kicad/atopile/__init__.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     3920 2024-03-23 03:04:45.000000 easyeda2ato-0.2.3/easyeda2kicad/atopile/export_ato.py
+drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 01:19:01.412773 easyeda2ato-0.2.3/easyeda2kicad/easyeda/
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)        0 2023-12-11 18:29:50.000000 easyeda2ato-0.2.3/easyeda2kicad/easyeda/__init__.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     2307 2024-03-15 22:15:55.000000 easyeda2ato-0.2.3/easyeda2kicad/easyeda/easyeda_api.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     9743 2024-03-15 22:15:55.000000 easyeda2ato-0.2.3/easyeda2kicad/easyeda/easyeda_importer.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)    14438 2024-03-15 22:15:55.000000 easyeda2ato-0.2.3/easyeda2kicad/easyeda/parameters_easyeda.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     1833 2023-12-11 18:29:50.000000 easyeda2ato-0.2.3/easyeda2kicad/easyeda/svg_path_parser.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     5263 2023-12-11 18:29:50.000000 easyeda2ato-0.2.3/easyeda2kicad/helpers.py
+drwxr-xr-x   0 narayanpowderly   (501) staff       (20)        0 2024-04-11 01:19:01.414111 easyeda2ato-0.2.3/easyeda2kicad/kicad/
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)        0 2023-12-11 18:29:50.000000 easyeda2ato-0.2.3/easyeda2kicad/kicad/__init__.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     4737 2024-03-15 22:15:55.000000 easyeda2ato-0.2.3/easyeda2kicad/kicad/export_kicad_3d_model.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)    18012 2023-12-11 18:29:50.000000 easyeda2ato-0.2.3/easyeda2kicad/kicad/export_kicad_footprint.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)    12792 2023-12-11 18:29:50.000000 easyeda2ato-0.2.3/easyeda2kicad/kicad/export_kicad_symbol.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     7207 2023-12-11 18:29:50.000000 easyeda2ato-0.2.3/easyeda2kicad/kicad/parameters_kicad_footprint.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)    22150 2023-12-11 18:29:50.000000 easyeda2ato-0.2.3/easyeda2kicad/kicad/parameters_kicad_symbol.py
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     1244 2023-12-11 18:09:41.000000 easyeda2ato-0.2.3/pyproject.toml
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)      446 2024-04-11 01:19:01.414893 easyeda2ato-0.2.3/setup.cfg
+-rw-r--r--   0 narayanpowderly   (501) staff       (20)     1721 2024-04-11 01:18:53.000000 easyeda2ato-0.2.3/setup.py
```

### Comparing `easyeda2ato-0.2.2/LICENSE` & `easyeda2ato-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/PKG-INFO` & `easyeda2ato-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyeda2ato
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python script that convert any electronic components from LCSC or EasyEDA to a Kicad library
 Home-page: https://github.com/uPesy/easyeda2kicad.py
 Author: uPesy
 Author-email: contact@upesy.com
 License: AGPL-3.0
 Project-URL: Code, https://github.com/uPesy/easyeda2kicad.py
 Keywords: easyeda kicad library conversion
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: easyeda2ato Version: 0.2.2 Summary: A Python script
+Metadata-Version: 2.1 Name: easyeda2ato Version: 0.2.3 Summary: A Python script
 that convert any electronic components from LCSC or EasyEDA to a Kicad library
 Home-page: https://github.com/uPesy/easyeda2kicad.py Author: uPesy Author-
 email: contact@upesy.com License: AGPL-3.0 Project-URL: Code, https://
 github.com/uPesy/easyeda2kicad.py Keywords: easyeda kicad library conversion
 Platform: any Classifier: Intended Audience :: Developers Classifier: License
 :: OSI Approved :: GNU Affero General Public License v3 Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `easyeda2ato-0.2.2/README.md` & `easyeda2ato-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2ato.egg-info/PKG-INFO` & `easyeda2ato-0.2.3/easyeda2ato.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyeda2ato
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python script that convert any electronic components from LCSC or EasyEDA to a Kicad library
 Home-page: https://github.com/uPesy/easyeda2kicad.py
 Author: uPesy
 Author-email: contact@upesy.com
 License: AGPL-3.0
 Project-URL: Code, https://github.com/uPesy/easyeda2kicad.py
 Keywords: easyeda kicad library conversion
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: easyeda2ato Version: 0.2.2 Summary: A Python script
+Metadata-Version: 2.1 Name: easyeda2ato Version: 0.2.3 Summary: A Python script
 that convert any electronic components from LCSC or EasyEDA to a Kicad library
 Home-page: https://github.com/uPesy/easyeda2kicad.py Author: uPesy Author-
 email: contact@upesy.com License: AGPL-3.0 Project-URL: Code, https://
 github.com/uPesy/easyeda2kicad.py Keywords: easyeda kicad library conversion
 Platform: any Classifier: Intended Audience :: Developers Classifier: License
 :: OSI Approved :: GNU Affero General Public License v3 Classifier: Natural
 Language :: English Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `easyeda2ato-0.2.2/easyeda2ato.egg-info/SOURCES.txt` & `easyeda2ato-0.2.3/easyeda2ato.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 easyeda2ato.egg-info/entry_points.txt
 easyeda2ato.egg-info/not-zip-safe
 easyeda2ato.egg-info/requires.txt
 easyeda2ato.egg-info/top_level.txt
 easyeda2kicad/__init__.py
 easyeda2kicad/__main__.py
 easyeda2kicad/helpers.py
+easyeda2kicad/atopile/__init__.py
 easyeda2kicad/atopile/export_ato.py
 easyeda2kicad/easyeda/__init__.py
 easyeda2kicad/easyeda/easyeda_api.py
 easyeda2kicad/easyeda/easyeda_importer.py
 easyeda2kicad/easyeda/parameters_easyeda.py
 easyeda2kicad/easyeda/svg_path_parser.py
 easyeda2kicad/kicad/__init__.py
```

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/__main__.py` & `easyeda2ato-0.2.3/easyeda2kicad/__main__.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/atopile/export_ato.py` & `easyeda2ato-0.2.3/easyeda2kicad/atopile/export_ato.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/easyeda/easyeda_api.py` & `easyeda2ato-0.2.3/easyeda2kicad/easyeda/easyeda_api.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/easyeda/easyeda_importer.py` & `easyeda2ato-0.2.3/easyeda2kicad/easyeda/easyeda_importer.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/easyeda/parameters_easyeda.py` & `easyeda2ato-0.2.3/easyeda2kicad/easyeda/parameters_easyeda.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/easyeda/svg_path_parser.py` & `easyeda2ato-0.2.3/easyeda2kicad/easyeda/svg_path_parser.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/helpers.py` & `easyeda2ato-0.2.3/easyeda2kicad/helpers.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/kicad/export_kicad_3d_model.py` & `easyeda2ato-0.2.3/easyeda2kicad/kicad/export_kicad_3d_model.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/kicad/export_kicad_footprint.py` & `easyeda2ato-0.2.3/easyeda2kicad/kicad/export_kicad_footprint.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/kicad/export_kicad_symbol.py` & `easyeda2ato-0.2.3/easyeda2kicad/kicad/export_kicad_symbol.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/kicad/parameters_kicad_footprint.py` & `easyeda2ato-0.2.3/easyeda2kicad/kicad/parameters_kicad_footprint.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/easyeda2kicad/kicad/parameters_kicad_symbol.py` & `easyeda2ato-0.2.3/easyeda2kicad/kicad/parameters_kicad_symbol.py`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/pyproject.toml` & `easyeda2ato-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyeda2ato-0.2.2/setup.py` & `easyeda2ato-0.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,29 +16,30 @@
     name="easyeda2ato",
     description=(
         "A Python script that convert any electronic components from LCSC or EasyEDA to"
         " a Kicad library"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.2.2",
+    version="0.2.3",
     author="uPesy",
     author_email="contact@upesy.com",
     url="https://github.com/uPesy/easyeda2kicad.py",
     project_urls={
         "Code": "https://github.com/uPesy/easyeda2kicad.py",
     },
     # download_url='',
     license="AGPL-3.0",
     py_modules=["easyeda2kicad"],
     platforms="any",
-    packages=find_packages(exclude=["tests", "utils"]),
+    packages=find_packages(),
     package_dir={"easyeda2kicad": "easyeda2kicad"},
     entry_points={"console_scripts": ["easyeda2kicad = easyeda2kicad.__main__:main"]},
     python_requires=">=3.6",
+    include_package_data=True,
     install_requires=production_dependencies,
     extras_require={"dev": development_dependencies},
     zip_safe=False,
     keywords="easyeda kicad library conversion",
     classifiers=[
         # More information at https://pypi.org/classifiers/.
         "Intended Audience :: Developers",
```

