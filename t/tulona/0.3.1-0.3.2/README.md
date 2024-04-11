# Comparing `tmp/tulona-0.3.1.tar.gz` & `tmp/tulona-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.3.1.tar", last modified: Tue Apr  9 15:15:56 2024, max compression
+gzip compressed data, was "tulona-0.3.2.tar", last modified: Wed Apr 10 18:09:13 2024, max compression
```

## Comparing `tulona-0.3.1.tar` & `tulona-0.3.2.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.378620 tulona-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-09 15:15:51.000000 tulona-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-04-09 15:15:56.378620 tulona-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-09 15:15:51.000000 tulona-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.370620 tulona-0.3.1/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.370620 tulona-0.3.1/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.374620 tulona-0.3.1/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.374620 tulona-0.3.1/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.374620 tulona-0.3.1/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.374620 tulona-0.3.1/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.374620 tulona-0.3.1/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.378620 tulona-0.3.1/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-09 15:15:51.000000 tulona-0.3.1/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:15:56.378620 tulona-0.3.1/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9766 2024-04-09 15:15:56.000000 tulona-0.3.1/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-09 15:15:56.000000 tulona-0.3.1/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:15:56.000000 tulona-0.3.1/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 15:15:56.000000 tulona-0.3.1/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 15:15:56.000000 tulona-0.3.1/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 15:15:56.000000 tulona-0.3.1/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 15:15:51.000000 tulona-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:15:56.378620 tulona-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.490989 tulona-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-10 18:09:04.000000 tulona-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-04-10 18:09:13.490989 tulona-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-04-10 18:09:04.000000 tulona-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.482989 tulona-0.3.2/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.486989 tulona-0.3.2/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.486989 tulona-0.3.2/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.486989 tulona-0.3.2/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.486989 tulona-0.3.2/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.486989 tulona-0.3.2/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.490989 tulona-0.3.2/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.490989 tulona-0.3.2/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 18:09:04.000000 tulona-0.3.2/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:09:13.490989 tulona-0.3.2/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-04-10 18:09:13.000000 tulona-0.3.2/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-10 18:09:13.000000 tulona-0.3.2/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:09:13.000000 tulona-0.3.2/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 18:09:13.000000 tulona-0.3.2/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-10 18:09:13.000000 tulona-0.3.2/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 18:09:13.000000 tulona-0.3.2/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-10 18:09:04.000000 tulona-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:09:13.490989 tulona-0.3.2/setup.cfg
```

### Comparing `tulona-0.3.1/LICENSE` & `tulona-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/PKG-INFO` & `tulona-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.3.1
+Version: 0.3.2
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -144,41 +144,34 @@
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
+
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
 * **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
+
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
 * **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
-  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
+  * Column[s] to compare is[are] specified in `tulona-project.yml` file as part of datasource configs, with `compare_column` property. Sample command:
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
 For debug level log, add `-v` or `--verbose` flag along with any command. For example:
```

### Comparing `tulona-0.3.1/README.rst` & `tulona-0.3.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -111,41 +111,34 @@
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
+
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
 * **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
+
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
 * **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
-  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
+  * Column[s] to compare is[are] specified in `tulona-project.yml` file as part of datasource configs, with `compare_column` property. Sample command:
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
 For debug level log, add `-v` or `--verbose` flag along with any command. For example:
```

### Comparing `tulona-0.3.1/core/tulona/adapter/connection.py` & `tulona-0.3.2/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/adapter/mssql.py` & `tulona-0.3.2/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/adapter/mysql.py` & `tulona-0.3.2/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/adapter/postgres.py` & `tulona-0.3.2/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/adapter/snowflake.py` & `tulona-0.3.2/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/cli/base.py` & `tulona-0.3.2/core/tulona/cli/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     # Override config outdir if provided in command line
     if kwargs["outdir"]:
         ctx.obj["project"]["outdir"] = kwargs["outdir"]
     outfile_fqn = get_outfile_fqn(
         outdir=ctx.obj["project"]["outdir"],
         ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-        infix="data_comparison",
+        infix="profiling",
     )
 
     task = ProfileTask(
         profile=ctx.obj["profile"],
         project=ctx.obj["project"],
         runtime=ctx.obj["runtime"],
         datasources=datasource_list,
@@ -174,24 +174,17 @@
 # @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 def compare_column(ctx, **kwargs):
     """
     Column name must be specified for task: compare-column
-    either by specifying 'compare_column' property in
-    at least one of the datasource[project] configs
+    by specifying 'compare_column' property in
+    all the datasource[project] configs
     (check sample tulona-project.yml file for example)
-    or with '--datasources' command line argument
-    using one of the following formats
-    (column name is same for option 3 and 4):-
-    1. <datasource1>:<col1>,<datasource2>:<col2>
-    2. <datasource1>:<col>,<datasource2>:<col>
-    3. <datasource1>:<col>,<datasource2>
-    4. <datasource1>,<datasource2>:<col>
     """
 
     if not kwargs["datasources"]:
         raise TulonaMissingArgumentError(
             "--datasources argument must be provided with command: compare-column"
         )
```

### Comparing `tulona-0.3.1/core/tulona/cli/params.py` & `tulona-0.3.2/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/config/profile.py` & `tulona-0.3.2/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/config/project.py` & `tulona-0.3.2/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/exceptions.py` & `tulona-0.3.2/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/task/base.py` & `tulona-0.3.2/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/task/compare.py` & `tulona-0.3.2/core/tulona/task/compare.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from tulona.task.base import BaseTask
 from tulona.task.helper import perform_comparison
 from tulona.task.profile import ProfileTask
 from tulona.util.dataframe import apply_column_exclusion
 from tulona.util.excel import highlight_mismatch_cells
 from tulona.util.filesystem import create_dir_if_not_exist
 from tulona.util.profiles import extract_profile_name, get_connection_profile
-from tulona.util.project import extract_table_name_from_config
 from tulona.util.sql import (
     build_filter_query_expression,
     get_column_query,
     get_query_output_as_df,
     get_table_data_query,
     get_table_fqn,
 )
@@ -134,15 +133,14 @@
 
         # Config extraction
         dbtype1, dbtype2 = dbtypes
         table_fqn1, table_fqn2 = table_fqns
         conman1, conman2 = connection_managers
         exclude_columns1, exclude_columns2 = exclude_columns_lol
 
-        log.info("Extracting row data")
         # TODO: push column exclusion down to the database/query
         primary_key = primary_key.lower()
         query_expr = None
 
         i = 0
         while i < 5:
             log.debug(f"Extraction iteration: {i + 1}/5")
@@ -205,15 +203,15 @@
                 f"Could not find common data between {table_fqn1} and {table_fqn2}"
             )
 
         log.debug("Preparing row comparison")
         df_row_comp = perform_comparison(
             ds_name_compressed_list, row_data_list, primary_key
         )
-        log.debug(f"Prepared comparision for {df_row_comp.shape[0]} rows")
+        log.debug(f"Prepared comparison for {df_row_comp.shape[0]} rows")
 
         log.debug(f"Writing comparison result into: {self.outfile_fqn}")
         _ = create_dir_if_not_exist(self.project["outdir"])
         with pd.ExcelWriter(
             self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
         ) as writer:
             df_row_comp.to_excel(writer, sheet_name="Row Comparison", index=False)
@@ -259,94 +257,100 @@
     def execute(self):
         log.info("------------------------ Starting task: compare-column")
         start_time = time.time()
 
         if len(self.datasources) != 2:
             raise ValueError("Comparison works between two entities, not more, not less.")
 
-        datasource1, datasource2 = self.datasources
-        if ":" in datasource1 and ":" in datasource2:
-            datasource1, column1 = datasource1.split(":")
-            datasource2, column2 = datasource2.split(":")
-        elif ":" in datasource1:
-            datasource1, column1 = datasource1.split(":")
-            column2 = column1
-        elif ":" in datasource2:
-            datasource2, column2 = datasource2.split(":")
-            column1 = column2
-        elif (
-            "compare_column" in self.project["datasources"][datasource1]
-            and "compare_column" in self.project["datasources"][datasource2]
-        ):
-            column1 = self.project["datasources"][datasource1]["compare_column"]
-            column2 = self.project["datasources"][datasource2]["compare_column"]
-        elif "compare_column" in self.project["datasources"][datasource1]:
-            column1 = self.project["datasources"][datasource1]["compare_column"]
-            column2 = column1
-        elif "compare_column" in self.project["datasources"][datasource2]:
-            column2 = self.project["datasources"][datasource2]["compare_column"]
-            column1 = column2
-        else:
-            raise TulonaMissingPropertyError(
-                "Column name must be specified for task: compare-column"
-                " either by specifying 'compare_column' property in"
-                " at least one of the datasource[project] configs"
-                " (check sample tulona-project.yml file for example)"
-                " or with '--datasources' command line argument"
-                " using one of the following formats"
-                " (column name is same for option 3 and 4):-"
-                " 1. <datasource1>:<col1>,<datasource2>:<col2>"
-                " 2. <datasource1>:<col>,<datasource2>:<col>"
-                " 3. <datasource1>:<col>,<datasource2>"
-                " 4. <datasource1>,<datasource2>:<col>"
-            )
-
-        ds_dict1 = self.project["datasources"][datasource1]
-        ds_dict2 = self.project["datasources"][datasource2]
-
-        dbtype1 = self.profile["profiles"][
-            extract_profile_name(self.project, datasource1)
-        ]["type"]
-        dbtype2 = self.profile["profiles"][
-            extract_profile_name(self.project, datasource2)
-        ]["type"]
-        table_name1 = extract_table_name_from_config(config=ds_dict1, dbtype=dbtype1)
-        table_name2 = extract_table_name_from_config(config=ds_dict2, dbtype=dbtype2)
-
-        log.debug(f"Extracting data from table: {table_name1}")
-        df1 = self.get_column_data(datasource1, table_name1, column1)
-        log.debug(f"Extracting data from table: {table_name2}")
-        df2 = self.get_column_data(datasource2, table_name2, column2)
-
-        df1 = df1.rename(columns={c: c.lower() for c in df2.columns})
-        df2 = df2.rename(columns={c: c.lower() for c in df2.columns})
-        column1, column2 = column1.lower(), column2.lower()
-
-        ds1_compressed = datasource1.replace("_", "")
-        ds2_compressed = datasource2.replace("_", "")
-
-        df_merge = pd.merge(
-            left=df1,
-            right=df2,
-            left_on=column1,
-            right_on=column2,
+        ds_compressed_names = []
+        compare_columns = []
+        column_df_list = []
+        for ds_name in self.datasources:
+            log.info(f"Processing data source {ds_name}")
+            ds_compressed_names.append(ds_name.replace("_", ""))
+            ds_config = self.project["datasources"][ds_name]
+
+            if "compare_column" in ds_config:
+                column = ds_config["compare_column"]
+                compare_columns.append(column)
+            else:
+                raise TulonaMissingPropertyError(
+                    "Property 'compare_column' must be specified for column comparison"
+                )
+            log.debug(f"Extracting data for column {column}")
+
+            dbtype = self.profile["profiles"][
+                extract_profile_name(self.project, ds_name)
+            ]["type"]
+            log.debug(f"Database type: {dbtype}")
+
+            # MySQL doesn't have logical database
+            if "database" in ds_config and dbtype.lower() != "mysql":
+                database = ds_config["database"]
+            else:
+                database = None
+            schema = ds_config["schema"]
+            table = ds_config["table"]
+            table_fqn = get_table_fqn(database, schema, table)
+            log.debug(f"Table FQN: {table_fqn}")
+
+            log.debug(f"Acquiring connection to the database of: {ds_name}")
+            connection_profile = get_connection_profile(
+                self.profile, self.project, ds_name
+            )
+            conman = self.get_connection_manager(conn_profile=connection_profile)
+
+            query = get_column_query(table_fqn, column)
+            try:
+                log.debug(f"Trying unquoted column name: {column}")
+                log.debug(f"Executing query: {query}")
+                df = get_query_output_as_df(connection_manager=conman, query_text=query)
+            except Exception as exp:
+                log.warning(f"Failed with error: {exp}")
+                log.debug(f'Trying quoted column name: "{column}"')
+                query = get_column_query(table_fqn, column, quoted=True)
+                log.debug(f"Executing query: {query}")
+                df = get_query_output_as_df(connection_manager=conman, query_text=query)
+
+            if df.shape[0] == 0:
+                raise ValueError(f"Table {table_fqn} doesn't have any data")
+
+            log.debug(f"Found {df.shape[0]} records in {table_fqn}")
+
+            df = df.rename(columns={c: c.lower() for c in df.columns})
+            column_df_list.append(df)
+
+        compare_columns = {c.lower() for c in compare_columns}
+        if len(compare_columns) > 1:
+            raise ValueError(
+                "Column comparison works only when the column name is same for both data source"
+                "(not case sensitive)"
+            )
+
+        log.debug("Perform comparison")
+        df_comp = perform_comparison(
+            ds_compressed_names=ds_compressed_names,
+            dataframes=column_df_list,
+            on=compare_columns.pop(),
             how="outer",
-            suffixes=("_left_" + ds1_compressed, "_right_" + ds2_compressed),
-            validate="one_to_one",
             indicator="presence",
+            validate="one_to_one",
         )
-        df_merge = df_merge[df_merge["presence"] != "both"]
-        log.debug(f"Found {df_merge.shape[0]} extra values both side combined")
+        df_comp = df_comp[df_comp["presence"] != "both"]
+        df_comp["presence"] = df_comp["presence"].map(
+            {"left_only": ds_compressed_names[0], "right_only": ds_compressed_names[1]}
+        )
+        log.debug(f"Found {df_comp.shape[0]} mismatches both side combined")
 
         log.debug(f"Writing output into: {self.outfile_fqn}")
         _ = create_dir_if_not_exist(self.project["outdir"])
         with pd.ExcelWriter(
             self.outfile_fqn, mode="a" if os.path.exists(self.outfile_fqn) else "w"
         ) as writer:
-            df_merge.to_excel(writer, sheet_name="Column Comparison", index=False)
+            df_comp.to_excel(writer, sheet_name="Column Comparison", index=False)
 
         end_time = time.time()
         log.info("------------------------ Finished task: compare-column")
         log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
 
 
 @dataclass
@@ -369,40 +373,49 @@
                 setattr(self, field.name, field.default)
 
     def execute(self):
         log.info("------------------------ Starting task: compare")
         start_time = time.time()
 
         # Metadata comparison
-        ProfileTask(
-            profile=self.profile,
-            project=self.project,
-            runtime=self.runtime,
-            datasources=self.datasources,
-            outfile_fqn=self.outfile_fqn,
-            compare=True,
-        ).execute()
+        try:
+            ProfileTask(
+                profile=self.profile,
+                project=self.project,
+                runtime=self.runtime,
+                datasources=self.datasources,
+                outfile_fqn=self.outfile_fqn,
+                compare=True,
+            ).execute()
+        except Exception as exc:
+            log.error(f"Profiling failed with error: {exc}")
 
         # Row comparison
-        CompareDataTask(
-            profile=self.profile,
-            project=self.project,
-            runtime=self.runtime,
-            datasources=self.datasources,
-            outfile_fqn=self.outfile_fqn,
-            sample_count=self.sample_count,
-        ).execute()
+        try:
+            CompareDataTask(
+                profile=self.profile,
+                project=self.project,
+                runtime=self.runtime,
+                datasources=self.datasources,
+                outfile_fqn=self.outfile_fqn,
+                sample_count=self.sample_count,
+            ).execute()
+        except Exception as exc:
+            log.error(f"Row comparison failed with error: {exc}")
 
         # Column comparison
-        CompareColumnTask(
-            profile=self.profile,
-            project=self.project,
-            runtime=self.runtime,
-            datasources=self.datasources,
-            outfile_fqn=self.outfile_fqn,
-        ).execute()
+        try:
+            CompareColumnTask(
+                profile=self.profile,
+                project=self.project,
+                runtime=self.runtime,
+                datasources=self.datasources,
+                outfile_fqn=self.outfile_fqn,
+            ).execute()
+        except Exception as exc:
+            log.error(f"Column comparison failed with error: {exc}")
 
         end_time = time.time()
         log.info("------------------------ Finished task: compare")
         log.info(
             f"Total time taken [profile, compare-data, compare-column]: {(end_time - start_time):.2f} seconds"
         )
```

### Comparing `tulona-0.3.1/core/tulona/task/helper.py` & `tulona-0.3.2/core/tulona/task/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import List
+from typing import List, Optional, Tuple, Union
 
 import pandas as pd
 
 from tulona.adapter.connection import ConnectionManager
 from tulona.util.sql import (
     get_metadata_query,
     get_metric_query,
@@ -71,17 +71,23 @@
     df = pd.merge(left=df_meta, right=df_metric, how="inner", on="column_name")
 
     return df
 
 
 # TODO: common param to toggle comparison result for common vs all columns
 def perform_comparison(
-    ds_compressed_names: List[str], dataframes: List[pd.DataFrame], primary_key: str
+    ds_compressed_names: List[str],
+    dataframes: List[pd.DataFrame],
+    on: str,
+    how: str = "inner",
+    suffixes: Tuple[str] = ("_x", "_y"),
+    indicator: Union[bool, str] = False,
+    validate: Optional[str] = None,
 ) -> pd.DataFrame:
-    primary_key = primary_key.lower()
+    primary_key = on.lower()
     common_columns = {c.lower() for c in dataframes[0].columns.tolist()}
 
     dataframes_final = []
     for df in dataframes[1:]:
         colset = {c.lower() for c in df.columns.tolist()}
         common_columns = common_columns.intersection(colset)
 
@@ -95,11 +101,19 @@
         )
         if pd.api.types.is_string_dtype(df[primary_key]):
             df[primary_key] = df[primary_key].str.lower()
         dataframes_final.append(df)
 
     df_merge = dataframes_final.pop()
     for df in dataframes_final:
-        df_merge = pd.merge(left=df_merge, right=df, on=primary_key, how="inner")
+        df_merge = pd.merge(
+            left=df_merge,
+            right=df,
+            on=primary_key,
+            how=how,
+            suffixes=suffixes,
+            indicator=indicator,
+            validate=validate,
+        )
     df_merge = df_merge[sorted(df_merge.columns.tolist())]
 
     return df_merge
```

### Comparing `tulona-0.3.1/core/tulona/task/ping.py` & `tulona-0.3.2/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/task/profile.py` & `tulona-0.3.2/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/task/scan.py` & `tulona-0.3.2/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/util/database.py` & `tulona-0.3.2/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/util/dataframe.py` & `tulona-0.3.2/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/util/excel.py` & `tulona-0.3.2/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/util/filesystem.py` & `tulona-0.3.2/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/util/profiles.py` & `tulona-0.3.2/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.1/core/tulona/util/sql.py` & `tulona-0.3.2/core/tulona/util/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         raise TulonaNotImplementedError(
             f"Extracting sample rows from source type {dbtype} is not implemented."
         )
 
     return query
 
 
-def get_column_query(table_name: str, column: str, quoted=False):
+def get_column_query(table_fqn: str, column: str, quoted=False):
     if quoted:
-        query = f"""select "{column}" from {table_name}"""
+        query = f"""select "{column}" from {table_fqn}"""
     else:
-        query = f"""select {column} from {table_name}"""
+        query = f"""select {column} from {table_fqn}"""
 
     return query
 
 
 def get_query_output_as_df(connection_manager, query_text: str):
     with connection_manager.engine.connect() as conn:
         df = pd.read_sql_query(query_text, conn)
```

### Comparing `tulona-0.3.1/core/tulona.egg-info/PKG-INFO` & `tulona-0.3.2/core/tulona.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.3.1
+Version: 0.3.2
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -144,41 +144,34 @@
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
+
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
 * **compare-data**: To compare sample data from two sources/tables. It will create a comparative view of all common columns from both sources/tables side by side (like: id_ds1 <-> id_ds2) and highlight mismatched values in the output excel file. By default it compares 20 common rows from both tables (subject to availabillity) but the number can be overridden with the command line argument `--sample-count`. Command samples:
 
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
+
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
 * **compare-column**: To compare columns from tables from two sources/tables. This is expecially useful when you want see if all the rows from one table/source is present in the other one by comparing the primary/unique key. The result will be an excel file with extra primary/unique keys from both sides. If both have the same set of primary/unique keys, essentially means they have the same rows, excel file will be empty. Command samples:
 
-  * Column[s] to compare is[are] specified in at least one of the datasource config in `tulona-project.yml` file with `compare_column` property:
+  * Column[s] to compare is[are] specified in `tulona-project.yml` file as part of datasource configs, with `compare_column` property. Sample command:
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the first data source, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with the second data source, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres,employee_mysql:Employee_ID``
-  * Column[s] to compare may/may not be specified in the datasource config in `tulona-project.yml` file with `compare_column` property(command line takes preference). In the command, column name is specified with both data sources, separated by colon(:):
-
-    ``tulona compare-column --datasources employee_postgres:Employee_ID,employee_mysql:Employee_ID``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
 For debug level log, add `-v` or `--verbose` flag along with any command. For example:
```

### Comparing `tulona-0.3.1/core/tulona.egg-info/SOURCES.txt` & `tulona-0.3.2/core/tulona.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,10 +29,9 @@
 core/tulona/task/scan.py
 core/tulona/util/__init__.py
 core/tulona/util/database.py
 core/tulona/util/dataframe.py
 core/tulona/util/excel.py
 core/tulona/util/filesystem.py
 core/tulona/util/profiles.py
-core/tulona/util/project.py
 core/tulona/util/sql.py
 core/tulona/util/yaml_parser.py
```

### Comparing `tulona-0.3.1/pyproject.toml` & `tulona-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.3.1"
+version = "0.3.2"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -96,15 +96,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.3.1"
+current_version = "0.3.2"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
```

