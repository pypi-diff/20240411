# Comparing `tmp/idc_index-0.4.2.tar.gz` & `tmp/idc_index-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Apr 10 02:39:09 2024, max compression
+gzip compressed data, last modified: Thu Apr 11 03:00:31 2024, max compression
```

## Comparing `idc_index-0.4.2.tar` & `idc_index-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      125 2024-04-10 02:39:09.000000 idc_index-0.4.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-10 02:39:09.000000 idc_index-0.4.2/.gitattributes
--rw-r--r--   0        0        0     2357 2024-04-10 02:39:09.000000 idc_index-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-10 02:39:09.000000 idc_index-0.4.2/.readthedocs.yaml
--rw-r--r--   0        0        0     2742 2024-04-10 02:39:09.000000 idc_index-0.4.2/noxfile.py
--rw-r--r--   0        0        0     2394 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      847 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1581 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      355 2024-04-10 02:39:09.000000 idc_index-0.4.2/.github/workflows/keep-alive.yaml
--rw-r--r--   0        0        0      851 2024-04-10 02:39:09.000000 idc_index-0.4.2/docs/conf.py
--rw-r--r--   0        0        0      196 2024-04-10 02:39:09.000000 idc_index-0.4.2/docs/index.md
--rw-r--r--   0        0        0      263 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/__init__.py
--rw-r--r--   0        0        0      411 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/_version.py
--rw-r--r--   0        0        0      118 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/_version.pyi
--rw-r--r--   0        0        0    25026 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/index.py
--rw-r--r--   0        0        0        0 2024-04-10 02:39:09.000000 idc_index-0.4.2/idc_index/py.typed
--rw-r--r--   0        0        0     1383 2024-04-10 02:39:09.000000 idc_index-0.4.2/queries/idc_index.sql
--rw-r--r--   0        0        0        0 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     3595 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/idcindex.py
--rw-r--r--   0        0        0      413 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/study_manifest_aws.s5cmd
--rw-r--r--   0        0        0      437 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/study_manifest_gcs.s5cmd
--rw-r--r--   0        0        0      175 2024-04-10 02:39:09.000000 idc_index-0.4.2/tests/test_package.py
--rw-r--r--   0        0        0     2265 2024-04-10 02:39:09.000000 idc_index-0.4.2/.gitignore
--rw-r--r--   0        0        0     1077 2024-04-10 02:39:09.000000 idc_index-0.4.2/LICENSE
--rw-r--r--   0        0        0     4290 2024-04-10 02:39:09.000000 idc_index-0.4.2/README.md
--rw-r--r--   0        0        0     6159 2024-04-10 02:39:09.000000 idc_index-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7592 2024-04-10 02:39:09.000000 idc_index-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-11 03:00:31.000000 idc_index-0.5.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-11 03:00:31.000000 idc_index-0.5.0/.gitattributes
+-rw-r--r--   0        0        0     2357 2024-04-11 03:00:31.000000 idc_index-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-11 03:00:31.000000 idc_index-0.5.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2742 2024-04-11 03:00:31.000000 idc_index-0.5.0/noxfile.py
+-rw-r--r--   0        0        0     2394 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      847 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1581 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      355 2024-04-11 03:00:31.000000 idc_index-0.5.0/.github/workflows/keep-alive.yaml
+-rw-r--r--   0        0        0      851 2024-04-11 03:00:31.000000 idc_index-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-04-11 03:00:31.000000 idc_index-0.5.0/docs/index.md
+-rw-r--r--   0        0        0      263 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/_version.py
+-rw-r--r--   0        0        0      118 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/_version.pyi
+-rw-r--r--   0        0        0    25127 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/index.py
+-rw-r--r--   0        0        0        0 2024-04-11 03:00:31.000000 idc_index-0.5.0/idc_index/py.typed
+-rw-r--r--   0        0        0     1383 2024-04-11 03:00:31.000000 idc_index-0.5.0/queries/idc_index.sql
+-rw-r--r--   0        0        0        0 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3779 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/idcindex.py
+-rw-r--r--   0        0        0      413 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/study_manifest_aws.s5cmd
+-rw-r--r--   0        0        0      437 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/study_manifest_gcs.s5cmd
+-rw-r--r--   0        0        0      175 2024-04-11 03:00:31.000000 idc_index-0.5.0/tests/test_package.py
+-rw-r--r--   0        0        0     2265 2024-04-11 03:00:31.000000 idc_index-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1077 2024-04-11 03:00:31.000000 idc_index-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4290 2024-04-11 03:00:31.000000 idc_index-0.5.0/README.md
+-rw-r--r--   0        0        0     6173 2024-04-11 03:00:31.000000 idc_index-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7617 2024-04-11 03:00:31.000000 idc_index-0.5.0/PKG-INFO
```

### Comparing `idc_index-0.4.2/.pre-commit-config.yaml` & `idc_index-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/noxfile.py` & `idc_index-0.5.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/.github/CONTRIBUTING.md` & `idc_index-0.5.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/.github/matchers/pylint.json` & `idc_index-0.5.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/.github/workflows/cd.yml` & `idc_index-0.5.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/.github/workflows/ci.yml` & `idc_index-0.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/docs/conf.py` & `idc_index-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/idc_index/index.py` & `idc_index-0.5.0/idc_index/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 else:
     from importlib.metadata import distribution
 
 import duckdb
 import idc_index_data
 import pandas as pd
 import psutil
+from packaging.version import Version
 
 logger = logging.getLogger(__name__)
 
 aws_endpoint_url = "https://s3.amazonaws.com"
 gcp_endpoint_url = "https://storage.googleapis.com"
 
 
@@ -86,16 +87,18 @@
 
     @staticmethod
     def _filter_by_dicom_series_uid(df_index, dicom_series_uid):
         return IDCClient._filter_dataframe_by_id(
             "SeriesInstanceUID", df_index, dicom_series_uid
         )
 
-    def get_idc_version(self):
-        return f"v{idc_index_data.__version__}"
+    @staticmethod
+    def get_idc_version():
+        idc_version = Version(idc_index_data.__version__).major
+        return f"v{idc_version}"
 
     def get_collections(self):
         unique_collections = self.index["collection_id"].unique()
         return unique_collections.tolist()
 
     def get_series_size(self, seriesInstanceUID):
         resp = self.index[["SeriesInstanceUID"] == seriesInstanceUID][
```

### Comparing `idc_index-0.4.2/queries/idc_index.sql` & `idc_index-0.5.0/queries/idc_index.sql`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/tests/idcindex.py` & `idc_index-0.5.0/tests/idcindex.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,19 @@
         logger = logging.getLogger("idc_index")
         logger.setLevel(logging.DEBUG)
 
     def test_get_collections(self):
         collections = self.client.get_collections()
         self.assertIsNotNone(collections)
 
+    def test_get_idc_version(self):
+        idc_version = self.client.get_idc_version()
+        self.assertIsNotNone(idc_version)
+        self.assertTrue(idc_version.startswith("v"))
+
     def test_get_patients(self):
         patients = self.client.get_patients(
             collection_id="tcga_gbm", outputFormat="list"
         )
 
         patients = self.client.get_patients(
             collection_id=["qin_prostate_repeatability", "phantom_fda"],
```

### Comparing `idc_index-0.4.2/.gitignore` & `idc_index-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/LICENSE` & `idc_index-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/README.md` & `idc_index-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `idc_index-0.4.2/pyproject.toml` & `idc_index-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [build-system]
-requires = ["hatchling", "hatch-vcs"]
-build-backend = "hatchling.build"
+requires = ["hatchling","hatch-vcs"]
 
+build-backend = "hatchling.build"
 
 [project]
 name = "idc-index"
 authors = [
   { name = "Andrey Fedorov", email = "andrey.fedorov@gmail.com" },
   { name = "Vamsi Thiriveedhi", email = "vthiriveedhi@mgh.harvard.edu" },
 ]
@@ -29,15 +29,16 @@
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dynamic = ["version"]
 dependencies = [
   'duckdb>=0.10.0',
-  "idc-index-data==17.0.2",
+  "idc-index-data==18.0.0",
+  "packaging",
   "pandas<2.2",
   "psutil",
   "pyarrow",
   "s5cmd",
 ]
 
 [project.optional-dependencies]
```

### Comparing `idc_index-0.4.2/PKG-INFO` & `idc_index-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: idc-index
-Version: 0.4.2
+Version: 0.5.0
 Summary: Package to query and download data from an index of ImagingDataCommons
 Project-URL: Homepage, https://github.com/ImagingDataCommons/idc-index
 Project-URL: Bug Tracker, https://github.com/ImagingDataCommons/idc-index/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index/releases
 Author-email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>
 License: MIT License
@@ -42,15 +42,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: duckdb>=0.10.0
-Requires-Dist: idc-index-data==17.0.2
+Requires-Dist: idc-index-data==18.0.0
+Requires-Dist: packaging
 Requires-Dist: pandas<2.2
 Requires-Dist: psutil
 Requires-Dist: pyarrow
 Requires-Dist: s5cmd
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
```

