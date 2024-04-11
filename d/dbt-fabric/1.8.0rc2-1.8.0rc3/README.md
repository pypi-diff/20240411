# Comparing `tmp/dbt-fabric-1.8.0rc2.tar.gz` & `tmp/dbt-fabric-1.8.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fabric-1.8.0rc2.tar", last modified: Fri Mar  1 12:59:32 2024, max compression
+gzip compressed data, was "dbt-fabric-1.8.0rc3.tar", last modified: Thu Mar 28 15:34:57 2024, max compression
```

## Comparing `dbt-fabric-1.8.0rc2.tar` & `dbt-fabric-1.8.0rc3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.674936 dbt-fabric-1.8.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-01 12:59:32.674936 dbt-fabric-1.8.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.662936 dbt-fabric-1.8.0rc2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.662936 dbt-fabric-1.8.0rc2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.666936 dbt-fabric-1.8.0rc2/dbt/adapters/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/adapters/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/adapters/fabric/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.662936 dbt-fabric-1.8.0rc2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.666936 dbt-fabric-1.8.0rc2/dbt/include/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.666936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.670936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/show.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.666936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.666936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.670936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.670936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.670936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.670936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.670936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.670936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.674936 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 12:59:32.674936 dbt-fabric-1.8.0rc2/dbt_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-01 12:59:32.000000 dbt-fabric-1.8.0rc2/dbt_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-01 12:59:32.000000 dbt-fabric-1.8.0rc2/dbt_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 12:59:32.000000 dbt-fabric-1.8.0rc2/dbt_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-01 12:59:32.000000 dbt-fabric-1.8.0rc2/dbt_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-01 12:59:32.000000 dbt-fabric-1.8.0rc2/dbt_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 12:59:32.674936 dbt-fabric-1.8.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-01 12:58:52.000000 dbt-fabric-1.8.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.075620 dbt-fabric-1.8.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-28 15:34:57.075620 dbt-fabric-1.8.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.063619 dbt-fabric-1.8.0rc3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.063619 dbt-fabric-1.8.0rc3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.067619 dbt-fabric-1.8.0rc3/dbt/adapters/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/adapters/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/adapters/fabric/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9548 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.063619 dbt-fabric-1.8.0rc3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.067619 dbt-fabric-1.8.0rc3/dbt/include/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.067619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.071619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/show.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.067619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.067619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.071619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.071619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.071619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.071619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.071619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.071619 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.075620 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:34:57.075620 dbt-fabric-1.8.0rc3/dbt_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-28 15:34:56.000000 dbt-fabric-1.8.0rc3/dbt_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-28 15:34:56.000000 dbt-fabric-1.8.0rc3/dbt_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:34:56.000000 dbt-fabric-1.8.0rc3/dbt_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-28 15:34:56.000000 dbt-fabric-1.8.0rc3/dbt_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-28 15:34:56.000000 dbt-fabric-1.8.0rc3/dbt_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:34:57.075620 dbt-fabric-1.8.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-03-28 15:34:08.000000 dbt-fabric-1.8.0rc3/setup.py
```

### Comparing `dbt-fabric-1.8.0rc2/LICENSE` & `dbt-fabric-1.8.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/PKG-INFO` & `dbt-fabric-1.8.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.0rc2
+Version: 1.8.0rc3
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.0rc2/README.md` & `dbt-fabric-1.8.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/adapters/fabric/__init__.py` & `dbt-fabric-1.8.0rc3/dbt/adapters/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_adapter.py` & `dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_column.py` & `dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_column.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_connection_manager.py` & `dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/adapters/fabric/fabric_credentials.py` & `dbt-fabric-1.8.0rc3/dbt/adapters/fabric/fabric_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/apply_grants.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/catalog.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/columns.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/indexes.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/metadata.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/relation.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/adapters/schema.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/incremental/merge.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/clone.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/table/table.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/models/view/view.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/seeds/helpers.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt/include/fabric/macros/materializations/tests/helpers.sql` & `dbt-fabric-1.8.0rc3/dbt/include/fabric/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/dbt_fabric.egg-info/PKG-INFO` & `dbt-fabric-1.8.0rc3/dbt_fabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.0rc2
+Version: 1.8.0rc3
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.0rc2/dbt_fabric.egg-info/SOURCES.txt` & `dbt-fabric-1.8.0rc3/dbt_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.0rc2/setup.py` & `dbt-fabric-1.8.0rc3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     author=", ".join(authors_list),
     url="https://github.com/microsoft/dbt-fabric",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "pyodbc>=4.0.35,<5.2.0",
         "azure-identity>=1.12.0",
-        "dbt-common~=0.1.6",
+        "dbt-common>=0.1.0b1,<2.0",
     ],
     cmdclass={
         "verify": VerifyVersionCommand,
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
```

