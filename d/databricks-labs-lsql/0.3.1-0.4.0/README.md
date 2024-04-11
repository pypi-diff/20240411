# Comparing `tmp/databricks_labs_lsql-0.3.1.tar.gz` & `tmp/databricks_labs_lsql-0.4.0.tar.gz`

## Comparing `databricks_labs_lsql-0.3.1.tar` & `databricks_labs_lsql-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/__about__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/__main__.py
--rw-r--r--   0        0        0    13017 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/backends.py
--rw-r--r--   0        0        0    23637 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/core.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/deployment.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/py.typed
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/LICENSE
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/NOTICE
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/README.md
--rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/labs/lsql/__about__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/labs/lsql/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/labs/lsql/__main__.py
+-rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/labs/lsql/backends.py
+-rw-r--r--   0        0        0    23637 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/labs/lsql/core.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/labs/lsql/deployment.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/databricks/labs/lsql/py.typed
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/NOTICE
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/README.md
+-rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.0/PKG-INFO
```

### Comparing `databricks_labs_lsql-0.3.1/databricks/labs/lsql/backends.py` & `databricks_labs_lsql-0.4.0/databricks/labs/lsql/backends.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     This class is used to define the interface for SQL backends. It is used to
     define the methods that are required to be implemented by any SQL backend
     that is used by the library. The methods defined in this class are used to
     execute SQL statements, fetch results from SQL statements, and save data
     to tables."""
 
     @abstractmethod
-    def execute(self, sql: str) -> None:
+    def execute(self, sql: str, *, catalog: str | None = None, schema: str | None = None) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def fetch(self, sql: str) -> Iterator[Any]:
+    def fetch(self, sql: str, *, catalog: str | None = None, schema: str | None = None) -> Iterator[Any]:
         raise NotImplementedError
 
     @abstractmethod
     def save_table(self, full_name: str, rows: Sequence[DataclassInstance], klass: Dataclass, mode: str = "append"):
         raise NotImplementedError
 
     def create_table(self, full_name: str, klass: Dataclass):
@@ -133,21 +133,21 @@
     def __init__(self, ws: WorkspaceClient, warehouse_id, *, max_records_per_batch: int = 1000, **kwargs):
         self._sql = StatementExecutionExt(ws, warehouse_id=warehouse_id, **kwargs)
         self._max_records_per_batch = max_records_per_batch
         debug_truncate_bytes = ws.config.debug_truncate_bytes
         # while unit-testing, this value will contain a mock
         self._debug_truncate_bytes = debug_truncate_bytes if isinstance(debug_truncate_bytes, int) else 96
 
-    def execute(self, sql: str) -> None:
+    def execute(self, sql: str, *, catalog: str | None = None, schema: str | None = None) -> None:
         logger.debug(f"[api][execute] {self._only_n_bytes(sql, self._debug_truncate_bytes)}")
-        self._sql.execute(sql)
+        self._sql.execute(sql, catalog=catalog, schema=schema)
 
-    def fetch(self, sql: str) -> Iterator[Row]:
+    def fetch(self, sql: str, *, catalog: str | None = None, schema: str | None = None) -> Iterator[Row]:
         logger.debug(f"[api][fetch] {self._only_n_bytes(sql, self._debug_truncate_bytes)}")
-        return self._sql.fetch_all(sql)
+        return self._sql.fetch_all(sql, catalog=catalog, schema=schema)
 
     def save_table(self, full_name: str, rows: Sequence[DataclassInstance], klass: Dataclass, mode="append"):
         rows = self._filter_none_rows(rows, klass)
         self.create_table(full_name, klass)
         if len(rows) == 0:
             return
         fields = dataclasses.fields(klass)
@@ -184,25 +184,33 @@
 
 
 class _SparkBackend(SqlBackend):
     def __init__(self, spark, debug_truncate_bytes):
         self._spark = spark
         self._debug_truncate_bytes = debug_truncate_bytes if debug_truncate_bytes is not None else 96
 
-    def execute(self, sql: str) -> None:
+    def execute(self, sql: str, *, catalog: str | None = None, schema: str | None = None) -> None:
         logger.debug(f"[spark][execute] {self._only_n_bytes(sql, self._debug_truncate_bytes)}")
         try:
+            if catalog:
+                self._spark.sql(f"USE CATALOG {catalog}")
+            if schema:
+                self._spark.sql(f"USE SCHEMA {schema}")
             self._spark.sql(sql)
         except Exception as e:
             error_message = str(e)
             raise self._api_error_from_message(error_message) from None
 
-    def fetch(self, sql: str) -> Iterator[Row]:
+    def fetch(self, sql: str, *, catalog: str | None = None, schema: str | None = None) -> Iterator[Row]:
         logger.debug(f"[spark][fetch] {self._only_n_bytes(sql, self._debug_truncate_bytes)}")
         try:
+            if catalog:
+                self._spark.sql(f"USE CATALOG {catalog}")
+            if schema:
+                self._spark.sql(f"USE SCHEMA {schema}")
             return iter(self._spark.sql(sql).collect())
         except Exception as e:
             error_message = str(e)
             raise self._api_error_from_message(error_message) from None
 
     def save_table(self, full_name: str, rows: Sequence[DataclassInstance], klass: Dataclass, mode: str = "append"):
         rows = self._filter_none_rows(rows, klass)
@@ -262,18 +270,18 @@
         seen_before = sql in self.queries
         self.queries.append(sql)
         if not seen_before and self._fails_on_first is not None:
             for match, failure in self._fails_on_first.items():
                 if match in sql:
                     raise self._api_error_from_message(failure) from None
 
-    def execute(self, sql):
+    def execute(self, sql, *, catalog=None, schema=None):
         self._sql(sql)
 
-    def fetch(self, sql) -> Iterator[Row]:
+    def fetch(self, sql, *, catalog=None, schema=None) -> Iterator[Row]:
         self._sql(sql)
         rows = []
         if self._rows:
             for pattern in self._rows.keys():
                 r = re.compile(pattern)
                 if r.search(sql):
                     logger.debug(f"Found match: {sql}")
```

### Comparing `databricks_labs_lsql-0.3.1/databricks/labs/lsql/core.py` & `databricks_labs_lsql-0.4.0/databricks/labs/lsql/core.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.1/databricks/labs/lsql/deployment.py` & `databricks_labs_lsql-0.4.0/databricks/labs/lsql/deployment.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.1/.gitignore` & `databricks_labs_lsql-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.1/LICENSE` & `databricks_labs_lsql-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.1/NOTICE` & `databricks_labs_lsql-0.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.1/README.md` & `databricks_labs_lsql-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.1/pyproject.toml` & `databricks_labs_lsql-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.1/PKG-INFO` & `databricks_labs_lsql-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-lsql
-Version: 0.3.1
+Version: 0.4.0
 Summary: Lightweight stateless SQL execution for Databricks with minimal dependencies
 Project-URL: Documentation, https://github.com/databrickslabs/lsql#readme
 Project-URL: Issues, https://github.com/databrickslabs/lsql/issues
 Project-URL: Source, https://github.com/databrickslabs/lsql
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
```

