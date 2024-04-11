# Comparing `tmp/harlequin_mysql-0.1.3.tar.gz` & `tmp/harlequin_mysql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin_mysql-0.1.3.tar", max compression
+gzip compressed data, was "harlequin_mysql-0.2.0.tar", max compression
```

## Comparing `harlequin_mysql-0.1.3.tar` & `harlequin_mysql-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-01-29 21:29:13.331625 harlequin_mysql-0.1.3/LICENSE
--rw-r--r--   0        0        0     1313 2024-01-29 21:29:13.331625 harlequin_mysql-0.1.3/README.md
--rw-r--r--   0        0        0     1408 2024-01-29 21:29:13.335625 harlequin_mysql-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       95 2024-01-29 21:29:13.335625 harlequin_mysql-0.1.3/src/harlequin_mysql/__init__.py
--rw-r--r--   0        0        0    10004 2024-01-29 21:29:13.335625 harlequin_mysql-0.1.3/src/harlequin_mysql/adapter.py
--rw-r--r--   0        0        0     2609 2024-01-29 21:29:13.335625 harlequin_mysql-0.1.3/src/harlequin_mysql/cli_options.py
--rw-r--r--   0        0        0     1616 2024-01-29 21:29:13.335625 harlequin_mysql-0.1.3/src/harlequin_mysql/completions.py
--rw-r--r--   0        0        0    25245 2024-01-29 21:29:13.335625 harlequin_mysql-0.1.3/src/harlequin_mysql/functions.tsv
--rw-r--r--   0        0        0    19404 2024-01-29 21:29:13.335625 harlequin_mysql-0.1.3/src/harlequin_mysql/keywords.csv
--rw-r--r--   0        0        0        0 2024-01-29 21:29:13.335625 harlequin_mysql-0.1.3/src/harlequin_mysql/py.typed
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 harlequin_mysql-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 16:58:58.685629 harlequin_mysql-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1313 2024-04-11 16:58:58.685629 harlequin_mysql-0.2.0/README.md
+-rw-r--r--   0        0        0     1408 2024-04-11 16:58:58.689629 harlequin_mysql-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       95 2024-04-11 16:58:58.689629 harlequin_mysql-0.2.0/src/harlequin_mysql/__init__.py
+-rw-r--r--   0        0        0    13600 2024-04-11 16:58:58.689629 harlequin_mysql-0.2.0/src/harlequin_mysql/adapter.py
+-rw-r--r--   0        0        0     2986 2024-04-11 16:58:58.689629 harlequin_mysql-0.2.0/src/harlequin_mysql/cli_options.py
+-rw-r--r--   0        0        0     1616 2024-04-11 16:58:58.689629 harlequin_mysql-0.2.0/src/harlequin_mysql/completions.py
+-rw-r--r--   0        0        0    25245 2024-04-11 16:58:58.689629 harlequin_mysql-0.2.0/src/harlequin_mysql/functions.tsv
+-rw-r--r--   0        0        0    19404 2024-04-11 16:58:58.689629 harlequin_mysql-0.2.0/src/harlequin_mysql/keywords.csv
+-rw-r--r--   0        0        0        0 2024-04-11 16:58:58.689629 harlequin_mysql-0.2.0/src/harlequin_mysql/py.typed
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 harlequin_mysql-0.2.0/PKG-INFO
```

### Comparing `harlequin_mysql-0.1.3/LICENSE` & `harlequin_mysql-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin_mysql-0.1.3/README.md` & `harlequin_mysql-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `harlequin_mysql-0.1.3/pyproject.toml` & `harlequin_mysql-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin-mysql"
-version = "0.1.3"
+version = "0.2.0"
 description = "A Harlequin adapter for MySQL."
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "harlequin_mysql", from = "src" },
 ]
```

### Comparing `harlequin_mysql-0.1.3/src/harlequin_mysql/adapter.py` & `harlequin_mysql-0.2.0/src/harlequin_mysql/adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import re
 from typing import Any, Sequence
 
 from harlequin import (
     HarlequinAdapter,
     HarlequinConnection,
     HarlequinCursor,
 )
@@ -12,45 +13,61 @@
 from harlequin.exception import (
     HarlequinConfigError,
     HarlequinConnectionError,
     HarlequinQueryError,
 )
 from mysql.connector import FieldType
 from mysql.connector.cursor import MySQLCursor
-from mysql.connector.pooling import MySQLConnectionPool
+from mysql.connector.errors import InternalError, PoolError
+from mysql.connector.pooling import (
+    MySQLConnectionPool,
+    PooledMySQLConnection,
+)
 from textual_fastdatatable.backend import AutoBackendType
 
 from harlequin_mysql.cli_options import MYSQLADAPTER_OPTIONS
 from harlequin_mysql.completions import load_completions
 
+USE_DATABASE_PROG = re.compile(
+    r"\s*use\s+([^\\/?%*:|\"<>.]{1,64})", flags=re.IGNORECASE
+)
+
 
 class HarlequinMySQLCursor(HarlequinCursor):
-    def __init__(self, cur: MySQLCursor, *_: Any, **__: Any) -> None:
+    def __init__(
+        self, cur: MySQLCursor, conn: PooledMySQLConnection, *_: Any, **__: Any
+    ) -> None:
         self.cur = cur
+        self.conn = conn
         self._limit: int | None = None
 
     def columns(self) -> list[tuple[str, str]]:
         assert self.cur.description is not None
         return [(col[0], self._get_short_type(col[1])) for col in self.cur.description]
 
     def set_limit(self, limit: int) -> "HarlequinMySQLCursor":
         self._limit = limit
         return self
 
     def fetchall(self) -> AutoBackendType:
         try:
             if self._limit is None:
-                return self.cur.fetchall()
+                results = self.cur.fetchall()
             else:
-                return self.cur.fetchmany(self._limit)
+                results = self.cur.fetchmany(self._limit)
+            return results
         except Exception as e:
             raise HarlequinQueryError(
                 msg=str(e),
                 title="Harlequin encountered an error while executing your query.",
             ) from e
+        finally:
+            self.conn.consume_results()
+            self.cur.close()
+            self.conn.close()
 
     @staticmethod
     def _get_short_type(type_id: int) -> str:
         mapping = {
             FieldType.BIT: "010",
             FieldType.BLOB: "0b",
             FieldType.DATE: "d",
@@ -89,43 +106,92 @@
         conn_str: Sequence[str],
         *_: Any,
         init_message: str = "",
         options: dict[str, Any],
     ) -> None:
         self.init_message = init_message
         try:
-            self.pool: MySQLConnectionPool = MySQLConnectionPool(
+            self._pool: MySQLConnectionPool = MySQLConnectionPool(
                 pool_name="harlequin",
-                pool_size=5,
                 pool_reset_session=False,
-                **options,
                 autocommit=True,
+                **options,
             )
         except Exception as e:
             raise HarlequinConnectionError(
                 msg=str(e), title="Harlequin could not connect to your database."
             ) from e
 
+    def safe_get_mysql_cursor(
+        self, buffered: bool = False
+    ) -> tuple[PooledMySQLConnection | None, MySQLCursor | None]:
+        """
+        Return None if the connection pool is exhausted, to avoid getting
+        in an unrecoverable state.
+        """
+        try:
+            conn = self._pool.get_connection()
+        except (InternalError, PoolError):
+            # if we're out of connections, we can't raise a query error,
+            # or we get in a state where we have cursors without fetched
+            # results, which requires a restart of Harlequin. Instead,
+            # just return None and silently fail (there isn't a sensible
+            # way to show an error to the user without aborting processing
+            # all the other cursors).
+            return None, None
+
+        try:
+            cur: MySQLCursor = conn.cursor(buffered=buffered)
+        except InternalError:
+            # cursor has an unread result. Try to consume the results,
+            # and try again.
+            conn.consume_results()
+            cur = conn.cursor(buffered=buffered)
+
+        return conn, cur
+
+    def set_pool_config(self, **config: Any) -> None:
+        """
+        Updates the config of the MySQL connection pool.
+        """
+        self._pool.set_config(**config)
+
     def execute(self, query: str) -> HarlequinCursor | None:
+        retval: HarlequinCursor | None = None
+
+        conn, cur = self.safe_get_mysql_cursor()
+        if conn is None or cur is None:
+            return None
+
         try:
-            conn = self.pool.get_connection()
-            cur = conn.cursor()
             cur.execute(query)
         except Exception as e:
+            cur.close()
+            conn.close()
             raise HarlequinQueryError(
                 msg=str(e),
                 title="Harlequin encountered an error while executing your query.",
             ) from e
         else:
             if cur.description is not None:
-                return HarlequinMySQLCursor(cur)
+                retval = HarlequinMySQLCursor(cur, conn=conn)
             else:
-                return None
-        finally:
-            conn.close()
+                cur.close()
+                conn.close()
+
+        # this is a hack to update all connections in the pool if the user
+        # changes the database for the active connection.
+        # it is impossible to check the database or other config
+        # of a connection with an open cursor, and we can't use a dedicated
+        # connection for user queries, since mysql only supports a single
+        # (unfetched) cursor per connection.
+        if match := USE_DATABASE_PROG.match(query):
+            new_db = match.group(1)
+            self.set_pool_config(database=new_db)
+        return retval
 
     def get_catalog(self) -> Catalog:
         databases = self._get_databases()
         db_items: list[CatalogItem] = []
         for (db,) in databases:
             relations = self._get_relations(db)
             rel_items: list[CatalogItem] = []
@@ -160,63 +226,87 @@
             )
         return Catalog(items=db_items)
 
     def get_completions(self) -> list[HarlequinCompletion]:
         return load_completions()
 
     def _get_databases(self) -> list[tuple[str]]:
-        conn = self.pool.get_connection()
-        cur = conn.cursor()
+        conn, cur = self.safe_get_mysql_cursor(buffered=True)
+        if conn is None or cur is None:
+            raise HarlequinConnectionError(
+                title="Connection pool exhausted",
+                msg=(
+                    "Connection pool exhausted. Try restarting Harlequin "
+                    "with a larger pool or running fewer queries at once."
+                ),
+            )
         cur.execute(
             """
             show databases
             where `Database` not in (
                 'sys', 'information_schema', 'performance_schema', 'mysql'
             )
             """
         )
-        results: list[tuple[str]] = cur.fetchall()
+        results: list[tuple[str]] = cur.fetchall()  # type: ignore
+        cur.close()
         conn.close()
         return results
 
     def _get_relations(self, db_name: str) -> list[tuple[str, str]]:
-        conn = self.pool.get_connection()
-        cur = conn.cursor()
+        conn, cur = self.safe_get_mysql_cursor(buffered=True)
+        if conn is None or cur is None:
+            raise HarlequinConnectionError(
+                title="Connection pool exhausted",
+                msg=(
+                    "Connection pool exhausted. Try restarting Harlequin "
+                    "with a larger pool or running fewer queries at once."
+                ),
+            )
         cur.execute(
             f"""
             select 
                 table_name, 
                 case 
                     when table_type like '%TABLE' then 't' 
                     else 'v' 
                 end as table_type
             from information_schema.tables
             where table_schema = '{db_name}'
             order by table_name asc
             ;"""
         )
-        results: list[tuple[str, str]] = cur.fetchall()
+        results: list[tuple[str, str]] = cur.fetchall()  # type: ignore
+        cur.close()
         conn.close()
         return results
 
     def _get_columns(self, db_name: str, rel_name: str) -> list[tuple[str, str]]:
-        conn = self.pool.get_connection()
-        cur = conn.cursor()
+        conn, cur = self.safe_get_mysql_cursor(buffered=True)
+        if conn is None or cur is None:
+            raise HarlequinConnectionError(
+                title="Connection pool exhausted",
+                msg=(
+                    "Connection pool exhausted. Try restarting Harlequin "
+                    "with a larger pool or running fewer queries at once."
+                ),
+            )
         cur.execute(
             f"""
             select column_name, data_type
             from information_schema.columns
             where
                 table_schema = '{db_name}'
                 and table_name = '{rel_name}'
                 and extra not like '%INVISIBLE%'
             order by ordinal_position asc
             ;"""
         )
-        results: list[tuple[str, str]] = cur.fetchall()
+        results: list[tuple[str, str]] = cur.fetchall()  # type: ignore
+        cur.close()
         conn.close()
         return results
 
     @staticmethod
     def _get_short_col_type(info_schema_type: str) -> str:
         mapping = {
             "bigint": "###",
@@ -262,14 +352,15 @@
         password2: str | None = None,
         password3: str | None = None,
         connection_timeout: str | int | None = None,
         ssl_ca: str | None = None,
         ssl_cert: str | None = None,
         ssl_disabled: str | bool | None = False,
         ssl_key: str | None = None,
+        pool_size: str | int | None = 5,
         **_: Any,
     ) -> None:
         if conn_str:
             raise HarlequinConnectionError(
                 f"Cannot provide a DSN to the MySQL adapter. Got:\n{conn_str}"
             )
         try:
@@ -285,14 +376,15 @@
                 "connection_timeout": int(connection_timeout)
                 if connection_timeout is not None
                 else None,
                 "ssl_ca": ssl_ca,
                 "ssl_cert": ssl_cert,
                 "ssl_disabled": ssl_disabled if ssl_disabled is not None else False,
                 "ssl_key": ssl_key,
+                "pool_size": int(pool_size) if pool_size is not None else 5,
             }
         except (ValueError, TypeError) as e:
             raise HarlequinConfigError(
                 msg=f"MySQL adapter received bad config value: {e}",
                 title="Harlequin could not initialize the selected adapter.",
             ) from e
```

### Comparing `harlequin_mysql-0.1.3/src/harlequin_mysql/cli_options.py` & `harlequin_mysql-0.2.0/src/harlequin_mysql/cli_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,14 +107,26 @@
     name="ssl-key",
     description="File containing the SSL key.",
     exists=True,
     dir_okay=False,
     short_decls=["--sslkey"],
 )
 
+pool_size = TextOption(
+    name="pool-size",
+    description=(
+        "The number of concurrent connections maintained by Harlequin. MySQL "
+        "only allows one cursor per connection, so this sets the number of queries "
+        "that can be executed at once in Harlequin."
+    ),
+    short_decls=["-n"],
+    default="5",
+    validator=_int_validator,
+)
+
 
 MYSQLADAPTER_OPTIONS = [
     host,
     port,
     unix_socket,
     database,
     user,
@@ -122,8 +134,9 @@
     password2,
     password3,
     connect_timeout,
     ssl_ca,
     ssl_cert,
     ssl_disabled,
     ssl_key,
+    pool_size,
 ]
```

### Comparing `harlequin_mysql-0.1.3/src/harlequin_mysql/completions.py` & `harlequin_mysql-0.2.0/src/harlequin_mysql/completions.py`

 * *Files identical despite different names*

### Comparing `harlequin_mysql-0.1.3/src/harlequin_mysql/functions.tsv` & `harlequin_mysql-0.2.0/src/harlequin_mysql/functions.tsv`

 * *Files identical despite different names*

### Comparing `harlequin_mysql-0.1.3/src/harlequin_mysql/keywords.csv` & `harlequin_mysql-0.2.0/src/harlequin_mysql/keywords.csv`

 * *Files identical despite different names*

### Comparing `harlequin_mysql-0.1.3/PKG-INFO` & `harlequin_mysql-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlequin-mysql
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Harlequin adapter for MySQL.
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

