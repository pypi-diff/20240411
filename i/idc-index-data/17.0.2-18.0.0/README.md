# Comparing `tmp/idc_index_data-17.0.2.tar.gz` & `tmp/idc_index_data-18.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idc_index_data-17.0.2.tar", last modified: Tue Apr  9 19:24:52 2024, max compression
+gzip compressed data, was "idc_index_data-18.0.0.tar", last modified: Thu Apr 11 02:25:44 2024, max compression
```

## Comparing `idc_index_data-17.0.2.tar` & `idc_index_data-18.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      125 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.gitattributes
--rw-r--r--   0        0        0     2858 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1089 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2217 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      313 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/workflows/keep-alive.yml
--rw-r--r--   0        0        0     2264 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.gitignore
--rw-r--r--   0        0        0     2338 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1352 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/CMakeLists.txt
--rw-r--r--   0        0        0     1054 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/LICENSE
--rw-r--r--   0        0        0     2293 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/README.md
--rw-r--r--   0        0        0      849 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/docs/conf.py
--rw-r--r--   0        0        0      201 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/docs/index.md
--rw-r--r--   0        0        0     5359 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/noxfile.py
--rw-r--r--   0        0        0     4198 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/pyproject.toml
--rw-r--r--   0        0        0     5034 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/scripts/python/idc_index_data_manager.py
--rwxr-xr-x   0        0        0     2653 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/scripts/python/update_idc_index_version.py
--rw-r--r--   0        0        0     1349 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/scripts/sql/idc_index.sql
--rw-r--r--   0        0        0     1058 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/src/idc_index_data/__init__.py
--rw-r--r--   0        0        0       49 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/src/idc_index_data/_version.pyi
--rw-r--r--   0        0        0        0 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/src/idc_index_data/py.typed
--rw-r--r--   0        0        0     1206 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/tests/test_package.py
--rw-r--r--   0        0        0     5431 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.gitattributes
+-rw-r--r--   0        0        0     2858 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1089 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2217 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      313 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.github/workflows/keep-alive.yml
+-rw-r--r--   0        0        0     2264 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.gitignore
+-rw-r--r--   0        0        0     2338 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1352 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/CMakeLists.txt
+-rw-r--r--   0        0        0     1054 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/LICENSE
+-rw-r--r--   0        0        0     2293 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/README.md
+-rw-r--r--   0        0        0      849 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/docs/conf.py
+-rw-r--r--   0        0        0      201 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/docs/index.md
+-rw-r--r--   0        0        0     5359 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/noxfile.py
+-rw-r--r--   0        0        0     4198 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5034 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/scripts/python/idc_index_data_manager.py
+-rwxr-xr-x   0        0        0     2653 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/scripts/python/update_idc_index_version.py
+-rw-r--r--   0        0        0     1349 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/scripts/sql/idc_index.sql
+-rw-r--r--   0        0        0     1058 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/src/idc_index_data/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/src/idc_index_data/_version.pyi
+-rw-r--r--   0        0        0        0 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/src/idc_index_data/py.typed
+-rw-r--r--   0        0        0     1206 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/tests/test_package.py
+-rw-r--r--   0        0        0     5431 2024-04-11 02:25:44.000000 idc_index_data-18.0.0/PKG-INFO
```

### Comparing `idc_index_data-17.0.2/.github/CONTRIBUTING.md` & `idc_index_data-18.0.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/.github/matchers/pylint.json` & `idc_index_data-18.0.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/.github/workflows/cd.yml` & `idc_index_data-18.0.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/.github/workflows/ci.yml` & `idc_index_data-18.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/.gitignore` & `idc_index_data-18.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/.pre-commit-config.yaml` & `idc_index_data-18.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/CMakeLists.txt` & `idc_index_data-18.0.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/LICENSE` & `idc_index_data-18.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/README.md` & `idc_index_data-18.0.0/README.md`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/docs/conf.py` & `idc_index_data-18.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/noxfile.py` & `idc_index_data-18.0.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/pyproject.toml` & `idc_index_data-18.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "requests"
 ]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "idc-index-data"
-version = "17.0.2"
+version = "18.0.0"
 authors = [
   { name = "Andrey Fedorov", email = "andrey.fedorov@gmail.com" },
   { name = "Vamsi Thiriveedhi", email = "vthiriveedhi@mgh.harvard.edu" },
   { name = "Jean-Christophe Fillion-Robin", email = "jchris.fillionr@kitware.com" },
 ]
 description = "ImagingDataCommons index to query and download data."
 readme = "README.md"
```

### Comparing `idc_index_data-17.0.2/scripts/python/idc_index_data_manager.py` & `idc_index_data-18.0.0/scripts/python/idc_index_data_manager.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/scripts/python/update_idc_index_version.py` & `idc_index_data-18.0.0/scripts/python/update_idc_index_version.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/scripts/sql/idc_index.sql` & `idc_index_data-18.0.0/scripts/sql/idc_index.sql`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
   ANY_VALUE(SeriesNumber) AS SeriesNumber,
   COUNT(dicom_all.SOPInstanceUID) AS instanceCount,
   ANY_VALUE(license_short_name) as license_short_name,
   # download related attributes
   ANY_VALUE(CONCAT(series_aws_url,"*")) AS series_aws_url,
   ROUND(SUM(SAFE_CAST(instance_size AS float64))/1000000, 2) AS series_size_MB,
 FROM
-  `bigquery-public-data.idc_v17.dicom_all` AS dicom_all
+  `bigquery-public-data.idc_v18.dicom_all` AS dicom_all
 JOIN
-  `bigquery-public-data.idc_v17.dicom_metadata_curated` AS dicom_curated
+  `bigquery-public-data.idc_v18.dicom_metadata_curated` AS dicom_curated
 ON
   dicom_all.SOPInstanceUID = dicom_curated.SOPInstanceUID
 GROUP BY
   SeriesInstanceUID
```

### Comparing `idc_index_data-17.0.2/src/idc_index_data/__init__.py` & `idc_index_data-18.0.0/src/idc_index_data/__init__.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.2/tests/test_package.py` & `idc_index_data-18.0.0/tests/test_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import importlib.metadata
 
 import pandas as pd
 from packaging.version import Version
 
 import idc_index_data as m
 
-EXPECTED_IDC_INDEX_VERSION = 17
+EXPECTED_IDC_INDEX_VERSION = 18
 
 
 def test_version():
     assert importlib.metadata.version("idc_index_data") == m.__version__
 
 
 def test_idc_index_version():
```

### Comparing `idc_index_data-17.0.2/PKG-INFO` & `idc_index_data-18.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idc-index-data
-Version: 17.0.2
+Version: 18.0.0
 Summary: ImagingDataCommons index to query and download data.
 Author-Email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>, Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 License: Copyright 2024 Andrey Fedorov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

