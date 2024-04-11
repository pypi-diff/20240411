# Comparing `tmp/molgenis-emx2-staging-migrator-10.50.1.tar.gz` & `tmp/molgenis_emx2_staging-migrator-8.213.11.dev1692184266583.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis-emx2-staging-migrator-10.50.1.tar", last modified: Wed Apr 10 11:56:58 2024, max compression
+gzip compressed data, was "molgenis_emx2_staging-migrator-8.213.11.dev1692184266583.tar", last modified: Wed Nov 15 15:09:13 2023, max compression
```

## Comparing `molgenis-emx2-staging-migrator-10.50.1.tar` & `molgenis_emx2_staging-migrator-8.213.11.dev1692184266583.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2024-04-10 11:56:58.554613 molgenis-emx2-staging-migrator-10.50.1/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1255 2024-04-10 11:56:58.553994 molgenis-emx2-staging-migrator-10.50.1/PKG-INFO
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      744 2024-04-04 09:18:46.000000 molgenis-emx2-staging-migrator-10.50.1/README.md
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      675 2024-04-04 09:18:46.000000 molgenis-emx2-staging-migrator-10.50.1/pyproject.toml
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       62 2024-04-10 07:14:00.000000 molgenis-emx2-staging-migrator-10.50.1/requirements.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       38 2024-04-10 11:56:58.554739 molgenis-emx2-staging-migrator-10.50.1/setup.cfg
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2024-04-10 11:56:58.546476 molgenis-emx2-staging-migrator-10.50.1/src/
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2024-04-10 11:56:58.550719 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       38 2024-04-04 09:18:46.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator/__init__.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       66 2024-04-04 09:18:46.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator/constants.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)    18872 2024-04-10 11:55:33.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator/migrator.py
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     7263 2024-04-04 09:54:04.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator/utils.py
-drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2024-04-10 11:56:58.553451 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator.egg-info/
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1255 2024-04-10 11:56:58.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator.egg-info/PKG-INFO
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      528 2024-04-10 11:56:58.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        1 2024-04-10 11:56:58.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       63 2024-04-10 11:56:58.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator.egg-info/requires.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       38 2024-04-10 11:56:58.000000 molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator.egg-info/top_level.txt
--rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        8 2024-04-10 11:56:47.000000 molgenis-emx2-staging-migrator-10.50.1/version.txt
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-11-15 15:09:13.291431 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1209 2023-11-15 15:09:13.290835 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/PKG-INFO
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      727 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/README.md
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      675 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/pyproject.toml
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       30 2023-11-15 15:08:21.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/requirements.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       38 2023-11-15 15:09:13.291565 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/setup.cfg
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-11-15 15:09:13.283259 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-11-15 15:09:13.287592 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     2074 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/SyncTables.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       95 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/__init__.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1005 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/__main__.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       73 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/constants.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      217 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/graphql_queries.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)    13313 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/migrator.py
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     8499 2023-11-15 15:07:28.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/utils.py
+drwxr-xr-x   0 ypezijlstramedgen   (501) staff       (20)        0 2023-11-15 15:09:13.290093 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator.egg-info/
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)     1209 2023-11-15 15:09:13.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)      678 2023-11-15 15:09:13.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)        1 2023-11-15 15:09:13.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       31 2023-11-15 15:09:13.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator.egg-info/requires.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       31 2023-11-15 15:09:13.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator.egg-info/top_level.txt
+-rw-r--r--   0 ypezijlstramedgen   (501) staff       (20)       26 2023-08-16 11:11:06.000000 molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/version.txt
```

### Comparing `molgenis-emx2-staging-migrator-10.50.1/PKG-INFO` & `molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-staging-migrator
-Version: 10.50.1
+Version: 8.213.11.dev1692184266583
 Summary: Python package for migrating Molgenis EMX2 staging areas to a catalogue.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: molgenis-emx2-pyclient>=10.48.9
 Requires-Dist: requests~=2.31.0
 Requires-Dist: pandas~=2.1.3
 
 # Installation
 
 ```console
-pip install molgenis-emx2-staging-migrator
+pip install molgenis_emx2_staging_migrator
 ```
 
 ## How to use
 
 Within your Python project import the class StagingMigrator and use it as a context manager
 
 ```py
 from molgenis_emx2_staging_migrator import StagingMigrator
 
-token = '...'
+username = 'username'
+password = '...'
 
-with StagingMigrator('https://example.molgeniscloud.org', token=token) as migrator:
+with StagingMigrator('https://example.molgeniscloud.org') as migrator:
+    migrator.signin(username, password)
 
     # Retrieve sign-in information
     print(migrator.status)
     
-    # Set the staging area and catalogue
-    migrator.set_staging_area('StagingExample')
+    migrator.set_staging_area('TestStaging')
     migrator.set_catalogue('catalogue')
     
-    # Execute the migration
     migrator.migrate()
     
 
 ```
 
 ## Development
 
 
-
+```
 
 ## Build
 
 ```console
 (venv) $ python -m build
 
-(venv) $ pip install dist/molgenis-emx2-staging_migrator*.whl
+(venv) $ pip install dist/molgenis_emx2_staging_migrator*.whl
 ```
```

### Comparing `molgenis-emx2-staging-migrator-10.50.1/README.md` & `molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # Installation
 
 ```console
-pip install molgenis-emx2-staging-migrator
+pip install molgenis_emx2_staging_migrator
 ```
 
 ## How to use
 
 Within your Python project import the class StagingMigrator and use it as a context manager
 
 ```py
 from molgenis_emx2_staging_migrator import StagingMigrator
 
-token = '...'
+username = 'username'
+password = '...'
 
-with StagingMigrator('https://example.molgeniscloud.org', token=token) as migrator:
+with StagingMigrator('https://example.molgeniscloud.org') as migrator:
+    migrator.signin(username, password)
 
     # Retrieve sign-in information
     print(migrator.status)
     
-    # Set the staging area and catalogue
-    migrator.set_staging_area('StagingExample')
+    migrator.set_staging_area('TestStaging')
     migrator.set_catalogue('catalogue')
     
-    # Execute the migration
     migrator.migrate()
     
 
 ```
 
 ## Development
 
 
-
+```
 
 ## Build
 
 ```console
 (venv) $ python -m build
 
-(venv) $ pip install dist/molgenis-emx2-staging_migrator*.whl
+(venv) $ pip install dist/molgenis_emx2_staging_migrator*.whl
 ```
```

### Comparing `molgenis-emx2-staging-migrator-10.50.1/pyproject.toml` & `molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
-requires = ["setuptools>=69.0"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "molgenis-emx2-staging-migrator"
+name = "molgenis_emx2_staging-migrator"
 description = "Python package for migrating Molgenis EMX2 staging areas to a catalogue."
 readme="README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator/migrator.py` & `molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/migrator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,381 +1,290 @@
 import logging
+import os
+import pathlib
 import time
 import zipfile
 from io import BytesIO
-from pathlib import Path
 from typing import TypeAlias, Literal
 
-from molgenis_emx2_pyclient import Client
-from molgenis_emx2_pyclient.exceptions import NoSuchSchemaException, NoSuchTableException
-from molgenis_emx2_pyclient.metadata import Schema, Table, Column
-from .constants import BASE_DIR
-from .utils import (find_cohort_references, construct_delete_variables, has_statement_of_consent,
-                    process_statement, prepare_pkey, query_columns_string)
+import pandas as pd
+from molgenis_emx2_pyclient.exceptions import NoSuchSchemaException
+
+from tools.pyclient.src.molgenis_emx2_pyclient import Client
+from tools.staging_migrator.src.molgenis_emx2_staging_migrator.constants import BASE_DIR
+from tools.staging_migrator.src.molgenis_emx2_staging_migrator.utils import get_cohort_ids, \
+    find_cohort_references, construct_delete_query, construct_delete_variables, has_statement_of_consent, \
+    process_statement, prepare_pkey
 
 log = logging.getLogger('Molgenis EMX2 Migrator')
 
 SchemaType: TypeAlias = Literal['source', 'target']
 
 
 class StagingMigrator(Client):
     """
     The StagingMigrator class is used to migrate updated data in a staging area to a catalogue.
     The class subclasses the Molgenis EMX2 Pyclient to access the API on the server
     """
 
-    def __init__(self, url: str,
-                 staging_area: str = None,
-                 catalogue: str = 'catalogue',
-                 table: str = 'Cohorts', token: str = None):
+    def __init__(self, url: str, staging_area: str = None, catalogue: str = 'catalogue'):
         """Sets up the StagingMigrator by logging in to the client."""
-        super().__init__(url=url, token=token)
+        super().__init__(url)
         self.staging_area = staging_area
         self.catalogue = catalogue
-        self.table = table
 
-    def __repr__(self):
-        class_name = type(self).__name__
-        args = [
-            f"staging_area={self.staging_area!r}",
-            f"catalogue={self.catalogue!r}",
-            f"table={self.table!r}"
-        ]
-        return f"{class_name}({', '.join(args)})"
+    def signin(self, username: str, password: str):
+        """Signs the user in to the server using the Client's signin method
+        and verifies the source schema and catalogue schema are on the server.
+        """
+        super().signin(username, password)
+        self._verify_schemas()
 
     def set_staging_area(self, staging_area: str):
         """Sets the staging area and verifies its existence."""
+        old_staging_area = self.staging_area
+
         self.staging_area = staging_area
-        self._verify_schemas()
+        try:
+            self._verify_schemas()
+        except NoSuchSchemaException:
+            self.staging_area = old_staging_area
 
     def set_catalogue(self, catalogue: str):
         """Sets the catalogue and verifies its existence."""
+        old_catalogue = self.catalogue
+
         self.catalogue = catalogue
-        self._verify_schemas()
+        try:
+            self._verify_schemas()
+        except NoSuchSchemaException:
+            self.catalogue = old_catalogue
 
-    def migrate(self, keep_zips: bool = False):
+    def migrate(self):
         """Performs the migration of the staging area to the catalogue."""
 
         # Download the target catalogue for upload in case of an error during execution
         self._download_schema_zip(schema=self.catalogue, schema_type='target', include_system_columns=False)
 
         # Delete the source tables from the target database
         log.info("Deleting staging area cohorts from the catalogue.")
         self._delete_staging_from_catalogue()
 
-        # Synchronize the organisations with SharedStaging
-        self.sync_shared_staging()
-
         # Create zipfile for uploading
         zip_stream = self._create_upload_zip()
 
         # Upload the zip to the target schema
         self._upload_zip_stream(zip_stream)
 
-        if not keep_zips:
-            # Remove any downloaded files from disk
-            self._cleanup()
+        # Remove any downloaded files from disk
+        self._cleanup()
 
     def _download_schema_zip(self, schema: str, schema_type: SchemaType,
                              include_system_columns: bool = True) -> str:
         """Download target schema as zip, save in case upload fails."""
-        filepath = BASE_DIR.joinpath(f"{schema_type}.zip")
-        if Path(filepath).exists():
-            Path(filepath).unlink()
-
+        filename = f"{BASE_DIR}/{schema_type}.zip"
+        if os.path.exists(filename):
+            os.remove(filename)
         api_zip_url = f"{self.url}/{schema}/api/zip"
         if include_system_columns:
             api_zip_url += '?includeSystemColumns=true'
-        resp = self.session.get(api_zip_url,
-                                headers={'x-molgenis-token': self.token},
-                                allow_redirects=True)
+        resp = self.session.get(api_zip_url, allow_redirects=True)
 
         if resp.content:
-            Path(filepath).write_bytes(resp.content)
-            log.debug(f"Downloaded {schema_type!r} schema to {filepath!s}.")
+            pathlib.Path(filename).write_bytes(resp.content)
+            log.debug(f"Downloaded '{schema_type}' schema to '{filename}'.")
         else:
             log.error("Error: download failed.")
-        return filepath
+        return filename
 
     def _delete_staging_from_catalogue(self):
         """
         Prepares the staging area by deleting data from tables
         that are later synchronized from the staging area.
         """
 
         # Gather the tables to delete from the target catalogue
-        tables_to_delete = find_cohort_references(self.get_schema_metadata(self.catalogue),
-                                                  self.catalogue, self.table)
+        tables_to_delete = find_cohort_references(self._schema_schema(self.catalogue))
 
-        cohort_ids = self._get_table_pkey_values()
-        metadata: Schema = self.get_schema_metadata(self.catalogue)
-        for table_name, ref_cols in tables_to_delete.items():
-            # Iterate over the tables that reference the core table of the staging area
-            # Check if any row matches this core table
-            table_meta = metadata.get_table(by='name', value=table_name)
-            table_id = table_meta.id
+        cohort_ids = get_cohort_ids(self.url, self.session, self.staging_area)
+        for table_name, ref_col in tables_to_delete.items():
+            # Iterate over the tables that reference the Cohorts table of the staging area
+            # Check if any row matches this Cohorts table
+            table_id = self._schema_schema(self.catalogue).get(table_name).get('id')
 
-            delete_rows = self._query_delete_rows(table_name, ref_cols, cohort_ids)
+            delete_rows = self._query_delete_rows(table_name, ref_col, cohort_ids)
 
             if len(delete_rows) == 0:
                 continue
             if not self._cohorts_in_ref_array(table_name):
-                log.debug(f"Deleting in table {table_name!r} row(s) with primary keys {delete_rows.get(table_id)}.")
+                log.debug(f"\nDeleting in table '{table_name}' row(s) with primary keys {delete_rows.get(table_id)}.")
 
                 # Delete the matching rows from the target catalogue table
                 self._delete_table_entries(table_id=table_id,
                                            pkeys=delete_rows.get(table_id))
             else:
-                log.debug(f"Updating row(s) with primary keys {delete_rows.get(table_id)}"
-                          f"\n in table {table_name}. (Not yet implemented)")
+                log.debug(f"\nUpdating row(s) with primary keys {delete_rows.get(table_id)}"
+                         f"\n in table {table_name}. (Not yet implemented)")
                 # TODO: implement following
                 # self._delete_from_ref_array(schema=catalogue, table_id=table_schema['id'],
                 #                             pkeys=response.json().get('data').get(table_schema['id']))
 
-    def sync_shared_staging(self):
-        """Synchronizes the records in the SharedStaging schema that are referenced
-        from the staging area with the relevant records in the catalogue.
-        """
-        staging_schema = self.get_schema_metadata(self.staging_area)
-        # Collect the tables in which a column references a table in the SharedStaging schema
-        ss_ref_tables: list[Table] = [_t for _t in staging_schema.get_tables(by='schemaName', value=self.staging_area)
-                                      if len(_t.get_columns(by='refSchemaName', value='SharedStaging'))]
-        if len(ss_ref_tables) == 0:
-            return
-
-        organisations = set()
-        for table in ss_ref_tables:
-            ref_cols: list[Column] = table.get_columns(by='refSchemaName', value='SharedStaging')
-            ref_col_strs = [f"{rc.id} {{\n      id\n    }}" for rc in ref_cols]
-            query = """{{\n  {} {{\n    {}\n  }}\n}}""".format(
-                table.id, "    \n    ".join(ref_col_strs))
-            response = self.session.post(url=f"{self.url}/{self.staging_area}/graphql",
-                                         json={"query": query},
-                                         headers={'x-molgenis-token': self.token})
-            data_response = response.json().get('data')
-            if len(data_response) > 0:
-                for record in data_response.values():
-                    for column in list(record[0].values()):
-                        if len(column) == 0:
-                            continue
-                        for entry in column[0].values():
-                            organisations.add(entry)
-        organisations = list(organisations)
-        if len(organisations) < 1:
-            return
-        # TODO combine the ids of Organisations in the responses
-        shared_schema = self.get_schema_metadata('SharedStaging')
-        search_query = self.__construct_pkey_query(shared_schema, 'Organisations', all_columns=True)
-        search_variables = construct_delete_variables(shared_schema, organisations, 'Organisations', 'id')
-        search_response = self.session.post(url=f"{self.url}/SharedStaging/graphql",
-                                            json={"query": search_query, "variables": search_variables},
-                                            headers={'x-molgenis-token': self.token})
-
-        mutation_query = "mutation insert($value: [OrganisationsInput]){insert(Organisations:$value){message}}"
-        for org in search_response.json().get('data').get('Organisations'):
-            mutation_variables = {"value": org}
-
-            mutation_response = self.session.post(url=f"{self.url}/{self.catalogue}/graphql",
-                                                  json={"query": mutation_query, "variables": mutation_variables},
-                                                  headers={'x-molgenis-token': self.token})
-
-            if mutation_response.status_code != 200:
-                if f"Key (id)=({org.get('id')}) already exists." in mutation_response.text:
-                    log.debug(f"Organisation {org.get('id')!r} already present.")
-                else:
-                    log.error(f"Unable to synchronize {org.get('id')!r} to {self.catalogue!r}.")
-            else:
-                log.debug(f"Successfully migrated organisation {org.get('id')!r} to {self.catalogue!r}.")
-
-    def _query_delete_rows(self, table_name: str, ref_cols: str | list,
+    def _query_delete_rows(self, table_name: str, ref_col: str,
                            cohort_ids: list) -> dict:
         """Queries the rows to be deleted from a table."""
-        schema_meta: Schema = self.get_schema_metadata(self.catalogue)
-        query = self.__construct_pkey_query(schema_meta, table_name)
-        variables = construct_delete_variables(self.get_schema_metadata(self.catalogue),
-                                               cohort_ids, table_name, ref_cols)
+        query = construct_delete_query(self._schema_schema(self.catalogue), table_name)
+        variables = construct_delete_variables(self._schema_schema(self.catalogue), cohort_ids, table_name, ref_col)
 
         response = self.session.post(url=f"{self.url}/{self.catalogue}/graphql",
-                                     json={"query": query, "variables": variables},
-                                     headers={'x-molgenis-token': self.token})
-
-        data = response.json().get('data')
-        if data is None:
-            data = {}
-        return data
+                                     json={"query": query, "variables": variables})
+        return response.json().get('data')
 
     def _delete_table_entries(self, table_id: str, pkeys: list):
         """Deletes the rows marked by the primary keys from the table."""
         query = (f"mutation delete($pkey:[{table_id}Input]) {{\n"
                  f"  delete({table_id}:$pkey) {{message}}\n"
                  f"}}")
 
         batch_size = 1000
         for _batch in range(0, len(pkeys), batch_size):
             variables = {'pkey': pkeys[_batch:_batch + batch_size]}
             response = self.session.post(
                 url=f"{self.url}/{self.catalogue}/graphql",
-                json={"query": query, "variables": variables},
-                headers={'x-molgenis-token': self.token}
+                json={"query": query, "variables": variables}
             )
             if response.status_code != 200:
                 log.error(response)
                 log.error(f"Deleting entries from table {table_id} failed.")
-            else:
-                log.info(response.json().get('data').get('delete').get('message'))
 
-    def _cohorts_in_ref_array(self, _table_name: str) -> bool:
+    def _cohorts_in_ref_array(self, _table: str) -> bool:
         """Returns True if cohorts are referenced in a referenced array in any column in this table."""
-        try:
-            _table_schema: Table = self.get_schema_metadata(self.catalogue).get_table(by='name', value=_table_name)
-        except ValueError:
-            raise NoSuchTableException(f"No table {_table_name!r} in schema {self.catalogue!r}.")
-        return len(_table_schema.get_columns(by=['columnType', 'refTable'], value=['REF_ARRAY', self.table])) > 0
+        _table_schema = self._schema_schema(self.catalogue)[_table]
+        return (len([col for col in _table_schema['columns']
+                     if ((col.get('columnType') == 'REF_ARRAY') & (col.get('refTable') == 'Cohorts'))]) > 0)
 
     def _verify_schemas(self):
         """Ensures the staging area and catalogue are available."""
         if self.staging_area is not None:
-            if self.staging_area not in self.schema_names:
-                raise NoSuchSchemaException(f"Schema {self.staging_area!r} not found on server."
-                                            f" Available schemas: {', '.join(self.schema_names)}.")
-        if self.catalogue not in self.schema_names:
-            raise NoSuchSchemaException(f"Schema {self.catalogue!r} not found on server."
-                                        f" Available schemas: {', '.join(self.schema_names)}.")
+            if self.staging_area not in self.schemas:
+                raise NoSuchSchemaException(f"Schema '{self.staging_area}' not found on server."
+                                            f" Available schemas: {', '.join(self.schemas)}.")
+        if self.catalogue not in self.schemas:
+            raise NoSuchSchemaException(f"Schema '{self.catalogue}' not found on server."
+                                        f" Available schemas: {', '.join(self.schemas)}.")
 
     def _create_upload_zip(self) -> BytesIO:
         """Combines the relevant tables of the staging area into a zipfile."""
-        tables_to_sync = find_cohort_references(self.get_schema_metadata(self.staging_area),
-                                                self.staging_area, self.table)
+        tables_to_sync = find_cohort_references(self._schema_schema(self.staging_area))
 
         source_file_path = self._download_schema_zip(schema=self.staging_area, schema_type='source',
                                                      include_system_columns=False)
 
         upload_stream = BytesIO()
 
         with (zipfile.ZipFile(source_file_path, 'r') as source_archive,
               zipfile.ZipFile(upload_stream, 'w', zipfile.ZIP_DEFLATED, False) as upload_archive):
             for file_name in source_archive.namelist():
                 if '_files/' in file_name:
                     upload_archive.writestr(file_name, BytesIO(source_archive.read(file_name)).getvalue())
                     continue
-                elif (table_name := Path(file_name).stem) not in tables_to_sync.keys():
+                elif (table_name := os.path.splitext(file_name)[0]) not in tables_to_sync.keys():
                     continue
 
                 _table = source_archive.read(file_name)
-                if consent_val := has_statement_of_consent(table_name, self.get_schema_metadata(self.staging_area)):
+                if consent_val := has_statement_of_consent(table_name, self._schema_schema(self.staging_area)):
                     _table = process_statement(table=_table, consent_val=consent_val)
+                # self._check_diff(file_name, _table)
                 upload_archive.writestr(file_name, BytesIO(_table).getvalue())
 
         log.info(f"Migrating tables {', '.join(tables_to_sync.keys())}.")
         return upload_stream
 
     def _upload_zip_stream(self, zip_stream: BytesIO, is_fallback: bool = False):
         """Uploads the zip file containing the tables from the staging area
         to the catalogue.
         """
         upload_url = f"{self.url}/{self.catalogue}/api/zip?async=true"
 
         response = self.session.post(
             url=upload_url,
-            files={'file': (f"{BASE_DIR}/upload.zip", zip_stream.getvalue())},
-            headers={'x-molgenis-token': self.token}
+            files={'file': (f'{BASE_DIR}/upload.zip', zip_stream.getvalue())}
         )
 
         response_status = response.status_code
         if response.status_code != 200:
             log.error(f"Migration failed with error {response_status}:\n{str(response.text)}")
             log.error("Uploading fallback zip.")
             self._upload_fallback_zip()
         else:
             response_url = f"{self.url}{response.json().get('url')}"
-            upload_status = self.session.get(response_url,
-                                             headers={'x-molgenis-token': self.token}).json().get('status')
+            upload_status = self.session.get(response_url).json().get('status')
             while upload_status == 'RUNNING':
                 time.sleep(2)
-                upload_status = self.session.get(response_url,
-                                                 headers={'x-molgenis-token': self.token}).json().get('status')
-            upload_description = self.session.get(response_url,
-                                                  headers={'x-molgenis-token': self.token}).json().get('description')
+                upload_status = self.session.get(response_url).json().get('status')
+            upload_description = self.session.get(response_url).json().get('description')
 
             if upload_status == 'ERROR':
                 log.error(f"Migration failed, reason: {upload_description}.")
-                log.debug(self.session.get(response_url, headers={'x-molgenis-token': self.token}).json())
+                log.debug(self.session.get(response_url).json())
                 if not is_fallback:
                     log.info("Uploading fallback zip.")
                     self._upload_fallback_zip()
                 else:
                     log.error("Restoring fallback zip failed.")
             else:
                 if is_fallback:
                     log.info("Fallback zip restored successfully.")
                 else:
                     log.info("Migrated successfully.")
 
+    @staticmethod
+    def _cleanup():
+        """Deletes the downloaded files after successful migration."""
+        zip_files = ['target.zip', 'source.zip', 'upload.zip']
+        for zp in zip_files:
+            filename = f"{BASE_DIR}/{zp}"
+            if os.path.exists(filename):
+                log.debug(f"Deleting file '{zp}'.")
+                os.remove(filename)
+
+    def _check_diff(self, file_name: str, source_table: bytes):
+        """Logs an overview of differences on this table compared to the table on the server."""
+        with zipfile.ZipFile(f"{BASE_DIR}/target.zip", 'r') as target_archive:
+            try:
+                target_table = target_archive.read(file_name)
+            except Exception as e:
+                print(e)
+
+        # Convert csv files to pandas DataFrame
+        source_df = pd.read_csv(BytesIO(source_table))
+        target_df = pd.read_csv(BytesIO(target_table))
+
+        if not (len(source_df) + len(target_df)):
+            return
+
+        # Get primary keys for these tables
+        p_keys = prepare_pkey(schema=self._schema_schema(self.staging_area), table_name=os.path.splitext(file_name)[0])
+
+        source_df[p_keys] = source_df[p_keys].astype(str)
+        target_df[p_keys] = target_df[p_keys].astype(str)
+
+        # Filter target_table on primary keys that are the same as the ones in the source_table
+        # target_df = target_df.loc[target_df == source_df]
+        merge = pd.merge(source_df, target_df, on=p_keys)
+        if len(merge):
+            print(merge)
+        # Output in case row exists in source but not target
+
+        # Output in case row exists in target but not source
+        # Output in case all rows are the same
+
     def _upload_fallback_zip(self):
         """Restores the catalogue to the state before deletion by uploading the downloaded target zip."""
         target_filename = f"{BASE_DIR}/target.zip"
         upload_stream = BytesIO()
         # Load the target.zip file as a stream
         with (zipfile.ZipFile(target_filename, 'r') as target_archive,
               zipfile.ZipFile(upload_stream, 'w', zipfile.ZIP_DEFLATED) as upload_archive):
             for file_name in target_archive.namelist():
-                if not file_name.startswith('molgenis'):
-                    upload_archive.writestr(file_name, BytesIO(target_archive.read(file_name)).getvalue())
+                upload_archive.writestr(file_name, BytesIO(target_archive.read(file_name)).getvalue())
         # Upload the stream
         self._upload_zip_stream(upload_stream, is_fallback=True)
-
-    def _get_table_pkey_values(self):
-        """Fetches the primary key values associated with the staging area's table."""
-
-        # Query server for cohort id
-        query = """{{\n  {} {{\n    id\n    name\n  }}\n}}""".format(self.table)
-        staging_url = f"{self.url}/{self.staging_area}/graphql"
-        response = self.session.post(url=staging_url,
-                                     headers={'x-molgenis-token': self.token},
-                                     json={"query": query})
-        response_data = response.json().get('data')
-        if response_data is None:
-            # Raise new error
-            raise NoSuchTableException(f"Table {self.table!r} not found on schema {self.staging_area!r}.")
-
-        # Return only if there is exactly one id/cohort in the Cohorts table
-        if self.table in response_data.keys():
-            if len(response_data[self.table]) < 1:
-                raise ValueError(
-                    f"Expected a value in table {self.table!r} in staging area {self.staging_area!r}"
-                    f" but found {len(response_data[self.table])!r}"
-                )
-        else:
-            raise ValueError(
-                f"Expected a value in table {self.table!r} in staging area {self.staging_area!r}"
-                f" but found none."
-            )
-
-        return [cohort['id'] for cohort in response_data[self.table]]
-
-    @staticmethod
-    def _cleanup():
-        """Deletes the downloaded files after successful migration."""
-        zip_files = ['target.zip', 'source.zip', 'upload.zip']
-        for zp in zip_files:
-            filename = f"{BASE_DIR}/{zp}"
-            if Path(filename).exists():
-                log.debug(f"Deleting file {zp!r}.")
-                Path(filename).unlink()
-
-    @staticmethod
-    def __construct_pkey_query(db_schema: Schema, table_name: str, all_columns: bool = False):
-        """Constructs a GraphQL query for finding the primary key values in a table."""
-        table_schema: Table = db_schema.get_table(by='name', value=table_name)
-        if all_columns:
-            pkeys = [prepare_pkey(db_schema, table_name, col.id) for col in table_schema.columns]
-            pkeys = [pk for pk in pkeys if pk is not None]
-        else:
-            pkeys = [prepare_pkey(db_schema, table_name, col.id) for col in table_schema.get_columns(by='key', value=1)]
-        table_id = table_schema.id
-        pkeys_print = query_columns_string(pkeys, indent=4)
-        _query = (f"query {table_id}($filter: {table_id}Filter) {{\n"
-                  f"  {table_id}(filter: $filter) {{\n"
-                  f"{pkeys_print}\n"
-                  f"  }}\n"
-                  f"}}")
-        return _query
```

### Comparing `molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator/utils.py` & `molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,47 +2,68 @@
 Utility functions for the StagingMigrator class.
 """
 import logging
 from io import BytesIO
 
 import pandas as pd
 
-from molgenis_emx2_pyclient.exceptions import NoSuchTableException
-from molgenis_emx2_pyclient.metadata import Schema, Table, Column
+from tools.pyclient.src.molgenis_emx2_pyclient.exceptions import IncorrectSchemaError
+from tools.staging_migrator.src.molgenis_emx2_staging_migrator.graphql_queries import Queries
 
 log = logging.getLogger(__name__)
 
 
-def prepare_pkey(schema: Schema, table_name: str, col_id: str | list = None) -> str | list | dict | None:
+def get_cohort_ids(server_url, session, staging_area) -> list | None:
+    """Fetches the id associated with the staging area's cohort."""
+
+    # Query server for cohort id
+    query = Queries.Cohorts
+    staging_url = f"{server_url}/{staging_area}/graphql"
+    response = session.post(url=staging_url,
+                            json={"query": query})
+    response_data = response.json().get('data')
+    if response_data is None:
+        # Raise new error
+        raise IncorrectSchemaError(f"Table 'Cohorts' not found on schema '{staging_area}'.")
+
+    # Return only if there is exactly one id/cohort in the Cohorts table
+    if "Cohorts" in response_data.keys():
+        if len(response_data['Cohorts']) < 1:
+            log.warning(
+                f'Expected a cohort in staging area "{staging_area}"'
+                f' but found {len(response_data["Cohorts"])}')
+            return None
+    else:
+        log.warning(
+            f'Expected a single cohort in staging area "{staging_area}"'
+            f' but found none.')
+        return None
+
+    return [cohort['id'] for cohort in response_data['Cohorts']]
+
+
+def prepare_pkey(schema: dict, table_name: str, col_id: str | list = None) -> str | list | dict | None:
     """Prepares a primary key by adding a reference to a table if necessary."""
-    try:
-        table_schema: Table = schema.get_table(by='name', value=table_name)
-    except ValueError:
-        raise NoSuchTableException(f"{table_name!r} not found in schema.")
     if not col_id:
         # Return the primary keys of a table if no column name is specified
-        return list(map(lambda col: col.id, table_schema.get_columns(by='key', value=1)))
-    if isinstance(col_id, list):
-        return {_col_id: prepare_pkey(schema, table_name, _col_id)[_col_id] for _col_id in col_id}
-    if isinstance(col_id, dict):
-        return [*prepare_pkey(schema, table_name),
-                *[{key: prepare_pkey(schema, value)} for (key, value) in col_id.items()]]
-
-    col_data: Column = table_schema.get_column(by='id', value=col_id)
+        return [col['id'] for col in schema[table_name]['columns'] if col.get('key') == 1]
+    col_data, = [col for col in schema[table_name]['columns'] if col['id'] == col_id]
     if col_id.startswith('mg_'):
         return None
     if col_data.get('columnType') == 'HEADING':
         return None
     elif col_data.get('columnType') == 'REFBACK':
         return None
     elif col_data.get('columnType') in ['ONTOLOGY', 'ONTOLOGY_ARRAY']:
-        return {col_id: 'name'}
+        ont_keys = prepare_pkey(schema, col_data.get('refTable'))
+        ont_cols = [prepare_pkey(schema, col_data['refTable'], ok) for ok in ont_keys]
+        return {col_id: ont_cols}
     elif col_data.get('columnType') in ['REF', 'REF_ARRAY']:
-        ref_keys = prepare_pkey(schema, col_data.get('refTableName'))
-        ref_cols = [prepare_pkey(schema, col_data.get('refTableName'), rk) for rk in ref_keys]
+        ref_keys = prepare_pkey(schema, col_data.get('refTable'))
+        ref_cols = [prepare_pkey(schema, col_data['refTable'], rk) for rk in ref_keys]
         return {col_id: ref_cols}
     elif col_data.get('columnType') == 'FILE':
         return {col_id: 'id'}
     else:
         return col_id
 
 
@@ -59,108 +80,113 @@
         vals = list(column.values())[0]
         return_val = (f"{indent * ' '}{col} {{\n"
                       f"{query_columns_string(vals, indent=indent + 2)}\n"
                       f"{indent * ' '}}}")
         return return_val
 
 
-def find_cohort_references(schema_schema: Schema, schema_name: str, base_table: str) -> dict:
+def find_cohort_references(schema_schema: dict) -> dict:
     """Finds the references in the target catalogue to the Cohorts table.
     References may be direct or indirect, such as the 'Subcohort counts' table
     that references the 'Subcohorts' table, which references the 'Cohorts' table directly.
     """
 
-    inheritance = {}
-    table_name = base_table
-    inherit = schema_schema.get_table(by='name', value=table_name).get('inheritName')
-    inheritance.update({table_name: inherit})
-    while inherit is not None:
-        table_name = inherit
-        inherit = schema_schema.get_table(by='name', value=str(table_name)).get('inheritName')
-        inheritance.update({table_name: inherit})
-
-    backward_refs = {
-        tab.name: [c.id for c in tab.get_columns(by='refSchemaName', value=schema_name)
-                   if c.get('refTableName') in inheritance.keys() and c.get('columnType') != 'REFBACK']
-        for tab in schema_schema.get_tables(by='schemaName', value=schema_name)
-    }
-    backward_refs[base_table] = 'id'
-
-    table_references = {
-        tab.name: {c.id: c.get('refTableName')
-                   for c in [*tab.get_columns(by=['columnType', 'refSchemaName'], value=['REF', schema_name]),
-                             *tab.get_columns(by=['columnType', 'refSchemaName'], value=['REF_ARRAY', schema_name])]}
-        for tab in schema_schema.get_tables(by='schemaName', value=schema_name)
-    }
+    def find_table_columns(_t_name: str, _t_values: dict):
+        _table_references = []
+        for _column in _t_values['columns']:
+            if _column.get('columnType') in ['REF', 'REF_ARRAY']:
+                if _column.get('refTable') in ['Cohorts', *cohort_inheritance.values()]:
+                    _table_references.append(_column['id'])
+                elif _column.get('refTable') != _t_name:
+                    _column_references = find_table_columns(_column['refTable'], schema_schema[_column['refTable']])
+                    if len(_column_references) > 0:
+                        _table_references.append(_column['id'])
+        return _table_references
+
+    cohort_inheritance = {'Cohorts': 'Data resources', 'Data resources': 'Extended resources',
+                          'Extended resources': 'Resources'}
+    cohort_references = dict()
+    for t_name, t_values in schema_schema.items():
+        if t_name in cohort_inheritance.keys():
+            table_references = ['id']
+        else:
+            table_references = find_table_columns(t_name, t_values)
+        if len(table_references) > 0:
+            cohort_references.update({t_name: table_references[0]})
 
     # Gather all backwards references to the tables
-    ref_backs = {}
-    for tab in table_references.keys():
-        ref_backs[tab] = []
-        for _tab in table_references.keys():
-            if tab == _tab:
-                continue
-            if tab in table_references[_tab].values():
-                ref_backs[tab].append(_tab)
-
-    for coh, inh in inheritance.items():
+    ref_backs = {
+        tab: [_tab for _tab in cohort_references.keys()
+              if len([_col for _col in schema_schema[_tab]['columns']
+                      if (_col.get('columnType') in ['REF', 'REF_ARRAY']) & (_col.get('refTable') == tab)]) > 0]
+        for tab in cohort_references.keys()
+    }
+    for coh, inh in cohort_inheritance.items():
         if coh in ref_backs.keys():
             ref_backs[coh].append(inh)
         else:
             ref_backs[coh] = [inh]
 
     def pop_dict(key):
         ref_backs.pop(key)
         return key
 
-    table_names = [_t.name for _t in schema_schema.tables]
-    other_tabs = [key for key in table_names if key not in ref_backs.keys()]
+    other_tabs = [key for key in schema_schema.keys() if key not in ref_backs.keys()]
     sequence = [pop_dict(tab) for (tab, refs) in ref_backs.copy().items() if len(refs) == 0]
     while len(ref_backs) > 0:
         for tab, refs in ref_backs.copy().items():
-            if all(map(lambda ref: ref in [*sequence, *other_tabs, None], refs)):
+            if all((ref in [*sequence, *other_tabs]) for ref in refs):
                 sequence.append(pop_dict(tab))
 
-    backward_refs = {s: backward_refs.copy()[s] for s in sequence if len(backward_refs.copy()[s])}
+    cohort_references = {s: cohort_references.copy()[s] for s in sequence}
+
+    return cohort_references
 
-    return backward_refs
+
+def construct_delete_query(db_schema: dict, table_name: str, all_columns: bool = False):
+    """Constructs a GraphQL query for deleting rows from a table."""
+    if all_columns:
+        pkeys = [prepare_pkey(db_schema, table_name, col['id']) for col in db_schema[table_name]['columns']]
+        pkeys = [pk for pk in pkeys if pk is not None]
+    else:
+        pkeys = [prepare_pkey(db_schema, table_name, col['id']) for col in db_schema[table_name]['columns'] if
+                 col.get('key') == 1]
+    table_id = db_schema[table_name]['id']
+    pkeys_print = query_columns_string(pkeys, indent=4)
+    _query = (f"query {table_id}($filter: {table_id}Filter) {{\n"
+              f"  {table_id}(filter: $filter) {{\n"
+              f"{pkeys_print}\n"
+              f"  }}\n"
+              f"}}")
+    return _query
 
 
-def construct_delete_variables(db_schema: Schema, cohort_ids: list, table_name: str, ref_col: str):
+def construct_delete_variables(db_schema: dict, cohort_ids: list, table_name: str, ref_col: str):
     """Constructs a variables filter for querying the GraphQL table on the desired column values."""
     pkeys = prepare_pkey(db_schema, table_name, ref_col)
-    # pkeys = [prepare_pkey(db_schema, table_name, col.id) for col in table_schema.get_columns(by='key', value=1)]
 
-    def prepare_key_part(_pkey: str | dict | list):
+    def prepare_key_part(_pkey: str | dict):
         if isinstance(_pkey, str):
             return {"equals": [{_pkey: _id} for _id in cohort_ids]}
         if isinstance(_pkey, dict):
             _key, _val = list(_pkey.items())[0]
-            for _key, _val in _pkey.items():
-                pass
             return {_key: prepare_key_part(_val[0])}
-        if isinstance(_pkey, list):
-            pass
 
     variables = {"filter": prepare_key_part(pkeys)}
 
     return variables
 
 
-def has_statement_of_consent(table_name: str, schema: Schema) -> int:
+def has_statement_of_consent(table_name: str, schema: dict) -> int:
     """Checks whether this table has a column that asks for a statement of consent."""
     consent_cols = ['statement of consent personal data',
                     'statement of consent email']
-    try:
-        table_schema = schema.get_table(by='name', value=table_name)
-    except ValueError:
-        raise NoSuchTableException(f"Table {table_name!r} not in schema.")
-    col_names = map(str, table_schema.columns)
+    col_names = [_col['name'] for _col in schema[table_name]['columns']]
 
-    return 1 * (consent_cols[0] in col_names) + 2 * (consent_cols[1] in col_names)
+    return 1*(consent_cols[0] in col_names) + 2*(consent_cols[1] in col_names)
 
 
 def process_statement(table: bytes, consent_val: int) -> bytes:
     """Processes any statement of consent by modifying the rows in the table for which no consent is given."""
     df = pd.read_csv(BytesIO(table))
 
     # Remove rows without any data consent
```

### Comparing `molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator.egg-info/PKG-INFO` & `molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 Metadata-Version: 2.1
-Name: molgenis-emx2-staging-migrator
-Version: 10.50.1
+Name: molgenis_emx2_staging-migrator
+Version: 8.213.11.dev1692184266583
 Summary: Python package for migrating Molgenis EMX2 staging areas to a catalogue.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: molgenis-emx2-pyclient>=10.48.9
 Requires-Dist: requests~=2.31.0
 Requires-Dist: pandas~=2.1.3
 
 # Installation
 
 ```console
-pip install molgenis-emx2-staging-migrator
+pip install molgenis_emx2_staging_migrator
 ```
 
 ## How to use
 
 Within your Python project import the class StagingMigrator and use it as a context manager
 
 ```py
 from molgenis_emx2_staging_migrator import StagingMigrator
 
-token = '...'
+username = 'username'
+password = '...'
 
-with StagingMigrator('https://example.molgeniscloud.org', token=token) as migrator:
+with StagingMigrator('https://example.molgeniscloud.org') as migrator:
+    migrator.signin(username, password)
 
     # Retrieve sign-in information
     print(migrator.status)
     
-    # Set the staging area and catalogue
-    migrator.set_staging_area('StagingExample')
+    migrator.set_staging_area('TestStaging')
     migrator.set_catalogue('catalogue')
     
-    # Execute the migration
     migrator.migrate()
     
 
 ```
 
 ## Development
 
 
-
+```
 
 ## Build
 
 ```console
 (venv) $ python -m build
 
-(venv) $ pip install dist/molgenis-emx2-staging_migrator*.whl
+(venv) $ pip install dist/molgenis_emx2_staging_migrator*.whl
 ```
```

### Comparing `molgenis-emx2-staging-migrator-10.50.1/src/molgenis_emx2_staging_migrator.egg-info/SOURCES.txt` & `molgenis_emx2_staging-migrator-8.213.11.dev1692184266583/src/molgenis_emx2_staging_migrator.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 README.md
 pyproject.toml
 requirements.txt
 version.txt
+src/molgenis_emx2_staging_migrator/SyncTables.py
 src/molgenis_emx2_staging_migrator/__init__.py
+src/molgenis_emx2_staging_migrator/__main__.py
 src/molgenis_emx2_staging_migrator/constants.py
+src/molgenis_emx2_staging_migrator/graphql_queries.py
 src/molgenis_emx2_staging_migrator/migrator.py
 src/molgenis_emx2_staging_migrator/utils.py
 src/molgenis_emx2_staging_migrator.egg-info/PKG-INFO
 src/molgenis_emx2_staging_migrator.egg-info/SOURCES.txt
 src/molgenis_emx2_staging_migrator.egg-info/dependency_links.txt
 src/molgenis_emx2_staging_migrator.egg-info/requires.txt
 src/molgenis_emx2_staging_migrator.egg-info/top_level.txt
```

