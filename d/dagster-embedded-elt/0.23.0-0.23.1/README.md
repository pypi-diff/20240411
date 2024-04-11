# Comparing `tmp/dagster-embedded-elt-0.23.0.tar.gz` & `tmp/dagster-embedded-elt-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.0.tar", last modified: Thu Apr  4 19:54:26 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.1.tar", last modified: Thu Apr 11 18:15:27 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.0.tar` & `dagster-embedded-elt-0.23.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.295620 dagster-embedded-elt-0.23.0/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-04 19:54:26.295620 dagster-embedded-elt-0.23.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.283619 dagster-embedded-elt-0.23.0/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.287619 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3768 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     5629 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.291620 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4931 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    17477 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:26.283619 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-04 19:54:26.000000 dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-04-04 19:54:26.295620 dagster-embedded-elt-0.23.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2024-04-04 19:44:08.000000 dagster-embedded-elt-0.23.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.058513 dagster-embedded-elt-0.23.1/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-11 18:15:27.058513 dagster-embedded-elt-0.23.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.034513 dagster-embedded-elt-0.23.1/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.038513 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.054513 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4931 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    17477 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.034513 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-04-11 18:15:27.062513 dagster-embedded-elt-0.23.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/setup.py
```

### Comparing `dagster-embedded-elt-0.23.0/LICENSE` & `dagster-embedded-elt-0.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/PKG-INFO` & `dagster-embedded-elt-0.23.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/translator.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 @dataclass
 class DagsterDltTranslator:
     @public
     def get_asset_key(self, resource: DltResource) -> AssetKey:
         """Defines asset key for a given dlt resource key and dataset name.
 
         Args:
-            resource_key (str): key of dlt resource
-            dataset_name (str): name of dlt dataset
+            resource (DltResource): dlt resource / transformer
 
         Returns:
             AssetKey of Dagster asset derived from dlt resource
 
         """
         return AssetKey(f"dlt_{resource.source_name}_{resource.name}")
```

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/PKG-INFO` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.0/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.0/setup.py` & `dagster-embedded-elt-0.23.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.0", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.1", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```

