# Comparing `tmp/airflow_tools-0.8.2.tar.gz` & `tmp/airflow_tools-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_tools-0.8.2.tar", max compression
+gzip compressed data, was "airflow_tools-0.8.4.tar", max compression
```

## Comparing `airflow_tools-0.8.2.tar` & `airflow_tools-0.8.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0    11358 2024-02-26 10:29:12.681236 airflow_tools-0.8.2/LICENSE.txt
--rw-r--r--   0        0        0     8788 2024-04-03 08:24:08.137208 airflow_tools-0.8.2/README.md
--rw-r--r--   0        0        0     1312 2024-04-04 14:12:08.276028 airflow_tools-0.8.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/__init__.py
--rw-r--r--   0        0        0       22 2024-04-04 14:12:08.276028 airflow_tools-0.8.2/src/airflow_tools/_version.py
--rw-r--r--   0        0        0     1794 2024-01-18 10:00:14.774290 airflow_tools-0.8.2/src/airflow_tools/compression_utils.py
--rw-r--r--   0        0        0     4426 2024-04-03 08:24:08.197207 airflow_tools-0.8.2/src/airflow_tools/data_lake_facade.py
--rw-r--r--   0        0        0      115 2024-01-03 14:54:38.107397 airflow_tools-0.8.2/src/airflow_tools/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.701235 airflow_tools-0.8.2/src/airflow_tools/filesystems/__init__.py
--rw-r--r--   0        0        0     2298 2024-03-20 11:42:50.252535 airflow_tools-0.8.2/src/airflow_tools/filesystems/filesystem_factory.py
--rw-r--r--   0        0        0      561 2024-04-03 08:24:08.209207 airflow_tools-0.8.2/src/airflow_tools/filesystems/filesystem_protocol.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.713235 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/__init__.py
--rw-r--r--   0        0        0     2382 2024-04-04 11:13:41.968166 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
--rw-r--r--   0        0        0     1974 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
--rw-r--r--   0        0        0     2472 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
--rw-r--r--   0        0        0     1586 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/local_filesystem.py
--rw-r--r--   0        0        0     2185 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/s3_filesystem.py
--rw-r--r--   0        0        0     1396 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/sftp_filesystem.py
--rw-r--r--   0        0        0     3877 2024-02-26 10:29:12.737235 airflow_tools-0.8.2/src/airflow_tools/notifications/slack/webhook.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.2/src/airflow_tools/providers/azure/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 11:42:50.252535 airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/__init__.py
--rw-r--r--   0        0        0     3396 2024-03-20 11:42:50.252535 airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/azure_databricks.py
--rw-r--r--   0        0        0     1619 2024-03-20 11:42:50.268535 airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/azure_file_share.py
--rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.2/src/airflow_tools/providers/data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-01-18 10:00:14.774290 airflow_tools-0.8.2/src/airflow_tools/providers/data_lake/operators/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-03 08:24:08.213207 airflow_tools-0.8.2/src/airflow_tools/providers/data_lake/operators/data_lake.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 10:29:12.737235 airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/__init__.py
--rw-r--r--   0        0        0     5437 2024-04-03 08:24:08.225207 airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/filesystem.py
--rw-r--r--   0        0        0     9802 2024-04-04 14:12:08.276028 airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/providers/http_to_data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
--rw-r--r--   0        0        0     9037 2024-04-03 08:24:08.257207 airflow_tools-0.8.2/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
--rw-r--r--   0        0        0     1108 2024-03-20 11:42:50.268535 airflow_tools-0.8.2/src/airflow_tools/providers/package.py
--rw-r--r--   0        0        0        0 2024-01-02 17:33:48.422489 airflow_tools-0.8.2/src/airflow_tools/py.typed
--rw-r--r--   0        0        0    10026 1970-01-01 00:00:00.000000 airflow_tools-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-15 09:01:15.875283 airflow_tools-0.8.4/LICENSE.txt
+-rw-r--r--   0        0        0     8788 2024-04-11 13:00:04.903032 airflow_tools-0.8.4/README.md
+-rw-r--r--   0        0        0     1312 2024-04-11 13:41:40.775249 airflow_tools-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.879171 airflow_tools-0.8.4/src/airflow_tools/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-11 13:41:49.632435 airflow_tools-0.8.4/src/airflow_tools/_version.py
+-rw-r--r--   0        0        0     1794 2024-03-15 09:01:15.879695 airflow_tools-0.8.4/src/airflow_tools/compression_utils.py
+-rw-r--r--   0        0        0     4426 2024-03-23 22:52:20.616265 airflow_tools-0.8.4/src/airflow_tools/data_lake_facade.py
+-rw-r--r--   0        0        0      115 2024-03-15 09:01:15.880246 airflow_tools-0.8.4/src/airflow_tools/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.880736 airflow_tools-0.8.4/src/airflow_tools/filesystems/__init__.py
+-rw-r--r--   0        0        0     2298 2024-03-15 14:21:53.853567 airflow_tools-0.8.4/src/airflow_tools/filesystems/filesystem_factory.py
+-rw-r--r--   0        0        0      561 2024-03-23 23:14:28.037837 airflow_tools-0.8.4/src/airflow_tools/filesystems/filesystem_protocol.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.882284 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/__init__.py
+-rw-r--r--   0        0        0     2382 2024-04-11 13:00:04.951649 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
+-rw-r--r--   0        0        0     1974 2024-03-24 00:50:06.290603 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
+-rw-r--r--   0        0        0     2472 2024-03-25 16:17:00.235954 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
+-rw-r--r--   0        0        0     1586 2024-03-24 00:21:54.773711 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/local_filesystem.py
+-rw-r--r--   0        0        0     2185 2024-03-24 00:50:06.294839 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/s3_filesystem.py
+-rw-r--r--   0        0        0     1396 2024-03-24 00:21:54.788482 airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/sftp_filesystem.py
+-rw-r--r--   0        0        0     3877 2024-03-15 09:01:15.884092 airflow_tools-0.8.4/src/airflow_tools/notifications/slack/webhook.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884537 airflow_tools-0.8.4/src/airflow_tools/providers/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884904 airflow_tools-0.8.4/src/airflow_tools/providers/azure/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.885232 airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/__init__.py
+-rw-r--r--   0        0        0     3396 2024-03-18 14:38:56.888663 airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/azure_databricks.py
+-rw-r--r--   0        0        0     1619 2024-03-15 09:01:15.885704 airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/azure_file_share.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886187 airflow_tools-0.8.4/src/airflow_tools/providers/data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886773 airflow_tools-0.8.4/src/airflow_tools/providers/data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     2355 2024-03-23 22:52:20.625836 airflow_tools-0.8.4/src/airflow_tools/providers/data_lake/operators/data_lake.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.887444 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.888053 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/__init__.py
+-rw-r--r--   0        0        0     6241 2024-04-11 13:40:29.952773 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/filesystem.py
+-rw-r--r--   0        0        0     9802 2024-04-11 13:00:04.955252 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
+-rw-r--r--   0        0        0      821 2024-04-11 13:00:04.959496 airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/tasks.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.890235 airflow_tools-0.8.4/src/airflow_tools/providers/http_to_data_lake/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891091 airflow_tools-0.8.4/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
+-rw-r--r--   0        0        0     9015 2024-04-11 13:00:04.964694 airflow_tools-0.8.4/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
+-rw-r--r--   0        0        0     1108 2024-03-18 14:38:56.889184 airflow_tools-0.8.4/src/airflow_tools/providers/package.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891899 airflow_tools-0.8.4/src/airflow_tools/py.typed
+-rw-r--r--   0        0        0    10026 1970-01-01 00:00:00.000000 airflow_tools-0.8.4/PKG-INFO
```

### Comparing `airflow_tools-0.8.2/LICENSE.txt` & `airflow_tools-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/README.md` & `airflow_tools-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/pyproject.toml` & `airflow_tools-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-tools"
-version = "0.8.2"
+version = "0.8.4"
 
 description = ""
 authors = ["Biel Llobera <biel_llobera@dkl.digital>"]
 readme = "README.md"
 include = ["src/airflow_tools"]
 
 [tool.poetry.dependencies]
```

### Comparing `airflow_tools-0.8.2/src/airflow_tools/compression_utils.py` & `airflow_tools-0.8.4/src/airflow_tools/compression_utils.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/data_lake_facade.py` & `airflow_tools-0.8.4/src/airflow_tools/data_lake_facade.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/filesystems/filesystem_factory.py` & `airflow_tools-0.8.4/src/airflow_tools/filesystems/filesystem_factory.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/filesystems/filesystem_protocol.py` & `airflow_tools-0.8.4/src/airflow_tools/filesystems/filesystem_protocol.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py` & `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py` & `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py` & `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/local_filesystem.py` & `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/local_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/s3_filesystem.py` & `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/s3_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/filesystems/impl/sftp_filesystem.py` & `airflow_tools-0.8.4/src/airflow_tools/filesystems/impl/sftp_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/notifications/slack/webhook.py` & `airflow_tools-0.8.4/src/airflow_tools/notifications/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/azure_databricks.py` & `airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/azure_databricks.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/providers/azure/hooks/azure_file_share.py` & `airflow_tools-0.8.4/src/airflow_tools/providers/azure/hooks/azure_file_share.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/providers/data_lake/operators/data_lake.py` & `airflow_tools-0.8.4/src/airflow_tools/providers/data_lake/operators/data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/filesystem.py` & `airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/filesystem.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from io import BytesIO
 from typing import TYPE_CHECKING, Optional, Protocol
 
 from airflow.hooks.base import BaseHook
 from airflow.models import BaseOperator
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 from airflow_tools.filesystems.filesystem_factory import FilesystemFactory
@@ -32,23 +33,25 @@
     def __init__(
         self,
         source_sql_conn_id: str,
         destination_fs_conn_id: str,
         sql: str,
         destination_path: str,
         batch_size: int | None = None,
+        create_file_on_success: str | None = None,
         *args,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.source_sql_conn_id = source_sql_conn_id
         self.destination_fs_conn_id = destination_fs_conn_id
         self.sql = sql
         self.destination_path = destination_path
         self.batch_size = batch_size
+        self.create_file_on_success = create_file_on_success
         self.files = []
 
     def execute(self, context):
         source_sql_hook: DbApiHook = BaseHook.get_connection(
             self.source_sql_conn_id
         ).get_hook()
 
@@ -65,14 +68,18 @@
             )
         )
         for i, df in enumerate(dfs, start=1):
             full_file_path = f"{self.destination_path.rstrip('/')}/part{i:04}.parquet"
             destination_fs_hook.write(df.to_parquet(index=False), full_file_path)
             self.files.append(full_file_path)
 
+        if self.create_file_on_success is not None and isinstance(self.create_file_on_success, str):
+            success_file_path = f"{self.destination_path.rstrip('/')}/{self.create_file_on_success}"
+            destination_fs_hook.write(BytesIO(), success_file_path)
+
 
 class FilesystemToFilesystem(BaseOperator):
     """
     Copies a file from a filesystem to another filesystem.
     """
 
     template_fields = ('source_path', 'destination_path')
@@ -80,23 +87,25 @@
     def __init__(
         self,
         source_fs_conn_id: str,
         destination_fs_conn_id: str,
         source_path: str,
         destination_path: str,
         data_transformation: Optional[Transformation] = None,
+        create_file_on_success: str | None = None,
         *args,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.source_fs_conn_id = source_fs_conn_id
         self.destination_fs_conn_id = destination_fs_conn_id
         self.source_path = source_path
         self.destination_path = destination_path
         self.data_transformation = data_transformation
+        self.create_file_on_success = create_file_on_success
 
     def execute(self, context):
         source_fs_hook = FilesystemFactory.get_data_lake_filesystem(
             connection=BaseHook.get_connection(self.source_fs_conn_id),
         )
         destination_fs_hook = FilesystemFactory.get_data_lake_filesystem(
             connection=BaseHook.get_connection(self.destination_fs_conn_id),
@@ -116,14 +125,18 @@
             full_destination_path = (
                 self.destination_path + file_name
                 if self.destination_path.endswith('/')
                 else self.destination_path
             )
             destination_fs_hook.write(data, full_destination_path)
 
+        if self.create_file_on_success is not None and isinstance(self.create_file_on_success, str):
+            success_file_path = '/'.join(self.destination_path.split('/')[:-1]) + '/' + self.create_file_on_success
+            destination_fs_hook.write(BytesIO(), success_file_path)
+
 
 class FilesystemDeleteOperator(BaseOperator):
     template_fields = ('filesystem_path',)
 
     def __init__(self, filesystem_conn_id: str, filesystem_path: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.filesystem_conn_id = filesystem_conn_id
```

### Comparing `airflow_tools-0.8.2/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py` & `airflow_tools-0.8.4/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py` & `airflow_tools-0.8.4/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         for response in self.paginate_sync(
             response=response,
             use_new_data_parameters_on_pagination=use_new_data_parameters_on_pagination,
         ):
             yield self.process_response(context=context, response=response)
 
     def paginate_sync(
-        self, response: Response, use_new_data_parameters_on_pagination=False
+        self, response: Response, use_new_data_parameters_on_pagination: bool = False
     ) -> Response | list[Response]:
         if not self.pagination_function:
             return None
 
         while True:
             next_page_params = self.pagination_function(response)
             if not next_page_params:
@@ -222,19 +222,19 @@
                 return parquet_to_binary(self.data, self.compression)
 
             case _:
                 raise NotImplementedError(f'Unknown save_format: {self.save_format}')
 
 
 def list_to_jsonl(data: list[dict], compression: 'CompressionOptions') -> BytesIO:
-    out = StringIO()
     df = pd.DataFrame(data)
+    out = BytesIO()
     df.to_json(out, orient='records', lines=True, compression=compression)
     out.seek(0)
-    return BytesIO(out.getvalue().encode())
+    return out
 
 
 def json_to_binary(data: dict, compression: 'CompressionOptions') -> BytesIO:
     json_string = json.dumps(data).encode()
     compressed_json = compress(compression, json_string)
     out = BytesIO(compressed_json)
     return out
```

### Comparing `airflow_tools-0.8.2/src/airflow_tools/providers/package.py` & `airflow_tools-0.8.4/src/airflow_tools/providers/package.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.2/PKG-INFO` & `airflow_tools-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-tools
-Version: 0.8.2
+Version: 0.8.4
 Summary: 
 Author: Biel Llobera
 Author-email: biel_llobera@dkl.digital
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.2 Summary: Author: Biel
+Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.4 Summary: Author: Biel
 Llobera Author-email: biel_llobera@dkl.digital Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: apache-
 airflow (>=2.8,<3.0) Requires-Dist: apache-airflow-providers-amazon
 (>=8.8.0,<9.0.0) Requires-Dist: apache-airflow-providers-microsoft-azure
 (>=8.0.0,<9.0.0) Requires-Dist: apache-airflow-providers-sftp (>=4.8.1,<5.0.0)
```

