# Comparing `tmp/jsonpickle-3.0.3.tar.gz` & `tmp/jsonpickle-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonpickle-3.0.3.tar", last modified: Tue Feb 20 03:42:36 2024, max compression
+gzip compressed data, was "jsonpickle-3.0.4.tar", last modified: Thu Apr 11 09:05:36 2024, max compression
```

## Comparing `jsonpickle-3.0.3.tar` & `jsonpickle-3.0.4.tar`

### file list

```diff
@@ -1,111 +1,110 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.880971 jsonpickle-3.0.3/
--rw-r--r--   0 david     (1000) david     (1000)       70 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/.coveragerc
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.852970 jsonpickle-3.0.3/.github/
--rw-r--r--   0 david     (1000) david     (1000)       39 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.852970 jsonpickle-3.0.3/.github/workflows/
--rw-r--r--   0 david     (1000) david     (1000)      994 2023-11-19 20:59:56.000000 jsonpickle-3.0.3/.github/workflows/lint.yml
--rw-r--r--   0 david     (1000) david     (1000)     1291 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/.github/workflows/test.yml
--rw-r--r--   0 david     (1000) david     (1000)      236 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/.gitignore
--rw-r--r--   0 david     (1000) david     (1000)       31 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/.isort.cfg
--rw-r--r--   0 david     (1000) david     (1000)      175 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/.pre-commit-config.yaml
--rw-r--r--   0 david     (1000) david     (1000)      139 2023-11-19 21:00:06.000000 jsonpickle-3.0.3/.readthedocs.yml
--rw-r--r--   0 david     (1000) david     (1000)     1833 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/BENCHMARKS.md
--rw-r--r--   0 david     (1000) david     (1000)    18946 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/CHANGES.rst
--rw-r--r--   0 david     (1000) david     (1000)     1547 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     2556 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/Makefile
--rw-r--r--   0 david     (1000) david     (1000)     6325 2024-02-20 03:42:36.880971 jsonpickle-3.0.3/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     5220 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/README.rst
--rw-r--r--   0 david     (1000) david     (1000)      468 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/appveyor.yml
--rw-r--r--   0 david     (1000) david     (1000)     1755 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/azure-pipelines.yml
--rw-r--r--   0 david     (1000) david     (1000)      761 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/conftest.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.852970 jsonpickle-3.0.3/contrib/
--rwxr-xr-x   0 david     (1000) david     (1000)      281 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/contrib/copy-docs
--rw-r--r--   0 david     (1000) david     (1000)     1468 2024-02-20 03:41:39.000000 jsonpickle-3.0.3/contrib/pyqt-reduce-handler.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.852970 jsonpickle-3.0.3/docs/
--rw-r--r--   0 david     (1000) david     (1000)     4266 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/docs/api.rst
--rw-r--r--   0 david     (1000) david     (1000)     1932 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/docs/conf.py
--rw-r--r--   0 david     (1000) david     (1000)     1798 2024-01-16 10:57:06.000000 jsonpickle-3.0.3/docs/contrib.rst
--rw-r--r--   0 david     (1000) david     (1000)      646 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/docs/extensions.rst
--rw-r--r--   0 david     (1000) david     (1000)       81 2024-01-16 10:47:47.000000 jsonpickle-3.0.3/docs/history.rst
--rw-r--r--   0 david     (1000) david     (1000)     2395 2024-01-16 10:57:12.000000 jsonpickle-3.0.3/docs/index.rst
--rw-r--r--   0 david     (1000) david     (1000)       35 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/docs/requirements.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.864971 jsonpickle-3.0.3/images/
--rw-r--r--   0 david     (1000) david     (1000)    83498 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-0.9.6-3.11.svg
--rw-r--r--   0 david     (1000) david     (1000)    83313 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-0.9.6-3.9.svg
--rw-r--r--   0 david     (1000) david     (1000)    83372 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-1.5.1-3.11.svg
--rw-r--r--   0 david     (1000) david     (1000)    83400 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-1.5.1-3.9.svg
--rw-r--r--   0 david     (1000) david     (1000)    83497 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-1.5.2-3.11.svg
--rw-r--r--   0 david     (1000) david     (1000)    82639 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-1.5.2-3.9.svg
--rw-r--r--   0 david     (1000) david     (1000)    83524 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-2.2.0-3.11.svg
--rw-r--r--   0 david     (1000) david     (1000)    83406 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-2.2.0-3.9.svg
--rw-r--r--   0 david     (1000) david     (1000)    83364 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-3.0.0-3.11.svg
--rw-r--r--   0 david     (1000) david     (1000)    84299 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/images/jsonpickle-3.0.0-3.9.svg
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.868970 jsonpickle-3.0.3/jsonpickle/
--rw-r--r--   0 david     (1000) david     (1000)     3137 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickle/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)    10013 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/jsonpickle/backend.py
--rw-r--r--   0 david     (1000) david     (1000)      398 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickle/compat.py
--rw-r--r--   0 david     (1000) david     (1000)      132 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickle/errors.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.868970 jsonpickle-3.0.3/jsonpickle/ext/
--rw-r--r--   0 david     (1000) david     (1000)        0 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickle/ext/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      558 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/jsonpickle/ext/gmpy.py
--rw-r--r--   0 david     (1000) david     (1000)    13551 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/jsonpickle/ext/numpy.py
--rw-r--r--   0 david     (1000) david     (1000)     8328 2023-11-19 20:59:56.000000 jsonpickle-3.0.3/jsonpickle/ext/pandas.py
--rw-r--r--   0 david     (1000) david     (1000)     8448 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/jsonpickle/handlers.py
--rw-r--r--   0 david     (1000) david     (1000)    30260 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/jsonpickle/pickler.py
--rw-r--r--   0 david     (1000) david     (1000)     1025 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/jsonpickle/tags.py
--rw-r--r--   0 david     (1000) david     (1000)    29339 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/jsonpickle/unpickler.py
--rw-r--r--   0 david     (1000) david     (1000)    14384 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/jsonpickle/util.py
--rw-r--r--   0 david     (1000) david     (1000)      448 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickle/version.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.868970 jsonpickle-3.0.3/jsonpickle.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     6325 2024-02-20 03:42:36.000000 jsonpickle-3.0.3/jsonpickle.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     2172 2024-02-20 03:42:36.000000 jsonpickle-3.0.3/jsonpickle.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2024-02-20 03:42:36.000000 jsonpickle-3.0.3/jsonpickle.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)      322 2024-02-20 03:42:36.000000 jsonpickle-3.0.3/jsonpickle.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)       11 2024-02-20 03:42:36.000000 jsonpickle-3.0.3/jsonpickle.egg-info/top_level.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.872971 jsonpickle-3.0.3/jsonpickleJS/
--rw-r--r--   0 david     (1000) david     (1000)      354 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/.gitignore
--rw-r--r--   0 david     (1000) david     (1000)     1550 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)     4674 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/README.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.844970 jsonpickle-3.0.3/jsonpickleJS/ext/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.872971 jsonpickle-3.0.3/jsonpickleJS/ext/require/
--rw-r--r--   0 david     (1000) david     (1000)     4035 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/ext/require/domReady.js
--rw-r--r--   0 david     (1000) david     (1000)     1549 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/ext/require/order.js
--rw-r--r--   0 david     (1000) david     (1000)    15233 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/ext/require/require.js
--rw-r--r--   0 david     (1000) david     (1000)    15464 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/ext/require/text.js
--rw-r--r--   0 david     (1000) david     (1000)      513 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/handlers.js
--rw-r--r--   0 david     (1000) david     (1000)     1427 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/main.js
--rw-r--r--   0 david     (1000) david     (1000)     8996 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/pickler.js
--rw-r--r--   0 david     (1000) david     (1000)      732 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/tags.js
--rw-r--r--   0 david     (1000) david     (1000)      867 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/testPickle.html
--rw-r--r--   0 david     (1000) david     (1000)      821 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/testUnpickle.html
--rw-r--r--   0 david     (1000) david     (1000)    11828 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/unpickler.js
--rw-r--r--   0 david     (1000) david     (1000)     2164 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/jsonpickleJS/util.js
--rw-r--r--   0 david     (1000) david     (1000)     8025 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/jsonpickle_benchmarks.py
--rw-r--r--   0 david     (1000) david     (1000)      354 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/pyproject.toml
--rw-r--r--   0 david     (1000) david     (1000)      380 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/pytest.ini
--rw-r--r--   0 david     (1000) david     (1000)      286 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/requirements-dev.txt
--rw-r--r--   0 david     (1000) david     (1000)     1498 2024-02-20 03:42:36.880971 jsonpickle-3.0.3/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)       92 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/setup.py
--rw-r--r--   0 david     (1000) david     (1000)     8960 2024-01-09 09:49:51.000000 jsonpickle-3.0.3/skeleton.md
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-02-20 03:42:36.880971 jsonpickle-3.0.3/tests/
--rw-r--r--   0 david     (1000) david     (1000)     5747 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/tests/backend_test.py
--rwxr-xr-x   0 david     (1000) david     (1000)     1182 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/benchmark.py
--rw-r--r--   0 david     (1000) david     (1000)     3054 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/bson_test.py
--rw-r--r--   0 david     (1000) david     (1000)    11356 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/collections_test.py
--rw-r--r--   0 david     (1000) david     (1000)     8752 2023-11-19 20:59:56.000000 jsonpickle-3.0.3/tests/datetime_test.py
--rw-r--r--   0 david     (1000) david     (1000)     2571 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/document_test.py
--rw-r--r--   0 david     (1000) david     (1000)     1566 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/tests/ecdsa_test.py
--rw-r--r--   0 david     (1000) david     (1000)     3153 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/feedparser_test.py
--rw-r--r--   0 david     (1000) david     (1000)     4775 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/handler_test.py
--rw-r--r--   0 david     (1000) david     (1000)      179 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/helper.py
--rw-r--r--   0 david     (1000) david     (1000)    59242 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/tests/jsonpickle_test.py
--rw-r--r--   0 david     (1000) david     (1000)    10864 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/numpy_test.py
--rw-r--r--   0 david     (1000) david     (1000)    35313 2023-11-19 20:59:56.000000 jsonpickle-3.0.3/tests/object_test.py
--rw-r--r--   0 david     (1000) david     (1000)     9753 2024-02-16 09:49:59.000000 jsonpickle-3.0.3/tests/pandas_test.py
--rw-r--r--   0 david     (1000) david     (1000)     2292 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/tests/sklearn_test.py
--rw-r--r--   0 david     (1000) david     (1000)     4138 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/tests/sqlalchemy_test.py
--rw-r--r--   0 david     (1000) david     (1000)     1663 2023-03-26 08:31:27.000000 jsonpickle-3.0.3/tests/stdlib_test.py
--rw-r--r--   0 david     (1000) david     (1000)     7558 2023-03-26 08:31:40.000000 jsonpickle-3.0.3/tests/util_test.py
--rw-r--r--   0 david     (1000) david     (1000)     8501 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/tests/wizard_test.py
--rw-r--r--   0 david     (1000) david     (1000)      895 2023-11-19 20:59:56.000000 jsonpickle-3.0.3/tests/zoneinfo_test.py
--rw-r--r--   0 david     (1000) david     (1000)     1062 2024-02-20 03:40:50.000000 jsonpickle-3.0.3/tox.ini
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.597614 jsonpickle-3.0.4/
+-rw-r--r--   0 david     (1000) david     (1000)       70 2024-02-20 03:40:50.000000 jsonpickle-3.0.4/.coveragerc
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.581614 jsonpickle-3.0.4/.github/
+-rw-r--r--   0 david     (1000) david     (1000)       39 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/.github/FUNDING.yml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.581614 jsonpickle-3.0.4/.github/workflows/
+-rw-r--r--   0 david     (1000) david     (1000)      994 2023-11-19 20:59:56.000000 jsonpickle-3.0.4/.github/workflows/lint.yml
+-rw-r--r--   0 david     (1000) david     (1000)     1291 2024-02-20 03:40:50.000000 jsonpickle-3.0.4/.github/workflows/test.yml
+-rw-r--r--   0 david     (1000) david     (1000)      243 2024-04-06 10:12:12.000000 jsonpickle-3.0.4/.gitignore
+-rw-r--r--   0 david     (1000) david     (1000)       31 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/.isort.cfg
+-rw-r--r--   0 david     (1000) david     (1000)      175 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 david     (1000) david     (1000)      139 2023-11-19 21:00:06.000000 jsonpickle-3.0.4/.readthedocs.yml
+-rw-r--r--   0 david     (1000) david     (1000)     1833 2023-03-26 08:31:40.000000 jsonpickle-3.0.4/BENCHMARKS.md
+-rw-r--r--   0 david     (1000) david     (1000)    19441 2024-04-11 08:42:32.000000 jsonpickle-3.0.4/CHANGES.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1547 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)     2554 2024-03-14 02:28:59.000000 jsonpickle-3.0.4/Makefile
+-rw-r--r--   0 david     (1000) david     (1000)     1215 2024-04-11 09:05:36.597614 jsonpickle-3.0.4/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     4436 2024-04-06 10:12:12.000000 jsonpickle-3.0.4/README.rst
+-rw-r--r--   0 david     (1000) david     (1000)      468 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/appveyor.yml
+-rw-r--r--   0 david     (1000) david     (1000)     1755 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/azure-pipelines.yml
+-rw-r--r--   0 david     (1000) david     (1000)      761 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/conftest.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.581614 jsonpickle-3.0.4/contrib/
+-rwxr-xr-x   0 david     (1000) david     (1000)      281 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/contrib/copy-docs
+-rw-r--r--   0 david     (1000) david     (1000)     1466 2024-02-20 03:46:29.000000 jsonpickle-3.0.4/contrib/pyqt-reduce-handler.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.585614 jsonpickle-3.0.4/docs/
+-rw-r--r--   0 david     (1000) david     (1000)     4266 2024-02-20 03:40:50.000000 jsonpickle-3.0.4/docs/api.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1807 2024-04-11 08:42:56.000000 jsonpickle-3.0.4/docs/conf.py
+-rw-r--r--   0 david     (1000) david     (1000)     1798 2024-01-16 10:57:06.000000 jsonpickle-3.0.4/docs/contrib.rst
+-rw-r--r--   0 david     (1000) david     (1000)      646 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/docs/extensions.rst
+-rw-r--r--   0 david     (1000) david     (1000)       81 2024-01-16 10:47:47.000000 jsonpickle-3.0.4/docs/history.rst
+-rw-r--r--   0 david     (1000) david     (1000)     2395 2024-01-16 10:57:12.000000 jsonpickle-3.0.4/docs/index.rst
+-rw-r--r--   0 david     (1000) david     (1000)       35 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/docs/requirements.txt
+-rw-r--r--   0 david     (1000) david     (1000)     2223 2024-04-11 08:57:07.000000 jsonpickle-3.0.4/garden.yaml
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.585614 jsonpickle-3.0.4/images/
+-rw-r--r--   0 david     (1000) david     (1000)    83498 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-0.9.6-3.11.svg
+-rw-r--r--   0 david     (1000) david     (1000)    83313 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-0.9.6-3.9.svg
+-rw-r--r--   0 david     (1000) david     (1000)    83372 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-1.5.1-3.11.svg
+-rw-r--r--   0 david     (1000) david     (1000)    83400 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-1.5.1-3.9.svg
+-rw-r--r--   0 david     (1000) david     (1000)    83497 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-1.5.2-3.11.svg
+-rw-r--r--   0 david     (1000) david     (1000)    82639 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-1.5.2-3.9.svg
+-rw-r--r--   0 david     (1000) david     (1000)    83524 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-2.2.0-3.11.svg
+-rw-r--r--   0 david     (1000) david     (1000)    83406 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-2.2.0-3.9.svg
+-rw-r--r--   0 david     (1000) david     (1000)    83364 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-3.0.0-3.11.svg
+-rw-r--r--   0 david     (1000) david     (1000)    84299 2024-03-19 04:23:33.000000 jsonpickle-3.0.4/images/jsonpickle-3.0.0-3.9.svg
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.589614 jsonpickle-3.0.4/jsonpickle/
+-rw-r--r--   0 david     (1000) david     (1000)     3069 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/jsonpickle/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     9945 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/jsonpickle/backend.py
+-rw-r--r--   0 david     (1000) david     (1000)      330 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/jsonpickle/compat.py
+-rw-r--r--   0 david     (1000) david     (1000)      132 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickle/errors.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.589614 jsonpickle-3.0.4/jsonpickle/ext/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickle/ext/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      558 2024-02-20 03:40:50.000000 jsonpickle-3.0.4/jsonpickle/ext/gmpy.py
+-rw-r--r--   0 david     (1000) david     (1000)    13511 2024-04-09 07:51:26.000000 jsonpickle-3.0.4/jsonpickle/ext/numpy.py
+-rw-r--r--   0 david     (1000) david     (1000)     8288 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/jsonpickle/ext/pandas.py
+-rw-r--r--   0 david     (1000) david     (1000)     8380 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/jsonpickle/handlers.py
+-rw-r--r--   0 david     (1000) david     (1000)    32101 2024-04-11 08:14:07.000000 jsonpickle-3.0.4/jsonpickle/pickler.py
+-rw-r--r--   0 david     (1000) david     (1000)      957 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/jsonpickle/tags.py
+-rw-r--r--   0 david     (1000) david     (1000)    30547 2024-04-11 07:49:01.000000 jsonpickle-3.0.4/jsonpickle/unpickler.py
+-rw-r--r--   0 david     (1000) david     (1000)    14758 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/jsonpickle/util.py
+-rw-r--r--   0 david     (1000) david     (1000)      448 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickle/version.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.589614 jsonpickle-3.0.4/jsonpickle.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     1215 2024-04-11 09:05:36.000000 jsonpickle-3.0.4/jsonpickle.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     2154 2024-04-11 09:05:36.000000 jsonpickle-3.0.4/jsonpickle.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2024-04-11 09:05:36.000000 jsonpickle-3.0.4/jsonpickle.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)      474 2024-04-11 09:05:36.000000 jsonpickle-3.0.4/jsonpickle.egg-info/requires.txt
+-rw-r--r--   0 david     (1000) david     (1000)       11 2024-04-11 09:05:36.000000 jsonpickle-3.0.4/jsonpickle.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.593614 jsonpickle-3.0.4/jsonpickleJS/
+-rw-r--r--   0 david     (1000) david     (1000)      354 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/.gitignore
+-rw-r--r--   0 david     (1000) david     (1000)     1550 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/LICENSE
+-rw-r--r--   0 david     (1000) david     (1000)     4674 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/README.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.577614 jsonpickle-3.0.4/jsonpickleJS/ext/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.593614 jsonpickle-3.0.4/jsonpickleJS/ext/require/
+-rw-r--r--   0 david     (1000) david     (1000)     4035 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/ext/require/domReady.js
+-rw-r--r--   0 david     (1000) david     (1000)     1549 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/ext/require/order.js
+-rw-r--r--   0 david     (1000) david     (1000)    15233 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/ext/require/require.js
+-rw-r--r--   0 david     (1000) david     (1000)    15464 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/ext/require/text.js
+-rw-r--r--   0 david     (1000) david     (1000)      513 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/handlers.js
+-rw-r--r--   0 david     (1000) david     (1000)     1427 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/main.js
+-rw-r--r--   0 david     (1000) david     (1000)     8996 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/pickler.js
+-rw-r--r--   0 david     (1000) david     (1000)      732 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/tags.js
+-rw-r--r--   0 david     (1000) david     (1000)      867 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/testPickle.html
+-rw-r--r--   0 david     (1000) david     (1000)      821 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/testUnpickle.html
+-rw-r--r--   0 david     (1000) david     (1000)    11828 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/unpickler.js
+-rw-r--r--   0 david     (1000) david     (1000)     2164 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/jsonpickleJS/util.js
+-rw-r--r--   0 david     (1000) david     (1000)     8025 2024-02-20 03:40:50.000000 jsonpickle-3.0.4/jsonpickle_benchmarks.py
+-rw-r--r--   0 david     (1000) david     (1000)      354 2024-02-20 03:40:50.000000 jsonpickle-3.0.4/pyproject.toml
+-rw-r--r--   0 david     (1000) david     (1000)      380 2024-04-08 04:55:52.000000 jsonpickle-3.0.4/pytest.ini
+-rw-r--r--   0 david     (1000) david     (1000)     1665 2024-04-11 09:05:36.597614 jsonpickle-3.0.4/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)     8960 2024-01-09 09:49:51.000000 jsonpickle-3.0.4/skeleton.md
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-11 09:05:36.597614 jsonpickle-3.0.4/tests/
+-rw-r--r--   0 david     (1000) david     (1000)     5671 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/backend_test.py
+-rwxr-xr-x   0 david     (1000) david     (1000)     1182 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/tests/benchmark.py
+-rw-r--r--   0 david     (1000) david     (1000)     3054 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/tests/bson_test.py
+-rw-r--r--   0 david     (1000) david     (1000)    11272 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/collections_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     8754 2024-03-12 01:50:32.000000 jsonpickle-3.0.4/tests/datetime_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     2571 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/tests/document_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     1498 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/ecdsa_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     3153 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/tests/feedparser_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     4775 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/tests/handler_test.py
+-rw-r--r--   0 david     (1000) david     (1000)      179 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/tests/helper.py
+-rw-r--r--   0 david     (1000) david     (1000)    59891 2024-04-11 07:49:01.000000 jsonpickle-3.0.4/tests/jsonpickle_test.py
+-rw-r--r--   0 david     (1000) david     (1000)    10796 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/numpy_test.py
+-rw-r--r--   0 david     (1000) david     (1000)    35245 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/object_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     9685 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/pandas_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     2224 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/sklearn_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     4404 2024-04-09 07:30:12.000000 jsonpickle-3.0.4/tests/sqlalchemy_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     1663 2023-03-26 08:31:27.000000 jsonpickle-3.0.4/tests/stdlib_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     7489 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/util_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     8433 2024-04-09 07:51:24.000000 jsonpickle-3.0.4/tests/wizard_test.py
+-rw-r--r--   0 david     (1000) david     (1000)      893 2024-03-12 01:50:32.000000 jsonpickle-3.0.4/tests/zoneinfo_test.py
+-rw-r--r--   0 david     (1000) david     (1000)     1070 2024-03-14 02:28:59.000000 jsonpickle-3.0.4/tox.ini
```

### Comparing `jsonpickle-3.0.3/.github/workflows/lint.yml` & `jsonpickle-3.0.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/.github/workflows/test.yml` & `jsonpickle-3.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/BENCHMARKS.md` & `jsonpickle-3.0.4/BENCHMARKS.md`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/CHANGES.rst` & `jsonpickle-3.0.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,26 @@
+v3.0.4
+======
+    * Fixed an issue with django.SafeString and other classes inheriting from
+      str having read-only attribute errors (#478) (+481)
+    * The test suite was made compatible with `pytest-ruff>=0.3.0`. (+482)
+    * A `garden.yaml` file was added for use with the
+      `garden <https://crates.io/crates/garden-tools>_` command runner. (+486)
+    * The test suite was updated to avoid deprecated SQLALchemy APIs.
+    * The `jaraco.packaging.sphinx` documentation dependency was removed.
+
 v3.0.3
 ======
     * Compatibilty with Pandas and Cython 3.0 was added. (#460) (+477)
     * Fixed a bug where pickling some built-in classes (e.g. zoneinfo) 
       could return a ``None`` module. (#447)
     * Fixed a bug where unpickling a missing class would return a different object
       instead of ``None``. (+471)
-    * Fixed the handling of missing classes when setting ``on_missing`` to ``warn`` or ``error``. (+471)
+    * Fixed the handling of missing classes when setting ``on_missing`` to ``warn``
+      or ``error``. (+471)
     * The test suite was made compatible with Python 3.12.
     * The tox configuration was updated to generate code coverage reports.
     * The suite now uses ``ruff`` to validate python code.
     * The documentation can now be built offline when ``rst.linker`` and
       ``jaraco.packaging.sphinx`` are not available.
 
 v3.0.2
@@ -332,15 +343,15 @@
     * Better support for collections.defaultdict with custom factories.
     * Added support for `queue.Queue` objects.
 
 v0.7.1
 ======
 
     * Added support for Python 3.4.
-    * Added support for :class:`posix.stat_result`.
+    * Added support for `posix.stat_result`.
 
 v0.7.0
 ======
 
     * Added ``handles`` decorator to :class:`jsonpickle.handlers.BaseHandler`,
       enabling simple declaration of a handler for a class.
     * `__getstate__()` and `__setstate__()` are now honored
@@ -361,15 +372,15 @@
     * Python 3.2 support, and additional fixes for Python 3.
 
 v0.6.0
 ======
 
     * Python 3 support!
     * :class:`time.struct_time` is now serialized using the built-in
-      :class:`jsonpickle.handlers.SimpleReduceHandler`.
+      `jsonpickle.handlers.SimpleReduceHandler`.
 
 v0.5.0
 ======
 
     * Non-string dictionary keys (e.g. ints, objects) are now supported
       by passing `keys=True` to :func:`jsonpickle.encode` and
       :func:`jsonpickle.decode`.
```

### Comparing `jsonpickle-3.0.3/LICENSE` & `jsonpickle-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/Makefile` & `jsonpickle-3.0.4/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 JOB_FLAGS := $(shell echo -- $(MAKEFLAGS) | grep -o -e '-j[0-9]\+' | head -n 1)
 # Extract just the number from "-j#".
 JOB_COUNT := $(shell printf '%s' "$(JOB_FLAGS)" | sed -e 's/-j//')
 # We have "-jX" from MAKEFLAGS but tox wants "--parallel X"
 DASH_J := $(shell echo -- $(JOB_FLAGS) -j$(nproc) | grep -o -e '-j[0-9]\+' | head -n 1)
 NUM_JOBS := $(shell printf %s "$(DASH_J)" | sed -e 's/-j//')
 
-TESTCMD ?= $(PYTEST) -p no:cacheprovier
+TESTCMD ?= $(PYTEST)
 BENCHMARKCMD ?= $(BENCHMARK)
 TOXCMD ?= $(TOX) run-parallel --parallel-live
 ifdef V
     TESTCMD += --verbose
     TOXCMD += -v
     BENCHMARKCMD += --benchmark-verbose
 endif
@@ -64,15 +64,15 @@
 	@echo "make tox            - run unit tests using tox"
 	@echo "make clean          - remove cruft"
 	@echo "make benchmark      - run pytest benchmarking"
 	@echo "make doc            - generate documentation using sphinx"
 .PHONY: help
 
 test::
-	$(TESTCMD) $(flags)
+	$(TESTCMD) jsonpickle tests $(flags)
 .PHONY: test
 
 tox::
 	$(TOXCMD) $(flags)
 .PHONY: tox
 
 benchmark::
```

### Comparing `jsonpickle-3.0.3/README.rst` & `jsonpickle-3.0.4/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,15 @@
    :target: https://github.com/jsonpickle/jsonpickle/blob/main/COPYING
    :alt: BSD
 
 
 jsonpickle
 ==========
 jsonpickle is a library for the two-way conversion of complex Python objects
-and `JSON <http://json.org/>`_.  jsonpickle builds upon the existing JSON
+and `JSON <http://json.org/>`_.  jsonpickle builds upon existing JSON
 encoders, such as simplejson, json, and ujson.
 
 .. warning::
 
    jsonpickle can execute arbitrary Python code.
 
    Please see the Security section for more details.
@@ -74,39 +74,25 @@
 
 Install from github for the latest changes:
 
 ::
 
     pip install git+https://github.com/jsonpickle/jsonpickle.git
 
-If you have the files checked out for development:
 
-::
-
-    git clone https://github.com/jsonpickle/jsonpickle.git
-    cd jsonpickle
-    python setup.py develop
-
-
-Numpy Support
+Numpy/Pandas Support
 =============
-jsonpickle includes a built-in numpy extension.  If would like to encode
-sklearn models, numpy arrays, and other numpy-based data then you must
-enable the numpy extension by registering its handlers::
+jsonpickle includes built-in numpy and pandas extensions.  If you would
+like to encode sklearn models, numpy arrays, pandas DataFrames, and other
+numpy/pandas-based data, then you must enable the numpy and/or pandas
+extensions by registering their handlers::
 
     >>> import jsonpickle.ext.numpy as jsonpickle_numpy
-    >>> jsonpickle_numpy.register_handlers()
-
-Pandas Support
-==============
-jsonpickle includes a built-in pandas extension.  If would like to encode
-pandas DataFrame or Series objects then you must enable the pandas extension
-by registering its handlers::
-
     >>> import jsonpickle.ext.pandas as jsonpickle_pandas
+    >>> jsonpickle_numpy.register_handlers()
     >>> jsonpickle_pandas.register_handlers()
 
 Development
 ===========
 
 Use `make` to run the unit tests::
 
@@ -132,20 +118,12 @@
 
 `jsonpickle` supports multiple Python versions, so using a combination of
 multiple virtualenvs and `tox` is useful in order to catch compatibility
 issues when developing.
 
 GPG Signing
 ===========
-Releases before v3.0.0 are signed with `davvid's key <https://keys.openpgp.org/vks/v1/by-fingerprint/FA41BF59C1B48E8C5F3DA61C8CE26BF4A9F606B0>`_. v3.0.0 and after are likely signed by `Theelx's key <https://github.com/Theelx.gpg>`_. All upcoming releases should be signed by one of these two keys, usually Theelx's key.
-
-jsonpickleJS
-============
-`jsonpickleJS <https://github.com/cuthbertLab/jsonpickleJS>`_
-is a javascript implementation of jsonpickle by Michael Scott Cuthbert.
-jsonpickleJS can be extremely useful for projects that have parallel data
-structures between Python and Javascript.
+Unfortunately, while versions of jsonpickle before 3.0.1 should still be signed, GPG signing support was removed from PyPi (https://blog.pypi.org/posts/2023-05-23-removing-pgp/) back in May 2023.
 
 License
 =======
 Licensed under the BSD License. See COPYING for details.
-See jsonpickleJS/LICENSE for details about the jsonpickleJS license.
```

### Comparing `jsonpickle-3.0.3/azure-pipelines.yml` & `jsonpickle-3.0.4/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/conftest.py` & `jsonpickle-3.0.4/conftest.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/contrib/pyqt-reduce-handler.py` & `jsonpickle-3.0.4/contrib/pyqt-reduce-handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 This example demonstrates how to add a custom handler to serialize
-Qt's QPointF class jsonpickle using PyQt4.
+Qt's QPointF class jsonpickle using qtpy.
 
 """
 
 import sys
 import unittest
 
-from PyQt4 import QtCore
+from qtpy import QtCore
 
 import jsonpickle
 from jsonpickle import handlers
 
 text_type = eval('unicode') if str is bytes else str
```

### Comparing `jsonpickle-3.0.3/docs/api.rst` & `jsonpickle-3.0.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/docs/conf.py` & `jsonpickle-3.0.4/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,53 +2,50 @@
 import sys
 
 try:
     import furo
 except ImportError:
     furo = None
 try:
-    import jaraco.packaging.sphinx as jaraco_packaging_sphinx
-except ImportError:
-    jaraco_packaging_sphinx = None
-try:
     import rst.linker as rst_linker
 except ImportError:
     rst_linker = None
 
 # Use the source tree.
 sys.path.insert(1, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.doctest',
     'sphinx.ext.todo',
     'sphinx.ext.coverage',
 ]
-if jaraco_packaging_sphinx is not None:
-    extensions += ['jaraco.packaging.sphinx']
 
+project = 'jsonpickle'
 master_doc = 'index'
 
 if furo is not None:
     html_theme = 'furo'
 
 # Link dates and other references in the changelog
 if rst_linker is not None:
     extensions += ['rst.linker']
+
+package_url = 'https://github.com/jsonpickle/jsonpickle'
 link_files = {
     '../CHANGES.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
-                url='{package_url}/issues/{issue}',
+                url=package_url + '/issues/{issue}',
             ),
             dict(
                 pattern=r'\B\+(?P<pull>\d+)',
-                url='{package_url}/pull/{pull}',
+                url=package_url + '/pull/{pull}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
```

### Comparing `jsonpickle-3.0.3/docs/contrib.rst` & `jsonpickle-3.0.4/docs/contrib.rst`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/docs/extensions.rst` & `jsonpickle-3.0.4/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/docs/index.rst` & `jsonpickle-3.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-0.9.6-3.11.svg` & `jsonpickle-3.0.4/images/jsonpickle-0.9.6-3.11.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-0.9.6-3.9.svg` & `jsonpickle-3.0.4/images/jsonpickle-0.9.6-3.9.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-1.5.1-3.11.svg` & `jsonpickle-3.0.4/images/jsonpickle-1.5.1-3.11.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-1.5.1-3.9.svg` & `jsonpickle-3.0.4/images/jsonpickle-1.5.1-3.9.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-1.5.2-3.11.svg` & `jsonpickle-3.0.4/images/jsonpickle-1.5.2-3.11.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-1.5.2-3.9.svg` & `jsonpickle-3.0.4/images/jsonpickle-1.5.2-3.9.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-2.2.0-3.11.svg` & `jsonpickle-3.0.4/images/jsonpickle-2.2.0-3.11.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-2.2.0-3.9.svg` & `jsonpickle-3.0.4/images/jsonpickle-2.2.0-3.9.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-3.0.0-3.11.svg` & `jsonpickle-3.0.4/images/jsonpickle-3.0.0-3.11.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/images/jsonpickle-3.0.0-3.9.svg` & `jsonpickle-3.0.4/images/jsonpickle-3.0.0-3.9.svg`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickle/__init__.py` & `jsonpickle-3.0.4/jsonpickle/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,16 +63,14 @@
 
 .. note::
 
    Please see the note in the :ref:`api-docs` when serializing dictionaries
    that contain non-string dictionary keys.
 
 """
-from __future__ import absolute_import, division, unicode_literals
-
 # Export other names not in __all__
 from .backend import JSONBackend  # noqa: F401
 from .backend import json
 from .handlers import register  # noqa: F401
 from .handlers import unregister  # noqa: F401
 from .pickler import Pickler  # noqa: F401
 from .pickler import encode
```

### Comparing `jsonpickle-3.0.3/jsonpickle/backend.py` & `jsonpickle-3.0.4/jsonpickle/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, division, unicode_literals
-
 from .compat import string_types
 
 
 class JSONBackend(object):
     """Manages encoding and decoding using various backends.
 
     It tries these modules in this order:
```

### Comparing `jsonpickle-3.0.3/jsonpickle/ext/gmpy.py` & `jsonpickle-3.0.4/jsonpickle/ext/gmpy.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickle/ext/numpy.py` & `jsonpickle-3.0.4/jsonpickle/ext/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-
 import ast
 import json
 import sys
 import warnings
 import zlib
 
 import numpy as np
```

### Comparing `jsonpickle-3.0.3/jsonpickle/ext/pandas.py` & `jsonpickle-3.0.4/jsonpickle/ext/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import
-
 import zlib
 from io import StringIO
 
 import pandas as pd
 
 from .. import decode, encode
 from ..handlers import BaseHandler, register, unregister
```

### Comparing `jsonpickle-3.0.3/jsonpickle/handlers.py` & `jsonpickle-3.0.4/jsonpickle/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 implement ``flatten`` and ``restore``.
 
 A handler can be bound to other types by calling
 :func:`jsonpickle.handlers.register`.
 
 """
 
-from __future__ import absolute_import, division, unicode_literals
-
 import array
 import copy
 import datetime
 import io
 import re
 import sys
 import threading
```

### Comparing `jsonpickle-3.0.3/jsonpickle/pickler.py` & `jsonpickle-3.0.4/jsonpickle/pickler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright (C) 2008 John Paulett (john -at- paulett.org)
-# Copyright (C) 2009-2018 David Aguilar (davvid -at- gmail.com)
+# Copyright (C) 2009-2024 David Aguilar (davvid -at- gmail.com)
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
-from __future__ import absolute_import, division, unicode_literals
-
 import decimal
 import inspect
 import itertools
 import sys
 import warnings
 from itertools import chain, islice
 
@@ -32,14 +30,15 @@
     use_decimal=False,
     numeric_keys=False,
     use_base85=False,
     fail_safe=None,
     indent=None,
     separators=None,
     include_properties=False,
+    handle_readonly=False,
 ):
     """Return a JSON formatted representation of value, a Python object.
 
     :param unpicklable: If set to ``False`` then the output will not contain the
         information necessary to turn the JSON data back into Python objects,
         but a simpler JSON stream is produced. It's recommended to set this
         parameter to ``False`` when your code does not rely on two objects
@@ -50,36 +49,42 @@
         If you want the output to not include the dtype for numpy arrays, add::
 
             jsonpickle.register(
                 numpy.generic, UnpicklableNumpyGenericHandler, base=True
             )
 
         before your pickling code.
-    :param max_depth: If set to a non-negative integer then jsonpickle will
-        not recurse deeper than 'max_depth' steps into the object.  Anything
-        deeper than 'max_depth' is represented using a Python repr() of the
-        object.
     :param make_refs: If set to False jsonpickle's referencing support is
         disabled.  Objects that are id()-identical won't be preserved across
         encode()/decode(), but the resulting JSON stream will be conceptually
         simpler.  jsonpickle detects cyclical objects and will break the cycle
         by calling repr() instead of recursing when make_refs is set False.
     :param keys: If set to True then jsonpickle will encode non-string
         dictionary keys instead of coercing them into strings via `repr()`.
         This is typically what you want if you need to support Integer or
         objects as dictionary keys.
-    :param numeric_keys: Only use this option if the backend supports integer
-        dict keys natively.  This flag tells jsonpickle to leave numeric keys
-        as-is rather than conforming them to json-friendly strings.
-        Using ``keys=True`` is the typical solution for integer keys, so only
-        use this if you have a specific use case where you want to allow the
-        backend to handle serialization of numeric dict keys.
+    :param max_depth: If set to a non-negative integer then jsonpickle will
+        not recurse deeper than 'max_depth' steps into the object.  Anything
+        deeper than 'max_depth' is represented using a Python repr() of the
+        object.
+    :param reset: Custom pickle handlers that use the `Pickler.flatten` method or
+        `jsonpickle.encode` function must call `encode` with `reset=False`
+        in order to retain object references during pickling.
+        This flag is not typically used outside of a custom handler or
+        `__getstate__` implementation.
+    :param backend: If set to an instance of jsonpickle.backend.JSONBackend,
+        jsonpickle will use that backend for deserialization.
     :param warn: If set to True then jsonpickle will warn when it
         returns None for an object which it cannot pickle
         (e.g. file descriptors).
+    :param context: Supply a pre-built Pickler or Unpickler object to the
+        `jsonpickle.encode` and `jsonpickle.decode` machinery instead
+        of creating a new instance. The `context` represents the currently
+        active Pickler and Unpickler objects when custom handlers are
+        invoked by jsonpickle.
     :param max_iter: If set to a non-negative integer then jsonpickle will
         consume at most `max_iter` items when pickling iterators.
     :param use_decimal: If set to True jsonpickle will allow Decimal
         instances to pass-through, with the assumption that the simplejson
         backend will be used in `use_decimal` mode.  In order to use this mode
         you will need to configure simplejson::
 
@@ -87,14 +92,20 @@
                                            use_decimal=True, sort_keys=True)
             jsonpickle.set_decoder_options('simplejson',
                                            use_decimal=True)
             jsonpickle.set_preferred_backend('simplejson')
 
         NOTE: A side-effect of the above settings is that float values will be
         converted to Decimal when converting to json.
+    :param numeric_keys: Only use this option if the backend supports integer
+        dict keys natively.  This flag tells jsonpickle to leave numeric keys
+        as-is rather than conforming them to json-friendly strings.
+        Using ``keys=True`` is the typical solution for integer keys, so only
+        use this if you have a specific use case where you want to allow the
+        backend to handle serialization of numeric dict keys.
     :param use_base85:
         If possible, use base85 to encode binary data. Base85 bloats binary data
         by 1/4 as opposed to base64, which expands it by 1/3. This argument is
         ignored on Python 2 because it doesn't support it.
     :param fail_safe: If set to a function exceptions are ignored when pickling
         and if a exception happens the function is called and the return value
         is used as the value for the object that caused the error
@@ -114,14 +125,19 @@
         not used by jsonpickle directly.
     :param include_properties:
         Include the names and values of class properties in the generated json.
         Properties are unpickled properly regardless of this setting, this is
         meant to be used if processing the json outside of Python. Certain types
         such as sets will not pickle due to not having a native-json equivalent.
         Defaults to ``False``.
+    :param handle_readonly:
+        Handle objects with readonly methods, such as Django's SafeString. This
+        basically prevents jsonpickle from raising an exception for such objects.
+        You MUST set ``handle_readonly=True`` for the decoding if you encode with
+        this flag set to ``True``.
 
     >>> encode('my string') == '"my string"'
     True
     >>> encode(36) == '36'
     True
     >>> encode({'foo': True}) == '{"foo": true}'
     True
@@ -139,14 +155,16 @@
         warn=warn,
         max_iter=max_iter,
         numeric_keys=numeric_keys,
         use_decimal=use_decimal,
         use_base85=use_base85,
         fail_safe=fail_safe,
         include_properties=include_properties,
+        handle_readonly=handle_readonly,
+        original_object=value,
     )
     return backend.encode(
         context.flatten(value, reset=reset), indent=indent, separators=separators
     )
 
 
 def _in_cycle(obj, objs, max_reached, make_refs):
@@ -186,14 +204,16 @@
         warn=False,
         max_iter=None,
         numeric_keys=False,
         use_decimal=False,
         use_base85=False,
         fail_safe=None,
         include_properties=False,
+        handle_readonly=False,
+        original_object=None,
     ):
         self.unpicklable = unpicklable
         self.make_refs = make_refs
         self.backend = backend or json
         self.keys = keys
         self.warn = warn
         self.numeric_keys = numeric_keys
@@ -208,26 +228,30 @@
         self._seen = []
         # maximum amount of items to take from a pickled iterator
         self._max_iter = max_iter
         # Whether to allow decimals to pass-through
         self._use_decimal = use_decimal
         # A cache of objects that have already been flattened.
         self._flattened = {}
+        # Used for util.is_readonly, see +483
+        self.handle_readonly = handle_readonly
 
         if self.use_base85:
             self._bytes_tag = tags.B85
             self._bytes_encoder = util.b85encode
         else:
             self._bytes_tag = tags.B64
             self._bytes_encoder = util.b64encode
 
         # ignore exceptions
         self.fail_safe = fail_safe
         self.include_properties = include_properties
 
+        self._original_object = original_object
+
     def _determine_sort_keys(self):
         for _, options in getattr(self.backend, '_encoder_options', {}).values():
             if options.get("sort_keys", False):
                 # the user has set one of the backends to sort keys
                 return True
         return False
 
@@ -289,17 +313,19 @@
         """
         is_new = self._log_ref(obj)
         # Pretend the object is new
         pretend_new = not self.unpicklable or not self.make_refs
         return pretend_new or is_new
 
     def _getref(self, obj):
+        """Return a "py/id" entry for the specified object"""
         return {tags.ID: self._objs.get(id(obj))}
 
     def _flatten(self, obj):
+        """Flatten an object and its guts into a json-safe representation"""
         if self.unpicklable and self.make_refs:
             result = self._flatten_impl(obj)
         else:
             try:
                 result = self._flattened[id(obj)]
             except KeyError:
                 result = self._flattened[id(obj)] = self._flatten_impl(obj)
@@ -413,14 +439,21 @@
             data = state
         return data
 
     def _flatten_key_value_pair(self, k, v, data):
         """Flatten a key/value pair into the passed-in dictionary."""
         if not util.is_picklable(k, v):
             return data
+        # TODO: use inspect.getmembers_static on 3.11+ because it avoids dynamic attribute lookups
+        if (
+            self.handle_readonly
+            and k in {attr for attr, val in inspect.getmembers(self._original_object)}
+            and util.is_readonly(self._original_object, k, v)
+        ):
+            return data
 
         if k is None:
             k = 'null'  # for compatibility with common json encoders
 
         if self.numeric_keys and isinstance(k, numeric_types):
             pass
         elif not isinstance(k, string_types):
@@ -454,15 +487,15 @@
             allslots = []
 
         # convert to set in case there are a lot of slots
         allslots_set = set(itertools.chain.from_iterable(allslots))
 
         # i don't like lambdas
         def valid_property(x):
-            return not x[0].startswith("__") and x[0] not in allslots_set
+            return not x[0].startswith('__') and x[0] not in allslots_set
 
         properties = [
             x[0] for x in inspect.getmembers(obj.__class__) if valid_property(x)
         ]
 
         properties_dict = {}
         for p_name in properties:
@@ -607,15 +640,17 @@
                     return data
 
         if has_class and not util.is_module(obj):
             if self.unpicklable:
                 data[tags.OBJECT] = class_name
 
             if has_getnewargs_ex:
-                data[tags.NEWARGSEX] = list(map(self._flatten, obj.__getnewargs_ex__()))
+                data[tags.NEWARGSEX] = [
+                    self._flatten(arg) for arg in obj.__getnewargs_ex__()
+                ]
 
             if has_getnewargs and not has_getnewargs_ex:
                 data[tags.NEWARGS] = self._flatten(obj.__getnewargs__())
 
             if has_getinitargs:
                 data[tags.INITARGS] = self._flatten(obj.__getinitargs__())
```

### Comparing `jsonpickle-3.0.3/jsonpickle/tags.py` & `jsonpickle-3.0.4/jsonpickle/tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 These tags are keys into the flattened dictionaries
 created by the Pickler class.  The Unpickler uses
 these custom key names to identify dictionaries
 that need to be specially handled.
 """
 
-from __future__ import absolute_import, division, unicode_literals
-
 BYTES = 'py/bytes'
 B64 = 'py/b64'
 B85 = 'py/b85'
 FUNCTION = 'py/function'
 ID = 'py/id'
 INITARGS = 'py/initargs'
 ITERATOR = 'py/iterator'
```

### Comparing `jsonpickle-3.0.3/jsonpickle/unpickler.py` & `jsonpickle-3.0.4/jsonpickle/unpickler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright (C) 2008 John Paulett (john -at- paulett.org)
-# Copyright (C) 2009-2018 David Aguilar (davvid -at- gmail.com)
+# Copyright (C) 2009-2024 David Aguilar (davvid -at- gmail.com)
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
-from __future__ import absolute_import, division, unicode_literals
-
 import dataclasses
 import sys
 import warnings
 
 from . import compat, errors, handlers, tags, util
 from .backend import json
 from .compat import numeric_types
@@ -21,50 +19,61 @@
     context=None,
     keys=False,
     reset=True,
     safe=False,
     classes=None,
     v1_decode=False,
     on_missing="ignore",
+    handle_readonly=False,
 ):
     """Convert a JSON string into a Python object.
 
-    The keyword argument 'keys' defaults to False.
-    If set to True then jsonpickle will decode non-string dictionary keys
-    into python objects via the jsonpickle protocol.
-
-    The keyword argument 'classes' defaults to None.
-    If set to a single class, or a sequence (list, set, tuple) of classes,
-    then the classes will be made available when constructing objects.
-    If set to a dictionary of class names to class objects, the class object
-    will be provided to jsonpickle to deserialize the class name into.
-    This can be used to give jsonpickle access to local classes that are not
-    available through the global module import scope, and the dict method can
-    be used to deserialize encoded objects into a new class.
-
-    The keyword argument 'safe' defaults to False.
-    If set to True, eval() is avoided, but backwards-compatible
-    (pre-0.7.0) deserialization of repr-serialized objects is disabled.
-
-    The keyword argument 'backend' defaults to None.
-    If set to an instance of jsonpickle.backend.JSONBackend, jsonpickle
-    will use that backend for deserialization.
-
-    The keyword argument 'v1_decode' defaults to False.
-    If set to True it enables you to decode objects serialized in jsonpickle v1.
-    Please do not attempt to re-encode the objects in the v1 format! Version 2's
-    format fixes issue #255, and allows dictionary identity to be preserved
-    through an encode/decode cycle.
-
-    The keyword argument 'on_missing' defaults to 'ignore'.
-    If set to 'error', it will raise an error if the class it's decoding is not
-    found. If set to 'warn', it will warn you in said case. If set to a
-    non-awaitable function, it will call said callback function with the class
-    name (a string) as the only parameter. Strings passed to on_missing are
-    lowercased automatically.
+    :param backend: If set to an instance of jsonpickle.backend.JSONBackend, jsonpickle
+        will use that backend for deserialization.
+
+    :param context: Supply a pre-built Pickler or Unpickler object to the
+        `jsonpickle.encode` and `jsonpickle.decode` machinery instead
+        of creating a new instance. The `context` represents the currently
+        active Pickler and Unpickler objects when custom handlers are
+        invoked by jsonpickle.
+
+    :param keys: If set to True then jsonpickle will decode non-string dictionary keys
+        into python objects via the jsonpickle protocol.
+
+    :param reset: Custom pickle handlers that use the `Pickler.flatten` method or
+        `jsonpickle.encode` function must call `encode` with `reset=False`
+        in order to retain object references during pickling.
+        This flag is not typically used outside of a custom handler or
+        `__getstate__` implementation.
+
+    :param safe: If set to True, eval() is avoided, but backwards-compatible
+        (pre-0.7.0) deserialization of repr-serialized objects is disabled.
+
+    :param classes: If set to a single class, or a sequence (list, set, tuple) of classes,
+        then the classes will be made available when constructing objects.
+        If set to a dictionary of class names to class objects, the class object
+        will be provided to jsonpickle to deserialize the class name into.
+        This can be used to give jsonpickle access to local classes that are not
+        available through the global module import scope, and the dict method can
+        be used to deserialize encoded objects into a new class.
+
+    :param v1_decode: If set to True it enables you to decode objects serialized in jsonpickle v1.
+        Please do not attempt to re-encode the objects in the v1 format! Version 2's
+        format fixes issue #255, and allows dictionary identity to be preserved
+        through an encode/decode cycle.
+
+    :param on_missing: If set to 'error', it will raise an error if the class it's decoding is not
+        found. If set to 'warn', it will warn you in said case. If set to a
+        non-awaitable function, it will call said callback function with the class
+        name (a string) as the only parameter. Strings passed to on_missing are
+        lowercased automatically.
+
+    :param handle_readonly: If set to True, the Unpickler will handle objects encoded with
+        'handle_readonly' properly. Do not set this flag for objects not encoded
+        with 'handle_readonly' set to True.
 
 
     >>> decode('"my string"') == 'my string'
     True
     >>> decode('36')
     36
     """
@@ -79,14 +88,15 @@
     backend = backend or json
     context = context or Unpickler(
         keys=keys,
         backend=backend,
         safe=safe,
         v1_decode=v1_decode,
         on_missing=on_missing,
+        handle_readonly=handle_readonly,
     )
     data = backend.decode(string)
     return context.restore(data, reset=reset, classes=classes)
 
 
 def _safe_hasattr(obj, attr):
     """Workaround unreliable hasattr() availability on sqlalchemy objects"""
@@ -147,18 +157,20 @@
         self._objs = objs
 
     def get(self):
         return self._objs[self._index]
 
 
 def _obj_setattr(obj, attr, proxy):
+    """Use setattr to update a proxy entry"""
     setattr(obj, attr, proxy.get())
 
 
 def _obj_setvalue(obj, idx, proxy):
+    """Use obj[key] assignments to update a proxy entry"""
     obj[idx] = proxy.get()
 
 
 def loadclass(module_and_name, classes=None):
     """Loads the module and returns the class.
 
     >>> cls = loadclass('datetime.datetime')
@@ -292,21 +304,28 @@
 
     """
     return tag in obj
 
 
 class Unpickler(object):
     def __init__(
-        self, backend=None, keys=False, safe=False, v1_decode=False, on_missing="ignore"
+        self,
+        backend=None,
+        keys=False,
+        safe=False,
+        v1_decode=False,
+        on_missing='ignore',
+        handle_readonly=False,
     ):
         self.backend = backend or json
         self.keys = keys
         self.safe = safe
         self.v1_decode = v1_decode
         self.on_missing = on_missing
+        self.handle_readonly = handle_readonly
 
         self.reset()
 
     def reset(self):
         """Resets the object's internal state."""
         # Map reference names to object instances
         self._namedict = {}
@@ -405,15 +424,15 @@
 
         """
         return '/' + '/'.join(self._namestack)
 
     def _mkref(self, obj):
         obj_id = id(obj)
         try:
-            self._obj_to_idx[obj_id]
+            _ = self._obj_to_idx[obj_id]
         except KeyError:
             self._obj_to_idx[obj_id] = len(self._objs)
             self._objs.append(obj)
             # Backwards compatibility: old versions of jsonpickle
             # produced "py/ref" references.
             self._namedict[self._refname()] = obj
         return obj
@@ -622,19 +641,22 @@
                         # useful for other code
                         setattr(instance, f"_{k}", value)
                     except dataclasses.FrozenInstanceError:
                         # issue #240
                         # i think this is the only way to set frozen dataclass attrs
                         object.__setattr__(instance, k, value)
                     except AttributeError as e:
-                        # some objects may raise this for read-only attributes (#422)
+                        # some objects may raise this for read-only attributes (#422) (#478)
                         if (
                             hasattr(instance, "__slots__")
                             and not len(instance.__slots__)
                             and issubclass(instance.__class__, int)
+                            and self.handle_readonly
+                            # we have to handle this separately because of +483
+                            and issubclass(instance.__class__, str)
                         ):
                             continue
                         raise e
                 else:
                     setattr(instance, f"_{instance.__class__.__name__}{k}", value)
 
             # This instance has an instance variable named `k` that is
@@ -693,15 +715,15 @@
                     instance.add(self._restore(v))
 
         if has_tag(obj, tags.STATE):
             instance = self._restore_state(obj, instance)
 
         return instance
 
-    def _restore_object_instance(self, obj, cls, class_name=""):
+    def _restore_object_instance(self, obj, cls, class_name=''):
         # This is a placeholder proxy object which allows child objects to
         # reference the parent object before it has been instantiated.
         proxy = _Proxy()
         self._mkref(proxy)
 
         # An object can install itself as its own factory, so load the factory
         # after the instance is available for referencing.
@@ -715,15 +737,15 @@
         if args:
             args = self._restore(args)
         if kwargs:
             kwargs = self._restore(kwargs)
 
         is_oldstyle = not (isinstance(cls, type) or getattr(cls, '__meta__', None))
         try:
-            if (not is_oldstyle) and hasattr(cls, '__new__'):
+            if not is_oldstyle and hasattr(cls, '__new__'):
                 # new style classes
                 if factory:
                     instance = cls.__new__(cls, factory, *args, **kwargs)
                     instance.default_factory = factory
                 else:
                     instance = cls.__new__(cls, *args, **kwargs)
             else:
@@ -828,14 +850,15 @@
                 self._namestack.pop()
         return data
 
     def _restore_tuple(self, obj):
         return tuple([self._restore(v) for v in obj[tags.TUPLE]])
 
     def _restore_tags(self, obj):
+        """Return the restoration function for the specified object"""
         try:
             if not tags.RESERVED <= set(obj) and type(obj) not in (list, dict):
 
                 def restore(x):
                     return x
 
                 return restore
```

### Comparing `jsonpickle-3.0.3/jsonpickle/util.py` & `jsonpickle-3.0.4/jsonpickle/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
 
 """Helper functions for pickling and unpickling.  Most functions assist in
 determining the type of an object.
 """
-from __future__ import absolute_import, division, unicode_literals
-
 import base64
 import collections
 import inspect
 import io
 import operator
 import sys
 import time
@@ -393,14 +391,28 @@
     return (
         callable(obj)
         and hasattr(obj, '__repr__')
         and repr(obj).startswith('<cyfunction ')
     )
 
 
+def is_readonly(obj, attr, value):
+    # CPython 3.11+ has 0-cost try/except, please use up-to-date versions!
+    try:
+        setattr(obj, attr, value)
+        return False
+    except AttributeError:
+        # this is okay, it means the attribute couldn't be set
+        return True
+    except TypeError:
+        # this should only be happening when obj is a dict
+        # as these errors happen when attr isn't a str
+        return True
+
+
 def in_dict(obj, key, default=False):
     """
     Returns true if key exists in obj.__dict__; false if not in.
     If obj.__dict__ is absent, return default
     """
     return (key in obj.__dict__) if getattr(obj, '__dict__', None) else default
```

### Comparing `jsonpickle-3.0.3/jsonpickle.egg-info/SOURCES.txt` & `jsonpickle-3.0.4/jsonpickle.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 CHANGES.rst
 LICENSE
 Makefile
 README.rst
 appveyor.yml
 azure-pipelines.yml
 conftest.py
+garden.yaml
 jsonpickle_benchmarks.py
 pyproject.toml
 pytest.ini
-requirements-dev.txt
 setup.cfg
-setup.py
 skeleton.md
 tox.ini
 .github/FUNDING.yml
 .github/workflows/lint.yml
 .github/workflows/test.yml
 contrib/copy-docs
 contrib/pyqt-reduce-handler.py
```

### Comparing `jsonpickle-3.0.3/jsonpickleJS/LICENSE` & `jsonpickle-3.0.4/jsonpickleJS/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/README.md` & `jsonpickle-3.0.4/jsonpickleJS/README.md`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/ext/require/domReady.js` & `jsonpickle-3.0.4/jsonpickleJS/ext/require/domReady.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/ext/require/order.js` & `jsonpickle-3.0.4/jsonpickleJS/ext/require/order.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/ext/require/require.js` & `jsonpickle-3.0.4/jsonpickleJS/ext/require/require.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/ext/require/text.js` & `jsonpickle-3.0.4/jsonpickleJS/ext/require/text.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/handlers.js` & `jsonpickle-3.0.4/jsonpickleJS/handlers.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/main.js` & `jsonpickle-3.0.4/jsonpickleJS/main.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/pickler.js` & `jsonpickle-3.0.4/jsonpickleJS/pickler.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/tags.js` & `jsonpickle-3.0.4/jsonpickleJS/tags.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/testPickle.html` & `jsonpickle-3.0.4/jsonpickleJS/testPickle.html`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/testUnpickle.html` & `jsonpickle-3.0.4/jsonpickleJS/testUnpickle.html`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/unpickler.js` & `jsonpickle-3.0.4/jsonpickleJS/unpickler.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickleJS/util.js` & `jsonpickle-3.0.4/jsonpickleJS/util.js`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/jsonpickle_benchmarks.py` & `jsonpickle-3.0.4/jsonpickle_benchmarks.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/setup.cfg` & `jsonpickle-3.0.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [metadata]
 license_file = LICENSE
 name = jsonpickle
 author = David Aguilar
 author_email = davvid@gmail.com
-description = Python library for serializing any arbitrary object graph into JSON
-long_description = file:README.rst
+description = Serialize any Python object to JSON
+long_description = Python library for serializing arbitrary object graphs into JSON
 url = https://github.com/jsonpickle/jsonpickle
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: JavaScript
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 platforms = 
 	POSIX
 	Windows
 keywords = 
@@ -41,31 +42,36 @@
 
 [options.extras_require]
 testing = 
 	pytest >= 3.5, !=3.7.3
 	pytest-checkdocs >= 1.2.3
 	pytest-cov
 	pytest-enabler >= 1.0.1
-	pytest-ruff
+	pytest-ruff >= 0.2.1
 	
+	bson
 	ecdsa
 	feedparser
 	gmpy2; python_version<"3.12"
 	numpy
 	pandas
 	pymongo
+	pytest-benchmark
+	pytest-benchmark[histogram]
 	scikit-learn
+	scipy>=1.9.3; python_version>"3.10"
+	scipy; python_version<="3.10"
 	simplejson
 	sqlalchemy
 	ujson
 docs = 
 	sphinx
-	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
-
-[options.entry_points]
+packaging = 
+	build
+	twine
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `jsonpickle-3.0.3/skeleton.md` & `jsonpickle-3.0.4/skeleton.md`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/tests/backend_test.py` & `jsonpickle-3.0.4/tests/backend_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, division, unicode_literals
-
 import decimal
 import unittest
 from hashlib import md5
 from warnings import warn
 
 from helper import SkippableTest
 
@@ -50,15 +48,15 @@
         self._is_installed(backend)
         jsonpickle.set_preferred_backend(backend)
 
     def tearDown(self):
         # always reset to default backend
         jsonpickle.set_preferred_backend('json')
 
-    def assertEncodeDecode(self, json_input):
+    def assert_roundtrip(self, json_input):
         expect = SAMPLE_DATA
         actual = jsonpickle.decode(json_input)
         self.assertEqual(expect['things'][0].name, actual['things'][0].name)
         self.assertEqual(expect['things'][0].child, actual['things'][0].child)
 
         pickled = jsonpickle.encode(SAMPLE_DATA)
         actual = jsonpickle.decode(pickled)
@@ -91,30 +89,30 @@
         expected_pickled = (
             '{"things": [{'
             '"py/object": "backend_test.Thing", '
             '"name": "data", '
             '"child": null} '
             ']}'
         )
-        self.assertEncodeDecode(expected_pickled)
+        self.assert_roundtrip(expected_pickled)
 
 
 class SimpleJsonTestCase(BackendBase):
     def setUp(self):
         self.set_preferred_backend('simplejson')
 
     def test_backend(self):
         expected_pickled = (
             '{"things": [{'
             '"py/object": "backend_test.Thing", '
             '"name": "data", '
             '"child": null}'
             ']}'
         )
-        self.assertEncodeDecode(expected_pickled)
+        self.assert_roundtrip(expected_pickled)
 
     def test_decimal(self):
         # Default behavior: Decimal is preserved
         obj = decimal.Decimal(0.5)
         as_json = jsonpickle.dumps(obj)
         clone = jsonpickle.loads(as_json)
         self.assertTrue(isinstance(clone, decimal.Decimal))
@@ -166,15 +164,15 @@
     def test_backend(self):
         expected_pickled = (
             '{"things":[{'
             r'"py\/object":"backend_test.Thing",'
             '"name":"data","child":null}'
             ']}'
         )
-        self.assertEncodeDecode(expected_pickled)
+        self.assert_roundtrip(expected_pickled)
 
 
 def suite():
     suite = unittest.TestSuite()
     suite.addTest(unittest.makeSuite(JsonTestCase))
     suite.addTest(unittest.makeSuite(UJsonTestCase))
     suite.addTest(unittest.makeSuite(SimpleJsonTestCase))
```

### Comparing `jsonpickle-3.0.3/tests/benchmark.py` & `jsonpickle-3.0.4/tests/benchmark.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/tests/bson_test.py` & `jsonpickle-3.0.4/tests/bson_test.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/tests/collections_test.py` & `jsonpickle-3.0.4/tests/collections_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 Unit tests for collections
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
-
 import sys
 from collections import OrderedDict, defaultdict
 
 import pytest
 
 import jsonpickle
```

### Comparing `jsonpickle-3.0.3/tests/datetime_test.py` & `jsonpickle-3.0.4/tests/datetime_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,18 +175,18 @@
         """
         # if sys.version_info >= (3, 9):
         from zoneinfo import ZoneInfo
 
         now = datetime.datetime.now()
 
         SaoPaulo = ZoneInfo('America/Sao_Paulo')
-        USEastern = ZoneInfo('US/Eastern')
+        NewYork = ZoneInfo('America/New_York')
 
         now_sp = now.replace(tzinfo=SaoPaulo)
-        now_us = now.replace(tzinfo=USEastern)
+        now_us = now.replace(tzinfo=NewYork)
 
         self._roundtrip(now_sp)
         self._roundtrip(now_us)
 
 
 class DateTimeAdvancedTestCase(unittest.TestCase):
     def setUp(self):
```

### Comparing `jsonpickle-3.0.3/tests/document_test.py` & `jsonpickle-3.0.4/tests/document_test.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/tests/ecdsa_test.py` & `jsonpickle-3.0.4/tests/ecdsa_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Test serializing ecdsa keys"""
 
-from __future__ import absolute_import, division, unicode_literals
-
 import unittest
 
 import pytest
 from helper import SkippableTest
 
 import jsonpickle
```

### Comparing `jsonpickle-3.0.3/tests/feedparser_test.py` & `jsonpickle-3.0.4/tests/feedparser_test.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/tests/handler_test.py` & `jsonpickle-3.0.4/tests/handler_test.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/tests/jsonpickle_test.py` & `jsonpickle-3.0.4/tests/jsonpickle_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright (C) 2008 John Paulett (john -at- paulett.org)
-# Copyright (C) 2009-2021 David Aguilar (davvid -at- gmail.com)
+# Copyright (C) 2009-2024 David Aguilar (davvid -at- gmail.com)
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
-from __future__ import absolute_import, division, unicode_literals
-
 import collections
 import os
 import unittest
 import warnings
 
 import pytest
 from helper import SkippableTest
@@ -47,14 +45,17 @@
 
 
 class Capture:
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
 
+    def __repr__(self):
+        return object.__repr__(self) + ('(%r, %r)' % (self.args, self.kwargs))
+
 
 class ThingWithProps:
     def _get_identity(self):
         keys = [self.dogs, self.monkies, self.name]
         return hash('-'.join([str(key) for key in keys]))
 
     identity = property(_get_identity)
@@ -160,14 +161,23 @@
             self.alpha == other.alpha
             and self.arr == other.arr
             and self.arr_len == other.arr_len
             and list(self.other_object) == list(other.other_object)
         )
 
 
+# see issue #478
+class SafeData:
+    __slots__ = ()
+
+
+class SafeString(str, SafeData):
+    __slots__ = ()
+
+
 def on_missing_callback(class_name):
     # not actually a runtime problem but it doesn't matter
     warnings.warn("The unpickler couldn't find %s" % class_name, RuntimeWarning)
 
 
 class PicklingTestCase(unittest.TestCase):
     def setUp(self):
@@ -190,21 +200,21 @@
 
     def test_py3_bytes_base64_default(self):
         data = os.urandom(16)
         encoded = util.b64encode(data)
         self.assertEqual({tags.B64: encoded}, self.pickler.flatten(data))
 
     def test_decode_base85(self):
-        pickled = {tags.B85: 'P{Y4;Xv4O{u^=-c'}
-        expected = u'P\u00ffth\u00f6\u00f1 3!'.encode('utf-8')
+        expected = 'Pÿthöñ 3!'.encode('utf-8')
+        pickled = {tags.B85: util.b85encode(expected)}
         self.assertEqual(expected, self.unpickler.restore(pickled))
 
     def test_base85_still_handles_base64(self):
-        pickled = {tags.B64: 'UMO/dGjDtsOxIDMh'}
-        expected = u'P\u00ffth\u00f6\u00f1 3!'.encode('utf-8')
+        expected = 'Pÿthöñ 3!'.encode('utf-8')
+        pickled = {tags.B64: util.b64encode(expected)}
         self.assertEqual(expected, self.unpickler.restore(pickled))
 
     def test_string(self):
         self.assertEqual('a string', self.pickler.flatten('a string'))
         self.assertEqual('a string', self.unpickler.restore('a string'))
 
     def test_unicode(self):
@@ -986,14 +996,25 @@
 
     def test_depth_tracking(self):
         liszt = []
         pickler = jsonpickle.Pickler()
         pickler.flatten([liszt, liszt, liszt, liszt, liszt])
         self.assertEqual(pickler._depth, -1)
 
+    def test_readonly_attrs(self):
+        s = SafeString("test")
+        pickled = jsonpickle.encode(s, handle_readonly=True)
+        pickled_json_dict = jsonpickle.backend.json.loads(pickled)
+        # make sure it's giving concise output by erroring if it includes
+        # a default method which is unnecessary
+        self.assertTrue("join" not in pickled_json_dict)
+        unpickled = jsonpickle.decode(pickled)
+        self.assertEqual(unpickled.__class__, SafeString)
+        self.assertEqual(unpickled, s)
+
 
 class PicklableNamedTuple(object):
     """
     A picklable namedtuple wrapper, to demonstrate the need
     for protocol 2 compatibility. Yes, this is contrived in
     its use of new, but it demonstrates the issue.
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jsonpickle-3.0.3/tests/numpy_test.py` & `jsonpickle-3.0.4/tests/numpy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, division, unicode_literals
-
 import datetime
 import warnings
 
 import pytest
 
 try:
     import numpy as np
```

### Comparing `jsonpickle-3.0.3/tests/object_test.py` & `jsonpickle-3.0.4/tests/object_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, division, unicode_literals
-
 import array
 import collections
 import datetime
 import decimal
 import enum
 import re
 import threading
```

### Comparing `jsonpickle-3.0.3/tests/pandas_test.py` & `jsonpickle-3.0.4/tests/pandas_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, division, unicode_literals
-
 import datetime
 
 import pytest
 
 try:
     import numpy as np
     import pandas as pd
```

### Comparing `jsonpickle-3.0.3/tests/sklearn_test.py` & `jsonpickle-3.0.4/tests/sklearn_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import absolute_import, division, unicode_literals
-
 import pytest
 
 try:
     import numpy as np
     import sklearn.datasets
     from sklearn.linear_model import LogisticRegression
     from sklearn.tree import DecisionTreeClassifier
```

### Comparing `jsonpickle-3.0.3/tests/sqlalchemy_test.py` & `jsonpickle-3.0.4/tests/sqlalchemy_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 
 from helper import SkippableTest
 
 import jsonpickle
 
 try:
     import sqlalchemy as sqa
+    from sqlalchemy import orm
     from sqlalchemy.ext import declarative
     from sqlalchemy.orm import Session
 
     HAS_SQA = True
 except ImportError:
     HAS_SQA = False
 
 if HAS_SQA:
-    Base = declarative.declarative_base()
+    # sqlalchemy.ext.declarative.declarative_base() was deprecated in SQLAlchemy 2.0
+    # and replaced by sqlalchemy.orm.declarative_base().
+    if hasattr(orm, 'declarative_base'):
+        Base = orm.declarative_base()
+    else:
+        Base = declarative.declarative_base()
 
     class Table(Base):
         __tablename__ = 'table'
         id = sqa.Column(sqa.Integer, primary_key=True)
         name = sqa.Column(sqa.Text)
         value = sqa.Column(sqa.Float)
```

### Comparing `jsonpickle-3.0.3/tests/stdlib_test.py` & `jsonpickle-3.0.4/tests/stdlib_test.py`

 * *Files identical despite different names*

### Comparing `jsonpickle-3.0.3/tests/util_test.py` & `jsonpickle-3.0.4/tests/util_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # Copyright (C) 2008 John Paulett (john -at- paulett.org)
 # Copyright (C) 2009-2018 David Aguilar (davvid -at- gmail.com)
 # All rights reserved.
 #
 # This software is licensed as described in the file COPYING, which
 # you should have received as part of this distribution.
-
-from __future__ import absolute_import, division, unicode_literals
-
 import doctest
 import io
 import time
 import unittest
 
 from jsonpickle import compat, util
```

### Comparing `jsonpickle-3.0.3/tests/wizard_test.py` & `jsonpickle-3.0.4/tests/wizard_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 http://www.petrounias.org/articles/2014/09/16/pickling-python-collections-with-non-built-in-type-keys-and-cycles/
 
 Includes functionality to assist with adding compatibility to jsonpickle.
 
 """
 
-from __future__ import absolute_import, division, unicode_literals
-
 import collections
 import unittest
 
 from jsonpickle import decode, encode
 
 
 class World(object):
```

### Comparing `jsonpickle-3.0.3/tests/zoneinfo_test.py` & `jsonpickle-3.0.4/tests/zoneinfo_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             unpickled = jsonpickle.decode(pickled)
             self.assertEqual(obj, unpickled)
 
         def test_zoneinfo(self):
             """
             jsonpickle should pickle a zoneinfo object
             """
-            self._roundtrip(ZoneInfo("Australia/Queensland"))
+            self._roundtrip(ZoneInfo("Australia/Brisbane"))
 
     def suite():
         suite = unittest.TestSuite()
         suite.addTest(unittest.makeSuite(ZoneInfoSimpleTestCase))
         return suite
 
     if __name__ == '__main__':
```

### Comparing `jsonpickle-3.0.3/tox.ini` & `jsonpickle-3.0.4/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [tox]
 minversion = 4.0
 envlist = clean,py36,py37,py38,py39,py310,py311,py312,report
 skip_missing_interpreters = true
 
 [testenv]
+allowlist_externals =
+	ruff
 passenv =
 	FORCE_COLOR
 commands =
-	python3 -m pytest -p no:cacheprovider --cov --cov-append --cov-report=term-missing jsonpickle tests {posargs}
+	python3 -m pytest --cov --cov-append --cov-report=term-missing jsonpickle tests {posargs}
 depends =
 	{py36,py37,py38,py39,py310,py311,py312}: clean
 	report: py36,py37,py38,py39,py310,py311,py312
 extras =
 	testing
 pip_version = pip
 sitepackages = true
```

