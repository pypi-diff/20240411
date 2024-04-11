# Comparing `tmp/fiboa-cli-0.3.0.tar.gz` & `tmp/fiboa-cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa-cli-0.3.0.tar", last modified: Wed Apr 10 13:24:57 2024, max compression
+gzip compressed data, was "fiboa-cli-0.3.1.tar", last modified: Thu Apr 11 15:17:38 2024, max compression
```

## Comparing `fiboa-cli-0.3.0.tar` & `fiboa-cli-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/create_geoparquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/validate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 13:24:57.000000 fiboa-cli-0.3.0/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:24:57.923783 fiboa-cli-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 13:24:52.000000 fiboa-cli-0.3.0/tests/test_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/create_geoparquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/tests/test_jsonschema.py
```

### Comparing `fiboa-cli-0.3.0/LICENSE` & `fiboa-cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.0/PKG-INFO` & `fiboa-cli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -67,15 +67,15 @@
 
 To create one or multiple fiboa-compliant GeoJSON file(s) for a fiboa-compliant GeoParquet file,
 you can for example run:
 
 - GeoJSON FeatureCollection:
   `fiboa create-geojson example.parquet -o dest-folder`
 - GeoJSON Features (with indentation and max. 100 features):
-  `fiboa create-geojson example.parquet -o dest-folder -n 100 -i 2 -f TRUE`
+  `fiboa create-geojson example.parquet -o dest-folder -n 100 -i 2 -f`
 
 Check `fiboa create-geoparquet --help` for more details.
 
 ## Inspect fiboa GeoParquet file
 
 To look into a fiboa GeoParquet file to get a rough understanding of the content, the following can be executed:
```

### Comparing `fiboa-cli-0.3.0/README.md` & `fiboa-cli-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 To create one or multiple fiboa-compliant GeoJSON file(s) for a fiboa-compliant GeoParquet file,
 you can for example run:
 
 - GeoJSON FeatureCollection:
   `fiboa create-geojson example.parquet -o dest-folder`
 - GeoJSON Features (with indentation and max. 100 features):
-  `fiboa create-geojson example.parquet -o dest-folder -n 100 -i 2 -f TRUE`
+  `fiboa create-geojson example.parquet -o dest-folder -n 100 -i 2 -f`
 
 Check `fiboa create-geoparquet --help` for more details.
 
 ## Inspect fiboa GeoParquet file
 
 To look into a fiboa GeoParquet file to get a rough understanding of the content, the following can be executed:
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli/__init__.py` & `fiboa-cli-0.3.1/fiboa_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,15 @@
     '--out', '-o',
     type=click.Path(exists=False),
     help='Folder to write the files to.',
     required=True
 )
 @click.option(
     '--features', '-f',
+    is_flag=True,
     type=click.BOOL,
     help='Create seperate GeoJSON Feature files.',
     default=False
 )
 @click.option(
     '--num', '-n',
     type=click.IntRange(min=1),
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli/convert.py` & `fiboa-cli-0.3.1/fiboa_cli/convert.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.0/fiboa_cli/convert_utils.py` & `fiboa-cli-0.3.1/fiboa_cli/convert_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from .const import STAC_TABLE_EXTENSION
 from .version import fiboa_version
 from .util import log, download_file, get_fs, to_iso8601
-from .create_geoparquet import create_geoparquet
+from .parquet import create_parquet
 
 from fsspec.implementations.local import LocalFileSystem
 
 import os
 import json
 import geopandas as gpd
 import pandas as pd
 
-STAC_TABLE_EXTENSION = "https://stac-extensions.github.io/table/v1.2.0/schema.json"
-
 def convert(
         output_file, cache_file,
         url, columns,
         id, title, description, bbox,
         provider_name = None,
         provider_url = None,
         source_coop_url = None,
         extensions = [],
         missing_schemas = {},
+        column_migrations = {},
+        migration = None,
         attribution = None,
         store_collection = False,
         license = "dl-de/by-2-0",
         compression = "brotli",
         **kwargs):
     """
     Converts a German field boundary datasets to fiboa.
@@ -34,31 +35,53 @@
 
     log("Local file is at: " + path)
     gdf = gpd.read_file(path, **kwargs)
 
     log("Loaded into GeoDataFrame:")
     print(gdf.head())
 
+    # 1. Run global migration
+    has_migration = callable(migration)
+    if has_migration:
+        log("Applying global migrations")
+        gdf = migration(gdf)
+
+    # 2. Run column migrations
+    has_col_migrations = len(column_migrations) > 0
+    if has_col_migrations:
+        log("Applying column migrations")
+        for key, fn in column_migrations.items():
+            if key in gdf.columns:
+                gdf[key] = fn(gdf[key])
+            else:
+                log(f"Column '{key}' not found in dataset, skipping migration", "warning")
+
+    if has_migration or has_col_migrations:
+        log("GeoDataFrame after migrations:")
+        print(gdf.head())
+
+    # 3. Duplicate columns if needed
     actual_columns = {}
     for old_key, new_key in columns.items():
         # If new keys are a list, duplicate the column
         if isinstance(new_key, list):
             for key in new_key:
                 gdf[key] = gdf.loc[:, old_key]
                 actual_columns[key] = key
-        # If new key is a string, rename the column
+        # If new key is a string, plan to rename the column
         elif old_key in gdf.columns:
             actual_columns[old_key] = new_key
         # If old key is not found, remove from the schema and warn
         else:
             log(f"Column '{old_key}' not found in dataset, removing from schema", "warning")
 
-    # Rename columns
+    # 4. Rename columns
     gdf.rename(columns = actual_columns, inplace = True)
-    # Remove all columns that are not listed
+
+    # 5. Remove all columns that are not listed
     drop_columns = list(set(gdf.columns) - set(actual_columns.values()))
     gdf.drop(columns = drop_columns, inplace = True)
 
     log("Changed GeoDataFrame to:")
     print(gdf.head())
 
     collection = create_collection(
@@ -73,15 +96,15 @@
     )
 
     log("Creating GeoParquet file: " + output_file)
     config = {
         "fiboa_version": fiboa_version,
     }
     columns = list(actual_columns.values())
-    pq_fields = create_geoparquet(gdf, columns, collection, output_file, config, missing_schemas, compression)
+    pq_fields = create_parquet(gdf, columns, collection, output_file, config, missing_schemas, compression)
 
     if store_collection:
         external_collection = add_asset_to_collection(collection, output_file, rows = len(gdf), columns = pq_fields)
         collection_file = os.path.join(os.path.dirname(output_file), "collection.json")
         log("Creating Collection file: " + collection_file)
         with open(collection_file, "w") as f:
             json.dump(external_collection, f, indent=2)
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli/create_geojson.py` & `fiboa-cli-0.3.1/fiboa_cli/create_geojson.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import json
 import os
 import pandas as pd
 
-from geopandas import GeoDataFrame
-
 from .util import load_parquet_data, load_parquet_schema, parse_metadata, to_iso8601
 
 
 def create_geojson(file, out, split = False, num = None, indent = None):
     if not os.path.exists(out):
         os.makedirs(out)
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli/create_geoparquet.py` & `fiboa-cli-0.3.1/fiboa_cli/create_geoparquet.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.0/fiboa_cli/describe.py` & `fiboa-cli-0.3.1/fiboa_cli/describe.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.0/fiboa_cli/geopandas.py` & `fiboa-cli-0.3.1/fiboa_cli/geopandas.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.0/fiboa_cli/jsonschema.py` & `fiboa-cli-0.3.1/fiboa_cli/jsonschema.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.0/fiboa_cli/jsonschema_template.py` & `fiboa-cli-0.3.1/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.0/fiboa_cli/parquet.py` & `fiboa-cli-0.3.1/fiboa_cli/parquet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import pyarrow as pa
 
 from geopandas import GeoDataFrame
 from shapely.geometry import shape
 
-from .const import PA_TYPE_MAP, GP_TYPE_MAP, GP_TO_PA_TYPE_MAP
+from .types import get_geopandas_dtype, get_pyarrow_type_for_geopandas, get_pyarrow_field
 from .util import log, load_fiboa_schema, load_file, merge_schemas
 from .geopandas import to_parquet
 
 def create_parquet(data, columns, collection, output_file, config, missing_schemas = {}, compression = "brotli"):
     # Load the data schema
     fiboa_schema = load_fiboa_schema(config)
     schemas = merge_schemas(missing_schemas, fiboa_schema)
@@ -35,31 +35,39 @@
 
     # Update the GeoDataFrame with the correct types etc.
     data = update_dataframe(data, columns, schemas)
 
     # Define the fields for the schema
     pq_fields = []
     for name in columns:
+        required_props = schemas.get("required", [])
         properties = schemas.get("properties", {})
+        required = name in required_props
         if name in properties:
             prop_schema = properties[name]
-            pa_type = create_type(prop_schema)
-            nullable = name not in schemas.get("required", [])
-            field = pa.field(name, pa_type, nullable = nullable)
+            try:
+                field = get_pyarrow_field(name, schema = prop_schema, required = required)
+            except Exception as e:
+                log(f"{name}: Skipped - {e}", "warning")
         else:
             pd_type = str(data[name].dtype) # pandas data type
-            pa_type = GP_TO_PA_TYPE_MAP.get(pd_type) # pyarrow data type
-            if pa_type is not None:
-                log(f"{name}: No schema defined, converting {pd_type} to nullable {pa_type}", "warning")
-                field = pa.field(name, pa_type, nullable = True)
-            else:
-                log(f"{name}: No schema defined and converter doesn't support {pd_type}, skipping field", "warning")
+            try:
+                pa_type = get_pyarrow_type_for_geopandas(pd_type, required) # pyarrow data type
+                if pa_type is not None:
+                    log(f"{name}: No schema defined, converting {pd_type} to nullable {pa_type}", "warning")
+                    field = get_pyarrow_field(name, pa_type = pa_type)
+            except Exception as e:
+                log(f"{name}: Skipped - {e}", "warning")
                 continue
 
-        pq_fields.append(field)
+        if field is None:
+            log(f"{name}: Skipped - invalid data type", "warning")
+            continue
+        else:
+            pq_fields.append(field)
 
     # Define the schema for the Parquet file
     pq_schema = pa.schema(pq_fields)
     pq_schema = pq_schema.with_metadata({"fiboa": json.dumps(collection).encode("utf-8")})
 
     # Write the data to the Parquet file
     # Proprietary function exported from geopandas to solve
@@ -92,41 +100,30 @@
 
     # Create the GeoDataFrame
     return GeoDataFrame(rows, columns=columns, geometry="geometry", crs="EPSG:4326")
 
 
 def update_dataframe(data, columns, schema):
     # Convert the data to the correct types
+    properties = schema.get("properties", {})
+    required_props = schema.get("required", [])
     for column in columns:
-        if column not in schema["properties"]:
+        if column not in properties:
             continue
-        dtype = schema["properties"][column].get("type")
+        schema = properties[column]
+        dtype = schema.get("type")
         if dtype == "geometry":
             continue
 
-        gp_type = GP_TYPE_MAP.get(dtype)
-        if gp_type is None:
-            log(f"{column}: No type conversion available for {dtype}")
-        elif callable(gp_type):
-            data[column] = gp_type(data[column])
-        else:
-            data[column] = data[column].astype(gp_type)
+        required = column in required_props
+        gp_type = get_geopandas_dtype(dtype, required, schema)
+        try:
+            if gp_type is None:
+                log(f"{column}: No type conversion available for {dtype}")
+            elif callable(gp_type):
+                data[column] = gp_type(data[column])
+            else:
+                data[column] = data[column].astype(gp_type, copy = False)
+        except Exception as e:
+            log(f"{column}: Can't convert to {dtype}: {e}", "warning")
 
     return data
-
-def create_type(schema):
-    dtype = schema.get("type")
-    if dtype is None:
-        raise Exception("No type specified")
-
-    pa_type = PA_TYPE_MAP.get(dtype)
-    if pa_type is None:
-        raise Exception(f"{dtype} is not supported yet")
-    elif callable(pa_type):
-        if dtype == "array":
-            pa_subtype = create_type(schema["items"])
-            pa_type = pa_type(pa_subtype)
-        elif dtype == "object":
-            log(f"Creation of object-typed properties not supported yet", "warning")
-            pass # todo
-
-    return pa_type
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli/util.py` & `fiboa-cli-0.3.1/fiboa_cli/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import json
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pandas as pd
 import re
 
 from urllib.parse import urlparse
-from geopandas import GeoDataFrame
 from fsspec import AbstractFileSystem
 from fsspec.implementations.http import HTTPFileSystem
 from fsspec.implementations.local import LocalFileSystem
 from pyarrow import NativeFile
 from pyarrow.fs import FSSpecHandler, PyFileSystem
 from tempfile import NamedTemporaryFile
 from typing import Union
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli/validate.py` & `fiboa-cli-0.3.1/fiboa_cli/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import pyarrow.types as pat
 
 from jsonschema.validators import Draft7Validator
-from .const import PA_TYPE_CHECK, STAC_COLLECTION_SCHEMA
+from .const import STAC_COLLECTION_SCHEMA
+from .types import PA_TYPE_CHECK
 from .jsonschema import create_jsonschema
 from .util import get_collection, log as log_, load_datatypes, load_file, load_fiboa_schema, load_parquet_data, load_parquet_schema, merge_schemas
 from .validate_data import validate_column
 
 def log(text: str, status="info"):
     # Indent logs
     log_("  - " + str(text), status)
@@ -260,17 +261,16 @@
         try:
             schema = load_file(STAC_COLLECTION_SCHEMA)
             errors = validate_json_schema(obj, schema)
             for error in errors:
                 log(f"Collection: {error.path}: {error.message}", "error")
 
             return len(errors) == 0
-        except:
-            log("Failed to validate STAC Collection", "warning")
-            return False
+        except Exception as e:
+            log(f"Failed to validate STAC Collection due to an internal error: {e}", "warning")
 
     return True
 
 
 def validate_json_schema(obj, schema):
     if isinstance(obj, (bytearray, bytes, str)):
         obj = json.loads(obj)
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli/validate_data.py` & `fiboa-cli-0.3.1/fiboa_cli/validate_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import pandas as pd
 from urllib.parse import urlparse
 
 def validate_column(data, rules):
-    for index, value in data.items():
+    for _, value in data.items():
         if pd.isna(value):
             # Skip validation for NaN values or implement special handling if required
             continue
 
         if isinstance(value, str):
             issues = validate_string(value, rules)
         elif isinstance(value, (int, float)):
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli/validate_schema.py` & `fiboa-cli-0.3.1/fiboa_cli/validate_schema.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.0/fiboa_cli.egg-info/PKG-INFO` & `fiboa-cli-0.3.1/fiboa_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -67,15 +67,15 @@
 
 To create one or multiple fiboa-compliant GeoJSON file(s) for a fiboa-compliant GeoParquet file,
 you can for example run:
 
 - GeoJSON FeatureCollection:
   `fiboa create-geojson example.parquet -o dest-folder`
 - GeoJSON Features (with indentation and max. 100 features):
-  `fiboa create-geojson example.parquet -o dest-folder -n 100 -i 2 -f TRUE`
+  `fiboa create-geojson example.parquet -o dest-folder -n 100 -i 2 -f`
 
 Check `fiboa create-geoparquet --help` for more details.
 
 ## Inspect fiboa GeoParquet file
 
 To look into a fiboa GeoParquet file to get a rough understanding of the content, the following can be executed:
```

### Comparing `fiboa-cli-0.3.0/fiboa_cli.egg-info/SOURCES.txt` & `fiboa-cli-0.3.1/fiboa_cli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 fiboa_cli/create_geojson.py
 fiboa_cli/create_geoparquet.py
 fiboa_cli/describe.py
 fiboa_cli/geopandas.py
 fiboa_cli/jsonschema.py
 fiboa_cli/jsonschema_template.py
 fiboa_cli/parquet.py
+fiboa_cli/types.py
 fiboa_cli/util.py
 fiboa_cli/validate.py
 fiboa_cli/validate_data.py
 fiboa_cli/validate_schema.py
 fiboa_cli/version.py
 fiboa_cli.egg-info/PKG-INFO
 fiboa_cli.egg-info/SOURCES.txt
```

### Comparing `fiboa-cli-0.3.0/setup.py` & `fiboa-cli-0.3.1/setup.py`

 * *Files identical despite different names*

