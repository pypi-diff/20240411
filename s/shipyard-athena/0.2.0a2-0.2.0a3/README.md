# Comparing `tmp/shipyard_athena-0.2.0a2.tar.gz` & `tmp/shipyard_athena-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_athena-0.2.0a2.tar", max compression
+gzip compressed data, was "shipyard_athena-0.2.0a3.tar", max compression
```

## Comparing `shipyard_athena-0.2.0a2.tar` & `shipyard_athena-0.2.0a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-08-14 16:50:02.434076 shipyard_athena-0.2.0a2/README.md
--rw-r--r--   0        0        0      672 2024-03-14 19:00:36.474424 shipyard_athena-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0       33 2023-08-14 16:50:02.434882 shipyard_athena-0.2.0a2/shipyard_athena/__init__.py
--rw-r--r--   0        0        0     7718 2024-03-14 19:00:27.886501 shipyard_athena-0.2.0a2/shipyard_athena/athena.py
--rw-r--r--   0        0        0      256 2024-03-14 18:08:17.993799 shipyard_athena-0.2.0a2/shipyard_athena/cli/authtest.py
--rw-r--r--   0        0        0     2932 2024-03-14 18:08:17.994533 shipyard_athena-0.2.0a2/shipyard_athena/cli/download_query.py
--rw-r--r--   0        0        0     2045 2024-03-14 18:08:17.995368 shipyard_athena-0.2.0a2/shipyard_athena/cli/execute_query.py
--rw-r--r--   0        0        0     2021 2024-03-14 19:00:27.821578 shipyard_athena-0.2.0a2/shipyard_athena/errors/exceptions.py
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 shipyard_athena-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-14 16:50:02.434076 shipyard_athena-0.2.0a3/README.md
+-rw-r--r--   0        0        0      672 2024-04-11 02:18:05.534300 shipyard_athena-0.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-08-14 16:50:02.434882 shipyard_athena-0.2.0a3/shipyard_athena/__init__.py
+-rw-r--r--   0        0        0     7719 2024-04-11 02:18:34.164226 shipyard_athena-0.2.0a3/shipyard_athena/athena.py
+-rw-r--r--   0        0        0      256 2024-04-01 19:04:10.712887 shipyard_athena-0.2.0a3/shipyard_athena/cli/authtest.py
+-rw-r--r--   0        0        0     2903 2024-04-11 02:18:34.119185 shipyard_athena-0.2.0a3/shipyard_athena/cli/download_query.py
+-rw-r--r--   0        0        0     2045 2024-04-01 19:04:10.714216 shipyard_athena-0.2.0a3/shipyard_athena/cli/execute_query.py
+-rw-r--r--   0        0        0     2021 2024-04-01 19:04:10.714528 shipyard_athena-0.2.0a3/shipyard_athena/errors/exceptions.py
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 shipyard_athena-0.2.0a3/PKG-INFO
```

### Comparing `shipyard_athena-0.2.0a2/pyproject.toml` & `shipyard_athena-0.2.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-athena"
-version = "0.2.0a2"
+version = "0.2.0a3"
 description = "A local client for connecting to and working with Amazon Athena"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_athena"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_athena-0.2.0a2/shipyard_athena/athena.py` & `shipyard_athena-0.2.0a3/shipyard_athena/athena.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,15 @@
                 status = self._fetch_query_execution_status(job_id)
                 logger.debug(f"Query status is {status}")
                 if status == "SUCCEEDED":
                     break
             response = self.s3.Bucket(self.bucket).download_file(
                 f'{log_folder}{"/" if log_folder else ""}{job_id}.csv', dest_path
             )
+
             logger.debug("Download complete")
             if response:
                 logger.debug(f"Contents of response: {response}")
         except ExitCodeException:
             raise
         except Exception as e:
             raise errs.FetchError(e)
```

### Comparing `shipyard_athena-0.2.0a2/shipyard_athena/cli/download_query.py` & `shipyard_athena-0.2.0a3/shipyard_athena/cli/download_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     try:
         args = get_args()
         access_key = args.aws_access_key_id
         secret_key = args.aws_secret_access_key
         region_name = args.aws_default_region if args.aws_default_region else None
         database = args.database if args.database else None
         bucket = args.bucket.strip("/")
-        log_folder = args.log_folder if args.log_folder else None
+        log_folder = args.log_folder
         query = args.query
         target_file = args.destination_file_name
         target_dir = args.destination_folder_name
         target_path = shipyard.files.combine_folder_and_file_name(
             folder_name=target_dir, file_name=target_file
         )
         if target_dir:
```

### Comparing `shipyard_athena-0.2.0a2/shipyard_athena/cli/execute_query.py` & `shipyard_athena-0.2.0a3/shipyard_athena/cli/execute_query.py`

 * *Files identical despite different names*

### Comparing `shipyard_athena-0.2.0a2/shipyard_athena/errors/exceptions.py` & `shipyard_athena-0.2.0a3/shipyard_athena/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_athena-0.2.0a2/PKG-INFO` & `shipyard_athena-0.2.0a3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-athena
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: A local client for connecting to and working with Amazon Athena
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

