# Comparing `tmp/orso-0.0.97.tar.gz` & `tmp/orso-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orso-0.0.97.tar", last modified: Sat Sep  2 12:41:09 2023, max compression
+gzip compressed data, was "orso-0.0.99.tar", last modified: Wed Sep  6 01:06:03 2023, max compression
```

## Comparing `orso-0.0.97.tar` & `orso-0.0.99.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.841451 orso-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (999)    11346 2023-09-02 12:40:57.000000 orso-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     2396 2023-09-02 12:41:09.841451 orso-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2167 2023-09-02 12:40:57.000000 orso-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.837451 orso-0.0.97/orso/
--rw-r--r--   0 runner    (1001) docker     (999)      156 2023-09-02 12:40:57.000000 orso-0.0.97/orso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.837451 orso-0.0.97/orso/bitarray/
--rw-r--r--   0 runner    (1001) docker     (999)       32 2023-09-02 12:40:57.000000 orso-0.0.97/orso/bitarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)   400485 2023-09-02 12:40:57.000000 orso-0.0.97/orso/bitarray/cbitarray.c
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.837451 orso-0.0.97/orso/cityhash/
--rw-r--r--   0 runner    (1001) docker     (999)       92 2023-09-02 12:40:57.000000 orso-0.0.97/orso/cityhash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    19319 2023-09-02 12:40:57.000000 orso-0.0.97/orso/cityhash/city.cc
--rw-r--r--   0 runner    (1001) docker     (999)   237362 2023-09-02 12:40:57.000000 orso-0.0.97/orso/cityhash/cityhash.cpp
--rw-r--r--   0 runner    (1001) docker     (999)   220171 2023-09-02 12:41:09.000000 orso-0.0.97/orso/compiled.c
--rw-r--r--   0 runner    (1001) docker     (999)     3761 2023-09-02 12:40:57.000000 orso-0.0.97/orso/converters.py
--rw-r--r--   0 runner    (1001) docker     (999)    14645 2023-09-02 12:40:57.000000 orso-0.0.97/orso/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (999)    15140 2023-09-02 12:40:57.000000 orso-0.0.97/orso/display.py
--rw-r--r--   0 runner    (1001) docker     (999)     1822 2023-09-02 12:40:57.000000 orso-0.0.97/orso/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.837451 orso-0.0.97/orso/filters/
--rw-r--r--   0 runner    (1001) docker     (999)       78 2023-09-02 12:40:57.000000 orso-0.0.97/orso/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4436 2023-09-02 12:40:57.000000 orso-0.0.97/orso/filters/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (999)     3457 2023-09-02 12:40:57.000000 orso-0.0.97/orso/filters/cuckoo_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.837451 orso-0.0.97/orso/logging/
--rw-r--r--   0 runner    (1001) docker     (999)      142 2023-09-02 12:40:57.000000 orso-0.0.97/orso/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2922 2023-09-02 12:40:57.000000 orso-0.0.97/orso/logging/add_level.py
--rw-r--r--   0 runner    (1001) docker     (999)     1944 2023-09-02 12:40:57.000000 orso-0.0.97/orso/logging/create_logger.py
--rw-r--r--   0 runner    (1001) docker     (999)     4785 2023-09-02 12:40:57.000000 orso-0.0.97/orso/logging/google_cloud_logger.py
--rw-r--r--   0 runner    (1001) docker     (999)     1445 2023-09-02 12:40:57.000000 orso-0.0.97/orso/logging/levels.py
--rw-r--r--   0 runner    (1001) docker     (999)     4601 2023-09-02 12:40:57.000000 orso-0.0.97/orso/logging/log_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.837451 orso-0.0.97/orso/profiler/
--rw-r--r--   0 runner    (1001) docker     (999)       71 2023-09-02 12:40:57.000000 orso-0.0.97/orso/profiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.841451 orso-0.0.97/orso/profiler/distogram/
--rw-r--r--   0 runner    (1001) docker     (999)    15497 2023-09-02 12:40:57.000000 orso-0.0.97/orso/profiler/distogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     9326 2023-09-02 12:40:57.000000 orso-0.0.97/orso/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (999)     3500 2023-09-02 12:40:57.000000 orso-0.0.97/orso/row.py
--rw-r--r--   0 runner    (1001) docker     (999)    13468 2023-09-02 12:40:57.000000 orso-0.0.97/orso/schema.py
--rw-r--r--   0 runner    (1001) docker     (999)    11181 2023-09-02 12:40:57.000000 orso-0.0.97/orso/tools.py
--rw-r--r--   0 runner    (1001) docker     (999)     1874 2023-09-02 12:40:57.000000 orso-0.0.97/orso/types.py
--rw-r--r--   0 runner    (1001) docker     (999)      601 2023-09-02 12:40:57.000000 orso-0.0.97/orso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.837451 orso-0.0.97/orso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2396 2023-09-02 12:41:09.000000 orso-0.0.97/orso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1246 2023-09-02 12:41:09.000000 orso-0.0.97/orso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-02 12:41:09.000000 orso-0.0.97/orso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-09-02 12:41:09.000000 orso-0.0.97/orso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        5 2023-09-02 12:41:09.000000 orso-0.0.97/orso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      341 2023-09-02 12:40:57.000000 orso-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-02 12:41:09.841451 orso-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1492 2023-09-02 12:40:57.000000 orso-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 12:41:09.841451 orso-0.0.97/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     1554 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_bitarray.py
--rw-r--r--   0 runner    (1001) docker     (999)      952 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_cityhash.py
--rw-r--r--   0 runner    (1001) docker     (999)     4777 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_converters_arrow.py
--rw-r--r--   0 runner    (1001) docker     (999)      565 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_converters_pandas.py
--rw-r--r--   0 runner    (1001) docker     (999)      565 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_converters_polars.py
--rw-r--r--   0 runner    (1001) docker     (999)     7389 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (999)     2011 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_fetching.py
--rw-r--r--   0 runner    (1001) docker     (999)     2175 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_filter_bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1344 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_filter_cuckoo_filter.py
--rw-r--r--   0 runner    (1001) docker     (999)      950 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (999)      691 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (999)     1549 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_row.py
--rw-r--r--   0 runner    (1001) docker     (999)     5771 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (999)     7980 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_schema_columns.py
--rw-r--r--   0 runner    (1001) docker     (999)     2924 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_single_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (999)     1375 2023-09-02 12:40:57.000000 orso-0.0.97/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.316387 orso-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (999)    11346 2023-09-06 01:05:50.000000 orso-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     2396 2023-09-06 01:06:03.316387 orso-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2167 2023-09-06 01:05:50.000000 orso-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.312387 orso-0.0.99/orso/
+-rw-r--r--   0 runner    (1001) docker     (999)      156 2023-09-06 01:05:50.000000 orso-0.0.99/orso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.312387 orso-0.0.99/orso/bitarray/
+-rw-r--r--   0 runner    (1001) docker     (999)       32 2023-09-06 01:05:50.000000 orso-0.0.99/orso/bitarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)   400485 2023-09-06 01:05:50.000000 orso-0.0.99/orso/bitarray/cbitarray.c
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.312387 orso-0.0.99/orso/cityhash/
+-rw-r--r--   0 runner    (1001) docker     (999)       92 2023-09-06 01:05:50.000000 orso-0.0.99/orso/cityhash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19319 2023-09-06 01:05:50.000000 orso-0.0.99/orso/cityhash/city.cc
+-rw-r--r--   0 runner    (1001) docker     (999)   237362 2023-09-06 01:05:50.000000 orso-0.0.99/orso/cityhash/cityhash.cpp
+-rw-r--r--   0 runner    (1001) docker     (999)   220171 2023-09-06 01:06:03.000000 orso-0.0.99/orso/compiled.c
+-rw-r--r--   0 runner    (1001) docker     (999)     3761 2023-09-06 01:05:50.000000 orso-0.0.99/orso/converters.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14645 2023-09-06 01:05:50.000000 orso-0.0.99/orso/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15140 2023-09-06 01:05:50.000000 orso-0.0.99/orso/display.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1822 2023-09-06 01:05:50.000000 orso-0.0.99/orso/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.312387 orso-0.0.99/orso/filters/
+-rw-r--r--   0 runner    (1001) docker     (999)       78 2023-09-06 01:05:50.000000 orso-0.0.99/orso/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4436 2023-09-06 01:05:50.000000 orso-0.0.99/orso/filters/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3457 2023-09-06 01:05:50.000000 orso-0.0.99/orso/filters/cuckoo_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.316387 orso-0.0.99/orso/logging/
+-rw-r--r--   0 runner    (1001) docker     (999)      142 2023-09-06 01:05:50.000000 orso-0.0.99/orso/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2922 2023-09-06 01:05:50.000000 orso-0.0.99/orso/logging/add_level.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1944 2023-09-06 01:05:50.000000 orso-0.0.99/orso/logging/create_logger.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4785 2023-09-06 01:05:50.000000 orso-0.0.99/orso/logging/google_cloud_logger.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1445 2023-09-06 01:05:50.000000 orso-0.0.99/orso/logging/levels.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4601 2023-09-06 01:05:50.000000 orso-0.0.99/orso/logging/log_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.316387 orso-0.0.99/orso/profiler/
+-rw-r--r--   0 runner    (1001) docker     (999)       71 2023-09-06 01:05:50.000000 orso-0.0.99/orso/profiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.316387 orso-0.0.99/orso/profiler/distogram/
+-rw-r--r--   0 runner    (1001) docker     (999)    15497 2023-09-06 01:05:50.000000 orso-0.0.99/orso/profiler/distogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9326 2023-09-06 01:05:50.000000 orso-0.0.99/orso/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3500 2023-09-06 01:05:50.000000 orso-0.0.99/orso/row.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15223 2023-09-06 01:05:50.000000 orso-0.0.99/orso/schema.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18397 2023-09-06 01:05:50.000000 orso-0.0.99/orso/tools.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1874 2023-09-06 01:05:50.000000 orso-0.0.99/orso/types.py
+-rw-r--r--   0 runner    (1001) docker     (999)      601 2023-09-06 01:05:50.000000 orso-0.0.99/orso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.312387 orso-0.0.99/orso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     2396 2023-09-06 01:06:03.000000 orso-0.0.99/orso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1246 2023-09-06 01:06:03.000000 orso-0.0.99/orso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-06 01:06:03.000000 orso-0.0.99/orso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       48 2023-09-06 01:06:03.000000 orso-0.0.99/orso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        5 2023-09-06 01:06:03.000000 orso-0.0.99/orso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      341 2023-09-06 01:05:50.000000 orso-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-06 01:06:03.316387 orso-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1492 2023-09-06 01:05:50.000000 orso-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-06 01:06:03.316387 orso-0.0.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)     1554 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_bitarray.py
+-rw-r--r--   0 runner    (1001) docker     (999)      952 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_cityhash.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4777 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_converters_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (999)      565 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_converters_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (999)      565 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_converters_polars.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7389 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2011 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2175 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_filter_bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1344 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_filter_cuckoo_filter.py
+-rw-r--r--   0 runner    (1001) docker     (999)      950 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (999)      691 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1549 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6107 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7980 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_schema_columns.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2770 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_single_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1375 2023-09-06 01:05:50.000000 orso-0.0.99/tests/test_types.py
```

### Comparing `orso-0.0.97/LICENSE` & `orso-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/PKG-INFO` & `orso-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orso
-Version: 0.0.97
+Version: 0.0.99
 Summary: 🐻 DataFrame Library
 Home-page: https://github.com/mabel-dev/orso/
 Author-email: justin.joyce@joocer.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `orso-0.0.97/README.md` & `orso-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/bitarray/cbitarray.c` & `orso-0.0.99/orso/bitarray/cbitarray.c`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/cityhash/city.cc` & `orso-0.0.99/orso/cityhash/city.cc`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/cityhash/cityhash.cpp` & `orso-0.0.99/orso/cityhash/cityhash.cpp`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/compiled.c` & `orso-0.0.99/orso/compiled.c`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/converters.py` & `orso-0.0.99/orso/converters.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/dataframe.py` & `orso-0.0.99/orso/dataframe.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/display.py` & `orso-0.0.99/orso/display.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/exceptions.py` & `orso-0.0.99/orso/exceptions.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/filters/bloom_filter.py` & `orso-0.0.99/orso/filters/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/filters/cuckoo_filter.py` & `orso-0.0.99/orso/filters/cuckoo_filter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/logging/add_level.py` & `orso-0.0.99/orso/logging/add_level.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/logging/create_logger.py` & `orso-0.0.99/orso/logging/create_logger.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/logging/google_cloud_logger.py` & `orso-0.0.99/orso/logging/google_cloud_logger.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/logging/levels.py` & `orso-0.0.99/orso/logging/levels.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/logging/log_formatter.py` & `orso-0.0.99/orso/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/profiler/distogram/__init__.py` & `orso-0.0.99/orso/profiler/distogram/__init__.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/profiler/profiler.py` & `orso-0.0.99/orso/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/row.py` & `orso-0.0.99/orso/row.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/schema.py` & `orso-0.0.99/orso/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,51 +21,98 @@
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import MutableMapping
 from typing import Optional
 from typing import Tuple
+from typing import Type
 from typing import Union
 from warnings import warn
 
 import numpy
+from data_expectations import Expectation
 
 from orso.exceptions import ColumnDefinitionError
 from orso.exceptions import DataValidationError
 from orso.tools import arrow_type_map
 from orso.tools import random_string
 from orso.types import ORSO_TO_PYTHON_MAP
 from orso.types import PYTHON_TO_ORSO_MAP
 from orso.types import OrsoTypes
 
+_MISSING_VALUE: str = str()
+
+
+class SchemaExpectation(Expectation):
+    column = _MISSING_VALUE
+
+    @classmethod
+    def load(cls: Type["Expectation"], serialized: Union[Dict[str, Any], str]) -> "Expectation":
+        """
+        Loads a serialized Expectation and returns it as an instance.
+
+        Parameters:
+            serialized: Serialized Expectation as a dictionary or JSON string.
+
+        Returns:
+            An Expectation instance populated with the serialized data.
+        """
+        import json
+        from copy import deepcopy
+
+        if isinstance(serialized, str):
+            serialized = dict(json.loads(serialized))
+        serialized_copy: dict = deepcopy(serialized)
+        if "expectation" not in serialized_copy:
+            raise ValueError("Missing 'expectation' key in Expectation.")
+        expectation = serialized_copy.pop("expectation")
+        column = serialized_copy.pop("column", _MISSING_VALUE)
+        ignore_nulls = serialized_copy.pop("ignore_nulls", True)
+        config = serialized_copy
+        return Expectation(
+            expectation=expectation, column=column, ignore_nulls=ignore_nulls, config=config
+        )
+
 
 @dataclass(init=False)
 class FlatColumn:
     """
     This is a standard column type.
     Unlike the other column types, we don't store the values for this Column
     here, we read them from the underlying data structure (orso/pyarrow/velox).
     """
 
     name: str
     type: OrsoTypes
     description: Optional[str] = None
     aliases: Optional[List[str]] = field(default_factory=list)  # type: ignore
     nullable: bool = True
-    expectations: Optional[list] = field(default_factory=list)
+    expectations: Optional[Expectation] = field(default_factory=list)
     identity: str = field(default_factory=random_string)
     precision: Optional[int] = None
     scale: Optional[int] = None
 
     def __init__(self, **kwargs):
         attributes = {f.name: f for f in fields(self.__class__)}
         for attribute in attributes:
             if attribute in kwargs:
-                setattr(self, attribute, kwargs[attribute])
+                value = kwargs[attribute]
+                # Special handling for 'expectations'
+                if attribute == "expectations" and value:
+                    value = [
+                        v
+                        if isinstance(v, Expectation)
+                        else SchemaExpectation.load(v).update({"column": kwargs["name"]})
+                        if v.get("column", _MISSING_VALUE) == _MISSING_VALUE
+                        else v
+                        for v in value
+                    ]
+
+                setattr(self, attribute, value)
             elif not isinstance(attributes[attribute].default, _MISSING_TYPE):
                 setattr(self, attribute, attributes[attribute].default)
             elif not isinstance(attributes[attribute].default_factory, _MISSING_TYPE):
                 setattr(self, attribute, attributes[attribute].default_factory())  # type:ignore
             else:
                 raise ColumnDefinitionError(attribute)
```

### Comparing `orso-0.0.97/orso/types.py` & `orso-0.0.99/orso/types.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/orso/version.py` & `orso-0.0.99/orso/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,9 +6,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__: str = "0.0.97"
+__version__: str = "0.0.99"
 __author__: str = "@joocer"
```

### Comparing `orso-0.0.97/orso.egg-info/PKG-INFO` & `orso-0.0.99/orso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orso
-Version: 0.0.97
+Version: 0.0.99
 Summary: 🐻 DataFrame Library
 Home-page: https://github.com/mabel-dev/orso/
 Author-email: justin.joyce@joocer.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `orso-0.0.97/orso.egg-info/SOURCES.txt` & `orso-0.0.99/orso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/setup.py` & `orso-0.0.99/setup.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_bitarray.py` & `orso-0.0.99/tests/test_bitarray.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_cityhash.py` & `orso-0.0.99/tests/test_cityhash.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_converters_arrow.py` & `orso-0.0.99/tests/test_converters_arrow.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_converters_pandas.py` & `orso-0.0.99/tests/test_converters_pandas.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_converters_polars.py` & `orso-0.0.99/tests/test_converters_polars.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_dataframe.py` & `orso-0.0.99/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_fetching.py` & `orso-0.0.99/tests/test_fetching.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_filter_bloom_filter.py` & `orso-0.0.99/tests/test_filter_bloom_filter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_filter_cuckoo_filter.py` & `orso-0.0.99/tests/test_filter_cuckoo_filter.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_profiler.py` & `orso-0.0.99/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_random.py` & `orso-0.0.99/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_row.py` & `orso-0.0.99/tests/test_row.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_schema.py` & `orso-0.0.99/tests/test_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,28 @@
     column_names = cities.schema.all_column_names()
     assert "name" in column_names
     assert "language" in column_names
     assert "geolocation" not in column_names
 
 
 def test_schema_persistance():
-    as_dict = cities.schema.to_dict()
-    from_dict = RelationSchema.from_dict(as_dict)
+    def strip_expectations(rel):
+        columns = []
+        for column in rel.columns:
+            column.expectations = []
+            columns.append(column)
+        rel.columns = columns
+        return rel
 
-    assert from_dict == cities.schema
+    as_dict = strip_expectations(cities.schema).to_dict()
+    from_dict = strip_expectations(RelationSchema.from_dict(as_dict))
+
+    assert strip_expectations(from_dict) == strip_expectations(cities.schema), strip_expectations(
+        from_dict
+    )
     assert as_dict == from_dict.to_dict()
 
 
 def test_validate_with_valid_data():
     # Test with valid data
     data = {
         "name": "New York",
```

### Comparing `orso-0.0.97/tests/test_schema_columns.py` & `orso-0.0.99/tests/test_schema_columns.py`

 * *Files identical despite different names*

### Comparing `orso-0.0.97/tests/test_types.py` & `orso-0.0.99/tests/test_types.py`

 * *Files identical despite different names*

