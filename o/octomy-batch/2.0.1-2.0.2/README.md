# Comparing `tmp/octomy-batch-2.0.1.tar.gz` & `tmp/octomy-batch-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-batch-2.0.1.tar", last modified: Sun Apr  7 18:14:12 2024, max compression
+gzip compressed data, was "octomy-batch-2.0.2.tar", last modified: Wed Apr 10 23:09:29 2024, max compression
```

## Comparing `octomy-batch-2.0.1.tar` & `octomy-batch-2.0.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.608600 octomy-batch-2.0.1/
--rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.1/.gitignore
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.600600 octomy-batch-2.0.1/.gitlab/
--rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.1/.gitlab/ci.yaml
--rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.1/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.1/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)     3130 2024-04-07 18:14:12.608600 octomy-batch-2.0.1/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.1/README.md
--rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-07 18:14:10.000000 octomy-batch-2.0.1/VERSION
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.600600 octomy-batch-2.0.1/bin/
--rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.1/bin/octomy-batch
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.600600 octomy-batch-2.0.1/code_quality/
--rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.1/code_quality/.flake8
--rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.1/code_quality/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.1/code_quality/mypy.ini
--rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.1/code_quality/pylintrc
--rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.1/config.json
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.592600 octomy-batch-2.0.1/octomy/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.596600 octomy-batch-2.0.1/octomy/batch/
--rw-r--r--   0 leo       (1000) leo       (1000)    20270 2024-04-07 18:06:20.000000 octomy-batch-2.0.1/octomy/batch/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.596600 octomy-batch-2.0.1/octomy/batch/filters/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.1/octomy/batch/filters/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.596600 octomy-batch-2.0.1/octomy/batch/filters/base/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.1/octomy/batch/filters/base/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.1/octomy/batch/filters/base/hello.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.596600 octomy-batch-2.0.1/octomy/batch/filters/utils/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.1/octomy/batch/filters/utils/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.1/octomy/batch/filters/utils/ping.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1285 2024-04-07 18:05:17.000000 octomy-batch-2.0.1/octomy/batch/filters/utils/test.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.596600 octomy-batch-2.0.1/octomy/batch/server/
--rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.1/octomy/batch/server/WebsiteIO.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.1/octomy/batch/server/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4424 2024-04-07 18:11:30.000000 octomy-batch-2.0.1/octomy/batch/types.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.600600 octomy-batch-2.0.1/octomy_batch.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     3130 2024-04-07 18:14:12.000000 octomy-batch-2.0.1/octomy_batch.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     1301 2024-04-07 18:14:12.000000 octomy-batch-2.0.1/octomy_batch.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-07 18:14:12.000000 octomy-batch-2.0.1/octomy_batch.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-07 18:14:12.000000 octomy-batch-2.0.1/octomy_batch.egg-info/namespace_packages.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-07 18:14:12.000000 octomy-batch-2.0.1/octomy_batch.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-07 18:14:12.000000 octomy-batch-2.0.1/octomy_batch.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.1/octomy_batch.egg-info/zip-safe
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.604600 octomy-batch-2.0.1/requirements/
--rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-06 23:31:18.000000 octomy-batch-2.0.1/requirements/requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-06 23:33:41.000000 octomy-batch-2.0.1/requirements/requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.1/requirements/test_requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.1/requirements/test_requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-07 18:14:12.608600 octomy-batch-2.0.1/setup.cfg
--rwxr-xr-x   0 leo       (1000) leo       (1000)     7024 2024-04-06 13:28:48.000000 octomy-batch-2.0.1/setup.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.604600 octomy-batch-2.0.1/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.1/tests/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.1/tests/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.604600 octomy-batch-2.0.1/tests/integration/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.1/tests/integration/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      130 2020-03-20 01:43:26.000000 octomy-batch-2.0.1/tests/integration/test_integration.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.604600 octomy-batch-2.0.1/tests/load/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.1/tests/load/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      123 2020-03-20 01:43:18.000000 octomy-batch-2.0.1/tests/load/test_load.py
--rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.1/tests/pytest.ini
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.604600 octomy-batch-2.0.1/tests/regressions/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.1/tests/regressions/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      130 2020-12-15 04:57:55.000000 octomy-batch-2.0.1/tests/regressions/test_regressions.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-07 18:14:12.604600 octomy-batch-2.0.1/tests/unit/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.1/tests/unit/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      202 2022-01-12 22:37:26.000000 octomy-batch-2.0.1/tests/unit/test_batch_processor.py
--rw-r--r--   0 leo       (1000) leo       (1000)      190 2022-01-12 22:37:26.000000 octomy-batch-2.0.1/tests/unit/test_server.py
--rw-r--r--   0 leo       (1000) leo       (1000)     3502 2022-01-12 22:37:26.000000 octomy-batch-2.0.1/tests/unit/test_unit.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.239354 octomy-batch-2.0.2/
+-rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.2/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.231353 octomy-batch-2.0.2/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.2/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.2/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.2/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     3130 2024-04-10 23:09:29.239354 octomy-batch-2.0.2/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.2/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-10 23:08:28.000000 octomy-batch-2.0.2/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.231353 octomy-batch-2.0.2/bin/
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.2/bin/octomy-batch
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.235354 octomy-batch-2.0.2/code_quality/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.2/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.2/code_quality/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.2/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.2/code_quality/pylintrc
+-rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.2/config.json
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.223353 octomy-batch-2.0.2/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.227353 octomy-batch-2.0.2/octomy/batch/
+-rw-r--r--   0 leo       (1000) leo       (1000)    20270 2024-04-07 18:06:20.000000 octomy-batch-2.0.2/octomy/batch/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.227353 octomy-batch-2.0.2/octomy/batch/filters/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.2/octomy/batch/filters/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.231353 octomy-batch-2.0.2/octomy/batch/filters/base/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.2/octomy/batch/filters/base/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.2/octomy/batch/filters/base/hello.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.231353 octomy-batch-2.0.2/octomy/batch/filters/utils/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.2/octomy/batch/filters/utils/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.2/octomy/batch/filters/utils/ping.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1285 2024-04-07 18:05:17.000000 octomy-batch-2.0.2/octomy/batch/filters/utils/test.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.231353 octomy-batch-2.0.2/octomy/batch/server/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.2/octomy/batch/server/WebsiteIO.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.2/octomy/batch/server/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4451 2024-04-10 23:07:15.000000 octomy-batch-2.0.2/octomy/batch/types.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.231353 octomy-batch-2.0.2/octomy_batch.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3130 2024-04-10 23:09:28.000000 octomy-batch-2.0.2/octomy_batch.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1301 2024-04-10 23:09:29.000000 octomy-batch-2.0.2/octomy_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-10 23:09:29.000000 octomy-batch-2.0.2/octomy_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-10 23:09:29.000000 octomy-batch-2.0.2/octomy_batch.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-10 23:09:29.000000 octomy-batch-2.0.2/octomy_batch.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-10 23:09:29.000000 octomy-batch-2.0.2/octomy_batch.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.2/octomy_batch.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.235354 octomy-batch-2.0.2/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-06 23:31:18.000000 octomy-batch-2.0.2/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-06 23:33:41.000000 octomy-batch-2.0.2/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.2/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.2/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-10 23:09:29.239354 octomy-batch-2.0.2/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7024 2024-04-06 13:28:48.000000 octomy-batch-2.0.2/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.235354 octomy-batch-2.0.2/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.2/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.2/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.235354 octomy-batch-2.0.2/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.2/tests/integration/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      130 2020-03-20 01:43:26.000000 octomy-batch-2.0.2/tests/integration/test_integration.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.235354 octomy-batch-2.0.2/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.2/tests/load/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      123 2020-03-20 01:43:18.000000 octomy-batch-2.0.2/tests/load/test_load.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.2/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.235354 octomy-batch-2.0.2/tests/regressions/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.2/tests/regressions/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      130 2020-12-15 04:57:55.000000 octomy-batch-2.0.2/tests/regressions/test_regressions.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:09:29.239354 octomy-batch-2.0.2/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.2/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      202 2022-01-12 22:37:26.000000 octomy-batch-2.0.2/tests/unit/test_batch_processor.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      190 2022-01-12 22:37:26.000000 octomy-batch-2.0.2/tests/unit/test_server.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     3502 2022-01-12 22:37:26.000000 octomy-batch-2.0.2/tests/unit/test_unit.py
```

### Comparing `octomy-batch-2.0.1/.gitlab/ci.yaml` & `octomy-batch-2.0.2/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/LICENSE` & `octomy-batch-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/PKG-INFO` & `octomy-batch-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 2.0.1
+Version: 2.0.2
 Summary: ('octomy/batch',)
 Home-page: https://gitlab.com/octomy/batch
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-batch-2.0.1/README.md` & `octomy-batch-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/bin/octomy-batch` & `octomy-batch-2.0.2/bin/octomy-batch`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/code_quality/Makefile` & `octomy-batch-2.0.2/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/code_quality/pylintrc` & `octomy-batch-2.0.2/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/config.json` & `octomy-batch-2.0.2/config.json`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/octomy/batch/__init__.py` & `octomy-batch-2.0.2/octomy/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/octomy/batch/filters/utils/ping.py` & `octomy-batch-2.0.2/octomy/batch/filters/utils/ping.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/octomy/batch/filters/utils/test.py` & `octomy-batch-2.0.2/octomy/batch/filters/utils/test.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/octomy/batch/server/WebsiteIO.py` & `octomy-batch-2.0.2/octomy/batch/server/WebsiteIO.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/octomy/batch/server/__init__.py` & `octomy-batch-2.0.2/octomy/batch/server/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/octomy/batch/types.py` & `octomy-batch-2.0.2/octomy/batch/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,17 +160,17 @@
 
 
 class WorkerStats(pydantic.BaseModel):
 	worker_id: str | None
 	job_count:float | None
 	ms_per_job:float | None
 	jobs_per_hour:float | None
-	first_active:datetime | None
-	current_job_started:datetime | None
-	last_job_finished:datetime | None
+	first_active:datetime.datetime | None
+	current_job_started:datetime.datetime | None
+	last_job_finished:datetime.datetime | None
 	run_time:int | None
 	work_time:int | None
 	idle_time:int | None
 	is_activbe:bool | None
 
 
 class Action(pydantic.BaseModel):
```

### Comparing `octomy-batch-2.0.1/octomy_batch.egg-info/PKG-INFO` & `octomy-batch-2.0.2/octomy_batch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 2.0.1
+Version: 2.0.2
 Summary: ('octomy/batch',)
 Home-page: https://gitlab.com/octomy/batch
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-batch-2.0.1/octomy_batch.egg-info/SOURCES.txt` & `octomy-batch-2.0.2/octomy_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/requirements/requirements.txt` & `octomy-batch-2.0.2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/requirements/test_requirements.txt` & `octomy-batch-2.0.2/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/setup.py` & `octomy-batch-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/tests/Makefile` & `octomy-batch-2.0.2/tests/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.1/tests/unit/test_unit.py` & `octomy-batch-2.0.2/tests/unit/test_unit.py`

 * *Files identical despite different names*

