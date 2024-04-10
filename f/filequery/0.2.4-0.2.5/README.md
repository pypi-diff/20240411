# Comparing `tmp/filequery-0.2.4.tar.gz` & `tmp/filequery-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filequery-0.2.4.tar", last modified: Fri Mar  1 03:42:01 2024, max compression
+gzip compressed data, was "filequery-0.2.5.tar", last modified: Wed Apr 10 22:58:45 2024, max compression
```

## Comparing `filequery-0.2.4.tar` & `filequery-0.2.5.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.627833 filequery-0.2.4/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1818 2023-02-19 00:56:16.000000 filequery-0.2.4/.gitignore
--rw-rw-r--   0 markus    (1000) markus    (1000)     1070 2023-02-19 00:24:28.000000 filequery-0.2.4/LICENSE
--rw-rw-r--   0 markus    (1000) markus    (1000)      330 2023-02-25 04:29:27.000000 filequery-0.2.4/Makefile
--rw-r--r--   0 markus    (1000) markus    (1000)     6323 2024-03-01 03:42:01.627833 filequery-0.2.4/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     5447 2024-02-29 04:12:58.000000 filequery-0.2.4/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.619833 filequery-0.2.4/example/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.619833 filequery-0.2.4/example/config_files/
--rw-rw-r--   0 markus    (1000) markus    (1000)       86 2023-03-10 02:53:30.000000 filequery-0.2.4/example/config_files/example0.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      115 2023-03-10 02:53:30.000000 filequery-0.2.4/example/config_files/example1.json
--rw-rw-r--   0 markus    (1000) markus    (1000)       94 2023-03-10 02:53:30.000000 filequery-0.2.4/example/config_files/example2.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      117 2023-03-10 02:53:30.000000 filequery-0.2.4/example/config_files/example3.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      155 2023-03-10 02:53:30.000000 filequery-0.2.4/example/config_files/example4.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      186 2023-03-23 01:10:40.000000 filequery-0.2.4/example/config_files/example5.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      147 2023-03-23 01:10:40.000000 filequery-0.2.4/example/config_files/example6.json
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.619833 filequery-0.2.4/example/data/
--rw-rw-r--   0 markus    (1000) markus    (1000)      353 2023-03-11 23:35:48.000000 filequery-0.2.4/example/data/json_test.json
--rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-02-24 02:58:55.000000 filequery-0.2.4/example/data/test.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)       69 2023-02-24 02:59:42.000000 filequery-0.2.4/example/data/test1.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)      231 2023-03-11 23:35:48.000000 filequery-0.2.4/example/json_list_test.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      200 2023-03-11 23:35:48.000000 filequery-0.2.4/example/json_test.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      260 2023-05-03 23:49:19.000000 filequery-0.2.4/example/ndjson_test.ndjson
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.623833 filequery-0.2.4/example/queries/
--rw-rw-r--   0 markus    (1000) markus    (1000)       75 2023-02-24 03:03:29.000000 filequery-0.2.4/example/queries/join.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.2.4/example/queries/json_csv_join.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.2.4/example/queries/json_query.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      120 2023-11-10 03:49:23.000000 filequery-0.2.4/example/queries/multi_query.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-11-20 23:45:42.000000 filequery-0.2.4/example/test.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)      632 2024-03-01 03:39:26.000000 filequery-0.2.4/pyproject.toml
--rw-rw-r--   0 markus    (1000) markus    (1000)      740 2024-02-29 04:12:58.000000 filequery-0.2.4/requirements-dev.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-02-29 04:12:58.000000 filequery-0.2.4/requirements.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       38 2024-03-01 03:42:01.627833 filequery-0.2.4/setup.cfg
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.615833 filequery-0.2.4/src/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.623833 filequery-0.2.4/src/filequery/
--rw-rw-r--   0 markus    (1000) markus    (1000)     6422 2023-11-30 01:17:27.000000 filequery-0.2.4/src/filequery/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)       78 2023-11-10 03:49:23.000000 filequery-0.2.4/src/filequery/__main__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      225 2023-11-10 03:49:23.000000 filequery-0.2.4/src/filequery/exceptions.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      248 2023-11-10 03:49:23.000000 filequery-0.2.4/src/filequery/file_query_args.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4072 2024-03-01 03:39:13.000000 filequery-0.2.4/src/filequery/filedb.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      102 2023-11-10 03:49:23.000000 filequery-0.2.4/src/filequery/filetype.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2925 2024-03-01 03:39:13.000000 filequery-0.2.4/src/filequery/queryresult.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.627833 filequery-0.2.4/src/filequery/tui/
--rw-rw-r--   0 markus    (1000) markus    (1000)    13040 2024-02-29 04:13:13.000000 filequery-0.2.4/src/filequery/tui/duckui.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2104 2024-01-13 23:26:57.000000 filequery-0.2.4/src/filequery/tui/help_content.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.627833 filequery-0.2.4/src/filequery/tui/screens/
--rw-rw-r--   0 markus    (1000) markus    (1000)      772 2024-02-29 04:13:13.000000 filequery-0.2.4/src/filequery/tui/screens/file_browser.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     1457 2024-02-29 04:13:13.000000 filequery-0.2.4/src/filequery/tui/screens/menu.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      159 2024-02-29 04:13:13.000000 filequery-0.2.4/src/filequery/tui/screens/menu_events.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.627833 filequery-0.2.4/src/filequery/tui/styles/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-02-29 04:13:13.000000 filequery-0.2.4/src/filequery/tui/styles/style.tcss
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.627833 filequery-0.2.4/src/filequery.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     6323 2024-03-01 03:42:01.000000 filequery-0.2.4/src/filequery.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1298 2024-03-01 03:42:01.000000 filequery-0.2.4/src/filequery.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-03-01 03:42:01.000000 filequery-0.2.4/src/filequery.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       55 2024-03-01 03:42:01.000000 filequery-0.2.4/src/filequery.egg-info/entry_points.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-03-01 03:42:01.000000 filequery-0.2.4/src/filequery.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       10 2024-03-01 03:42:01.000000 filequery-0.2.4/src/filequery.egg-info/top_level.txt
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-03-01 03:42:01.627833 filequery-0.2.4/tests/
--rw-rw-r--   0 markus    (1000) markus    (1000)        0 2023-02-19 00:27:10.000000 filequery-0.2.4/tests/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    10538 2024-03-01 03:39:13.000000 filequery-0.2.4/tests/test_filequery.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.207952 filequery-0.2.5/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1818 2023-02-19 00:56:16.000000 filequery-0.2.5/.gitignore
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1070 2023-02-19 00:24:28.000000 filequery-0.2.5/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)      330 2024-04-10 22:57:14.000000 filequery-0.2.5/Makefile
+-rw-r--r--   0 markus    (1000) markus    (1000)     6323 2024-04-10 22:58:45.207952 filequery-0.2.5/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     5447 2024-02-29 04:12:58.000000 filequery-0.2.5/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.199952 filequery-0.2.5/example/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.199952 filequery-0.2.5/example/config_files/
+-rw-rw-r--   0 markus    (1000) markus    (1000)       86 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example0.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      115 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example1.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)       94 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example2.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      117 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example3.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      155 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example4.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      186 2023-03-23 01:10:40.000000 filequery-0.2.5/example/config_files/example5.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      147 2023-03-23 01:10:40.000000 filequery-0.2.5/example/config_files/example6.json
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.199952 filequery-0.2.5/example/data/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      353 2023-03-11 23:35:48.000000 filequery-0.2.5/example/data/json_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-02-24 02:58:55.000000 filequery-0.2.5/example/data/test.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)       69 2023-02-24 02:59:42.000000 filequery-0.2.5/example/data/test1.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)       48 2024-04-10 22:55:58.000000 filequery-0.2.5/example/data/test_null.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)      231 2023-03-11 23:35:48.000000 filequery-0.2.5/example/json_list_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      200 2023-03-11 23:35:48.000000 filequery-0.2.5/example/json_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      260 2023-05-03 23:49:19.000000 filequery-0.2.5/example/ndjson_test.ndjson
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/example/queries/
+-rw-rw-r--   0 markus    (1000) markus    (1000)       75 2023-02-24 03:03:29.000000 filequery-0.2.5/example/queries/join.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.2.5/example/queries/json_csv_join.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.2.5/example/queries/json_query.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      120 2023-11-10 03:49:23.000000 filequery-0.2.5/example/queries/multi_query.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-11-20 23:45:42.000000 filequery-0.2.5/example/test.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)      632 2024-04-10 22:56:32.000000 filequery-0.2.5/pyproject.toml
+-rw-rw-r--   0 markus    (1000) markus    (1000)      740 2024-03-29 01:47:08.000000 filequery-0.2.5/requirements-dev.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-03-29 01:46:52.000000 filequery-0.2.5/requirements.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2024-04-10 22:58:45.207952 filequery-0.2.5/setup.cfg
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.195952 filequery-0.2.5/src/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     6422 2023-11-30 01:17:27.000000 filequery-0.2.5/src/filequery/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)       78 2023-11-10 03:49:23.000000 filequery-0.2.5/src/filequery/__main__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      225 2023-11-10 03:49:23.000000 filequery-0.2.5/src/filequery/exceptions.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      248 2023-11-10 03:49:23.000000 filequery-0.2.5/src/filequery/file_query_args.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4067 2024-04-10 22:36:41.000000 filequery-0.2.5/src/filequery/filedb.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      102 2023-11-10 03:49:23.000000 filequery-0.2.5/src/filequery/filetype.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2925 2024-03-01 05:00:43.000000 filequery-0.2.5/src/filequery/queryresult.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery/tui/
+-rw-rw-r--   0 markus    (1000) markus    (1000)    12714 2024-04-10 22:55:58.000000 filequery-0.2.5/src/filequery/tui/duckui.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2104 2024-01-13 23:26:57.000000 filequery-0.2.5/src/filequery/tui/help_content.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery/tui/screens/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      772 2024-02-29 04:13:13.000000 filequery-0.2.5/src/filequery/tui/screens/file_browser.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1457 2024-02-29 04:13:13.000000 filequery-0.2.5/src/filequery/tui/screens/menu.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      159 2024-02-29 04:13:13.000000 filequery-0.2.5/src/filequery/tui/screens/menu_events.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery/tui/styles/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-02-29 04:13:13.000000 filequery-0.2.5/src/filequery/tui/styles/style.tcss
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     6323 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1325 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       55 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/entry_points.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       10 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/top_level.txt
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/tests/
+-rw-rw-r--   0 markus    (1000) markus    (1000)        0 2023-02-19 00:27:10.000000 filequery-0.2.5/tests/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    10538 2024-04-08 02:25:37.000000 filequery-0.2.5/tests/test_filequery.py
```

### Comparing `filequery-0.2.4/.gitignore` & `filequery-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/LICENSE` & `filequery-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/PKG-INFO` & `filequery-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: filequery
-Version: 0.2.4
+Version: 0.2.5
 Summary: Query CSV and Parquet files using SQL
 Author-email: Markus Hutnik <markus@markushutnik.com>
 License: MIT
 Project-URL: repository, https://github.com/MarkyMan4/filequery
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: duckdb==0.10.0
+Requires-Dist: duckdb==0.10.1
 Requires-Dist: importlib-metadata==6.8.0
 Requires-Dist: linkify-it-py==2.0.2
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdit-py-plugins==0.4.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: numpy==1.26.1
 Requires-Dist: Pygments==2.16.1
```

### Comparing `filequery-0.2.4/README.md` & `filequery-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/pyproject.toml` & `filequery-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "filequery"
 authors = [{ name = "Markus Hutnik", email = "markus@markushutnik.com" }]
 description = "Query CSV and Parquet files using SQL"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = ["Programming Language :: Python :: 3"]
 license = { text = "MIT" }
-version = "0.2.4"
+version = "0.2.5"
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [project.scripts]
 filequery = "filequery:fq_cli_handler"
```

### Comparing `filequery-0.2.4/requirements-dev.txt` & `filequery-0.2.5/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 bleach==6.0.0
 build==0.10.0
 certifi==2022.12.7
 cffi==1.15.1
 charset-normalizer==3.0.1
 cryptography==39.0.1
 docutils==0.19
-duckdb==0.10.0
+duckdb==0.10.1
 idna==3.4
 importlib-metadata==6.8.0
 jaraco.classes==3.2.3
 jeepney==0.8.0
 keyring==23.13.1
 linkify-it-py==2.0.2
 markdown-it-py==3.0.0
```

### Comparing `filequery-0.2.4/src/filequery/__init__.py` & `filequery-0.2.5/src/filequery/__init__.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/src/filequery/filedb.py` & `filequery-0.2.5/src/filequery/filedb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import duckdb
 
 from .exceptions import InvalidFileTypeException
 from .filetype import FileType
 from .queryresult import QueryResult
 
 READ_FUNCS = {
-    FileType.CSV: "read_csv_auto",
+    FileType.CSV: "read_csv",
     FileType.PARQUET: "read_parquet",
     FileType.JSON: "read_json_auto",
     FileType.NDJSON: "read_ndjson_auto",
 }
 
 # mapping from file extension to FileType
 FILE_EXT_MAP = {
```

### Comparing `filequery-0.2.4/src/filequery/queryresult.py` & `filequery-0.2.5/src/filequery/queryresult.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/src/filequery/tui/duckui.py` & `filequery-0.2.5/src/filequery/tui/duckui.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         self.conn = conn
 
         if self.conn is None:
             self.conn = duckdb.connect(":memory:")
 
         # mapping from tab ID to editor content, tab IDs are "tab-1", "tab-2" and so on
         self.tab_content = defaultdict(str)
+        
+        # keep track of last query ran, so if user exports result, can use a duckdb copy statement
+        self.last_query = ""
 
         super().__init__()
 
     def _get_table_list(self) -> List[str]:
         """
         get the list of tables in the database
 
@@ -139,27 +142,15 @@
         # after submit, hide this dialog and refocus on text editor
         self.save_sql_input.display = False
         self.text_area.focus()
 
     @on(Input.Submitted, selector="#result-file-input")
     def handle_result_file_name_input(self):
         try:
-            with open(self.save_result_input.value, "w") as f:
-                cols = self.result_table.columns
-                rows = self.result_table._data
-
-                formatted_cols = [f'"{cols[col].label}"' for col in cols]
-                f.write(",".join(formatted_cols))
-                f.write("\n")
-
-                for row in rows:
-                    row_data = rows[row]
-                    formatted_row = [f'"{row_data[col]}"' for col in row_data]
-                    f.write(",".join(formatted_row))
-                    f.write("\n")
+            self.conn.execute(f"copy ({self.last_query}) to '{self.save_result_input.value}' (header)")
         except:
             # ignore for now, find a way to display an error message
             pass
 
         # after submit, hide this dialog and refocus on text editor
         self.save_result_input.display = False
         self.text_area.focus()
@@ -356,26 +347,25 @@
 
         result = None
         cur = self.conn.cursor()
 
         try:
             cur.execute(query)
             result = cur.fetchall()
+            self.last_query = query
         except Exception as e:
             self._display_error_in_table(str(e))
             cur.close()
             return
 
         try:
             col_names = [col[0] for col in cur.description]
             self.result_table.clear(columns=True)
             self.result_table.add_columns(*col_names)
             self.result_table.add_rows(result)
         except Exception as e:
             self._display_error_in_table(str(e))
         finally:
             cur.close()
-            cur.close()
-            cur.close()
 
         # after executing a statement, update the table list in case any tables were created or dropped
         self._refresh_table_tree()
```

### Comparing `filequery-0.2.4/src/filequery/tui/help_content.py` & `filequery-0.2.5/src/filequery/tui/help_content.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/src/filequery/tui/screens/file_browser.py` & `filequery-0.2.5/src/filequery/tui/screens/file_browser.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/src/filequery/tui/screens/menu.py` & `filequery-0.2.5/src/filequery/tui/screens/menu.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/src/filequery/tui/styles/style.tcss` & `filequery-0.2.5/src/filequery/tui/styles/style.tcss`

 * *Files identical despite different names*

### Comparing `filequery-0.2.4/src/filequery.egg-info/PKG-INFO` & `filequery-0.2.5/src/filequery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: filequery
-Version: 0.2.4
+Version: 0.2.5
 Summary: Query CSV and Parquet files using SQL
 Author-email: Markus Hutnik <markus@markushutnik.com>
 License: MIT
 Project-URL: repository, https://github.com/MarkyMan4/filequery
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: duckdb==0.10.0
+Requires-Dist: duckdb==0.10.1
 Requires-Dist: importlib-metadata==6.8.0
 Requires-Dist: linkify-it-py==2.0.2
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdit-py-plugins==0.4.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: numpy==1.26.1
 Requires-Dist: Pygments==2.16.1
```

### Comparing `filequery-0.2.4/src/filequery.egg-info/SOURCES.txt` & `filequery-0.2.5/src/filequery.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 example/config_files/example3.json
 example/config_files/example4.json
 example/config_files/example5.json
 example/config_files/example6.json
 example/data/json_test.json
 example/data/test.csv
 example/data/test1.csv
+example/data/test_null.csv
 example/queries/join.sql
 example/queries/json_csv_join.sql
 example/queries/json_query.sql
 example/queries/multi_query.sql
 src/filequery/__init__.py
 src/filequery/__main__.py
 src/filequery/exceptions.py
```

### Comparing `filequery-0.2.4/tests/test_filequery.py` & `filequery-0.2.5/tests/test_filequery.py`

 * *Files identical despite different names*

