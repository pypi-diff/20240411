# Comparing `tmp/database-mysql-local-0.0.285.tar.gz` & `tmp/database-mysql-local-0.0.286.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-mysql-local-0.0.285.tar", last modified: Sat Apr  6 17:18:19 2024, max compression
+gzip compressed data, was "database-mysql-local-0.0.286.tar", last modified: Thu Apr 11 16:45:39 2024, max compression
```

## Comparing `database-mysql-local-0.0.285.tar` & `database-mysql-local-0.0.286.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:18:19.019203 database-mysql-local-0.0.285/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-06 17:18:19.019203 database-mysql-local-0.0.285/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:18:19.011203 database-mysql-local-0.0.285/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:18:19.015203 database-mysql-local-0.0.285/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38968 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31705 2024-04-06 17:17:46.000000 database-mysql-local-0.0.285/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-04-06 17:17:43.000000 database-mysql-local-0.0.285/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:18:19.015203 database-mysql-local-0.0.285/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 17:18:19.000000 database-mysql-local-0.0.285/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:18:19.019203 database-mysql-local-0.0.285/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-06 17:17:18.000000 database-mysql-local-0.0.285/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:45:39.279912 database-mysql-local-0.0.286/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-11 16:45:39.279912 database-mysql-local-0.0.286/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:45:39.275912 database-mysql-local-0.0.286/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:45:39.279912 database-mysql-local-0.0.286/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39453 2024-04-11 16:45:06.000000 database-mysql-local-0.0.286/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31705 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-04-11 16:45:03.000000 database-mysql-local-0.0.286/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-11 16:44:39.000000 database-mysql-local-0.0.286/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:45:39.279912 database-mysql-local-0.0.286/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-11 16:45:39.000000 database-mysql-local-0.0.286/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-11 16:45:39.000000 database-mysql-local-0.0.286/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:45:39.000000 database-mysql-local-0.0.286/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 16:45:39.000000 database-mysql-local-0.0.286/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 16:45:39.000000 database-mysql-local-0.0.286/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-11 16:45:06.000000 database-mysql-local-0.0.286/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:45:39.279912 database-mysql-local-0.0.286/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-11 16:45:06.000000 database-mysql-local-0.0.286/setup.py
```

### Comparing `database-mysql-local-0.0.285/PKG-INFO` & `database-mysql-local-0.0.286/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.285
+Version: 0.0.286
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database-mysql-local-0.0.285/README.md` & `database-mysql-local-0.0.286/README.md`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/connector.py` & `database-mysql-local-0.0.286/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/constants.py` & `database-mysql-local-0.0.286/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/cursor.py` & `database-mysql-local-0.0.286/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/generic_crud.py` & `database-mysql-local-0.0.286/database_mysql_local/src/generic_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,16 @@
                 inserted_id = self._get_existing_duplicate_id(table_name, exception)
             else:
                 raise exception
 
         return inserted_id
 
     def upsert(self, *, schema_name: str = None, table_name: str = None, view_table_name: str = None,
-               data_json: dict = None, data_json_compare: dict = None, order_by: str = None) -> Optional[int]:
+               data_json: dict = None, data_json_compare: dict = None, order_by: str = None,
+               compare_with_or: bool = False) -> Optional[int]:
         """Inserts a new row into the table, or updates an existing row if a row with the
           same values as data_json_compare exists,
           and returns the id of the new row or None if an error occurred."""
         schema_name = schema_name or self.schema_name
         table_name = table_name or self.default_table_name
         view_table_name = view_table_name or self.default_view_table_name
         id_column_name = self.generate_id_column_name(table_name)
@@ -113,19 +114,26 @@
             self.logger.warning(log_message="GenericCRUD.upsert: data_json is empty")
             return None
         if not data_json_compare:
             return GenericCRUD.insert(self, schema_name=schema_name, table_name=table_name, data_json=data_json,
                                       ignore_duplicate=True)
 
         columns, values, processed_data_json_compare = process_insert_data_json(data_json=data_json_compare)
-        table_id = GenericCRUD.select_one_value_by_where(
-            self, schema_name=schema_name, view_table_name=view_table_name, select_clause_value=id_column_name,
-            where=" AND ".join([f"{key}=%s" for key in processed_data_json_compare.keys()]),
-            params=tuple(processed_data_json_compare.values()),
-            order_by=order_by)
+        if compare_with_or:
+            table_id = GenericCRUD.select_one_value_by_where(
+                self, schema_name=schema_name, view_table_name=view_table_name, select_clause_value=id_column_name,
+                where=" OR ".join([f"{key}=%s" for key in processed_data_json_compare.keys()]),
+                params=tuple(processed_data_json_compare.values()),
+                order_by=order_by)
+        else:
+            table_id = GenericCRUD.select_one_value_by_where(
+                self, schema_name=schema_name, view_table_name=view_table_name, select_clause_value=id_column_name,
+                where=" AND ".join([f"{key}=%s" for key in processed_data_json_compare.keys()]),
+                params=tuple(processed_data_json_compare.values()),
+                order_by=order_by)
         if table_id:
             GenericCRUD.update_by_id(self, schema_name=schema_name, table_name=table_name,
                                      id_column_name=id_column_name,
                                      id_column_value=table_id, data_json=data_json)
             return table_id
         else:
             return GenericCRUD.insert(self, schema_name=schema_name, table_name=table_name, data_json=data_json,
```

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/generic_crud_ml.py` & `database-mysql-local-0.0.286/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/generic_mapping.py` & `database-mysql-local-0.0.286/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/point.py` & `database-mysql-local-0.0.286/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/polygon.py` & `database-mysql-local-0.0.286/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/table_definition.py` & `database-mysql-local-0.0.286/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/to_sql_interface.py` & `database-mysql-local-0.0.286/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local/src/utils.py` & `database-mysql-local-0.0.286/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/database_mysql_local.egg-info/PKG-INFO` & `database-mysql-local-0.0.286/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.285
+Version: 0.0.286
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database-mysql-local-0.0.285/database_mysql_local.egg-info/SOURCES.txt` & `database-mysql-local-0.0.286/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.285/pyproject.toml` & `database-mysql-local-0.0.286/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.285" # https://pypi.org/project/database-mysql-local
+version = "0.0.286" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database-mysql-local-0.0.285/setup.py` & `database-mysql-local-0.0.286/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.285',
+    version='0.0.286',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

