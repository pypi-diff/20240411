# Comparing `tmp/harlequin_risingwave-0.2.0.tar.gz` & `tmp/harlequin_risingwave-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin_risingwave-0.2.0.tar", max compression
+gzip compressed data, was "harlequin_risingwave-0.2.1.tar", max compression
```

## Comparing `harlequin_risingwave-0.2.0.tar` & `harlequin_risingwave-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-04-11 02:21:32.370979 harlequin_risingwave-0.2.0/LICENSE
--rw-r--r--   0        0        0     1536 2024-04-11 06:01:59.525587 harlequin_risingwave-0.2.0/README.md
--rw-r--r--   0        0        0       78 2024-04-11 02:34:20.970680 harlequin_risingwave-0.2.0/harlequin_risingwave/__init__.py
--rw-r--r--   0        0        0     6572 2024-04-11 08:46:17.045938 harlequin_risingwave-0.2.0/harlequin_risingwave/adapter.py
--rw-r--r--   0        0        0     1388 2024-04-11 03:04:09.846137 harlequin_risingwave-0.2.0/harlequin_risingwave/completion.py
--rw-r--r--   0        0        0     1113 2024-04-11 08:47:44.049377 harlequin_risingwave-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 harlequin_risingwave-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 02:21:32.370979 harlequin_risingwave-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1536 2024-04-11 06:01:59.525587 harlequin_risingwave-0.2.1/README.md
+-rw-r--r--   0        0        0       78 2024-04-11 02:34:20.970680 harlequin_risingwave-0.2.1/harlequin_risingwave/__init__.py
+-rw-r--r--   0        0        0     6443 2024-04-11 09:07:16.927885 harlequin_risingwave-0.2.1/harlequin_risingwave/adapter.py
+-rw-r--r--   0        0        0     1388 2024-04-11 03:04:09.846137 harlequin_risingwave-0.2.1/harlequin_risingwave/completion.py
+-rw-r--r--   0        0        0     1113 2024-04-11 09:08:27.990178 harlequin_risingwave-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 harlequin_risingwave-0.2.1/PKG-INFO
```

### Comparing `harlequin_risingwave-0.2.0/LICENSE` & `harlequin_risingwave-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin_risingwave-0.2.0/README.md` & `harlequin_risingwave-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `harlequin_risingwave-0.2.0/harlequin_risingwave/adapter.py` & `harlequin_risingwave-0.2.1/harlequin_risingwave/adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,74 +26,74 @@
         databases = self._get_databases()
         db_items: list[CatalogItem] = []
         for (db,) in databases:
             schemas = self._get_schemas(db)
             schema_items: list[CatalogItem] = []
             for (schema,) in schemas:
                 table_catalog = CatalogItem(
-                    qualified_identifier=f'"{db}"."{schema}"."table"',
-                    query_name=f'"{db}"."{schema}"."table"',
+                    qualified_identifier=f"{db}.{schema}.table",
+                    query_name=f"{db}.{schema}.table",
                     label="table",
                     type_label="t",
                     children=self._get_table(db, schema, "BASE TABLE", "table", "t"),
                 )
 
                 view_catalog = CatalogItem(
-                    qualified_identifier=f'"{db}"."{schema}"."view"',
-                    query_name=f'"{db}"."{schema}"."view"',
+                    qualified_identifier=f"{db}.{schema}.view",
+                    query_name=f"{db}.{schema}.view",
                     label="view",
                     type_label="v",
                     children=self._get_table(db, schema, "VIEW", "view", "v"),
                 )
 
                 materialized_view_catalog = CatalogItem(
-                    qualified_identifier=f'"{db}"."{schema}"."materialized_view"',
-                    query_name=f'"{db}"."{schema}"."materialized_view"',
+                    qualified_identifier=f"{db}.{schema}.materialized_view",
+                    query_name=f"{db}.{schema}.materialized_view",
                     label="materialized_view",
                     type_label="mv",
                     children=self._get_table(
                         db, schema, "MATERIALIZED VIEW", "materialized_view", "mv"
                     ),
                 )
 
                 source_catalog = CatalogItem(
-                    qualified_identifier=f'"{db}"."{schema}"."source"',
-                    query_name=f'"{db}"."{schema}"."source"',
+                    qualified_identifier=f"{db}.{schema}.source",
+                    query_name=f"{db}.{schema}.source",
                     label="source",
                     type_label="source",
                     children=self._get_table(db, schema, "SOURCE", "source", "source"),
                 )
 
                 sink_catalog = CatalogItem(
-                    qualified_identifier=f'"{db}"."{schema}"."sink"',
-                    query_name=f'"{db}"."{schema}"."sink"',
+                    qualified_identifier=f"{db}.{schema}.sink",
+                    query_name=f"{db}.{schema}.sink",
                     label="sink",
                     type_label="sink",
                     children=self._get_table(db, schema, "SINK", "sink", "sink"),
                 )
 
                 schema_items.append(
                     CatalogItem(
-                        qualified_identifier=f'"{db}"."{schema}"',
-                        query_name=f'"{db}"."{schema}"',
+                        qualified_identifier=f"{db}.{schema}",
+                        query_name=f"{db}.{schema}",
                         label=schema,
                         type_label="s",
                         children=[
                             table_catalog,
                             view_catalog,
                             materialized_view_catalog,
                             source_catalog,
                             sink_catalog,
                         ],
                     )
                 )
             db_items.append(
                 CatalogItem(
-                    qualified_identifier=f'"{db}"',
-                    query_name=f'"{db}"',
+                    qualified_identifier=db,
+                    query_name=db,
                     label=db,
                     type_label="db",
                     children=schema_items,
                 )
             )
         return Catalog(items=db_items)
 
@@ -136,22 +136,22 @@
                     and table_type = '{table_type}'
                 order by table_name asc;
                 """
             )
             table_names: list[str] = [row[0] for row in cur.fetchall()]
             tables = [
                 CatalogItem(
-                    qualified_identifier=f'"{dbname}"."{schema}"."{table_identifier}"."{table_name}"',
-                    query_name=f'"{table_name}"',
+                    qualified_identifier=f"{dbname}.{schema}.{table_name}",
+                    query_name=f"{dbname}.{schema}.{table_name}",
                     label=table_name,
                     type_label=type_label,
                     children=[
                         CatalogItem(
-                            qualified_identifier=f'"{dbname}"."{schema}"."{table_identifier}"."{table_name}"."{col}"',
-                            query_name=f'"{col}"',
+                            qualified_identifier=f"{dbname}.{schema}.{table_name}.{col}",
+                            query_name=col,
                             label=col,
                             type_label=self._get_short_type(col_type),
                         )
                         for col, col_type in self._get_columns(
                             dbname, schema, table_name
                         )
                     ],
```

### Comparing `harlequin_risingwave-0.2.0/harlequin_risingwave/completion.py` & `harlequin_risingwave-0.2.1/harlequin_risingwave/completion.py`

 * *Files identical despite different names*

### Comparing `harlequin_risingwave-0.2.0/pyproject.toml` & `harlequin_risingwave-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin-risingwave"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Harlequin adapter for Risingwave."
 authors = ["ZhengYu, Xu <zen-xu@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `harlequin_risingwave-0.2.0/PKG-INFO` & `harlequin_risingwave-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlequin-risingwave
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Harlequin adapter for Risingwave.
 License: MIT
 Author: ZhengYu, Xu
 Author-email: zen-xu@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

