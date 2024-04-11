# Comparing `tmp/bodo_platform_utils-0.1.1.tar.gz` & `tmp/bodo_platform_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodo_platform_utils-0.1.1.tar", last modified: Fri Mar  8 01:34:57 2024, max compression
+gzip compressed data, was "bodo_platform_utils-0.1.2.tar", last modified: Thu Apr 11 15:18:30 2024, max compression
```

## Comparing `bodo_platform_utils-0.1.1.tar` & `bodo_platform_utils-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:34:57.082964 bodo_platform_utils-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-08 01:34:57.082964 bodo_platform_utils-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:34:57.082964 bodo_platform_utils-0.1.1/bodo_platform_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/bodo_platform_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-08 01:34:57.082964 bodo_platform_utils-0.1.1/bodo_platform_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/bodo_platform_utils/bodosqlwrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/bodo_platform_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/bodo_platform_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/bodo_platform_utils/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/bodo_platform_utils/utils_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 01:34:57.082964 bodo_platform_utils-0.1.1/bodo_platform_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-08 01:34:57.000000 bodo_platform_utils-0.1.1/bodo_platform_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-08 01:34:57.000000 bodo_platform_utils-0.1.1/bodo_platform_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 01:34:57.000000 bodo_platform_utils-0.1.1/bodo_platform_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-08 01:34:57.000000 bodo_platform_utils-0.1.1/bodo_platform_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-08 01:34:57.000000 bodo_platform_utils-0.1.1/bodo_platform_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-08 01:34:57.082964 bodo_platform_utils-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    82560 2024-03-08 01:33:53.000000 bodo_platform_utils-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:18:30.147946 bodo_platform_utils-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 15:18:30.147946 bodo_platform_utils-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:18:30.151946 bodo_platform_utils-0.1.2/bodo_platform_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/bodo_platform_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 15:18:30.151946 bodo_platform_utils-0.1.2/bodo_platform_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/bodo_platform_utils/bodosqlwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/bodo_platform_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/bodo_platform_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/bodo_platform_utils/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/bodo_platform_utils/utils_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:18:30.147946 bodo_platform_utils-0.1.2/bodo_platform_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 15:18:30.000000 bodo_platform_utils-0.1.2/bodo_platform_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 15:18:30.000000 bodo_platform_utils-0.1.2/bodo_platform_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:18:30.000000 bodo_platform_utils-0.1.2/bodo_platform_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 15:18:30.000000 bodo_platform_utils-0.1.2/bodo_platform_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 15:18:30.000000 bodo_platform_utils-0.1.2/bodo_platform_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-11 15:18:30.151946 bodo_platform_utils-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82560 2024-04-11 15:17:07.000000 bodo_platform_utils-0.1.2/versioneer.py
```

### Comparing `bodo_platform_utils-0.1.1/LICENSE` & `bodo_platform_utils-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.1.1/PKG-INFO` & `bodo_platform_utils-0.1.2/bodo_platform_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bodo_platform_utils
-Version: 0.1.1
+Name: bodo-platform-utils
+Version: 0.1.2
 Summary: This is package contains utility functions to retrieve data from Cloud Providers for platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-utils
 Author: Bodo Inc
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodo_platform_utils-0.1.1/bodo_platform_utils/bodosqlwrapper.py` & `bodo_platform_utils-0.1.2/bodo_platform_utils/bodosqlwrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Example usage: python -u BodoSQLWrapper.py -c creds.json -f query.sql
-# To see all options, run: python -u BodoSQLWrapper.py --help
+# Example usage: python -m bodo_platform_utils.bodosqlwrapper --catalog CATALOG -f query.sql
+# To see all options, run: python -m bodo_platform_utils.bodosqlwrapper --help
 
 import argparse
-import json
+import os
 import time
 from urllib.parse import urlencode
 import logging
 
 import bodo
 import bodosql
 from bodosql.context_ext import typeof_bodo_sql
 import bodo.utils.tracing as tracing
+from bodo.sql_plan_cache import BodoSqlPlanCache
 import numba
 
 from .catalog import get_data
 
 # Turn verbose mode on
 bodo.set_verbose_level(2)
 bodo_logger = bodo.user_logging.get_current_bodo_verbose_logger()
@@ -62,14 +63,35 @@
     if sf_out_table_name != "":
         print("Saving output to Snowflake table: ", sf_out_table_name)
         t0 = time.time()
         output.to_sql(sf_out_table_name, sf_write_conn, if_exists="replace")
         print(f"Finished snowflake write. It took {time.time() - t0} seconds.")
 
 
+def get_cache_loc_from_dispatcher(dispatcher) -> str:
+    """
+    Get the location of the cached binary from the dispatcher
+    object of a function.
+    In case we aren't able to get the location, None
+    will be returned.
+
+    Args:
+        dispatcher: Dispatcher function for the query.
+    """
+    try:
+        cache_dir = dispatcher.stats.cache_path
+        cache_key = dispatcher._cache._index_key(
+            dispatcher.signatures[0], dispatcher.targetctx.codegen()
+        )
+        cache_file_name = dispatcher._cache._cache_file._load_index().get(cache_key)
+        return os.path.join(cache_dir, cache_file_name)
+    except Exception:
+        return None
+
+
 def run_sql_query_wrapper(
     dispatcher,
     sql_text,
     bc,
     sf_write_conn,
     sf_out_table_name,
     print_output,
@@ -139,15 +161,15 @@
         )
 
     database = args.database if args.database else catalog.get("database")
     if database is None:
         raise ValueError(
             "No database specified in either the credentials file or through the arguments."
         )
-    
+
     # Schema can be None for backwards compatibility
     schema = args.schema if args.schema else catalog.get("schema")
 
     # Create connection params
     connection_params = {"role": catalog["role"]} if "role" in catalog else {}
     if schema is not None:
         connection_params["schema"] = schema
@@ -156,34 +178,35 @@
     bsql_catalog = bodosql.SnowflakeCatalog(
         username=catalog["username"],
         password=catalog["password"],
         account=catalog["accountName"],
         warehouse=warehouse,
         database=database,
         connection_params=connection_params,
+        iceberg_volume=args.iceberg_volume,
     )
 
     # Create context
     bc = bodosql.BodoSQLContext(catalog=bsql_catalog)
 
     # Generate the plan and write it to a file
     if args.generate_plan_filename:
-        plan_text = bc.generate_plan(sql_text)
+        plan_text = bc.generate_plan(sql_text, show_cost=True)
         if bodo.get_rank() == 0:
             with open(args.generate_plan_filename, "w") as f:
                 f.write(plan_text)
-            print("Saved Plan to: ", args.generate_plan_filename)
+            print("[INFO] Saved Plan to: ", args.generate_plan_filename)
 
     # Convert to pandas and write to file
     if args.pandas_out_filename:
         pandas_text = bc.convert_to_pandas(sql_text)
         if bodo.get_rank() == 0:
             with open(args.pandas_out_filename, "w") as f:
                 f.write(pandas_text)
-            print("Saved Pandas Version to: ", args.pandas_out_filename)
+            print("[INFO] Saved Pandas Version to: ", args.pandas_out_filename)
 
     sf_write_conn = ""
     sf_out_table_name = ""
     if args.sf_out_table_loc:
         params = {"warehouse": bsql_catalog.warehouse}
         db, schema, sf_out_table_name = (
             args.sf_out_table_loc.split(".") if args.sf_out_table_loc else ("", "", "")
@@ -201,24 +224,40 @@
     t0 = time.time()
     dispatcher = bodo.jit(
         (numba.types.literal(sql_text), typeof_bodo_sql(bc, None)), cache=True
     )(run_sql_query)
     compilation_time = time.time() - t0
     bodo.barrier()  # Wait for all ranks to finish compilation
 
+    cache_hit: bool = dispatcher._cache_hits[dispatcher.signatures[0]] != 0
     if write_metrics:
         metrics_file.write(
             f"Compilation time: {float(compilation_time)}\n".encode("utf-8")
         )
-        metrics_file.write(
-            f"Ran from cache: { dispatcher._cache_hits[dispatcher.signatures[0]] != 0}\n".encode(
-                "utf-8"
+        metrics_file.write(f"Ran from cache: {cache_hit}\n".encode("utf-8"))
+
+    cache_loc = get_cache_loc_from_dispatcher(dispatcher)
+    if cache_loc and (bodo.get_rank() == 0):
+        print(
+            "[INFO] Binary {} {}".format(
+                "loaded from" if cache_hit else "saved to",
+                cache_loc,
             )
         )
 
+    # Get the cache key based on the sql string
+    plan_location: str | None = BodoSqlPlanCache.get_cache_loc(sql_text)
+    if plan_location and (bodo.get_rank() == 0):
+        if os.path.isfile(plan_location):
+            print(f"[INFO] SQL Plan cached at {plan_location}.")
+        else:
+            print(
+                f"[WARN] Expected SQL Plan to be cached at {plan_location}, but it wasn't found."
+            )
+
     # Run the query if not compile only
     if not args.compile_only:
         run_sql_query_wrapper(
             dispatcher,
             sql_text,
             bc,
             sf_write_conn,
@@ -323,11 +362,17 @@
     parser.add_argument(
         "-co",
         "--compile_only",
         required=False,
         action="store_true",
         help="Optional: If provided, the query will be compiled and the execution will be skipped.",
     )
+    parser.add_argument(
+        "--iceberg_volume",
+        required=False,
+        default=None,
+        help="Optional: Iceberg volume to use for writing as an iceberg table",
+    )
 
     args = parser.parse_args()
 
     main(args)
```

### Comparing `bodo_platform_utils-0.1.1/bodo_platform_utils/catalog.py` & `bodo_platform_utils-0.1.2/bodo_platform_utils/catalog.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.1.1/bodo_platform_utils/config.py` & `bodo_platform_utils-0.1.2/bodo_platform_utils/config.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.1.1/bodo_platform_utils/secrets.py` & `bodo_platform_utils-0.1.2/bodo_platform_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.1.1/bodo_platform_utils.egg-info/PKG-INFO` & `bodo_platform_utils-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bodo-platform-utils
-Version: 0.1.1
+Name: bodo_platform_utils
+Version: 0.1.2
 Summary: This is package contains utility functions to retrieve data from Cloud Providers for platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-utils
 Author: Bodo Inc
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodo_platform_utils-0.1.1/setup.py` & `bodo_platform_utils-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.1.1/versioneer.py` & `bodo_platform_utils-0.1.2/versioneer.py`

 * *Files identical despite different names*

