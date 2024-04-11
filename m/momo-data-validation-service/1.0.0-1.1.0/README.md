# Comparing `tmp/momo-data-validation-service-1.0.0.tar.gz` & `tmp/momo-data-validation-service-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momo-data-validation-service-1.0.0.tar", last modified: Thu Apr 11 00:53:18 2024, max compression
+gzip compressed data, was "momo-data-validation-service-1.1.0.tar", last modified: Thu Apr 11 01:04:47 2024, max compression
```

## Comparing `momo-data-validation-service-1.0.0.tar` & `momo-data-validation-service-1.1.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.480817 momo-data-validation-service-1.0.0/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    11358 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/LICENSE
--rw-r--r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    45954 2024-04-11 00:53:18.480817 momo-data-validation-service-1.0.0/PKG-INFO
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    44079 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/README.md
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.448825 momo-data-validation-service-1.0.0/data_validation/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      718 2024-04-11 00:51:14.000000 momo-data-validation-service-1.0.0/data_validation/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    26509 2024-04-09 07:00:39.000000 momo-data-validation-service-1.0.0/data_validation/__main__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1986 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/app.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    48902 2024-04-03 08:52:32.000000 momo-data-validation-service-1.0.0/data_validation/cli_tools.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      881 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/client_info.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    10055 2024-04-03 08:53:31.000000 momo-data-validation-service-1.0.0/data_validation/clients.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14254 2024-04-05 09:03:48.000000 momo-data-validation-service-1.0.0/data_validation/combiner.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    40169 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/config_manager.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     5244 2024-04-11 00:51:19.000000 momo-data-validation-service-1.0.0/data_validation/consts.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14688 2024-04-05 04:52:49.000000 momo-data-validation-service-1.0.0/data_validation/data_validation_module.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      687 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/exceptions.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1269 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/jellyfish_distance.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2521 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/metadata.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    16257 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/partition_builder.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.452824 momo-data-validation-service-1.0.0/data_validation/query_builder/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      575 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/query_builder/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2583 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/query_builder/partition_row_builder.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    19246 2024-04-05 09:03:17.000000 momo-data-validation-service-1.0.0/data_validation/query_builder/query_builder.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3710 2024-03-27 04:01:18.000000 momo-data-validation-service-1.0.0/data_validation/query_builder/random_row_builder.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.452824 momo-data-validation-service-1.0.0/data_validation/result_handlers/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/result_handlers/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3970 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/result_handlers/bigquery.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2526 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/result_handlers/text.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14320 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/schema_validation.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1773 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/secret_manager.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    10173 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/state_manager.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    16109 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/data_validation/validation_builder.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.476818 momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/
--rw-r--r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    45954 2024-04-11 00:53:18.000000 momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/PKG-INFO
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3295 2024-04-11 00:53:18.000000 momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/SOURCES.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        1 2024-04-11 00:53:18.000000 momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/dependency_links.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       66 2024-04-11 00:53:18.000000 momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/entry_points.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      614 2024-04-11 00:53:18.000000 momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/requires.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       28 2024-04-11 00:53:18.000000 momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/top_level.txt
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       67 2024-04-11 00:53:18.480817 momo-data-validation-service-1.0.0/setup.cfg
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3023 2024-04-11 00:49:46.000000 momo-data-validation-service-1.0.0/setup.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.444826 momo-data-validation-service-1.0.0/third_party/
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.448825 momo-data-validation-service-1.0.0/third_party/ibis/
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.472819 momo-data-validation-service-1.0.0/third_party/ibis/ibis_addon/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_addon/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2515 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_addon/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    20735 2024-04-10 03:40:35.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_addon/operations.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.472819 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     6916 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1378 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      934 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/client.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2748 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1517 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2300 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/registry.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.472819 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/tests/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        1 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4999 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1292 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.472819 momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2649 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1264 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1024 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1492 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/datatypes.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    15919 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/registry.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.472819 momo-data-validation-service-1.0.0/third_party/ibis/ibis_impala/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_impala/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     7187 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_impala/api.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.472819 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mssql/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2987 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mssql/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1237 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mssql/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1315 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mssql/datatypes.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.472819 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mysql/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mysql/__init__.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.472819 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4596 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1509 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_mysql/compiler.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.476818 momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3043 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1228 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1085 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     6593 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/datatypes.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14411 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/registry.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.476818 momo-data-validation-service-1.0.0/third_party/ibis/ibis_postgres/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      101 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_postgres/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4126 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_postgres/client.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      839 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_postgres/datatypes.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.476818 momo-data-validation-service-1.0.0/third_party/ibis/ibis_redshift/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4053 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_redshift/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1170 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_redshift/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1543 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_redshift/compiler.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.476818 momo-data-validation-service-1.0.0/third_party/ibis/ibis_snowflake/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_snowflake/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1148 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_snowflake/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1986 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_snowflake/datatypes.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.476818 momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     9164 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1210 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/api.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1810 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     7034 2024-03-20 09:17:53.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/datatypes.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     8568 2024-03-27 04:03:19.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/registry.py
-drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 00:53:18.476818 momo-data-validation-service-1.0.0/third_party/ibis/ibis_trino/
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       92 2024-04-02 06:55:24.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_trino/__init__.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2288 2024-04-10 03:08:36.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_trino/compiler.py
--rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      891 2024-04-03 07:43:34.000000 momo-data-validation-service-1.0.0/third_party/ibis/ibis_trino/datatypes.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    11358 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/LICENSE
+-rw-r--r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    45975 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/PKG-INFO
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    44079 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/README.md
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.001188 momo-data-validation-service-1.1.0/data_validation/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      718 2024-04-11 00:51:14.000000 momo-data-validation-service-1.1.0/data_validation/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    26509 2024-04-09 07:00:39.000000 momo-data-validation-service-1.1.0/data_validation/__main__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1986 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/app.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    48902 2024-04-03 08:52:32.000000 momo-data-validation-service-1.1.0/data_validation/cli_tools.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      881 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/client_info.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    10055 2024-04-03 08:53:31.000000 momo-data-validation-service-1.1.0/data_validation/clients.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14254 2024-04-05 09:03:48.000000 momo-data-validation-service-1.1.0/data_validation/combiner.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    40169 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/config_manager.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     5244 2024-04-11 00:51:19.000000 momo-data-validation-service-1.1.0/data_validation/consts.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14688 2024-04-05 04:52:49.000000 momo-data-validation-service-1.1.0/data_validation/data_validation.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      687 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/exceptions.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1269 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/jellyfish_distance.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2521 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/metadata.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    16257 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/partition_builder.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.001188 momo-data-validation-service-1.1.0/data_validation/query_builder/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      575 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/query_builder/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2583 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/query_builder/partition_row_builder.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    19246 2024-04-05 09:03:17.000000 momo-data-validation-service-1.1.0/data_validation/query_builder/query_builder.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3710 2024-03-27 04:01:18.000000 momo-data-validation-service-1.1.0/data_validation/query_builder/random_row_builder.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.001188 momo-data-validation-service-1.1.0/data_validation/result_handlers/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/result_handlers/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3970 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/result_handlers/bigquery.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2526 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/result_handlers/text.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14320 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/schema_validation.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1773 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/secret_manager.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    10173 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/state_manager.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    16109 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/data_validation/validation_builder.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/
+-rw-r--r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    45975 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/PKG-INFO
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3288 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        1 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       66 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/entry_points.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      620 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/requires.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       28 2024-04-11 01:04:46.000000 momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/top_level.txt
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       67 2024-04-11 01:04:47.025191 momo-data-validation-service-1.1.0/setup.cfg
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3036 2024-04-11 01:03:30.000000 momo-data-validation-service-1.1.0/setup.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:46.993187 momo-data-validation-service-1.1.0/third_party/
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:46.997187 momo-data-validation-service-1.1.0/third_party/ibis/
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2515 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    20735 2024-04-10 03:40:35.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/operations.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     6916 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1378 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      934 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/client.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2748 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1517 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2300 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/registry.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/tests/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        1 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4999 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1292 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2649 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1264 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1024 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1492 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    15919 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/registry.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_impala/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_impala/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     7187 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_impala/api.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2987 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1237 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1315 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/datatypes.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/__init__.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/base_sql_compiler/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/base_sql_compiler/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4596 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1509 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/compiler.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.017190 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     3043 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1228 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1085 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     6593 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)    14411 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/registry.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      101 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4126 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/client.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      839 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/datatypes.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     4053 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1170 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1543 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/compiler.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1148 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1986 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/datatypes.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     9164 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1210 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/api.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     1810 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     7034 2024-03-20 09:17:53.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/datatypes.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     8568 2024-03-27 04:03:19.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/registry.py
+drwxrwxr-x   0 dungnguyen24  (1000) dungnguyen24  (1000)        0 2024-04-11 01:04:47.021191 momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)       92 2024-04-02 06:55:24.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/__init__.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)     2288 2024-04-10 03:08:36.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/compiler.py
+-rw-rw-r--   0 dungnguyen24  (1000) dungnguyen24  (1000)      891 2024-04-03 07:43:34.000000 momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/datatypes.py
```

### Comparing `momo-data-validation-service-1.0.0/LICENSE` & `momo-data-validation-service-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/PKG-INFO` & `momo-data-validation-service-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momo-data-validation-service
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package to enable easy data validation
 Home-page: https://glab.mservice.io/ai-data-platform/uncategorized-projects/professional-services-data-validator
 Author: Nguyen Thuy Dung
 Author-email: dung.nguyen24@mservice.com.vn
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -38,14 +38,15 @@
 Requires-Dist: setuptools>=34.0.0
 Requires-Dist: jellyfish==1.0.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: Flask==2.3.2
 Requires-Dist: parsy==2.1
 Requires-Dist: google-cloud-secret-manager<=2.15.0
 Requires-Dist: ibis-framework[trino]
+Requires-Dist: trino
 Requires-Dist: wheel
 Provides-Extra: apache-airflow
 Requires-Dist: 1.10.11; extra == "apache-airflow"
 Provides-Extra: pyspark
 Requires-Dist: 3.0.0; extra == "pyspark"
 
 # Data Validation Tool
```

### Comparing `momo-data-validation-service-1.0.0/README.md` & `momo-data-validation-service-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/__init__.py` & `momo-data-validation-service-1.1.0/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/__main__.py` & `momo-data-validation-service-1.1.0/data_validation/__main__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/app.py` & `momo-data-validation-service-1.1.0/data_validation/app.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/cli_tools.py` & `momo-data-validation-service-1.1.0/data_validation/cli_tools.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/client_info.py` & `momo-data-validation-service-1.1.0/data_validation/client_info.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/clients.py` & `momo-data-validation-service-1.1.0/data_validation/clients.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/combiner.py` & `momo-data-validation-service-1.1.0/data_validation/combiner.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/config_manager.py` & `momo-data-validation-service-1.1.0/data_validation/config_manager.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/consts.py` & `momo-data-validation-service-1.1.0/data_validation/consts.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/data_validation_module.py` & `momo-data-validation-service-1.1.0/data_validation/data_validation.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/exceptions.py` & `momo-data-validation-service-1.1.0/data_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/jellyfish_distance.py` & `momo-data-validation-service-1.1.0/data_validation/jellyfish_distance.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/metadata.py` & `momo-data-validation-service-1.1.0/data_validation/metadata.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/partition_builder.py` & `momo-data-validation-service-1.1.0/data_validation/partition_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/query_builder/__init__.py` & `momo-data-validation-service-1.1.0/data_validation/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/query_builder/partition_row_builder.py` & `momo-data-validation-service-1.1.0/data_validation/query_builder/partition_row_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/query_builder/query_builder.py` & `momo-data-validation-service-1.1.0/data_validation/query_builder/query_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/query_builder/random_row_builder.py` & `momo-data-validation-service-1.1.0/data_validation/query_builder/random_row_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/result_handlers/bigquery.py` & `momo-data-validation-service-1.1.0/data_validation/result_handlers/bigquery.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/result_handlers/text.py` & `momo-data-validation-service-1.1.0/data_validation/result_handlers/text.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/schema_validation.py` & `momo-data-validation-service-1.1.0/data_validation/schema_validation.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/secret_manager.py` & `momo-data-validation-service-1.1.0/data_validation/secret_manager.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/state_manager.py` & `momo-data-validation-service-1.1.0/data_validation/state_manager.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/data_validation/validation_builder.py` & `momo-data-validation-service-1.1.0/data_validation/validation_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/PKG-INFO` & `momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momo-data-validation-service
-Version: 1.0.0
+Version: 1.1.0
 Summary: A package to enable easy data validation
 Home-page: https://glab.mservice.io/ai-data-platform/uncategorized-projects/professional-services-data-validator
 Author: Nguyen Thuy Dung
 Author-email: dung.nguyen24@mservice.com.vn
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -38,14 +38,15 @@
 Requires-Dist: setuptools>=34.0.0
 Requires-Dist: jellyfish==1.0.0
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: Flask==2.3.2
 Requires-Dist: parsy==2.1
 Requires-Dist: google-cloud-secret-manager<=2.15.0
 Requires-Dist: ibis-framework[trino]
+Requires-Dist: trino
 Requires-Dist: wheel
 Provides-Extra: apache-airflow
 Requires-Dist: 1.10.11; extra == "apache-airflow"
 Provides-Extra: pyspark
 Requires-Dist: 3.0.0; extra == "pyspark"
 
 # Data Validation Tool
```

### Comparing `momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/SOURCES.txt` & `momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 data_validation/app.py
 data_validation/cli_tools.py
 data_validation/client_info.py
 data_validation/clients.py
 data_validation/combiner.py
 data_validation/config_manager.py
 data_validation/consts.py
-data_validation/data_validation_module.py
+data_validation/data_validation.py
 data_validation/exceptions.py
 data_validation/jellyfish_distance.py
 data_validation/metadata.py
 data_validation/partition_builder.py
 data_validation/schema_validation.py
 data_validation/secret_manager.py
 data_validation/state_manager.py
```

### Comparing `momo-data-validation-service-1.0.0/momo_data_validation_service.egg-info/requires.txt` & `momo-data-validation-service-1.1.0/momo_data_validation_service.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 setuptools>=34.0.0
 jellyfish==1.0.0
 tabulate==0.9.0
 Flask==2.3.2
 parsy==2.1
 google-cloud-secret-manager<=2.15.0
 ibis-framework[trino]
+trino
 wheel
 
 [apache-airflow]
 1.10.11
 
 [pyspark]
 3.0.0
```

### Comparing `momo-data-validation-service-1.0.0/setup.py` & `momo-data-validation-service-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import os
 
 import setuptools
 
 name = "momo-data-validation-service"
 description = "A package to enable easy data validation"
-version = "1.0.0"
+version = "1.1.0"
 release_status = "Development Status :: 3 - Alpha"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 dependencies = [
     # Dependency corrections from our requirements
@@ -51,14 +51,15 @@
     "setuptools>=34.0.0",
     "jellyfish==1.0.0",
     "tabulate==0.9.0",
     "Flask==2.3.2",
     "parsy==2.1",
     "google-cloud-secret-manager<=2.15.0",
     "ibis-framework[trino]",
+    "trino",
     "wheel",
 ]
 
 extras_require = {
     "apache-airflow": "1.10.11",
     "pyspark": "3.0.0",
 }
```

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_addon/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_addon/operations.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_addon/operations.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/__init__.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/client.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/client.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/compiler.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/datatypes.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/registry.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/registry.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/__init__.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/compiler.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/datatypes.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_db2/registry.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_db2/registry.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_impala/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_impala/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_mssql/__init__.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_mssql/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_mssql/datatypes.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mssql/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/base_sql_compiler/select_builder.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_mysql/compiler.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_mysql/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/__init__.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/compiler.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/datatypes.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_oracle/registry.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_oracle/registry.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_postgres/client.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/client.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_postgres/datatypes.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_postgres/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_redshift/__init__.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_redshift/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_redshift/compiler.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_redshift/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_snowflake/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_snowflake/datatypes.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_snowflake/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/__init__.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/api.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/api.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/compiler.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/datatypes.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/datatypes.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_teradata/registry.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_teradata/registry.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_trino/compiler.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/compiler.py`

 * *Files identical despite different names*

### Comparing `momo-data-validation-service-1.0.0/third_party/ibis/ibis_trino/datatypes.py` & `momo-data-validation-service-1.1.0/third_party/ibis/ibis_trino/datatypes.py`

 * *Files identical despite different names*

