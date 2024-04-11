# Comparing `tmp/data2rdf-1.1.0.tar.gz` & `tmp/data2rdf-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data2rdf-1.1.0.tar", last modified: Thu Mar 21 09:45:01 2024, max compression
+gzip compressed data, was "data2rdf-2.0.0rc0.tar", last modified: Thu Apr 11 13:39:24 2024, max compression
```

## Comparing `data2rdf-1.1.0.tar` & `data2rdf-2.0.0rc0.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.278975 data2rdf-1.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-03-21 09:44:56.000000 data2rdf-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-21 09:45:01.278975 data2rdf-1.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-03-21 09:44:56.000000 data2rdf-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.274975 data2rdf-1.1.0/data2rdf/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6592 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/abox_template_generation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1614 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/annotation_confs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9579 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/annotation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.274975 data2rdf-1.1.0/data2rdf/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      915 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/cli/abox_conversion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5564 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/csv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.274975 data2rdf-1.1.0/data2rdf/emmo_lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/emmo_lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3053 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/emmo_lib/chowlk_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1686 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/emmo_lib/emmo_unit_prefixes.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     3945 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/emmo_lib/emmo_units.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     4481 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/emmo_lib/emmo_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/emmo_lib/get_emmo_label_mappping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2024 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/emmo_lib/get_emmo_unit_prefix_df.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8653 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/excel_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16607 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/pipeline_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8078 2024-03-21 09:44:56.000000 data2rdf-1.1.0/data2rdf/rdf_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.278975 data2rdf-1.1.0/data2rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-21 09:45:01.000000 data2rdf-1.1.0/data2rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-21 09:45:01.000000 data2rdf-1.1.0/data2rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 09:45:01.000000 data2rdf-1.1.0/data2rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-21 09:45:01.000000 data2rdf-1.1.0/data2rdf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-21 09:45:01.000000 data2rdf-1.1.0/data2rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-21 09:45:01.000000 data2rdf-1.1.0/data2rdf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1796 2024-03-21 09:45:01.278975 data2rdf-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-03-21 09:44:56.000000 data2rdf-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.274975 data2rdf-1.1.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.274975 data2rdf-1.1.0/tests/csv_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/csv_pipeline_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.274975 data2rdf-1.1.0/tests/csv_pipeline_test/input/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/csv_pipeline_test/input/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      840 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/csv_pipeline_test/test_abox_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2555 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/csv_pipeline_test/test_csv2rdf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/csv_pipeline_test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:45:01.278975 data2rdf-1.1.0/tests/xls_pipeline_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/xls_pipeline_test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      840 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/xls_pipeline_test/test_abox_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2090 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/xls_pipeline_test/test_excel2rdf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-03-21 09:44:56.000000 data2rdf-1.1.0/tests/xls_pipeline_test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2505 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/data2rdf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6212 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/abox_template_generation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7614 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/annotation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/data2rdf/chowlk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/chowlk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2610 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/chowlk/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5092 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/csv_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8035 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/excel_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16621 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/pipeline_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/data2rdf/qudt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/qudt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/qudt/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9129 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/data2rdf/rdf_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/data2rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-11 13:39:23.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-11 13:39:24.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:39:23.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 13:39:23.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 13:39:24.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 13:39:24.000000 data2rdf-2.0.0rc0/data2rdf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1939 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      104 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/tests/csv_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.013297 data2rdf-2.0.0rc0/tests/csv_pipeline_test/input/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/input/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/test_abox_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/test_csv2rdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/csv_pipeline_test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:24.017297 data2rdf-2.0.0rc0/tests/xls_pipeline_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/xls_pipeline_test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      882 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/xls_pipeline_test/test_abox_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/xls_pipeline_test/test_excel2rdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      177 2024-04-11 13:39:18.000000 data2rdf-2.0.0rc0/tests/xls_pipeline_test/test_utils.py
```

### Comparing `data2rdf-1.1.0/LICENSE` & `data2rdf-2.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `data2rdf-1.1.0/PKG-INFO` & `data2rdf-2.0.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 1.1.0
+Version: 2.0.0rc0
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
-Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy
-Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de
+Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
+Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.0.0
 Requires-Dist: chowlk-unofficial-fork==0.0.2
+Requires-Dist: lru-cache<1
 Requires-Dist: openpyxl<4,>=3
 Requires-Dist: pandas<3,>=2
+Requires-Dist: pydantic<3,>=2
+Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
 Requires-Dist: python-magic==0.4.27
-Requires-Dist: rdflib==6.2.0
+Requires-Dist: rdflib<7,>=6
+Requires-Dist: requests
 Requires-Dist: tables==3.8.0
 Provides-Extra: dev
 Requires-Dist: bumpver==2021.1114; extra == "dev"
 Requires-Dist: dunamai==1.7.0; extra == "dev"
 Provides-Extra: docs
+Requires-Dist: html5lib==1.1; extra == "docs"
 Requires-Dist: ipython==8.12.3; extra == "docs"
 Requires-Dist: jinja2==3.1.3; extra == "docs"
 Requires-Dist: jupyter==1.0.0; extra == "docs"
 Requires-Dist: myst-parser==2.0.0; extra == "docs"
 Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 Requires-Dist: sphinx==6.2.1; extra == "docs"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `data2rdf-1.1.0/README.md` & `data2rdf-2.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `data2rdf-1.1.0/data2rdf/abox_template_generation.py` & `data2rdf-2.0.0rc0/data2rdf/abox_template_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 from pathlib import Path
 
 from rdflib import Graph, Literal, URIRef
 from rdflib.namespace import OWL, RDF, RDFS, SKOS
 
-from data2rdf.emmo_lib import chowlk_utils
+from data2rdf.chowlk.utils import add_emmo_name_to_diagrams
 
 
 def run_chowlk(inputfile, outputfile):
     from chowlk.transformations import transform_ontology
     from chowlk.utils import read_drawio_xml
 
     logging.info(
@@ -146,17 +146,15 @@
         # filename = pathlib.Path(self.xml_path).name
 
         # self.mod_xml_path = os.path.join(out_path, filename.replace(".xml",".mod.xml"))
         # self.ttl_path = os.path.join(out_path, filename.replace('.xml','.ttl'))
         # self.ttl_path_ns = os.path.join(out_path, filename.replace('.xml','.ns.ttl'))
 
     def xml_conversion(self):
-        chowlk_utils.add_emmo_name_to_diagrams(
-            self.xml_path, self.mod_xml_path
-        )
+        add_emmo_name_to_diagrams(self.xml_path, self.mod_xml_path)
 
     def run_chowlk(self):
         run_chowlk(self.mod_xml_path, self.ttl_path)
 
     def add_individual_labels(self):
         add_individual_labels(self.ttl_path, self.ttl_path)
 
@@ -191,16 +189,7 @@
     def create_output_next_to_file(self):
         top_folder_path = os.path.dirname(os.path.abspath(self.xml_path))
         folder_path = os.path.join(top_folder_path, self.base_file_name)
         os.makedirs(folder_path, exist_ok=True)
         self.set_output_paths(folder_path)
 
         self.run_pipeline()
-
-
-# FOLDER_PATH = os.path.dirname(os.path.abspath(__file__))
-# TT_EXAMPLE_PATH = os.path.join(FOLDER_PATH, "tests", "tensile_test_example")
-# XML_FILE_PATH = os.path.join(TT_EXAMPLE_PATH,"tensile_test_method_v6.xml")
-# OUTPUT_PATH = os.path.join(TT_EXAMPLE_PATH)
-
-# abox_pipeline = ABoxScaffoldPipeline(XML_FILE_PATH, OUTPUT_PATH)
-# abox_pipeline.run_pipeline()
```

### Comparing `data2rdf-1.1.0/data2rdf/annotation_pipeline.py` & `data2rdf-2.0.0rc0/data2rdf/annotation_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import os
 from pathlib import Path
 
+import pandas as pd
 from rdflib import Graph
 
-from data2rdf.abox_template_generation import (
-    add_individual_labels,
-    convert_abox_namespace,
-)
+from data2rdf.abox_template_generation import convert_abox_namespace
+from data2rdf.config import config
 from data2rdf.csv_parser import CSVParser
 from data2rdf.excel_parser import ExcelParser
-from data2rdf.mapper import Mapper, merge_same_as_individuals
 from data2rdf.rdf_generation import RDFGenerator
 
 parser_choice = {
     "csv": CSVParser,
     "excel": ExcelParser,
 }
 
@@ -25,32 +23,32 @@
     The mapping is updated. Hence the already created mapping is kept, only the mapping choices are renewed.
 
     Attributes:
         input_file (str): The file path for the file used as input for the pipeline. Must be a file that can be processed with the provided parser (e.g. csv / excel).
         parser(str): The parser used to read the meta data and column data from the file (csv or excel).
         parser_args(dict): A dict with specific arguments for the parser. Is passed to the parser as kwargs.
         mapping_file(str): The file path for the mapping_file (in .xlsx excel format).
-        template(str): The file path for the abox template (in .ttl format).
         output(str): The path for the output folder. This is where all the output files will be stored. The folder will be created.
+        template(str, optional): The file path for the abox template (in .ttl format).
         base_iri(str): An iri used as base for the generated graph entities. The base will be extended by an automatically generated uuid such as: base_iri/uuid#entity
         mapping_db(str, optional): The file path for a mapping database. Can be used to predict possible mappings based on the mapping_file
         only_use_base_iri (bool): In some cases it is not good to automatically add an UUID to the iri. E.g. mapping of the iri to the generated file IDs of the DSMS.
         data_download_iri (str): Download location of the columns. E.g.: https://127.0.0.1/id. This will be added as downloadURL to the created columns. This url can than be used to serve the columns e.g. as json. The DSMS rest-api uses this url.
     """
 
     def __init__(
         self,
         input_file,
         parser,
         parser_args,
-        template,
         mapping_file,
         output,
+        template=None,
         mapping_db=None,
-        base_iri="http://www.test2.de",
+        base_iri=config.base_iri,
         only_use_base_iri=True,
         data_download_iri=None,
     ):
         self.input_file = input_file
 
         self.parser = parser_choice[parser]
         self.parser_args = parser_args
@@ -84,21 +82,14 @@
         self.data_storage_path = os.path.join(
             self.output, f"{self.input_file_name}.datastorage.hdf5"
         )
         self.data_graph = os.path.join(
             self.output, f"{self.input_file_name}.metadata.ttl"
         )
 
-        self.mapping_table = os.path.join(
-            self.output, f"{self.input_file_name}.mapping-result.xlsx"
-        )
-        self.mapping_ttl = os.path.join(
-            self.output, f"{self.input_file_name}.mapping.ttl"
-        )
-
         self.mapping_prediction = os.path.join(
             self.output, f"{self.input_file_name}.predicted-mapping.csv"
         )
 
         self.unique_abox_template = os.path.join(
             self.output, f"{self.input_file_name}.abox.ttl"
         )
@@ -118,31 +109,52 @@
             **self.parser_args,
         )
 
         self.parser.parser_data()
         self.parser.generate_excel_spreadsheet(self.generic_output)
         self.parser.generate_data_storage()
 
+    def generate_file_uri(self):
+        """Get the file uri to be used as prefix in the knowledge graph."""
+        file_meta_df = pd.read_excel(
+            self.generic_output, sheet_name="file", engine="openpyxl"
+        )
+        file_meta_df.set_index("index", inplace=True)
+
+        if self.only_use_base_iri:
+            self.file_uri = file_meta_df.loc["namespace", "value"] + "/"
+        else:
+            self.file_uri = (
+                "/".join(
+                    [
+                        file_meta_df.loc["namespace", "value"],
+                        file_meta_df.loc["uuid", "value"],
+                    ]
+                )
+                + "#"
+            )
+
     def write_rdf(self):
         """
         Generates a RDF graph representation of the parsed data. This graph uses a generic data model.
         Each meta data point and column creates one OWL individual.
         The quantities are described using EMMO and EMMO units.
         The graph itself is not yet interoperable. It is only a conversion of the data to RDF.
         Interoperability is achieved when the created individuals are mapped to
         individuals of the process graph (created with the abox template).
         """
 
         self.writer = RDFGenerator(
-            self.generic_output, self.only_use_base_iri, self.data_download_iri
+            self.generic_output,
+            self.mapping_file,
+            self.file_uri,
+            self.data_download_iri,
         )
 
-        self.file_uri = (
-            self.writer.generate_file_json()
-        )  # store the file uri and use for the abox
+        self.writer.generate_file_json()
         self.writer.generate_meta_json()
         self.writer.generate_column_json()
 
         self.writer.to_ttl(self.data_graph)
 
     def convert_abox_template(self):
         """
@@ -151,88 +163,37 @@
         achieved by changing the namespace to a unique namespace.
         """
 
         convert_abox_namespace(
             self.template, self.unique_abox_template, unique_uri=self.file_uri
         )
 
-        add_individual_labels(
-            self.unique_abox_template, self.unique_abox_template
-        )
-
-    def update_mapping(self):
-        """
-        Takes the mapping file and adds the new mapping choices extracted from the data graph and the process
-        graph. The mapping matches need to be adjusted manually by the uses.
-        This means, that the for example a data set
-        with a slightly different naming convention (E.g.: Prüfer vs Pruefer vs Tester ...) can
-        be used for the same pipeline. The mapping only needs to be adjusted for the data entities
-        with names different to the original mapping.
-        This applies as well to a changed method graph.
-
-        To make is even easier for the user the mapping is also predicted using a word match algorithm and a
-        DB with known mapping (currently extracted from the synonyms of the stahldigital ontology).
-        The user can use the predicted mapping as a guide to create the new one.
-        """
-
-        self.mapper = Mapper(
-            self.data_graph, self.unique_abox_template, self.mapping_file
-        )
-        self.mapper.update_mapping_template()
-
-        if self.mapping_db:
-            self.mapper.predict_mapping(
-                self.mapping_prediction, self.mapping_db
-            )
-
-    def create_mapping(self):
-        """
-        Maps the data individuals and the process individuals based on the label matches provided in the
-        mapping excel. Mapping means in this context, that an OWL:sameAs relation points from the data individual to
-        the corresponding process individual. An OWl-reasoner (e.g. AllegroGraph) can
-        infer that those two individuals are actually the same.
-
-        The mapping is exported as a mapping table, that provides verbose
-        information of the individuals and the mapping
-        as well as a .ttl file, that exports the mapping as a RDF graph.
-        """
-
-        self.mapper = Mapper(
-            self.data_graph, self.unique_abox_template, self.mapping_file
-        )
-        self.mapper.map_data_and_abox(worksheet="sameas")
-        self.mapper.export_merged_mapping_table(self.mapping_table)
-        self.mapper.export_mapping_as_ttl(self.mapping_ttl)
-
     def run_pipeline(self):
         """
         Runs the complete pipeline with all required steps.
         """
 
         self.create_output()
         self.parse_data()
+        self.generate_file_uri()
         self.write_rdf()
-        self.convert_abox_template()
-        self.update_mapping()
-        self.create_mapping()
+        if self.template:
+            self.convert_abox_template()
 
-    def export_graph(self, merge_same_as=True):
+    def export_graph(self):
         """
         Exports a merged rdflib graph of the data, process and mapping output.
         Can be used e.g. to load the data into a triple store using rdflib.
         """
 
         g = Graph(identifier=self.base_iri)
-        g.parse(self.unique_abox_template, format="ttl")
-        g.parse(self.mapping_ttl, format="ttl")
+        if self.template:
+            g.parse(self.unique_abox_template, format="ttl")
         g.parse(self.data_graph, format="ttl")
 
-        if merge_same_as:
-            g = merge_same_as_individuals(g)
-
         return g
 
     def export_ttl(self, f_path):
         """
         Exports a merged .ttl file graph of the data, process and mapping output.
         Can be used e.g. to load the data into a triple store using the stores file upload functionality
         (e.g. AllegroGraph).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `data2rdf-1.1.0/data2rdf/csv_parser.py` & `data2rdf-2.0.0rc0/data2rdf/csv_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         self.header_sep = header_sep
         self.column_sep = column_sep
         self.header_length = header_length
 
     def parser_data(self):
         self.get_file_encoding()
         self.load_file()
-        self.generate_file_uuid()
         self.parse_meta_data()
         self.split_meta_df()
         self.parse_table()
         self.generate_column_df()
         self.generate_file_meta_df()
         self.clean_table_df()
 
@@ -131,18 +130,7 @@
         self.column_df = pd.DataFrame(self.df_table.iloc[0, :])
         self.column_df.columns = ["unit"]
         self.column_df["titles"] = self.column_df.index
         self.column_df.index.name = "index"
 
     def clean_table_df(self):
         self.df_table = self.df_table.iloc[1:, :]
-
-    def generate_excel_spreadsheet(self, output_path):
-        with pd.ExcelWriter(output_path, engine="openpyxl") as writer:
-            self.file_meta_df.to_excel(writer, "file")
-            self.column_df.to_excel(writer, "column_meta")
-            self.meta_df.to_excel(writer, "meta")
-
-    def generate_data_storage(self):
-        self.df_table.to_hdf(
-            self.data_storage_path, key=self.data_storage_group_name
-        )
```

### Comparing `data2rdf-1.1.0/data2rdf/emmo_lib/chowlk_utils.py` & `data2rdf-2.0.0rc0/data2rdf/chowlk/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import re
 
 import pandas as pd
 from rdflib import Graph
 from rdflib.namespace import SKOS
 
-# pd.set_option('display.max_colwidth', None)  # or 199
-# pd.set_option('display.max_columns', None)  # or 1000
-
 
 def add_emmo_name_to_diagrams(
     input_file,
     output_file,
     emmo_ontology="https://emmo-repo.github.io/versions/1.0.0-alpha2/emmo.ttl",
 ):
     """
@@ -73,16 +70,7 @@
                     entity.split(":")[0], individual_name
                 )
                 text = text.replace(entity, new_entity)
 
     # store new XML
     with open(output_file, "w") as output_file:
         output_file.write(text)
-
-
-# INPUT_FILE = os.path.join("method_graph","tensile_test_method.xml")
-# OUTPUT_FILE = os.path.join("method_graph","tensile_test_method_conv.xml")
-# EMMO_ONTOLOGY = os.path.join("emmo","emmo.ttl")
-
-# add_emmo_name_to_diagrams(INPUT_FILE, OUTPUT_FILE, EMMO_ONTOLOGY)
-
-# TODO: Take care, that only EMMO namespaces are converted !!
```

### Comparing `data2rdf-1.1.0/data2rdf/excel_parser.py` & `data2rdf-2.0.0rc0/data2rdf/excel_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,14 @@
             namespace,
         )
 
         self.location_mapping_f_path = location_mapping_f_path
 
     def parser_data(self):
         self.load_file()
-        self.generate_file_uuid()
         self.load_mapping_file()
         self.parse_meta_data()
         self.generate_column_df()
         self.parse_table()
         self.generate_file_meta_df()
 
     def load_mapping_file(self):
@@ -212,23 +211,7 @@
                     "start": col_start_pos,
                     "end": col_end_pos,
                     "worksheet": sheet,
                 }
             )
 
         self.column_df = pd.DataFrame(column_data)
-        # print(self.column_df)
-
-    # def clean_table_df(self):
-    #    self.df_table = self.df_table.iloc[1:,:]
-
-    def generate_excel_spreadsheet(self, output_path):
-        with pd.ExcelWriter(output_path, engine="openpyxl") as writer:
-            self.file_meta_df.to_excel(writer, "file")
-            self.column_df.to_excel(writer, "column_meta")
-            self.meta_df.to_excel(writer, "meta")
-
-    def generate_data_storage(self):
-        # print(self.df_table)
-        self.df_table.to_hdf(
-            self.data_storage_path, key=self.data_storage_group_name
-        )
```

### Comparing `data2rdf-1.1.0/data2rdf/mapper.py` & `data2rdf-2.0.0rc0/data2rdf/mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import os
+# import os
 from string import Template
 
 import pandas as pd
-from openpyxl.styles import Font
+
+# from openpyxl.styles import Font
 from rdflib import Graph, URIRef
 from rdflib.namespace import OWL, RDFS, SKOS
 
-from data2rdf.annotation_confs import annotations
-
-# from data2rdf.key_map_prediction import prediction_key_map_based_on_db
+from data2rdf.data2rdf.config import annotations
 
 
 def merge_same_as_individuals(graph, convert_data_label_to_alt_label=True):
     """
     The mapper creates an OWL.sameAs relation between the data individuals and the method individuals.
     In some cases it is better to merge the individuals into one. This makes it simpler to navigate the graph.
     The merging is done by copying all relation from and to the data individuals onto the representative method individual.
@@ -206,44 +205,40 @@
     filter(?ind != <http://www.w3.org/2002/07/owl#NamedIndividual>)
     }
     """
 
     # convert method query to df
     qres = method_graph.query(method_label_query)
     method_ind_df = pd.DataFrame(
-        qres, columns=["Method Individuals", "Method Label Match"]
+        qres, columns=["Method Individuals", "Class type"]
     )
 
     # literals can not be matched using pandas merge
     # method_ind_df = method_ind_df.astype(str)
     # Pandas version above 1.1.5 doesn't convert literals to string using astype properly
     method_ind_df = method_ind_df.applymap(str)
 
     # convert the data individuals and their labels to df
     qres = data_graph.query(data_label_query)
-    data_ind_df = pd.DataFrame(
-        qres, columns=["Data Individuals", "Data Label Match"]
-    )
+    data_ind_df = pd.DataFrame(qres, columns=["Data Individuals", "Key"])
 
     # literals can not be matched using pandas merge
     # data_ind_df = data_ind_df.astype(str)
     # Pandas version above 1.1.5 doesn't convert literals to string using astype properly
     data_ind_df = data_ind_df.applymap(str)
 
     # use left join (left means the rows of the mapping file are preserved, see SQL join)
     # this allows to observe where the mapping is incomplete
 
     # merge mapping with data individuals
-    merged_mapping = pd.merge(
-        mapping_df, data_ind_df, how="left", on=["Data Label Match"]
-    )
+    merged_mapping = pd.merge(mapping_df, data_ind_df, how="left", on=["Key"])
 
     # merge mapping with method individuals
     merged_mapping = pd.merge(
-        merged_mapping, method_ind_df, how="left", on=["Method Label Match"]
+        merged_mapping, method_ind_df, how="left", on=["Class type"]
     )
 
     return merged_mapping
 
 
 def convert_mapping2graph(merged_mapping, mapping_output_file):
     """
@@ -268,96 +263,96 @@
                 URIRef(mapping["Method Individuals"]),
             )
         )
 
     mapping_graph.serialize(mapping_output_file, format="ttl")
 
 
-def create_mapping_template(
-    data_graph_file, method_graph_file, mapping_output, worksheet="sameas"
-):
-    data_graph = Graph()
-    data_graph.parse(data_graph_file, format="ttl")
-
-    method_graph = Graph()
-    method_graph.parse(method_graph_file, format="ttl")
-
-    # from the data we take only meta_data and column_data
-    data_label_query_template = Template(
-        """
-    PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
-    PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
-    PREFIX csvw: <http://www.w3.org/ns/csvw#>
-
-    SELECT distinct ?label
-    WHERE {
-    {?ind rdf:type <$meta>} UNION {?ind rdf:type <$column>} .
-    ?ind rdfs:label ?label
-    }
-    """
-    )
-
-    data_label_query = data_label_query_template.substitute(
-        column=annotations["column_class"], meta=annotations["meta_data_type"]
-    )
-
-    # from the method we take all named individuals
-    method_class_query = """
-    PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
-    PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
-    PREFIX csvw: <http://www.w3.org/ns/csvw#>
-
-    SELECT distinct ?label
-    WHERE {
-    ?ind rdf:type <http://www.w3.org/2002/07/owl#NamedIndividual> .
-    ?ind rdfs:label ?label .
-    filter(?ind != <http://www.w3.org/2002/07/owl#NamedIndividual>)
-    }
-    """
-
-    # convert method query to df
-    qres = method_graph.query(method_class_query)
-    method_ind_df = pd.DataFrame(qres, columns=["Method Labels"])
-    method_ind_df = method_ind_df.astype(str)
-    # literals can not be matched using pandas merge
-    # method_ind_df.sort_values(by = "Method Labels", inplace=True)
-    # convert the data individuals and their labels to df
-    qres = data_graph.query(data_label_query)
-    data_ind_df = pd.DataFrame(qres, columns=["Data Labels"])
-    data_ind_df = data_ind_df.astype(
-        str
-    )  # literals can not be matched using pandas merge
-    # data_ind_df.sort_values(by = "Data Labels", inplace=True)
-
-    # merge options and choices
-    match_table_df = pd.concat([method_ind_df, data_ind_df], axis=1)
-    match_table_df.columns = ["Method Label Choice", "Data Label Choice"]
-    # match_table_df.sort_values(by = ["Method Label Choice","Data Label Choice"], inplace=True)
-    # print(match_table_df)
-
-    for col in match_table_df:
-        match_table_df[col] = match_table_df[col].sort_values(
-            ignore_index=True
-        )
-
-    with pd.ExcelWriter(mapping_output, engine="openpyxl") as writer:
-        match_table_df.to_excel(writer, sheet_name=worksheet, index=False)
-
-        sheet = writer.sheets[worksheet]
+# def create_mapping_template(
+#     data_graph_file, method_graph_file, mapping_output, worksheet="sameas"
+# ):
+#     data_graph = Graph()
+#     data_graph.parse(data_graph_file, format="ttl")
+
+#     method_graph = Graph()
+#     method_graph.parse(method_graph_file, format="ttl")
+
+#     # from the data we take only meta_data and column_data
+#     data_label_query_template = Template(
+#         """
+#     PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
+#     PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
+#     PREFIX csvw: <http://www.w3.org/ns/csvw#>
+
+#     SELECT distinct ?label
+#     WHERE {
+#     {?ind rdf:type <$meta>} UNION {?ind rdf:type <$column>} .
+#     ?ind rdfs:label ?label
+#     }
+#     """
+#     )
+
+#     data_label_query = data_label_query_template.substitute(
+#         column=annotations["column_class"], meta=annotations["meta_data_type"]
+#     )
+
+#     # from the method we take all named individuals
+#     method_class_query = """
+#     PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
+#     PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
+#     PREFIX csvw: <http://www.w3.org/ns/csvw#>
+
+#     SELECT distinct ?label
+#     WHERE {
+#     ?ind rdf:type <http://www.w3.org/2002/07/owl#NamedIndividual> .
+#     ?ind rdfs:label ?label .
+#     filter(?ind != <http://www.w3.org/2002/07/owl#NamedIndividual>)
+#     }
+#     """
+
+#     # convert method query to df
+#     qres = method_graph.query(method_class_query)
+#     method_ind_df = pd.DataFrame(qres, columns=["Method Labels"])
+#     method_ind_df = method_ind_df.astype(str)
+#     # literals can not be matched using pandas merge
+#     # method_ind_df.sort_values(by = "Method Labels", inplace=True)
+#     # convert the data individuals and their labels to df
+#     qres = data_graph.query(data_label_query)
+#     data_ind_df = pd.DataFrame(qres, columns=["Data Labels"])
+#     data_ind_df = data_ind_df.astype(
+#         str
+#     )  # literals can not be matched using pandas merge
+#     # data_ind_df.sort_values(by = "Data Labels", inplace=True)
+
+#     # merge options and choices
+#     match_table_df = pd.concat([method_ind_df, data_ind_df], axis=1)
+#     match_table_df.columns = ["Method Label Choice", "Data Label Choice"]
+#     # match_table_df.sort_values(by = ["Method Label Choice","Data Label Choice"], inplace=True)
+#     # print(match_table_df)
+
+#     for col in match_table_df:
+#         match_table_df[col] = match_table_df[col].sort_values(
+#             ignore_index=True
+#         )
+
+#     with pd.ExcelWriter(mapping_output, engine="openpyxl") as writer:
+#         match_table_df.to_excel(writer, sheet_name=worksheet, index=False)
+
+#         sheet = writer.sheets[worksheet]
+
+#         # add column header
+#         sheet["D1"] = "Data Label Match"
+#         sheet["D1"].font = Font(bold=True)
+#         sheet["C1"] = "Method Label Match"
+#         sheet["C1"].font = Font(bold=True)
 
-        # add column header
-        sheet["D1"] = "Data Label Match"
-        sheet["D1"].font = Font(bold=True)
-        sheet["C1"] = "Method Label Match"
-        sheet["C1"].font = Font(bold=True)
+#         # end_choice = len(match_table_df.index) + 2
 
-        # end_choice = len(match_table_df.index) + 2
-
-        for col in "ABCD":
-            sheet.column_dimensions[col].width = 30
+#         for col in "ABCD":
+#             sheet.column_dimensions[col].width = 30
 
 
 # FOLDER_PATH = os.path.dirname(os.path.abspath(__file__))
 # TT_EXAMPLE_PATH = os.path.join(FOLDER_PATH, "tests/tensile_test_example_excel")
 
 # FILE_PATH = os.path.join(TT_EXAMPLE_PATH,"AFZ1-Fz-S1Q.xlsm")
 # LOCATION_MAPPING_FILE_PATH =
@@ -381,80 +376,80 @@
 
 
 def report_merge_result(merged_mapping_df):
     """
     Report the number of successfully mapped data individuals.
     """
 
-    data_count = merged_mapping_df["Data Label Choice"].dropna().count()
+    data_count = merged_mapping_df["Key"].dropna().count()
     mapping_count = len(merged_mapping_df.dropna())
 
     print(
         f"Of {data_count} data individuals, {mapping_count} were successfully mapped to the method. See the data.mapping-result.xlsx file for mapping results."
     )
 
 
 class Mapper:
     def __init__(self, data_graph_path, method_graph_path, mapping_path):
         self.data_graph_path = data_graph_path
         self.method_graph_path = method_graph_path
         self.mapping_path = mapping_path
 
-    def create_mapping_template(self, worksheet="sameas"):
-        if os.path.isfile(self.mapping_path):
-            raise FileExistsError(
-                "Mapping file exists, use update_mapping_template to update the choices but keep matches"
-            )
-
-        create_mapping_template(
-            self.data_graph_path,
-            self.method_graph_path,
-            self.mapping_path,
-            worksheet,
-        )
+    # def create_mapping_template(self, worksheet="sameas"):
+    #     if os.path.isfile(self.mapping_path):
+    #         raise FileExistsError(
+    #             "Mapping file exists, use update_mapping_template to update the choices but keep matches"
+    #         )
+
+    #     create_mapping_template(
+    #         self.data_graph_path,
+    #         self.method_graph_path,
+    #         self.mapping_path,
+    #         worksheet,
+    #     )
 
     def update_mapping_template(self, worksheet="sameas"):
         # if the mapping does not exist create it
-        if not os.path.isfile(self.mapping_path):
-            self.create_mapping_template()
-            return True
+        # if not os.path.isfile(self.mapping_path):
+        #     self.create_mapping_template()
+        #     return True
 
         mappings_to_keep = pd.read_excel(
             self.mapping_path,
             sheet_name=worksheet,
             engine="openpyxl",
         )
 
-        create_mapping_template(
-            self.data_graph_path,
-            self.method_graph_path,
-            self.mapping_path,
-            worksheet,
-        )
+        # create_mapping_template(
+        #     self.data_graph_path,
+        #     self.method_graph_path,
+        #     self.mapping_path,
+        #     worksheet,
+        # )
         # self.create_mapping_template()
 
         mappings_to_change = pd.read_excel(
             open(self.mapping_path, "rb"),
             sheet_name=worksheet,
             engine="openpyxl",
         )
 
         mappings_to_change.loc[
-            :, ["Method Label Match", "Data Label Match"]
-        ] = mappings_to_keep.loc[:, ["Method Label Match", "Data Label Match"]]
+            :, ["Class type", "Key", "Annotation"]
+        ] = mappings_to_keep.loc[:, ["Class type", "Key", "Annotation"]]
 
         with pd.ExcelWriter(self.mapping_path, engine="openpyxl") as writer:
             mappings_to_change.to_excel(
                 writer, sheet_name=worksheet, index=False
             )
 
-            sheet = writer.sheets[worksheet]
+            # sheet = writer.sheets[worksheet]
 
-            for col in "ABCD":
-                sheet.column_dimensions[col].width = 30
+            # for col in "ABCD":
+            #     sheet.column_dimensions[col].width = 30
 
     #   def predict_mapping(self, prediction_path, key_map_db, worksheet="sameas"):
     #      prediction_key_map_based_on_db(
     #           self.mapping_path, prediction_path, key_map_db, worksheet
     #      )
 
     def map_data_and_abox(self, worksheet="sameas"):
```

### Comparing `data2rdf-1.1.0/data2rdf/parser.py` & `data2rdf-2.0.0rc0/data2rdf/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,17 +31,17 @@
             data_storage_path
             if data_storage_path
             else f"{f_path}.datastorage.hdf5"
         )
         self.data_storage_group_name = data_storage_group_name
         self.namespace = namespace
         self.id_uuid = str(uuid.uuid4())
-
-    def generate_file_uuid(self):
-        self.id_uuid = str(uuid.uuid4())
+        self.column_df = None
+        self.df_table = None
+        self.meta_df = None
 
     def generate_file_meta_df(self):
         self.file_meta_df = pd.DataFrame(
             {
                 "value": [
                     self.f_path,
                     self.server_f_path,
@@ -49,14 +49,25 @@
                     self.id_uuid,
                 ]
             },
             index=["file_path", "server_file_path", "namespace", "uuid"],
         )
         self.file_meta_df.index.name = "index"
 
+    def generate_excel_spreadsheet(self, output_path):
+        with pd.ExcelWriter(output_path, engine="openpyxl") as writer:
+            self.file_meta_df.to_excel(writer, "file")
+            self.column_df.to_excel(writer, "column_meta")
+            self.meta_df.to_excel(writer, "meta")
+
+    def generate_data_storage(self):
+        self.df_table.to_hdf(
+            self.data_storage_path, key=self.data_storage_group_name
+        )
+
     # def generate_file_meta_df(self):
     #     self.file_meta_df = pd.Series()
     #     # self.file_meta_df["encoding"] = self.encoding
     #     # self.file_meta_df["headerRowCount"] = self.header_length
     #     # self.file_meta_df["delimiter"] = self.column_sep
     #     # self.file_meta_df["skipRows"] = 1
     #     self.file_meta_df["file_path"] = self.f_path
@@ -73,9 +84,17 @@
         pass
 
     @abstractmethod
     def parse_meta_data(self):
         pass
 
     @abstractmethod
-    def generate_data_storage(self):
+    def generate_column_df(self):
+        pass
+
+    @abstractmethod
+    def parse_table(self):
+        pass
+
+    @abstractmethod
+    def parser_data(self):
         pass
```

### Comparing `data2rdf-1.1.0/data2rdf.egg-info/PKG-INFO` & `data2rdf-2.0.0rc0/data2rdf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
 Name: data2rdf
-Version: 1.1.0
+Version: 2.0.0rc0
 Summary: A generic pipeline that can be used to map raw data to RDF.
 Home-page: https://github.com/MI-FraunhoferIWM/data2rdf
-Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy
-Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de
+Author: Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
+Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.0.0
 Requires-Dist: chowlk-unofficial-fork==0.0.2
+Requires-Dist: lru-cache<1
 Requires-Dist: openpyxl<4,>=3
 Requires-Dist: pandas<3,>=2
+Requires-Dist: pydantic<3,>=2
+Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
 Requires-Dist: python-magic==0.4.27
-Requires-Dist: rdflib==6.2.0
+Requires-Dist: rdflib<7,>=6
+Requires-Dist: requests
 Requires-Dist: tables==3.8.0
 Provides-Extra: dev
 Requires-Dist: bumpver==2021.1114; extra == "dev"
 Requires-Dist: dunamai==1.7.0; extra == "dev"
 Provides-Extra: docs
+Requires-Dist: html5lib==1.1; extra == "docs"
 Requires-Dist: ipython==8.12.3; extra == "docs"
 Requires-Dist: jinja2==3.1.3; extra == "docs"
 Requires-Dist: jupyter==1.0.0; extra == "docs"
 Requires-Dist: myst-parser==2.0.0; extra == "docs"
 Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 Requires-Dist: sphinx==6.2.1; extra == "docs"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `data2rdf-1.1.0/setup.cfg` & `data2rdf-2.0.0rc0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 [metadata]
 name = data2rdf
-version = v1.1.0
+version = v2.0.0rc0
 description = A generic pipeline that can be used to map raw data to RDF.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/data2rdf
-author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy
-author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de
+author = Paul Zierep, Yoav Nahshon, Pablo de Andres, Deepu Krishnareddy, Matthias Büschelberger
+author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de, deepu.krishnareddy@iwm.fraunhofer.de, matthias.bueschelberger@iwm.fraunhofer.de
 license = BSD-3-Clause
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 install_requires = 
 	beautifulsoup4>=4.0.0
 	chowlk-unofficial-fork==0.0.2
+	lru-cache<1
 	openpyxl>=3,<4
 	pandas>=2,<3
+	pydantic>=2,<3
+	pydantic-settings
 	python-dotenv
 	python-magic==0.4.27
-	rdflib==6.2.0
+	rdflib>=6,<7
+	requests
 	tables==3.8.0
 python_requires = >=3.8
 include_package_data = True
 
 [options.entry_points]
 console_scripts = 
 	abox_conv = data2rdf.cli.abox_conversion:terminal
 
 [options.extras_require]
 dev = 
 	bumpver==2021.1114
 	dunamai==1.7.0
 docs = 
+	html5lib==1.1
 	ipython==8.12.3
 	jinja2==3.1.3
 	jupyter==1.0.0
 	myst-parser==2.0.0
 	nbsphinx==0.9.3
 	sphinx==6.2.1
 	sphinx-autobuild==2021.3.14
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `data2rdf-1.1.0/tests/csv_pipeline_test/test_abox_pipeline.py` & `data2rdf-2.0.0rc0/tests/xls_pipeline_test/test_abox_pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import os
-import shutil
-import unittest
+# import os
+# import shutil
+# import unittest
 
-from data2rdf.cli.abox_conversion import run_abox_pipeline_for_folder
+# from data2rdf.cli.abox_conversion import run_abox_pipeline_for_folder
 
-from .test_utils import check_file_identifier_in_folder
+# from .test_utils import check_file_identifier_in_folder
 
-test_folder = os.path.dirname(os.path.abspath(__file__))
-abox_folder_path = os.path.join(test_folder, "input", "method-graph")
-output_folder = os.path.join(abox_folder_path, "tensile_test_method_v6")
+# test_folder = os.path.dirname(os.path.abspath(__file__))
+# abox_folder_path = os.path.join(test_folder, "input", "method-graph")
+# output_folder = os.path.join(abox_folder_path, "tensile_test_method_v6")
 
 
-class TestAboxPipeline(unittest.TestCase):
-    def setUp(self):
-        shutil.rmtree(output_folder, ignore_errors=True)
-        run_abox_pipeline_for_folder(abox_folder_path)
+# class TestAboxPipeline(unittest.TestCase):
+#     def setUp(self):
+#         shutil.rmtree(output_folder, ignore_errors=True)
+#         run_abox_pipeline_for_folder(abox_folder_path)
 
-    def test_file_exist(self):
-        self.assertTrue(
-            check_file_identifier_in_folder(output_folder, ".mod.ttl")
-        )
-        self.assertTrue(
-            check_file_identifier_in_folder(output_folder, ".mod.xml")
-        )
+#     def test_file_exist(self):
+#         self.assertTrue(
+#             check_file_identifier_in_folder(output_folder, ".mod.ttl")
+#         )
+#         self.assertTrue(
+#             check_file_identifier_in_folder(output_folder, ".mod.xml")
+#         )
 
 
-if __name__ == "__main__":
-    unittest.main()
+# if __name__ == "__main__":
+#     unittest.main()
```

### Comparing `data2rdf-1.1.0/tests/csv_pipeline_test/test_csv2rdf.py` & `data2rdf-2.0.0rc0/tests/csv_pipeline_test/test_csv2rdf.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 working_folder = os.path.join(test_folder, "input")
 
 output_folder = os.path.join(test_folder, "output")
 
 template = os.path.join(
     working_folder,
     "method-graph",
-    "tensile_test_method_v6",
     "tensile_test_method_v6.mod.ttl",
 )
 mapping_file = os.path.join(
     working_folder, "mapping", "tensile_test_mapping.xlsx"
 )
 raw_data = os.path.join(working_folder, "data", "DX56_D_FZ2_WR00_43.TXT")
 
@@ -29,17 +28,17 @@
 
 class TestAnnotationPipelineCSV(unittest.TestCase):
     def setUp(self):
         self.pipeline = AnnotationPipeline(
             raw_data,
             parser,
             parser_args,
-            template,
             mapping_file,
             output_folder,
+            template=template,
         )
 
         shutil.rmtree(output_folder, ignore_errors=True)
 
         self.pipeline.run_pipeline()
 
     def test_file_exist(self):
@@ -49,19 +48,14 @@
         self.assertTrue(
             check_file_identifier_in_folder(
                 self.pipeline.output, "generic.xlsx"
             )
         )
         self.assertTrue(
             check_file_identifier_in_folder(
-                self.pipeline.output, "mapping.ttl"
-            )
-        )
-        self.assertTrue(
-            check_file_identifier_in_folder(
                 self.pipeline.output, "datastorage.hdf5"
             )
         )
         self.assertTrue(
             check_file_identifier_in_folder(
                 self.pipeline.output, "metadata.ttl"
             )
```

### Comparing `data2rdf-1.1.0/tests/xls_pipeline_test/test_abox_pipeline.py` & `data2rdf-2.0.0rc0/tests/csv_pipeline_test/test_abox_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import os
-import shutil
-import unittest
+# import os
+# import shutil
+# import unittest
 
-from data2rdf.cli.abox_conversion import run_abox_pipeline_for_folder
+# from .test_utils import check_file_identifier_in_folder
 
-from .test_utils import check_file_identifier_in_folder
+# test_folder = os.path.dirname(os.path.abspath(__file__))
+# abox_folder_path = os.path.join(test_folder, "input", "method-graph")
+# output_folder = os.path.join(abox_folder_path, "tensile_test_method_v6")
 
-test_folder = os.path.dirname(os.path.abspath(__file__))
-abox_folder_path = os.path.join(test_folder, "input", "method-graph")
-output_folder = os.path.join(abox_folder_path, "tensile_test_method_v6")
 
+# class TestAboxPipeline(unittest.TestCase):
+#     def setUp(self):
+#         shutil.rmtree(output_folder, ignore_errors=True)
 
-class TestAboxPipeline(unittest.TestCase):
-    def setUp(self):
-        shutil.rmtree(output_folder, ignore_errors=True)
-        run_abox_pipeline_for_folder(abox_folder_path)
+#     def test_file_exist(self):
+#         self.assertTrue(
+#             check_file_identifier_in_folder(output_folder, ".mod.ttl")
+#         )
+#         self.assertTrue(
+#             check_file_identifier_in_folder(output_folder, ".mod.xml")
+#         )
 
-    def test_file_exist(self):
-        self.assertTrue(
-            check_file_identifier_in_folder(output_folder, ".mod.ttl")
-        )
-        self.assertTrue(
-            check_file_identifier_in_folder(output_folder, ".mod.xml")
-        )
 
-
-if __name__ == "__main__":
-    unittest.main()
+# if __name__ == "__main__":
+#     unittest.main()
```

### Comparing `data2rdf-1.1.0/tests/xls_pipeline_test/test_excel2rdf.py` & `data2rdf-2.0.0rc0/tests/xls_pipeline_test/test_excel2rdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 working_folder = os.path.join(test_folder, "input")
 
 output_folder = os.path.join(test_folder, "output")
 
 template = os.path.join(
     working_folder,
     "method-graph",
-    "tensile_test_method_v6",
     "tensile_test_method_v6.mod.ttl",
 )
 
 mapping_file = os.path.join(working_folder, "mapping", "mapping.xlsx")
 raw_data = os.path.join(working_folder, "data", "AFZ1-Fz-S1Q.xlsm")
 location_mapping = os.path.join(
     working_folder, "mapping", "location_mapping.xlsx"
@@ -42,17 +41,17 @@
 
 class TestAnnotationPipelineExcel(unittest.TestCase):
     def setUp(self):
         self.pipeline = AnnotationPipeline(
             raw_data,
             parser,
             parser_args,
-            template,
             mapping_file,
             output_folder,
+            template=template,
         )
 
         shutil.rmtree(output_folder, ignore_errors=True)
 
         self.pipeline.run_pipeline()
 
     def test_file_exist(self):
@@ -62,19 +61,14 @@
         self.assertTrue(
             check_file_identifier_in_folder(
                 self.pipeline.output, "generic.xlsx"
             )
         )
         self.assertTrue(
             check_file_identifier_in_folder(
-                self.pipeline.output, "mapping.ttl"
-            )
-        )
-        self.assertTrue(
-            check_file_identifier_in_folder(
                 self.pipeline.output, "datastorage.hdf5"
             )
         )
         self.assertTrue(
             check_file_identifier_in_folder(
                 self.pipeline.output, "metadata.ttl"
             )
```

