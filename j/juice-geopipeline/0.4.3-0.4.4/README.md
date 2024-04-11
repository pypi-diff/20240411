# Comparing `tmp/juice_geopipeline-0.4.3-py3-none-any.whl.zip` & `tmp/juice_geopipeline-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,19 @@
-Zip file size: 13694 bytes, number of entries: 13
+Zip file size: 24992 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       93 b- defN 23-Aug-31 07:16 geopipeline/__init__.py
 -rw-r--r--  2.0 unx     1818 b- defN 23-Aug-30 15:47 geopipeline/__main__.py
 -rw-r--r--  2.0 unx     6413 b- defN 24-Mar-04 14:43 geopipeline/cli.py
 -rw-r--r--  2.0 unx     5514 b- defN 24-Mar-05 09:39 geopipeline/science_planning.py
 -rw-r--r--  2.0 unx     3037 b- defN 23-Nov-27 19:37 geopipeline/setup.py
 -rw-r--r--  2.0 unx     4413 b- defN 23-Nov-27 19:35 geopipeline/time.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Nov-30 23:57 geopipeline/geometry/__init__.py
+-rw-r--r--  2.0 unx    16152 b- defN 24-Mar-05 11:21 geopipeline/geometry/derived.py
+-rw-r--r--  2.0 unx    45748 b- defN 24-Mar-06 14:19 geopipeline/geometry/finder.py
+-rw-r--r--  2.0 unx     1303 b- defN 24-Feb-26 12:02 geopipeline/geometry/support.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Nov-30 23:57 geopipeline/models/__init__.py
 -rw-r--r--  2.0 unx     5088 b- defN 23-Dec-12 01:35 geopipeline/models/magnetic_field.py
--rw-r--r--  2.0 unx     5293 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      244 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1095 b- defN 24-Apr-09 10:51 juice_geopipeline-0.4.3.dist-info/RECORD
-13 files, 33112 bytes uncompressed, 11848 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx     5346 b- defN 24-Apr-11 13:53 juice_geopipeline-0.4.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 13:53 juice_geopipeline-0.4.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      244 b- defN 24-Apr-11 13:53 juice_geopipeline-0.4.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-11 13:53 juice_geopipeline-0.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1446 b- defN 24-Apr-11 13:53 juice_geopipeline-0.4.4.dist-info/RECORD
+17 files, 96719 bytes uncompressed, 22594 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -12,29 +12,41 @@
 
 Filename: geopipeline/setup.py
 Comment: 
 
 Filename: geopipeline/time.py
 Comment: 
 
+Filename: geopipeline/geometry/__init__.py
+Comment: 
+
+Filename: geopipeline/geometry/derived.py
+Comment: 
+
+Filename: geopipeline/geometry/finder.py
+Comment: 
+
+Filename: geopipeline/geometry/support.py
+Comment: 
+
 Filename: geopipeline/models/__init__.py
 Comment: 
 
 Filename: geopipeline/models/magnetic_field.py
 Comment: 
 
-Filename: juice_geopipeline-0.4.3.dist-info/METADATA
+Filename: juice_geopipeline-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: juice_geopipeline-0.4.3.dist-info/WHEEL
+Filename: juice_geopipeline-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: juice_geopipeline-0.4.3.dist-info/entry_points.txt
+Filename: juice_geopipeline-0.4.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: juice_geopipeline-0.4.3.dist-info/top_level.txt
+Filename: juice_geopipeline-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: juice_geopipeline-0.4.3.dist-info/RECORD
+Filename: juice_geopipeline-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `juice_geopipeline-0.4.3.dist-info/METADATA` & `juice_geopipeline-0.4.4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: juice-geopipeline
-Version: 0.4.3
+Version: 0.4.4
 Author: Marc Costa
 Author-email: marc.costa@ext.esa.int
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: planetary-coverage
 Requires-Dist: python-dotenv
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: pytest
 Requires-Dist: numpy
+Requires-Dist: PyAstronomy
+Requires-Dist: astroquery
 Provides-Extra: dev
 Requires-Dist: autoflake ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
 Requires-Dist: flake8-bugbear ; extra == 'dev'
 Requires-Dist: flake8-builtins ; extra == 'dev'
 Requires-Dist: flake8-comprehensions ; extra == 'dev'
```

