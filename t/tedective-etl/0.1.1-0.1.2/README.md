# Comparing `tmp/tedective_etl-0.1.1.tar.gz` & `tmp/tedective_etl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedective_etl-0.1.1.tar", max compression
+gzip compressed data, was "tedective_etl-0.1.2.tar", max compression
```

## Comparing `tedective_etl-0.1.1.tar` & `tedective_etl-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3779 2024-04-11 13:07:15.255428 tedective_etl-0.1.1/README.md
--rw-r--r--   0        0        0     1180 2024-04-11 13:08:11.942997 tedective_etl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:40:09.538488 tedective_etl-0.1.1/tedective_etl/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 10:14:51.437671 tedective_etl-0.1.1/tedective_etl/currency/__init__.py
--rw-r--r--   0        0        0        1 2024-04-10 13:45:35.427005 tedective_etl-0.1.1/tedective_etl/currency/rates.json
--rw-r--r--   0        0        0     1096 2024-04-11 10:14:58.034299 tedective_etl-0.1.1/tedective_etl/currency/update.py
--rw-r--r--   0        0        0     5632 2024-04-10 13:49:59.842809 tedective_etl-0.1.1/tedective_etl/dedupe.py
--rw-r--r--   0        0        0    14149 2024-04-09 20:35:56.560161 tedective_etl-0.1.1/tedective_etl/graph.py
--rw-r--r--   0        0        0    18394 2024-04-11 10:14:58.034299 tedective_etl-0.1.1/tedective_etl/main.py
--rw-r--r--   0        0        0    52887 2024-04-11 10:14:58.034299 tedective_etl-0.1.1/tedective_etl/schema/ocds.py
--rw-r--r--   0        0        0     4469 2024-04-05 14:40:09.542488 tedective_etl-0.1.1/tedective_etl/search.py
--rw-r--r--   0        0        0       62 2024-04-05 14:40:09.542488 tedective_etl-0.1.1/tedective_etl/server.py
--rw-r--r--   0        0        0        0 2024-04-05 14:40:09.542488 tedective_etl-0.1.1/tedective_etl/ted_to_ocds/__init__.py
--rw-r--r--   0        0        0     7781 2024-04-11 10:14:58.034299 tedective_etl-0.1.1/tedective_etl/ted_to_ocds/extractors.py
--rw-r--r--   0        0        0     6292 2024-04-05 14:40:09.542488 tedective_etl-0.1.1/tedective_etl/ted_to_ocds/process.py
--rw-r--r--   0        0        0      178 2024-04-05 14:40:09.542488 tedective_etl-0.1.1/tedective_etl/ted_to_ocds/trackers.py
--rw-r--r--   0        0        0    15886 2024-04-11 10:14:58.038299 tedective_etl-0.1.1/tedective_etl/ted_to_ocds/transform.py
--rw-r--r--   0        0        0     3518 2024-04-11 10:14:58.038299 tedective_etl-0.1.1/tedective_etl/utils.py
--rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 tedective_etl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3779 2024-04-11 14:10:08.207308 tedective_etl-0.1.2/README.md
+-rw-r--r--   0        0        0     1175 2024-04-11 21:51:51.847643 tedective_etl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 14:40:09.538488 tedective_etl-0.1.2/tedective_etl/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:14:51.437671 tedective_etl-0.1.2/tedective_etl/currency/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 13:17:38.965153 tedective_etl-0.1.2/tedective_etl/currency/rates.json
+-rw-r--r--   0        0        0     1096 2024-04-11 13:15:59.170324 tedective_etl-0.1.2/tedective_etl/currency/update.py
+-rw-r--r--   0        0        0     5632 2024-04-11 13:17:43.785095 tedective_etl-0.1.2/tedective_etl/dedupe.py
+-rw-r--r--   0        0        0    14149 2024-04-11 13:17:47.029057 tedective_etl-0.1.2/tedective_etl/graph.py
+-rw-r--r--   0        0        0    18394 2024-04-11 13:17:50.581014 tedective_etl-0.1.2/tedective_etl/main.py
+-rw-r--r--   0        0        0    52887 2024-04-11 13:17:55.408956 tedective_etl-0.1.2/tedective_etl/schema/ocds.py
+-rw-r--r--   0        0        0     4469 2024-04-11 13:18:33.060502 tedective_etl-0.1.2/tedective_etl/search.py
+-rw-r--r--   0        0        0       62 2024-04-11 13:18:01.080888 tedective_etl-0.1.2/tedective_etl/server.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:40:09.542488 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/__init__.py
+-rw-r--r--   0        0        0     7781 2024-04-11 13:18:10.044780 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/extractors.py
+-rw-r--r--   0        0        0     6292 2024-04-11 13:18:12.740748 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/process.py
+-rw-r--r--   0        0        0      178 2024-04-11 13:18:17.776687 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/trackers.py
+-rw-r--r--   0        0        0    15886 2024-04-11 13:18:20.804650 tedective_etl-0.1.2/tedective_etl/ted_to_ocds/transform.py
+-rw-r--r--   0        0        0     3518 2024-04-11 13:18:24.264608 tedective_etl-0.1.2/tedective_etl/utils.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 tedective_etl-0.1.2/PKG-INFO
```

### Comparing `tedective_etl-0.1.1/README.md` & `tedective_etl-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/pyproject.toml` & `tedective_etl-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tedective-etl"
-version = "0.1.1"
+version = "0.1.2"
 description = "The XML-to-OCDS parser for the TEDective project based on lxml"
 authors = ["Free Software Foundation Europe e.V. <tedective@fsfe.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "tedective_etl"}]
 
 [tool.poetry.urls]
@@ -13,35 +13,35 @@
 "Documentation" = "https://docs.tedective.org"
 
 [tool.poetry.scripts]
 run-server = "tedective_etl.server:run_luigid"
 run-pipeline = "tedective_etl.main:run_pipeline"
 
 [tool.poetry.dependencies]
-python = "^3.11"
-fingerprints = "^1.1.1"
+python = "^3.10"
+fingerprints = "1.1.1"
 ftfy = "6.1.1"
 lxml = "4.9.3"
 orjson = "3.8.9"
 phonenumbers = "8.13.18"
 rich = "13.5.2"
 python-dateutil = "2.8.2"
-datamodel-code-generator = {extras = ["http"], version = "^0.22.1"}
+datamodel-code-generator = {extras = ["http"], version = "0.22.1"}
 orjsonl = "0.3.1"
 kuzu = "0.3.2"
 pandas = "2.1.4"
 pyarrow = "14.0.2"
 jupyter = "1.0.0"
 phonetics = "1.0.5"
 splink = "3.9.11"
 meilisearch = "0.30.0"
 luigi = "3.5.0"
 pyicu = "2.12"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
-black = "^23.7.0"
-isort = "^5.12.0"
+pytest = "7.4.0"
+black = "23.7.0"
+isort = "5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tedective_etl-0.1.1/tedective_etl/currency/update.py` & `tedective_etl-0.1.2/tedective_etl/currency/update.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/dedupe.py` & `tedective_etl-0.1.2/tedective_etl/dedupe.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/graph.py` & `tedective_etl-0.1.2/tedective_etl/graph.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/main.py` & `tedective_etl-0.1.2/tedective_etl/main.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/schema/ocds.py` & `tedective_etl-0.1.2/tedective_etl/schema/ocds.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/search.py` & `tedective_etl-0.1.2/tedective_etl/search.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/ted_to_ocds/extractors.py` & `tedective_etl-0.1.2/tedective_etl/ted_to_ocds/extractors.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/ted_to_ocds/process.py` & `tedective_etl-0.1.2/tedective_etl/ted_to_ocds/process.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/ted_to_ocds/transform.py` & `tedective_etl-0.1.2/tedective_etl/ted_to_ocds/transform.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/tedective_etl/utils.py` & `tedective_etl-0.1.2/tedective_etl/utils.py`

 * *Files identical despite different names*

### Comparing `tedective_etl-0.1.1/PKG-INFO` & `tedective_etl-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: tedective-etl
-Version: 0.1.1
+Version: 0.1.2
 Summary: The XML-to-OCDS parser for the TEDective project based on lxml
 License: AGPL-3.0-or-later
 Author: Free Software Foundation Europe e.V.
 Author-email: tedective@fsfe.org
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: datamodel-code-generator[http] (>=0.22.1,<0.23.0)
-Requires-Dist: fingerprints (>=1.1.1,<2.0.0)
+Requires-Dist: datamodel-code-generator[http] (==0.22.1)
+Requires-Dist: fingerprints (==1.1.1)
 Requires-Dist: ftfy (==6.1.1)
 Requires-Dist: jupyter (==1.0.0)
 Requires-Dist: kuzu (==0.3.2)
 Requires-Dist: luigi (==3.5.0)
 Requires-Dist: lxml (==4.9.3)
 Requires-Dist: meilisearch (==0.30.0)
 Requires-Dist: orjson (==3.8.9)
```

