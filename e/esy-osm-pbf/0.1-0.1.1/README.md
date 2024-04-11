# Comparing `tmp/esy-osm-pbf-0.1.tar.gz` & `tmp/esy-osm-pbf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esy-osm-pbf-0.1.tar", last modified: Thu Apr 11 08:56:32 2024, max compression
+gzip compressed data, was "esy-osm-pbf-0.1.1.tar", last modified: Thu Apr 11 09:08:12 2024, max compression
```

## Comparing `esy-osm-pbf-0.1.tar` & `esy-osm-pbf-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 08:56:32.694184 esy-osm-pbf-0.1/
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1088 2024-04-11 07:30:25.000000 esy-osm-pbf-0.1/LICENSE
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     3892 2024-04-11 08:56:32.694184 esy-osm-pbf-0.1/PKG-INFO
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1666 2024-04-11 07:30:25.000000 esy-osm-pbf-0.1/README.md
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1053 2024-04-11 07:38:10.000000 esy-osm-pbf-0.1/pyproject.toml
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       38 2024-04-11 08:56:32.694184 esy-osm-pbf-0.1/setup.cfg
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 08:56:32.690184 esy-osm-pbf-0.1/src/
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 08:56:32.690184 esy-osm-pbf-0.1/src/esy/
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 08:56:32.690184 esy-osm-pbf-0.1/src/esy/osm/
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 08:56:32.694184 esy-osm-pbf-0.1/src/esy/osm/pbf/
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1934 2024-04-11 07:30:25.000000 esy-osm-pbf-0.1/src/esy/osm/pbf/__init__.py
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     7558 2024-04-11 07:30:25.000000 esy-osm-pbf-0.1/src/esy/osm/pbf/file.py
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1783 2024-04-11 06:31:34.000000 esy-osm-pbf-0.1/src/esy/osm/pbf/fileformat_pb2.py
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     3184 2024-04-11 06:31:34.000000 esy-osm-pbf-0.1/src/esy/osm/pbf/index.py
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     8525 2024-04-11 06:31:34.000000 esy-osm-pbf-0.1/src/esy/osm/pbf/osmformat_pb2.py
--rwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)     1835 2024-04-11 07:30:25.000000 esy-osm-pbf-0.1/src/esy/osm/pbf/test.py
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 08:56:32.694184 esy-osm-pbf-0.1/src/esy_osm_pbf.egg-info/
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     3892 2024-04-11 08:56:32.000000 esy-osm-pbf-0.1/src/esy_osm_pbf.egg-info/PKG-INFO
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)      394 2024-04-11 08:56:32.000000 esy-osm-pbf-0.1/src/esy_osm_pbf.egg-info/SOURCES.txt
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)        1 2024-04-11 08:56:32.000000 esy-osm-pbf-0.1/src/esy_osm_pbf.egg-info/dependency_links.txt
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       27 2024-04-11 08:56:32.000000 esy-osm-pbf-0.1/src/esy_osm_pbf.egg-info/requires.txt
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)        4 2024-04-11 08:56:32.000000 esy-osm-pbf-0.1/src/esy_osm_pbf.egg-info/top_level.txt
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 09:08:12.358933 esy-osm-pbf-0.1.1/
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1088 2024-04-11 07:30:25.000000 esy-osm-pbf-0.1.1/LICENSE
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     4215 2024-04-11 09:08:12.358933 esy-osm-pbf-0.1.1/PKG-INFO
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1987 2024-04-11 09:05:27.000000 esy-osm-pbf-0.1.1/README.md
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1055 2024-04-11 09:06:26.000000 esy-osm-pbf-0.1.1/pyproject.toml
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       38 2024-04-11 09:08:12.358933 esy-osm-pbf-0.1.1/setup.cfg
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 09:08:12.354933 esy-osm-pbf-0.1.1/src/
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 09:08:12.354933 esy-osm-pbf-0.1.1/src/esy/
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 09:08:12.354933 esy-osm-pbf-0.1.1/src/esy/osm/
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 09:08:12.358933 esy-osm-pbf-0.1.1/src/esy/osm/pbf/
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     2255 2024-04-11 09:05:44.000000 esy-osm-pbf-0.1.1/src/esy/osm/pbf/__init__.py
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     7558 2024-04-11 07:30:25.000000 esy-osm-pbf-0.1.1/src/esy/osm/pbf/file.py
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1783 2024-04-11 06:31:34.000000 esy-osm-pbf-0.1.1/src/esy/osm/pbf/fileformat_pb2.py
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     3184 2024-04-11 06:31:34.000000 esy-osm-pbf-0.1.1/src/esy/osm/pbf/index.py
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     8525 2024-04-11 06:31:34.000000 esy-osm-pbf-0.1.1/src/esy/osm/pbf/osmformat_pb2.py
+-rwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)     1835 2024-04-11 07:30:25.000000 esy-osm-pbf-0.1.1/src/esy/osm/pbf/test.py
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-11 09:08:12.358933 esy-osm-pbf-0.1.1/src/esy_osm_pbf.egg-info/
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     4215 2024-04-11 09:08:12.000000 esy-osm-pbf-0.1.1/src/esy_osm_pbf.egg-info/PKG-INFO
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)      394 2024-04-11 09:08:12.000000 esy-osm-pbf-0.1.1/src/esy_osm_pbf.egg-info/SOURCES.txt
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)        1 2024-04-11 09:08:12.000000 esy-osm-pbf-0.1.1/src/esy_osm_pbf.egg-info/dependency_links.txt
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       27 2024-04-11 09:08:12.000000 esy-osm-pbf-0.1.1/src/esy_osm_pbf.egg-info/requires.txt
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)        4 2024-04-11 09:08:12.000000 esy-osm-pbf-0.1.1/src/esy_osm_pbf.egg-info/top_level.txt
```

### Comparing `esy-osm-pbf-0.1/LICENSE` & `esy-osm-pbf-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esy-osm-pbf-0.1/PKG-INFO` & `esy-osm-pbf-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esy-osm-pbf
-Version: 0.1
+Version: 0.1.1
 Summary: Low-level Python library to interact with OSM PBF files
 Author-email: Ontje Lünsdorf <ontje.luensdorf@dlr.de>
 License: MIT License
         
         Copyright (c) 2024, German Aerospace Center (DLR)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -93,7 +93,14 @@
 # Team
 
 `esy.osm.pbf` is developed by the
 [DLR](https://www.dlr.de/EN/Home/home_node.html) Institute of
 [Networked Energy Systems](https://www.dlr.de/ve/en/desktopdefault.aspx/tabid-12472/21440_read-49440/)
 in the departement for
 [Energy Systems Analysis (ESY)](https://www.dlr.de/ve/en/desktopdefault.aspx/tabid-12471/21741_read-49802/).
+
+# Acknowledgements
+
+The authors would like to thank the Federal Government and the Heads of
+Government of the Länder, as well as the Joint Science Conference (GWK), for
+their funding and support within the framework of the NFDI4Ing consortium.
+Funded by the German Research Foundation (DFG) - project number 442146713.
```

### Comparing `esy-osm-pbf-0.1/README.md` & `esy-osm-pbf-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -45,7 +45,14 @@
 # Team
 
 `esy.osm.pbf` is developed by the
 [DLR](https://www.dlr.de/EN/Home/home_node.html) Institute of
 [Networked Energy Systems](https://www.dlr.de/ve/en/desktopdefault.aspx/tabid-12472/21440_read-49440/)
 in the departement for
 [Energy Systems Analysis (ESY)](https://www.dlr.de/ve/en/desktopdefault.aspx/tabid-12471/21741_read-49802/).
+
+# Acknowledgements
+
+The authors would like to thank the Federal Government and the Heads of
+Government of the Länder, as well as the Joint Science Conference (GWK), for
+their funding and support within the framework of the NFDI4Ing consortium.
+Funded by the German Research Foundation (DFG) - project number 442146713.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esy-osm-pbf-0.1/pyproject.toml` & `esy-osm-pbf-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'esy-osm-pbf'
 description = 'Low-level Python library to interact with OSM PBF files'
-version = '0.1'
+version = '0.1.1'
 license = {file = 'LICENSE'}
 readme = 'README.md'
 requires-python = '>= 3.5'
 dependencies = ['protobuf >= 3.20']
 keywords = ['OSM', 'OpenStreetMap', 'PBF', 'protobuf']
 classifiers = [
     'Development Status :: 5 - Production/Stable',
```

### Comparing `esy-osm-pbf-0.1/src/esy/osm/pbf/__init__.py` & `esy-osm-pbf-0.1.1/src/esy/osm/pbf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,21 @@
 # Team
 
 `esy.osm.pbf` is developed by the
 [DLR](https://www.dlr.de/EN/Home/home_node.html) Institute of
 [Networked Energy Systems](https://www.dlr.de/ve/en/desktopdefault.aspx/tabid-12472/21440_read-49440/)
 in the departement for
 [Energy Systems Analysis (ESY)](https://www.dlr.de/ve/en/desktopdefault.aspx/tabid-12471/21741_read-49802/).
+
+# Acknowledgements
+
+The authors would like to thank the Federal Government and the Heads of
+Government of the Länder, as well as the Joint Science Conference (GWK), for
+their funding and support within the framework of the NFDI4Ing consortium.
+Funded by the German Research Foundation (DFG) - project number 442146713.
 '''
 
 import importlib.metadata
 
 from esy.osm.pbf.file import (
     File, Node, Way, Relation, iter_blocks, read_blob, iter_primitive_block,
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `esy-osm-pbf-0.1/src/esy/osm/pbf/file.py` & `esy-osm-pbf-0.1.1/src/esy/osm/pbf/file.py`

 * *Files identical despite different names*

### Comparing `esy-osm-pbf-0.1/src/esy/osm/pbf/fileformat_pb2.py` & `esy-osm-pbf-0.1.1/src/esy/osm/pbf/fileformat_pb2.py`

 * *Files identical despite different names*

### Comparing `esy-osm-pbf-0.1/src/esy/osm/pbf/index.py` & `esy-osm-pbf-0.1.1/src/esy/osm/pbf/index.py`

 * *Files identical despite different names*

### Comparing `esy-osm-pbf-0.1/src/esy/osm/pbf/osmformat_pb2.py` & `esy-osm-pbf-0.1.1/src/esy/osm/pbf/osmformat_pb2.py`

 * *Files identical despite different names*

### Comparing `esy-osm-pbf-0.1/src/esy/osm/pbf/test.py` & `esy-osm-pbf-0.1.1/src/esy/osm/pbf/test.py`

 * *Files identical despite different names*

### Comparing `esy-osm-pbf-0.1/src/esy_osm_pbf.egg-info/PKG-INFO` & `esy-osm-pbf-0.1.1/src/esy_osm_pbf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esy-osm-pbf
-Version: 0.1
+Version: 0.1.1
 Summary: Low-level Python library to interact with OSM PBF files
 Author-email: Ontje Lünsdorf <ontje.luensdorf@dlr.de>
 License: MIT License
         
         Copyright (c) 2024, German Aerospace Center (DLR)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -93,7 +93,14 @@
 # Team
 
 `esy.osm.pbf` is developed by the
 [DLR](https://www.dlr.de/EN/Home/home_node.html) Institute of
 [Networked Energy Systems](https://www.dlr.de/ve/en/desktopdefault.aspx/tabid-12472/21440_read-49440/)
 in the departement for
 [Energy Systems Analysis (ESY)](https://www.dlr.de/ve/en/desktopdefault.aspx/tabid-12471/21741_read-49802/).
+
+# Acknowledgements
+
+The authors would like to thank the Federal Government and the Heads of
+Government of the Länder, as well as the Joint Science Conference (GWK), for
+their funding and support within the framework of the NFDI4Ing consortium.
+Funded by the German Research Foundation (DFG) - project number 442146713.
```

