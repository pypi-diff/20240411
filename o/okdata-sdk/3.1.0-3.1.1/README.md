# Comparing `tmp/okdata-sdk-3.1.0.tar.gz` & `tmp/okdata-sdk-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okdata-sdk-3.1.0.tar", last modified: Wed Jan 10 06:58:01 2024, max compression
+gzip compressed data, was "okdata-sdk-3.1.1.tar", last modified: Thu Apr 11 08:18:55 2024, max compression
```

## Comparing `okdata-sdk-3.1.0.tar` & `okdata-sdk-3.1.1.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/
--rw-r--r--   0 simen     (1000) simen     (1000)     1077 2020-02-10 07:59:59.000000 okdata-sdk-3.1.0/LICENSE
--rw-r--r--   0 simen     (1000) simen     (1000)    10212 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/PKG-INFO
--rw-r--r--   0 simen     (1000) simen     (1000)     9506 2022-05-03 14:04:37.000000 okdata-sdk-3.1.0/README.md
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.429884 okdata-sdk-3.1.0/okdata/
--rw-r--r--   0 simen     (1000) simen     (1000)       56 2020-12-16 13:38:56.000000 okdata-sdk-3.1.0/okdata/__init__.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.429884 okdata-sdk-3.1.0/okdata/sdk/
--rw-r--r--   0 simen     (1000) simen     (1000)       45 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/__init__.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.429884 okdata-sdk-3.1.0/okdata/sdk/auth/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/auth/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3507 2022-04-25 08:38:59.000000 okdata-sdk-3.1.0/okdata/sdk/auth/auth.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata/sdk/auth/credentials/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/auth/credentials/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1380 2022-04-25 08:38:59.000000 okdata-sdk-3.1.0/okdata/sdk/auth/credentials/client_credentials.py
--rw-r--r--   0 simen     (1000) simen     (1000)      368 2022-04-25 08:38:59.000000 okdata-sdk-3.1.0/okdata/sdk/auth/credentials/common.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1137 2022-04-25 08:38:59.000000 okdata-sdk-3.1.0/okdata/sdk/auth/credentials/password_grant.py
--rw-r--r--   0 simen     (1000) simen     (1000)      503 2021-03-01 07:50:29.000000 okdata-sdk-3.1.0/okdata/sdk/auth/util.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4771 2022-05-03 14:04:37.000000 okdata-sdk-3.1.0/okdata/sdk/config.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata/sdk/data/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/data/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     8649 2024-01-10 06:52:01.000000 okdata-sdk-3.1.0/okdata/sdk/data/dataset.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1247 2021-02-09 08:09:22.000000 okdata-sdk-3.1.0/okdata/sdk/data/download.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1861 2021-04-29 11:41:43.000000 okdata-sdk-3.1.0/okdata/sdk/data/upload.py
--rw-r--r--   0 simen     (1000) simen     (1000)       96 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/exceptions.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1287 2021-04-08 10:45:31.000000 okdata-sdk-3.1.0/okdata/sdk/file_cache.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1166 2023-02-06 14:11:58.000000 okdata-sdk-3.1.0/okdata/sdk/io_utils.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata/sdk/permission/
--rw-r--r--   0 simen     (1000) simen     (1000)     2396 2024-01-08 14:01:10.000000 okdata-sdk-3.1.0/okdata/sdk/permission/client.py
--rw-r--r--   0 simen     (1000) simen     (1000)      336 2022-04-25 08:38:59.000000 okdata-sdk-3.1.0/okdata/sdk/permission/user_types.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata/sdk/pipelines/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3065 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/client.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     2140 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/pipeline.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4744 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/pipeline_base.py
--rw-r--r--   0 simen     (1000) simen     (1000)     2606 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/pipeline_input.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3693 2022-12-09 12:12:16.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/pipeline_instance.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1028 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schema.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/
--rw-r--r--   0 simen     (1000) simen     (1000)      857 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/pipeline-inputs.json
--rw-r--r--   0 simen     (1000) simen     (1000)     1088 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/pipeline-instances.json
--rw-r--r--   0 simen     (1000) simen     (1000)      922 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/pipelines.json
--rw-r--r--   0 simen     (1000) simen     (1000)      526 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/schemas.json
--rw-r--r--   0 simen     (1000) simen     (1000)     2703 2022-06-21 13:35:01.000000 okdata-sdk-3.1.0/okdata/sdk/sdk.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata/sdk/status/
--rw-r--r--   0 simen     (1000) simen     (1000)       56 2020-11-10 09:16:41.000000 okdata-sdk-3.1.0/okdata/sdk/status/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)      755 2022-04-25 08:38:59.000000 okdata-sdk-3.1.0/okdata/sdk/status/status.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata/sdk/team/
--rw-r--r--   0 simen     (1000) simen     (1000)     3023 2023-04-21 10:49:18.000000 okdata-sdk-3.1.0/okdata/sdk/team/client.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/okdata_sdk.egg-info/
--rw-r--r--   0 simen     (1000) simen     (1000)    10212 2024-01-10 06:58:01.000000 okdata-sdk-3.1.0/okdata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 simen     (1000) simen     (1000)     1540 2024-01-10 06:58:01.000000 okdata-sdk-3.1.0/okdata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        1 2024-01-10 06:58:01.000000 okdata-sdk-3.1.0/okdata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        7 2024-01-10 06:58:01.000000 okdata-sdk-3.1.0/okdata_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        1 2024-01-10 06:58:01.000000 okdata-sdk-3.1.0/okdata_sdk.egg-info/not-zip-safe
--rw-r--r--   0 simen     (1000) simen     (1000)      101 2024-01-10 06:58:01.000000 okdata-sdk-3.1.0/okdata_sdk.egg-info/requires.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        7 2024-01-10 06:58:01.000000 okdata-sdk-3.1.0/okdata_sdk.egg-info/top_level.txt
--rw-r--r--   0 simen     (1000) simen     (1000)      262 2023-08-14 10:34:59.000000 okdata-sdk-3.1.0/pyproject.toml
--rw-r--r--   0 simen     (1000) simen     (1000)       38 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/setup.cfg
--rw-r--r--   0 simen     (1000) simen     (1000)     1709 2024-01-10 06:56:16.000000 okdata-sdk-3.1.0/setup.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-01-10 06:58:01.433884 okdata-sdk-3.1.0/tests/
--rw-r--r--   0 simen     (1000) simen     (1000)     5095 2022-04-25 08:38:59.000000 okdata-sdk-3.1.0/tests/test_utils.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.583303 okdata-sdk-3.1.1/
+-rw-r--r--   0 simen     (1000) simen     (1000)     1077 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/LICENSE
+-rw-r--r--   0 simen     (1000) simen     (1000)    10212 2024-04-11 08:18:55.583303 okdata-sdk-3.1.1/PKG-INFO
+-rw-r--r--   0 simen     (1000) simen     (1000)     9506 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/README.md
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.579303 okdata-sdk-3.1.1/okdata/
+-rw-r--r--   0 simen     (1000) simen     (1000)       56 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/__init__.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.579303 okdata-sdk-3.1.1/okdata/sdk/
+-rw-r--r--   0 simen     (1000) simen     (1000)       45 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/__init__.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.579303 okdata-sdk-3.1.1/okdata/sdk/auth/
+-rw-r--r--   0 simen     (1000) simen     (1000)        0 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/auth/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4633 2024-04-11 08:13:22.000000 okdata-sdk-3.1.1/okdata/sdk/auth/auth.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.579303 okdata-sdk-3.1.1/okdata/sdk/auth/credentials/
+-rw-r--r--   0 simen     (1000) simen     (1000)        0 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/auth/credentials/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1382 2024-04-11 08:11:27.000000 okdata-sdk-3.1.1/okdata/sdk/auth/credentials/client_credentials.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      368 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/auth/credentials/common.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1137 2024-04-04 12:59:20.000000 okdata-sdk-3.1.1/okdata/sdk/auth/credentials/password_grant.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4771 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/config.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.579303 okdata-sdk-3.1.1/okdata/sdk/data/
+-rw-r--r--   0 simen     (1000) simen     (1000)        0 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/data/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     8649 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/data/dataset.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1247 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/data/download.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1861 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/data/upload.py
+-rw-r--r--   0 simen     (1000) simen     (1000)       96 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/exceptions.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1287 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/file_cache.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1166 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/io_utils.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.579303 okdata-sdk-3.1.1/okdata/sdk/permission/
+-rw-r--r--   0 simen     (1000) simen     (1000)     2396 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/permission/client.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      336 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/permission/user_types.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.579303 okdata-sdk-3.1.1/okdata/sdk/pipelines/
+-rw-r--r--   0 simen     (1000) simen     (1000)        0 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     3065 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/client.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.579303 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/
+-rw-r--r--   0 simen     (1000) simen     (1000)        0 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     2140 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/pipeline.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4744 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/pipeline_base.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     2606 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/pipeline_input.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     3693 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/pipeline_instance.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1028 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schema.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.583303 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/
+-rw-r--r--   0 simen     (1000) simen     (1000)      857 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/pipeline-inputs.json
+-rw-r--r--   0 simen     (1000) simen     (1000)     1088 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/pipeline-instances.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      922 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/pipelines.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      526 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/schemas.json
+-rw-r--r--   0 simen     (1000) simen     (1000)     2703 2024-04-04 12:44:35.000000 okdata-sdk-3.1.1/okdata/sdk/sdk.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.583303 okdata-sdk-3.1.1/okdata/sdk/status/
+-rw-r--r--   0 simen     (1000) simen     (1000)       56 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/status/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      755 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/status/status.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.583303 okdata-sdk-3.1.1/okdata/sdk/team/
+-rw-r--r--   0 simen     (1000) simen     (1000)     3023 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/okdata/sdk/team/client.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.583303 okdata-sdk-3.1.1/okdata_sdk.egg-info/
+-rw-r--r--   0 simen     (1000) simen     (1000)    10212 2024-04-11 08:18:55.000000 okdata-sdk-3.1.1/okdata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 simen     (1000) simen     (1000)     1516 2024-04-11 08:18:55.000000 okdata-sdk-3.1.1/okdata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)        1 2024-04-11 08:18:55.000000 okdata-sdk-3.1.1/okdata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)        7 2024-04-11 08:18:55.000000 okdata-sdk-3.1.1/okdata_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)        1 2024-04-11 08:18:55.000000 okdata-sdk-3.1.1/okdata_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 simen     (1000) simen     (1000)       72 2024-04-11 08:18:55.000000 okdata-sdk-3.1.1/okdata_sdk.egg-info/requires.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)        7 2024-04-11 08:18:55.000000 okdata-sdk-3.1.1/okdata_sdk.egg-info/top_level.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)      262 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/pyproject.toml
+-rw-r--r--   0 simen     (1000) simen     (1000)       38 2024-04-11 08:18:55.583303 okdata-sdk-3.1.1/setup.cfg
+-rw-r--r--   0 simen     (1000) simen     (1000)     1775 2024-04-11 08:15:33.000000 okdata-sdk-3.1.1/setup.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-04-11 08:18:55.583303 okdata-sdk-3.1.1/tests/
+-rw-r--r--   0 simen     (1000) simen     (1000)     5095 2024-02-23 13:25:19.000000 okdata-sdk-3.1.1/tests/test_utils.py
```

### Comparing `okdata-sdk-3.1.0/LICENSE` & `okdata-sdk-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/PKG-INFO` & `okdata-sdk-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okdata-sdk
-Version: 3.1.0
+Version: 3.1.1
 Summary: SDK for origo dataplatform
 Home-page: https://github.com/oslokommune/okdata-sdk-python
 Author: Oslo Origo
 Author-email: dataplattform@oslo.kommune.no
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `okdata-sdk-3.1.0/README.md` & `okdata-sdk-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/auth/credentials/client_credentials.py` & `okdata-sdk-3.1.1/okdata/sdk/auth/credentials/client_credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional
 
-from keycloak.exceptions import KeycloakGetError  # type: ignore
+from keycloak.exceptions import KeycloakPostError  # type: ignore
 from keycloak.keycloak_openid import KeycloakOpenID  # type: ignore
 
 from okdata.sdk.auth.credentials.common import (
     TokenProvider,
     TokenProviderNotInitialized,
     TokenRefreshError,
 )
@@ -31,12 +31,12 @@
             client_id=self.client_id,
             client_secret_key=self.client_secret,
         )
 
     def refresh_token(self, refresh_token):
         try:
             return self.client.refresh_token(refresh_token=refresh_token)
-        except KeycloakGetError as e:
+        except KeycloakPostError as e:
             raise TokenRefreshError(str(e))
 
     def new_token(self):
         return self.client.token(grant_type=["client_credentials"])
```

### Comparing `okdata-sdk-3.1.0/okdata/sdk/auth/credentials/password_grant.py` & `okdata-sdk-3.1.1/okdata/sdk/auth/credentials/password_grant.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/config.py` & `okdata-sdk-3.1.1/okdata/sdk/config.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/data/dataset.py` & `okdata-sdk-3.1.1/okdata/sdk/data/dataset.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/data/download.py` & `okdata-sdk-3.1.1/okdata/sdk/data/download.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/data/upload.py` & `okdata-sdk-3.1.1/okdata/sdk/data/upload.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/file_cache.py` & `okdata-sdk-3.1.1/okdata/sdk/file_cache.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/io_utils.py` & `okdata-sdk-3.1.1/okdata/sdk/io_utils.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/permission/client.py` & `okdata-sdk-3.1.1/okdata/sdk/permission/client.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/client.py` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/client.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/pipeline.py` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/pipeline.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/pipeline_base.py` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/pipeline_input.py` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/pipeline_input.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/pipeline_instance.py` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/pipeline_instance.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schema.py` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schema.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/pipeline-inputs.json` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/pipeline-inputs.json`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/pipeline-instances.json` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/pipeline-instances.json`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/pipelines.json` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/pipelines.json`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/pipelines/resources/schemas/schemas.json` & `okdata-sdk-3.1.1/okdata/sdk/pipelines/resources/schemas/schemas.json`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/sdk.py` & `okdata-sdk-3.1.1/okdata/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/status/status.py` & `okdata-sdk-3.1.1/okdata/sdk/status/status.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata/sdk/team/client.py` & `okdata-sdk-3.1.1/okdata/sdk/team/client.py`

 * *Files identical despite different names*

### Comparing `okdata-sdk-3.1.0/okdata_sdk.egg-info/PKG-INFO` & `okdata-sdk-3.1.1/okdata_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okdata-sdk
-Version: 3.1.0
+Version: 3.1.1
 Summary: SDK for origo dataplatform
 Home-page: https://github.com/oslokommune/okdata-sdk-python
 Author: Oslo Origo
 Author-email: dataplattform@oslo.kommune.no
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `okdata-sdk-3.1.0/okdata_sdk.egg-info/SOURCES.txt` & `okdata-sdk-3.1.1/okdata_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 okdata/sdk/config.py
 okdata/sdk/exceptions.py
 okdata/sdk/file_cache.py
 okdata/sdk/io_utils.py
 okdata/sdk/sdk.py
 okdata/sdk/auth/__init__.py
 okdata/sdk/auth/auth.py
-okdata/sdk/auth/util.py
 okdata/sdk/auth/credentials/__init__.py
 okdata/sdk/auth/credentials/client_credentials.py
 okdata/sdk/auth/credentials/common.py
 okdata/sdk/auth/credentials/password_grant.py
 okdata/sdk/data/__init__.py
 okdata/sdk/data/dataset.py
 okdata/sdk/data/download.py
```

### Comparing `okdata-sdk-3.1.0/setup.py` & `okdata-sdk-3.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="okdata-sdk",
-    version="3.1.0",
+    version="3.1.1",
     author="Oslo Origo",
     author_email="dataplattform@oslo.kommune.no",
     description="SDK for origo dataplatform",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oslokommune/okdata-sdk-python",
     package_data={"okdata": ["py.typed"]},
     packages=setuptools.find_namespace_packages(
         include="okdata.sdk.*", exclude=["tests*"]
     ),
     namespace_packages=["okdata"],
     install_requires=[
         "jsonschema",
-        "PyJWT>=2.0.0",
-        "python-jose>=3.1.0,<4.0.0",
-        "python-keycloak",
+        # Versions prior to 3.9.1 depends on the vulnerable (and seemingly
+        # abandoned) python-jose library.
+        "python-keycloak>=3.9.1,<4",
         "requests>=2.25,<3",
         "urllib3>=1.26,<2",
     ],
     data_files=[
         (
             "schema",
             [
```

### Comparing `okdata-sdk-3.1.0/tests/test_utils.py` & `okdata-sdk-3.1.1/tests/test_utils.py`

 * *Files identical despite different names*

