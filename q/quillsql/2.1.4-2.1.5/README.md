# Comparing `tmp/quillsql-2.1.4.tar.gz` & `tmp/quillsql-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quillsql-2.1.4.tar", last modified: Tue Mar 19 17:56:07 2024, max compression
+gzip compressed data, was "quillsql-2.1.5.tar", last modified: Wed Apr 10 23:49:30 2024, max compression
```

## Comparing `quillsql-2.1.4.tar` & `quillsql-2.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-03-19 17:56:07.058543 quillsql-2.1.4/
--rw-r--r--   0 shawn      (501) staff       (20)     1809 2024-03-19 17:56:07.058385 quillsql-2.1.4/PKG-INFO
--rw-r--r--   0 shawn      (501) staff       (20)     1394 2024-02-28 03:00:41.000000 quillsql-2.1.4/README.md
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-03-19 17:56:07.055167 quillsql-2.1.4/quillsql/
--rw-r--r--   0 shawn      (501) staff       (20)       70 2024-01-12 01:03:02.000000 quillsql-2.1.4/quillsql/__init__.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-03-19 17:56:07.056241 quillsql-2.1.4/quillsql/assets/
--rw-r--r--   0 shawn      (501) staff       (20)       44 2024-03-18 18:58:55.000000 quillsql-2.1.4/quillsql/assets/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)    40768 2024-02-28 03:00:41.000000 quillsql-2.1.4/quillsql/assets/pgtypes.py
--rw-r--r--   0 shawn      (501) staff       (20)     7544 2024-03-04 18:48:48.000000 quillsql-2.1.4/quillsql/core.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-03-19 17:56:07.057591 quillsql-2.1.4/quillsql/db/
--rw-r--r--   0 shawn      (501) staff       (20)       62 2024-02-28 03:00:41.000000 quillsql-2.1.4/quillsql/db/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)     4220 2024-03-04 18:48:48.000000 quillsql-2.1.4/quillsql/db/bigquery.py
--rw-r--r--   0 shawn      (501) staff       (20)     2570 2024-03-01 01:29:00.000000 quillsql-2.1.4/quillsql/db/cached_connection.py
--rw-r--r--   0 shawn      (501) staff       (20)     2054 2024-02-28 03:00:41.000000 quillsql-2.1.4/quillsql/db/db_helper.py
--rw-r--r--   0 shawn      (501) staff       (20)     2799 2024-03-01 01:29:00.000000 quillsql-2.1.4/quillsql/db/postgres.py
--rw-r--r--   0 shawn      (501) staff       (20)      161 2024-01-12 01:03:02.000000 quillsql-2.1.4/quillsql/error.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-03-19 17:56:07.058043 quillsql-2.1.4/quillsql/utils/
--rw-r--r--   0 shawn      (501) staff       (20)       75 2024-02-28 03:00:41.000000 quillsql-2.1.4/quillsql/utils/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)      678 2024-02-28 03:00:41.000000 quillsql-2.1.4/quillsql/utils/run_query_processes.py
--rw-r--r--   0 shawn      (501) staff       (20)      297 2024-02-28 03:00:41.000000 quillsql-2.1.4/quillsql/utils/schema_conversion.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-03-19 17:56:07.058220 quillsql-2.1.4/quillsql.egg-info/
--rw-r--r--   0 shawn      (501) staff       (20)     1809 2024-03-19 17:56:07.000000 quillsql-2.1.4/quillsql.egg-info/PKG-INFO
--rw-r--r--   0 shawn      (501) staff       (20)      519 2024-03-19 17:56:07.000000 quillsql-2.1.4/quillsql.egg-info/SOURCES.txt
--rw-r--r--   0 shawn      (501) staff       (20)        1 2024-03-19 17:56:07.000000 quillsql-2.1.4/quillsql.egg-info/dependency_links.txt
--rw-r--r--   0 shawn      (501) staff       (20)       86 2024-03-19 17:56:07.000000 quillsql-2.1.4/quillsql.egg-info/requires.txt
--rw-r--r--   0 shawn      (501) staff       (20)        9 2024-03-19 17:56:07.000000 quillsql-2.1.4/quillsql.egg-info/top_level.txt
--rw-r--r--   0 shawn      (501) staff       (20)       38 2024-03-19 17:56:07.058583 quillsql-2.1.4/setup.cfg
--rw-r--r--   0 shawn      (501) staff       (20)      569 2024-03-19 17:55:51.000000 quillsql-2.1.4/setup.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-04-10 23:49:30.539900 quillsql-2.1.5/
+-rw-r--r--   0 shawn      (501) staff       (20)     1809 2024-04-10 23:49:30.539732 quillsql-2.1.5/PKG-INFO
+-rw-r--r--   0 shawn      (501) staff       (20)     1394 2024-02-28 03:00:41.000000 quillsql-2.1.5/README.md
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-04-10 23:49:30.537634 quillsql-2.1.5/quillsql/
+-rw-r--r--   0 shawn      (501) staff       (20)       70 2024-01-12 01:03:02.000000 quillsql-2.1.5/quillsql/__init__.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-04-10 23:49:30.538419 quillsql-2.1.5/quillsql/assets/
+-rw-r--r--   0 shawn      (501) staff       (20)       44 2024-03-18 18:58:55.000000 quillsql-2.1.5/quillsql/assets/__init__.py
+-rw-r--r--   0 shawn      (501) staff       (20)    40768 2024-02-28 03:00:41.000000 quillsql-2.1.5/quillsql/assets/pgtypes.py
+-rw-r--r--   0 shawn      (501) staff       (20)     7557 2024-04-10 22:18:41.000000 quillsql-2.1.5/quillsql/core.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-04-10 23:49:30.539015 quillsql-2.1.5/quillsql/db/
+-rw-r--r--   0 shawn      (501) staff       (20)       62 2024-02-28 03:00:41.000000 quillsql-2.1.5/quillsql/db/__init__.py
+-rw-r--r--   0 shawn      (501) staff       (20)     4220 2024-03-04 18:48:48.000000 quillsql-2.1.5/quillsql/db/bigquery.py
+-rw-r--r--   0 shawn      (501) staff       (20)     2570 2024-03-01 01:29:00.000000 quillsql-2.1.5/quillsql/db/cached_connection.py
+-rw-r--r--   0 shawn      (501) staff       (20)     2054 2024-02-28 03:00:41.000000 quillsql-2.1.5/quillsql/db/db_helper.py
+-rw-r--r--   0 shawn      (501) staff       (20)     2799 2024-03-01 01:29:00.000000 quillsql-2.1.5/quillsql/db/postgres.py
+-rw-r--r--   0 shawn      (501) staff       (20)      161 2024-01-12 01:03:02.000000 quillsql-2.1.5/quillsql/error.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-04-10 23:49:30.539348 quillsql-2.1.5/quillsql/utils/
+-rw-r--r--   0 shawn      (501) staff       (20)       75 2024-02-28 03:00:41.000000 quillsql-2.1.5/quillsql/utils/__init__.py
+-rw-r--r--   0 shawn      (501) staff       (20)      673 2024-04-10 22:18:41.000000 quillsql-2.1.5/quillsql/utils/run_query_processes.py
+-rw-r--r--   0 shawn      (501) staff       (20)      297 2024-02-28 03:00:41.000000 quillsql-2.1.5/quillsql/utils/schema_conversion.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2024-04-10 23:49:30.539540 quillsql-2.1.5/quillsql.egg-info/
+-rw-r--r--   0 shawn      (501) staff       (20)     1809 2024-04-10 23:49:30.000000 quillsql-2.1.5/quillsql.egg-info/PKG-INFO
+-rw-r--r--   0 shawn      (501) staff       (20)      519 2024-04-10 23:49:30.000000 quillsql-2.1.5/quillsql.egg-info/SOURCES.txt
+-rw-r--r--   0 shawn      (501) staff       (20)        1 2024-04-10 23:49:30.000000 quillsql-2.1.5/quillsql.egg-info/dependency_links.txt
+-rw-r--r--   0 shawn      (501) staff       (20)       86 2024-04-10 23:49:30.000000 quillsql-2.1.5/quillsql.egg-info/requires.txt
+-rw-r--r--   0 shawn      (501) staff       (20)        9 2024-04-10 23:49:30.000000 quillsql-2.1.5/quillsql.egg-info/top_level.txt
+-rw-r--r--   0 shawn      (501) staff       (20)       38 2024-04-10 23:49:30.539934 quillsql-2.1.5/setup.cfg
+-rw-r--r--   0 shawn      (501) staff       (20)      569 2024-04-10 22:19:21.000000 quillsql-2.1.5/setup.py
```

### Comparing `quillsql-2.1.4/PKG-INFO` & `quillsql-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quillsql
-Version: 2.1.4
+Version: 2.1.5
 Summary: Quill SDK for Python.
 Home-page: https://github.com/quill-sql/quill-python
 Author: Quill
 Author-email: shawn@quillsql.com
 Description-Content-Type: text/markdown
 Requires-Dist: psycopg2-binary
 Requires-Dist: requests
```

### Comparing `quillsql-2.1.4/README.md` & `quillsql-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `quillsql-2.1.4/quillsql/assets/pgtypes.py` & `quillsql-2.1.5/quillsql/assets/pgtypes.py`

 * *Files identical despite different names*

### Comparing `quillsql-2.1.4/quillsql/core.py` & `quillsql-2.1.5/quillsql/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             return {"error": str(err), "status": "error"}
 
     def run_queries(self, queries, pkDatabaseType, databaseType, metadata=None, runQueryConfig=None):
         results = {}
         if not queries:
             return {"queryResults": []}
         if databaseType and databaseType.lower() != pkDatabaseType.lower():
-            return {"dbMismatched": True, "backendDatbaseType": pkDatabaseType}
+            return {"dbMismatched": True, "backendDatabaseType": pkDatabaseType}
         if runQueryConfig and runQueryConfig.get("arrayToMap"):
             array_to_map(
                 queries, runQueryConfig.get("arrayToMap"), metadata, self.target_connection
             )
             return {"queryResults": []}
         elif runQueryConfig and runQueryConfig.get("getColumns"):
             query_results = self.target_connection.query(queries[0].strip().rstrip(";") + ' limit 1')
@@ -137,18 +137,16 @@
         else:
             if runQueryConfig and runQueryConfig.get("limitThousand"):
                 queries = [query.strip().rstrip(";") + " limit 1000" for query in queries]
             elif runQueryConfig and runQueryConfig.get("limitBy"):
                 queries = [query.strip().rstrip(";") + " limit " + runQueryConfig.get("limitBy") for query in queries]
             query_results = [self.target_connection.query(query) for query in queries]
             results["queryResults"] = query_results
-            if runQueryConfig and runQueryConfig.get("removeFields"):
-                results["queryResults"] = remove_fields(
-                    query_results, runQueryConfig.get("removeFields")
-                )
+            if runQueryConfig and runQueryConfig.get("fieldsToRemove"):
+                results["queryResults"] = [ remove_fields(query_result, runQueryConfig.get("fieldsToRemove")) for query_result in results["queryResults"]]
             if runQueryConfig and runQueryConfig.get("convertDatatypes"):
                 for query_result in results["queryResults"]:
                     query_result["fields"] = [
                         {
                             "name": field["name"],
                             "displayName": field["name"],
                             "field": field["name"],
```

### Comparing `quillsql-2.1.4/quillsql/db/bigquery.py` & `quillsql-2.1.5/quillsql/db/bigquery.py`

 * *Files identical despite different names*

### Comparing `quillsql-2.1.4/quillsql/db/cached_connection.py` & `quillsql-2.1.5/quillsql/db/cached_connection.py`

 * *Files identical despite different names*

### Comparing `quillsql-2.1.4/quillsql/db/db_helper.py` & `quillsql-2.1.5/quillsql/db/db_helper.py`

 * *Files identical despite different names*

### Comparing `quillsql-2.1.4/quillsql/db/postgres.py` & `quillsql-2.1.5/quillsql/db/postgres.py`

 * *Files identical despite different names*

### Comparing `quillsql-2.1.4/quillsql/utils/run_query_processes.py` & `quillsql-2.1.5/quillsql/utils/run_query_processes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 
-def remove_fields(query_result, cursor_description, fields_to_remove):
+def remove_fields(query_result, fields_to_remove):
   fields = [
-      {"name": desc[0], "dataTypeID": desc[1]}
-      for desc in cursor_description
-      if desc[0] in fields_to_remove
+      {"name": field['name'], "dataTypeID": field['dataTypeID']}
+      for field in query_result['fields']
+      if field['name'] not in fields_to_remove
   ]
-  rows = [dict(json.loads(json.dumps(row, default=str))) for row in query_result]
-
+  rows = [row for row in query_result['rows']]
   for row in rows:
     for field in fields_to_remove:
       if field in row:
           del row[field]
-  return {fields, rows}
+  return {"fields": fields, "rows": rows}
 
 def array_to_map(queries, array_to_map, metadata, target_pool):
   for i in range(len(queries)):
     query_result = target_pool.query(queries[i])
     metadata[array_to_map.get("arrayName")][i][array_to_map.get("field")] = query_result.get("rows")
```

### Comparing `quillsql-2.1.4/quillsql.egg-info/PKG-INFO` & `quillsql-2.1.5/quillsql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quillsql
-Version: 2.1.4
+Version: 2.1.5
 Summary: Quill SDK for Python.
 Home-page: https://github.com/quill-sql/quill-python
 Author: Quill
 Author-email: shawn@quillsql.com
 Description-Content-Type: text/markdown
 Requires-Dist: psycopg2-binary
 Requires-Dist: requests
```

### Comparing `quillsql-2.1.4/quillsql.egg-info/SOURCES.txt` & `quillsql-2.1.5/quillsql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quillsql-2.1.4/setup.py` & `quillsql-2.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="quillsql",
-    version="2.1.4",
+    version="2.1.5",
     packages=find_packages(),
     install_requires=[
         "psycopg2-binary",
         "requests",
         "redis",
         "python-dotenv",
         "pytest",
```

