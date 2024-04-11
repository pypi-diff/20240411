# Comparing `tmp/deirokay-1.1.1.tar.gz` & `tmp/deirokay-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deirokay-1.1.1.tar", last modified: Thu Mar 14 13:35:00 2024, max compression
+gzip compressed data, was "deirokay-1.2.0.tar", last modified: Thu Apr 11 12:15:05 2024, max compression
```

## Comparing `deirokay-1.1.1.tar` & `deirokay-1.2.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.231083 deirokay-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-14 13:34:55.000000 deirokay-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-14 13:35:00.231083 deirokay-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-14 13:34:55.000000 deirokay-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.223083 deirokay-1.1.1/deirokay/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.227083 deirokay-1.1.1/deirokay/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/airflow/deirokay_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/history_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.227083 deirokay-1.1.1/deirokay/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.227083 deirokay-1.1.1/deirokay/parser/reader/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/reader/dask_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/reader/pandas_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.227083 deirokay-1.1.1/deirokay/parser/treaters/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.227083 deirokay-1.1.1/deirokay/parser/treaters/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/base_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/boolean_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/date_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/datetime64_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/decimal_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/float_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/integer_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/numeric_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/string_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/time_treater.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/builtin/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/parser/treaters/multibackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.227083 deirokay-1.1.1/deirokay/statements/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.231083 deirokay-1.1.1/deirokay/statements/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/builtin/base_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/builtin/column_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    18085 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/builtin/contain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/builtin/not_null.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/builtin/row_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/builtin/statistic_in_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/builtin/unique.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/statements/multibackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-03-14 13:34:55.000000 deirokay-1.1.1/deirokay/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.223083 deirokay-1.1.1/deirokay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-14 13:35:00.000000 deirokay-1.1.1/deirokay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-14 13:35:00.000000 deirokay-1.1.1/deirokay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 13:35:00.000000 deirokay-1.1.1/deirokay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-14 13:35:00.000000 deirokay-1.1.1/deirokay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 13:35:00.000000 deirokay-1.1.1/deirokay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 13:35:00.000000 deirokay-1.1.1/deirokay.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-14 13:35:00.231083 deirokay-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-14 13:34:55.000000 deirokay-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.908739 deirokay-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 12:14:49.000000 deirokay-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-11 12:15:05.908739 deirokay-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-11 12:14:49.000000 deirokay-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.900739 deirokay-1.2.0/deirokay/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.900739 deirokay-1.2.0/deirokay/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/airflow/deirokay_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/history_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.900739 deirokay-1.2.0/deirokay/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.904739 deirokay-1.2.0/deirokay/parser/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/reader/dask_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/reader/pandas_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.904739 deirokay-1.2.0/deirokay/parser/treaters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.904739 deirokay-1.2.0/deirokay/parser/treaters/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/base_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/boolean_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/date_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/datetime64_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/decimal_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/float_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/integer_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/numeric_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/string_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/time_treater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/builtin/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/parser/treaters/multibackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.904739 deirokay-1.2.0/deirokay/statements/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.908739 deirokay-1.2.0/deirokay/statements/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/builtin/base_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/builtin/column_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19744 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/builtin/contain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/builtin/not_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/builtin/row_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/builtin/statistic_in_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/builtin/unique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/statements/multibackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-11 12:14:49.000000 deirokay-1.2.0/deirokay/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:15:05.900739 deirokay-1.2.0/deirokay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-11 12:15:05.000000 deirokay-1.2.0/deirokay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-11 12:15:05.000000 deirokay-1.2.0/deirokay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:15:05.000000 deirokay-1.2.0/deirokay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-11 12:15:05.000000 deirokay-1.2.0/deirokay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 12:15:05.000000 deirokay-1.2.0/deirokay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:15:05.000000 deirokay-1.2.0/deirokay.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-11 12:15:05.908739 deirokay-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-11 12:14:49.000000 deirokay-1.2.0/setup.py
```

### Comparing `deirokay-1.1.1/LICENSE` & `deirokay-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/PKG-INFO` & `deirokay-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deirokay
-Version: 1.1.1
+Version: 1.2.0
 Summary: A tool for data profiling and data validation
 Home-page: https://github.com/bigdatabr/deirokay
 Author: Marcos Bressan
 Author-email: marcos.bressan@bigdata.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deirokay-1.1.1/README.md` & `deirokay-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/_typing.py` & `deirokay-1.2.0/deirokay/_typing.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/_utils.py` & `deirokay-1.2.0/deirokay/_utils.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/airflow/deirokay_operator.py` & `deirokay-1.2.0/deirokay/airflow/deirokay_operator.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/backend.py` & `deirokay-1.2.0/deirokay/backend.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/enums.py` & `deirokay-1.2.0/deirokay/enums.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/exceptions.py` & `deirokay-1.2.0/deirokay/exceptions.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/fs.py` & `deirokay-1.2.0/deirokay/fs.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/history_template.py` & `deirokay-1.2.0/deirokay/history_template.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/loader.py` & `deirokay-1.2.0/deirokay/parser/loader.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/reader/__init__.py` & `deirokay-1.2.0/deirokay/parser/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/reader/dask_reader.py` & `deirokay-1.2.0/deirokay/parser/reader/dask_reader.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/reader/pandas_reader.py` & `deirokay-1.2.0/deirokay/parser/reader/pandas_reader.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/__init__.py` & `deirokay-1.2.0/deirokay/parser/treaters/__init__.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/__init__.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/base_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/base_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/boolean_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/boolean_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/date_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/date_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/datetime64_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/datetime64_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/decimal_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/decimal_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/float_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/float_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/integer_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/integer_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/numeric_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/numeric_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/string_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/string_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/time_treater.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/time_treater.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/builtin/validator.py` & `deirokay-1.2.0/deirokay/parser/treaters/builtin/validator.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/parser/treaters/multibackend.py` & `deirokay-1.2.0/deirokay/parser/treaters/multibackend.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/profiler.py` & `deirokay-1.2.0/deirokay/profiler.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/builtin/__init__.py` & `deirokay-1.2.0/deirokay/statements/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/builtin/base_statement.py` & `deirokay-1.2.0/deirokay/statements/builtin/base_statement.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/builtin/column_expression.py` & `deirokay-1.2.0/deirokay/statements/builtin/column_expression.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/builtin/contain.py` & `deirokay-1.2.0/deirokay/statements/builtin/contain.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,19 @@
       is set to True.
       Either `parser` or `parsers` must be declared.
     * `min_occurrences`: a global minimum number of occurrences for
       each of the `values`. Default: 1 for `all` and `all_and_only`
       rules, 0 for `only`.
     * `max_occurrences`: a global maximum number of occurrences for
       each of the `values`. Default: `inf` (unbounded).
+    * `tolerance_%`: The allowed percentage tolerance when using the rule
+      `only` and `all`. For example, if you define an `only` rule with the
+      values `["a", "b", "c"], but value "d" was also in the df, with a 25%
+      toleranace, the validation will pass, that is, at most 25% of the
+      unique values on the df weren't on the `values` list.
     * `occurrences_per_value`: a list of dictionaries overriding the
       global boundaries. Each dictionary may have the following keys:
 
         * `values` (required): a list of values to which the
           occurrence bounds below must apply to.
         * `min_occurrences`: a minimum number of occurrences for these
           values. Default: global `min_occurrences` parameter.
@@ -83,15 +88,15 @@
     The `all_and_only` rule checks both if all the `values` declared
     are present in the scope and if only they are present (not
     tolerating values not declared).
     Use it when you know all the possible values for the scope and you
     are sure that they will be always present.
 
     The `min_occurrences` and `max_occurrences` parameters are applied
-    applied to all the `values` declared, and only these. It means you
+    to all the `values` declared, and only these. It means you
     cannot (yet) specify boundaries for values you did't declare.
 
     Null values are considered valid for the purpose of the statement
     evaluation and must be explicitely passed in `values` if you wish
     to allow them (or not).
 
     You may also notice that, by tweaking the expected number of
@@ -120,53 +125,53 @@
                     "values": ["right-handed", "left-handed", "ambidextrous"],
                     "parser": {"dtype": "string"}
                 }
             ]
         }
 
     * You have a table of servers containg a column `role` which may
-      contain the values `master` and `slave`.
-      You want to be sure that there is always one and only one master
+      contain the values `controller` and `worker`.
+      You want to be sure that there is always one and only one controller
       server in the data.
 
     .. code-block:: json
 
         {
             "scope": "role",
             "statements": [
                 {
                     "type": "contain",
                     "rule": "all",
-                    "values": ["master"],
+                    "values": ["controller"],
                     "parser": {"dtype": "string"},
                     "min_occurrences": 1,
                     "max_occurrences": 1
                 }
             ]
         }
 
     You may also extend the previous example by making some adjustments
-    to ensure that there is no other value than `master` and `role`
+    to ensure that there is no other value than `controller` and `worker`
     in the data. Make notice that although the `rule` below is changed
     to `only`, the statement above is still contemplated by the
     `occurrences_per_value` parameter in the following validation item:
 
     .. code-block:: json
 
         {
             "scope": "role",
             "statements": [
                 {
                     "type": "contain",
                     "rule": "only",
-                    "values": ["master", "slave"],
+                    "values": ["controller", "worker"],
                     "parser": {"dtype": "string"},
                     "occurrences_per_value": [
                         {
-                            "values": ["master"],
+                            "values": ["controller"],
                             "min_occurrences": 1,
                             "max_occurrences": 1
                         }
                     ]
                 }
             ]
         }
@@ -233,66 +238,48 @@
         "rule",
         "values",
         "multicolumn",
         "parser",
         "parsers",
         "min_occurrences",
         "max_occurrences",
+        "tolerance_%",
         "occurrences_per_value",
         "report_limit",
     ]
     supported_backends: List[Backend] = [Backend.PANDAS, Backend.DASK]
 
-    DEFAULT_MIN_OCCURRENCES = {"all": (1, 0), "only": (0, 0), "all_and_only": (1, 0)}
-    DEFAULT_MAX_OCCURRENCES = {
-        "all": (numpy.inf, numpy.inf),
-        "only": (numpy.inf, 0),
-        "all_and_only": (numpy.inf, 0),
-    }
     DEFAULT_REPORT_LIMIT = 32
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         self.rule = self.options["rule"]
         assert self.rule in ("all", "only", "all_and_only")
+        self.tolerance_perc = self.options.get("tolerance_%", 0)
+        if self.tolerance_perc > 0 and self.rule == "all_and_only":
+            raise ValueError(
+                "It's not possible to set a tolerance_perc with the rule 'all_and_only'"
+            )
         self.multicolumn = self.options.get("multicolumn", False)
         _parsers = self.options.get("parser") or self.options["parsers"]
         if self.multicolumn:
             self.parsers = _parsers
         else:
             self.parsers = [_parsers]
         self.treaters = [
             get_treater_instance(parser, backend=self.get_backend())
             for parser in self.parsers
         ]
 
-        self.min_occurrences = self.options.get("min_occurrences", None)
-        self.max_occurrences = self.options.get("max_occurrences", None)
+        self.min_occurrences = self.options.get("min_occurrences", 0)
+        self.max_occurrences = self.options.get("max_occurrences", numpy.inf)
         self.occurrences_per_value = self.options.get("occurrences_per_value", [])
         self.report_limit = self.options.get("report_limit", NODEFAULT)
 
-        self._set_default_minmax_occurrences()
-
-    def _set_default_minmax_occurrences(self) -> None:
-        final_min = noneor(
-            self.min_occurrences, Contain.DEFAULT_MIN_OCCURRENCES[self.rule][0]
-        )
-        final_max = noneor(
-            self.max_occurrences, Contain.DEFAULT_MAX_OCCURRENCES[self.rule][0]
-        )
-        if self.max_occurrences is not None and self.max_occurrences < final_min:
-            final_min = self.max_occurrences
-        if self.min_occurrences is not None and self.min_occurrences > final_max:
-            final_max = self.min_occurrences
-        assert final_min >= 0
-        assert final_max >= 0
-        self.min_occurrences = final_min
-        self.max_occurrences = final_max
-
     def _generate_analysis(self, value_counts):
         if self.multicolumn:
 
             def _unpack_row(row, *args):
                 return (*row, *args)
 
         else:
@@ -322,51 +309,35 @@
             col: parser for col, parser in zip(value_counts.index.names, self.parsers)
         }
         data_treater(occurrence_limits, options, backend=Backend.PANDAS)
 
         occurrence_limits.drop_duplicates(
             subset=value_counts.index.names, keep="first", inplace=True
         )
+        occurrence_limits["in_values"] = True
         occurrence_limits.set_index(value_counts.index.names, inplace=True)
 
         analysis = (
             value_counts.to_frame()
             .reset_index()
             .merge(occurrence_limits.reset_index(), how="outer")
         )
         analysis["count"].fillna(0, inplace=True)
-        analysis["min"].fillna(
-            Contain.DEFAULT_MIN_OCCURRENCES[self.rule][1], inplace=True
-        )
-        analysis["max"].fillna(
-            Contain.DEFAULT_MAX_OCCURRENCES[self.rule][1], inplace=True
-        )
-        analysis["result"] = analysis["count"].ge(analysis["min"]) & analysis[
-            "count"
-        ].le(analysis["max"])
+        analysis["min"].fillna(0, inplace=True)
+        analysis["max"].fillna(numpy.inf, inplace=True)
+        analysis["in_values"].fillna(False, inplace=True)
+        analysis["occurrences_result"] = analysis["count"].ge(
+            analysis["min"]
+        ) & analysis["count"].le(analysis["max"])
         return analysis
 
     def _generate_report(self, analysis):
-        columns = [analysis[col] for col in analysis.columns[:-4]]
-        serialized = (
-            treater.serialize(column) for treater, column in zip(self.treaters, columns)
-        )
-        rows = zip(*(s["values"] for s in serialized))
-        rows = (list(row) for row in rows)
-        values_report = sorted(
-            [
-                {
-                    "value": value_row,
-                    "count": analysis_row.count,
-                    "result": analysis_row.result,
-                }
-                for value_row, analysis_row in zip(rows, analysis.itertuples())
-            ],
-            key=lambda x: x["result"],
-        )
+        values_report = self._create_values_report(analysis)
+        values_report = sorted(values_report, key=lambda x: x["result"])
+        rule_report = self._create_rule_report(analysis)
 
         if (
             self.report_limit is NODEFAULT
             and len(values_report) > Contain.DEFAULT_REPORT_LIMIT
         ):
             self.report_limit = Contain.DEFAULT_REPORT_LIMIT
             warnings.warn(
@@ -382,17 +353,76 @@
         return {
             "values": (
                 values_report
                 if self.report_limit is NODEFAULT
                 else values_report
                 if self.report_limit is None
                 else values_report[: self.report_limit]
-            )
+            ),
+            "rule_report": rule_report,
         }
 
+    def _create_values_report(self, analysis):
+        columns = [analysis[col] for col in analysis.columns[:-4]]
+        serialized = (
+            treater.serialize(column) for treater, column in zip(self.treaters, columns)
+        )
+        rows = zip(*(s["values"] for s in serialized))
+        rows = (list(row) for row in rows)
+        values_report = [
+            {
+                "value": value_row,
+                "count": analysis_row.count,
+                "result": analysis_row.occurrences_result,
+            }
+            for value_row, analysis_row in zip(rows, analysis.itertuples())
+        ]
+        return values_report
+
+    def _create_rule_report(self, analysis):
+        values_in_df = analysis[(analysis["count"] > 0)]
+        perc_in_values = float(values_in_df["in_values"].mean() * 100)
+
+        in_values = analysis[(analysis["in_values"]) & (analysis["max"] > 0)]
+        if len(in_values):
+            perc_values_in_df = float((in_values["count"] > 0).mean()) * 100
+        else:
+            perc_values_in_df = 0
+
+        if self.rule == "only":
+            result = perc_in_values >= 100 - self.tolerance_perc
+            return {
+                "rule": self.rule,
+                "perc_in_values": perc_in_values,
+                "tolerance_%": self.tolerance_perc,
+                "result": result,
+            }
+        elif self.rule == "all":
+            in_values = analysis[(analysis["in_values"]) & (analysis["max"] > 0)]
+            if len(in_values):
+                result = perc_values_in_df >= 100 - self.tolerance_perc
+                return {
+                    "rule": self.rule,
+                    "perc_values_in_df": perc_values_in_df,
+                    "tolerance_%": self.tolerance_perc,
+                    "result": result,
+                }
+            else:
+                return {
+                    "rule": self.rule,
+                    "result": True,  # All the values have check of not contain
+                }
+        elif self.rule == "all_and_only":
+            return {
+                "rule": self.rule,
+                "perc_in_values": perc_in_values,
+                "perc_values_in_df": perc_values_in_df,
+                "result": perc_in_values == 100 and perc_values_in_df == 100,
+            }
+
     @report(Backend.PANDAS)
     def _report_pandas(self, df: "pandas.DataFrame") -> dict:
         # Concat all columns
         _cols = df.columns.tolist()
 
         if not self.multicolumn:
             # Columns are assumed to be of same Dtype
@@ -413,15 +443,17 @@
 
         value_counts = df.groupby(_cols, dropna=False)[_cols[0]].size().rename("count")
         analysis = self._generate_analysis(value_counts.compute())
         return self._generate_report(analysis)
 
     # docstr-coverage:inherited
     def result(self, report: dict) -> bool:
-        return all(item["result"] for item in report["values"])
+        values_result = all(item["result"] for item in report["values"])
+        rule_result = report["rule_report"]["result"]
+        return values_result and rule_result
 
     @profile(Backend.PANDAS)
     @staticmethod
     def _profile_pandas(df: "pandas.DataFrame") -> DeirokayStatement:
         if any(dtype != df.dtypes for dtype in df.dtypes):
             raise NotImplementedError("Refusing to mix up different types of columns")
```

### Comparing `deirokay-1.1.1/deirokay/statements/builtin/not_null.py` & `deirokay-1.2.0/deirokay/statements/builtin/not_null.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/builtin/row_count.py` & `deirokay-1.2.0/deirokay/statements/builtin/row_count.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/builtin/statistic_in_interval.py` & `deirokay-1.2.0/deirokay/statements/builtin/statistic_in_interval.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/builtin/unique.py` & `deirokay-1.2.0/deirokay/statements/builtin/unique.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/loader.py` & `deirokay-1.2.0/deirokay/statements/loader.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/statements/multibackend.py` & `deirokay-1.2.0/deirokay/statements/multibackend.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay/validator.py` & `deirokay-1.2.0/deirokay/validator.py`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/deirokay.egg-info/PKG-INFO` & `deirokay-1.2.0/deirokay.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deirokay
-Version: 1.1.1
+Version: 1.2.0
 Summary: A tool for data profiling and data validation
 Home-page: https://github.com/bigdatabr/deirokay
 Author: Marcos Bressan
 Author-email: marcos.bressan@bigdata.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deirokay-1.1.1/deirokay.egg-info/SOURCES.txt` & `deirokay-1.2.0/deirokay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deirokay-1.1.1/setup.py` & `deirokay-1.2.0/setup.py`

 * *Files identical despite different names*

