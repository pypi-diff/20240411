# Comparing `tmp/cbor2-5.6.2.tar.gz` & `tmp/cbor2-5.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbor2-5.6.2.tar", last modified: Mon Feb 19 18:23:50 2024, max compression
+gzip compressed data, was "cbor2-5.6.3.tar", last modified: Wed Apr 10 22:17:51 2024, max compression
```

## Comparing `cbor2-5.6.2.tar` & `cbor2-5.6.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.726218 cbor2-5.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.714218 cbor2-5.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.718218 cbor2-5.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-19 18:23:38.000000 cbor2-5.6.2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-19 18:23:38.000000 cbor2-5.6.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-19 18:23:38.000000 cbor2-5.6.2/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.718218 cbor2-5.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-02-19 18:23:38.000000 cbor2-5.6.2/.github/workflows/cifuzz.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-02-19 18:23:38.000000 cbor2-5.6.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-02-19 18:23:38.000000 cbor2-5.6.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-19 18:23:38.000000 cbor2-5.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-19 18:23:38.000000 cbor2-5.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-19 18:23:38.000000 cbor2-5.6.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-19 18:23:38.000000 cbor2-5.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-02-19 18:23:50.726218 cbor2-5.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-02-19 18:23:38.000000 cbor2-5.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.718218 cbor2-5.6.2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-19 18:23:38.000000 cbor2-5.6.2/benchmarks/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.718218 cbor2-5.6.2/benchmarks/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-19 18:23:38.000000 cbor2-5.6.2/benchmarks/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-02-19 18:23:38.000000 cbor2-5.6.2/benchmarks/tests/test_vs_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.718218 cbor2-5.6.2/cbor2/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30156 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    29762 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-19 18:23:38.000000 cbor2-5.6.2/cbor2/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.726218 cbor2-5.6.2/cbor2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-02-19 18:23:50.000000 cbor2-5.6.2/cbor2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-02-19 18:23:50.000000 cbor2-5.6.2/cbor2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 18:23:50.000000 cbor2-5.6.2/cbor2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-19 18:23:50.000000 cbor2-5.6.2/cbor2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-19 18:23:50.000000 cbor2-5.6.2/cbor2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-19 18:23:50.000000 cbor2-5.6.2/cbor2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.722218 cbor2-5.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-19 18:23:38.000000 cbor2-5.6.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-19 18:23:38.000000 cbor2-5.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-02-19 18:23:38.000000 cbor2-5.6.2/docs/customizing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-19 18:23:38.000000 cbor2-5.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-02-19 18:23:38.000000 cbor2-5.6.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-02-19 18:23:38.000000 cbor2-5.6.2/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-02-19 18:23:38.000000 cbor2-5.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.722218 cbor2-5.6.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      887 2024-02-19 18:23:38.000000 cbor2-5.6.2/scripts/coverage.sh
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-19 18:23:38.000000 cbor2-5.6.2/scripts/coverage_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-19 18:23:38.000000 cbor2-5.6.2/scripts/half_float_tables.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7722 2024-02-19 18:23:38.000000 cbor2-5.6.2/scripts/ref_leak_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8574 2024-02-19 18:23:38.000000 cbor2-5.6.2/scripts/speed_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 18:23:50.726218 cbor2-5.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-19 18:23:38.000000 cbor2-5.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.726218 cbor2-5.6.2/source/
--rw-r--r--   0 runner    (1001) docker     (127)    71475 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    69931 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/encoder.c
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    38105 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/halffloat.c
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/halffloat.h
--rw-r--r--   0 runner    (1001) docker     (127)    29803 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/module.c
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/module.h
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/tags.c
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-19 18:23:38.000000 cbor2-5.6.2/source/tags.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:50.726218 cbor2-5.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/examples.cbor.b64
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/examples.json
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/hypothesis_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    30481 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18661 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-02-19 18:23:38.000000 cbor2-5.6.2/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.788780 cbor2-5.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.776780 cbor2-5.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.776780 cbor2-5.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-10 22:17:46.000000 cbor2-5.6.3/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 22:17:46.000000 cbor2-5.6.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-10 22:17:46.000000 cbor2-5.6.3/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.780779 cbor2-5.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-10 22:17:46.000000 cbor2-5.6.3/.github/workflows/cifuzz.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-10 22:17:46.000000 cbor2-5.6.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-10 22:17:46.000000 cbor2-5.6.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 22:17:46.000000 cbor2-5.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-10 22:17:46.000000 cbor2-5.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 22:17:46.000000 cbor2-5.6.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-10 22:17:46.000000 cbor2-5.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-10 22:17:51.788780 cbor2-5.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-10 22:17:46.000000 cbor2-5.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.780779 cbor2-5.6.3/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 22:17:46.000000 cbor2-5.6.3/benchmarks/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.780779 cbor2-5.6.3/benchmarks/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-10 22:17:46.000000 cbor2-5.6.3/benchmarks/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-10 22:17:46.000000 cbor2-5.6.3/benchmarks/tests/test_vs_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.780779 cbor2-5.6.3/cbor2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29762 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-10 22:17:46.000000 cbor2-5.6.3/cbor2/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.788780 cbor2-5.6.3/cbor2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-10 22:17:51.000000 cbor2-5.6.3/cbor2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-10 22:17:51.000000 cbor2-5.6.3/cbor2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:17:51.000000 cbor2-5.6.3/cbor2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 22:17:51.000000 cbor2-5.6.3/cbor2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-10 22:17:51.000000 cbor2-5.6.3/cbor2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 22:17:51.000000 cbor2-5.6.3/cbor2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.784779 cbor2-5.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 22:17:46.000000 cbor2-5.6.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-10 22:17:46.000000 cbor2-5.6.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-10 22:17:46.000000 cbor2-5.6.3/docs/customizing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-10 22:17:46.000000 cbor2-5.6.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-10 22:17:46.000000 cbor2-5.6.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-10 22:17:46.000000 cbor2-5.6.3/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-10 22:17:46.000000 cbor2-5.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.784779 cbor2-5.6.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      887 2024-04-10 22:17:46.000000 cbor2-5.6.3/scripts/coverage.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-10 22:17:46.000000 cbor2-5.6.3/scripts/coverage_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-10 22:17:46.000000 cbor2-5.6.3/scripts/half_float_tables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7722 2024-04-10 22:17:46.000000 cbor2-5.6.3/scripts/ref_leak_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8574 2024-04-10 22:17:46.000000 cbor2-5.6.3/scripts/speed_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:17:51.788780 cbor2-5.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-10 22:17:46.000000 cbor2-5.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.784779 cbor2-5.6.3/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    71548 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69934 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/encoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38105 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/halffloat.c
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/halffloat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30049 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/module.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/tags.c
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 22:17:46.000000 cbor2-5.6.3/source/tags.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:51.788780 cbor2-5.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/examples.cbor.b64
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/examples.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/hypothesis_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30481 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18661 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-10 22:17:46.000000 cbor2-5.6.3/tests/test_types.py
```

### Comparing `cbor2-5.6.2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `cbor2-5.6.3/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/.github/ISSUE_TEMPLATE/features_request.yaml` & `cbor2-5.6.3/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/.github/workflows/cifuzz.yml` & `cbor2-5.6.3/.github/workflows/cifuzz.yml`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/.github/workflows/publish.yml` & `cbor2-5.6.3/.github/workflows/publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,22 @@
       if: runner.os == 'Linux'
       uses: docker/setup-qemu-action@v3
       with:
         platforms: arm64
     - name: Build wheels
       uses: pypa/cibuildwheel@v2.16.5
       env:
+        CBOR2_BUILD_C_EXTENSION: "1"
         CIBW_SKIP: pp* cp36* cp37*
         CIBW_ARCHS: auto64
         CIBW_ARCHS_MACOS: x86_64 arm64
         CIBW_ARCHS_LINUX: x86_64 aarch64
-    - uses: actions/upload-artifact@v3
+    - uses: actions/upload-artifact@v4
       with:
-        name: wheels
+        name: wheels-${{ matrix.os }}
         path: wheelhouse/*.whl
 
   sdist-purewheel:
     runs-on: ubuntu-latest
     environment: release
     steps:
     - uses: actions/checkout@v4
@@ -45,30 +46,30 @@
         python-version: 3.x
     - name: Install dependencies
       run: pip install build
     - name: Create sdist and pure-Python wheel
       run: python -m build .
       env:
         CBOR2_BUILD_C_EXTENSION: "0"
-    - uses: actions/upload-artifact@v3
+    - uses: actions/upload-artifact@v4
       with:
         name: sdist
         path: dist/*
 
   publish:
     needs:
       - binary-wheels
       - sdist-purewheel
     runs-on: ubuntu-latest
     environment: release
     permissions:
       id-token: write
     steps:
     - name: Download generated packaging artifacts
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
     - name: Move the packages to dist/
       run: |
         mkdir dist
         mv */*.whl */*.tar.gz dist
     - name: Upload packages
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `cbor2-5.6.2/.github/workflows/test.yml` & `cbor2-5.6.3/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,19 @@
         allow-prereleases: true
         cache: pip
         cache-dependency-path: pyproject.toml
     - name: Install dependencies
       run: pip install -e .[test]
       env:
         CFLAGS: "-UNDEBUG"
+        CBOR2_BUILD_C_EXTENSION: "${{ matrix.python-version == 'pypy-3.10' && '0' || '1' }}"
     - name: Test with pytest
       run: coverage run -m pytest -v
+      env:
+        TZ: America/New_York
     - name: Generate coverage report
       run: coverage xml
     - name: Upload Coverage
       uses: coverallsapp/github-action@v2
       with:
         parallel: true
         file: coverage.xml
```

### Comparing `cbor2-5.6.2/.pre-commit-config.yaml` & `cbor2-5.6.3/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This is the configuration file for pre-commit (https://pre-commit.com/).
 # To use:
 # * Install pre-commit (https://pre-commit.com/#installation)
 # * Copy this file as ".pre-commit-config.yaml"
 # * Run "pre-commit install".
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       - id: mypy
         additional_dependencies:
           - pytest
         files: cbor2/.+
 
   - repo: https://github.com/pre-commit/pygrep-hooks
```

### Comparing `cbor2-5.6.2/LICENSE.txt` & `cbor2-5.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/PKG-INFO` & `cbor2-5.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbor2
-Version: 5.6.2
+Version: 5.6.3
 Summary: CBOR (de)serializer with extensive tag support
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 Maintainer-email: "Kio Smallwood (Sekenre)" <kio@mothers-arms.co.uk>
 License: MIT
 Project-URL: Changelog, https://cbor2.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Documentation, https://cbor2.readthedocs.org/en/latest/
 Project-URL: Source Code, https://github.com/agronholm/cbor2
```

### Comparing `cbor2-5.6.2/README.rst` & `cbor2-5.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/benchmarks/tests/conftest.py` & `cbor2-5.6.3/benchmarks/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/benchmarks/tests/test_vs_json.py` & `cbor2-5.6.3/benchmarks/tests/test_vs_json.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/cbor2/__init__.py` & `cbor2-5.6.3/cbor2/__init__.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/cbor2/_decoder.py` & `cbor2-5.6.3/cbor2/_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,20 +246,18 @@
             old_fp = self.fp
             self.fp = fp
             retval = self._decode()
             self.fp = old_fp
             return retval
 
     @overload
-    def _decode_length(self, subtype: int) -> int:
-        ...
+    def _decode_length(self, subtype: int) -> int: ...
 
     @overload
-    def _decode_length(self, subtype: int, allow_indefinite: Literal[True]) -> int | None:
-        ...
+    def _decode_length(self, subtype: int, allow_indefinite: Literal[True]) -> int | None: ...
 
     def _decode_length(self, subtype: int, allow_indefinite: bool = False) -> int | None:
         if subtype < 24:
             return subtype
         elif subtype == 24:
             return self.read(1)[0]
         elif subtype == 25:
```

### Comparing `cbor2-5.6.2/cbor2/_encoder.py` & `cbor2-5.6.3/cbor2/_encoder.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/cbor2/_types.py` & `cbor2-5.6.3/cbor2/_types.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/cbor2/tool.py` & `cbor2-5.6.3/cbor2/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command-line tool for CBOR diagnostics and testing"""
+
 from __future__ import annotations
 
 import argparse
 import base64
 import decimal
 import fractions
 import io
```

### Comparing `cbor2-5.6.2/cbor2/types.py` & `cbor2-5.6.3/cbor2/types.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/cbor2.egg-info/PKG-INFO` & `cbor2-5.6.3/cbor2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbor2
-Version: 5.6.2
+Version: 5.6.3
 Summary: CBOR (de)serializer with extensive tag support
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 Maintainer-email: "Kio Smallwood (Sekenre)" <kio@mothers-arms.co.uk>
 License: MIT
 Project-URL: Changelog, https://cbor2.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Documentation, https://cbor2.readthedocs.org/en/latest/
 Project-URL: Source Code, https://github.com/agronholm/cbor2
```

### Comparing `cbor2-5.6.2/cbor2.egg-info/SOURCES.txt` & `cbor2-5.6.3/cbor2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/docs/api.rst` & `cbor2-5.6.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/docs/conf.py` & `cbor2-5.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/docs/customizing.rst` & `cbor2-5.6.3/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/docs/usage.rst` & `cbor2-5.6.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/docs/versionhistory.rst` & `cbor2-5.6.3/docs/versionhistory.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Version history
 ===============
 
 .. currentmodule:: cbor2
 
 This library adheres to `Semantic Versioning <http://semver.org/>`_.
 
+**5.6.3** (2024-04-11)
+
+- Fixed decoding of epoch-based dates being affected by the local time zone in the C extension
+
 **5.6.2** (2024-02-19)
 
 - Fixed ``__hash__()`` of the C version of the ``CBORTag`` type crashing when there's a recursive
   reference cycle
 - Fixed type annotation for the file object in ``cbor2.dump()``, ``cbor2.load()``, ``CBOREncoder``
   and ``CBORDecoder`` to be ``IO[bytes]`` instead of ``BytesIO``
 - Worked around a `CPython bug <https://github.com/python/cpython/issues/99612>`_ that caused
```

### Comparing `cbor2-5.6.2/pyproject.toml` & `cbor2-5.6.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -93,14 +93,21 @@
 skip_missing_interpreters = true
 minversion = 4.0.0
 
 [testenv]
 commands = python -m pytest {posargs}
 package = editable
 extras = test
+setenv =
+  TZ=America/New_York
+  CBOR2_BUILD_C_EXTENSION=1
+
+[testenv:pypy3]
+setenv =
+  TZ=America/New_York
 
 [testenv:docs]
 extras = doc
 commands = sphinx-build -W -n docs build/sphinx
 package = wheel
 
 [testenv:.pkg-docs]
```

### Comparing `cbor2-5.6.2/scripts/coverage.sh` & `cbor2-5.6.3/scripts/coverage.sh`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/scripts/coverage_server.py` & `cbor2-5.6.3/scripts/coverage_server.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/scripts/half_float_tables.py` & `cbor2-5.6.3/scripts/half_float_tables.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/scripts/ref_leak_test.py` & `cbor2-5.6.3/scripts/ref_leak_test.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/scripts/speed_test.py` & `cbor2-5.6.3/scripts/speed_test.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/setup.py` & `cbor2-5.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/source/decoder.c` & `cbor2-5.6.3/source/decoder.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
+#include <datetime.h>
 #include <string.h>
 #include <stdbool.h>
 #include <limits.h>
 #if __FreeBSD__
 #include <sys/endian.h>
 #elif __APPLE__
 #include <libkern/OSByteOrder.h>
 #elif ! _WIN32
 #include <endian.h>
 #endif
 #include <stdint.h>
 #include <math.h>
 #include <structmember.h>
-#include <datetime.h>
 #include "module.h"
 #include "halffloat.h"
 #include "tags.h"
 #include "decoder.h"
 
 #if __APPLE__
 #define be16toh(x) OSSwapBigToHostInt16(x)
@@ -345,15 +345,15 @@
         Py_RETURN_FALSE;
 }
 
 
 // Utility functions /////////////////////////////////////////////////////////
 
 static int
-raise_from(const PyObject *new_exc_type, const char *message) {
+raise_from(PyObject *new_exc_type, const char *message) {
     // This requires the error indicator to be set
     PyObject *cause;
 #if PY_VERSION_HEX >= 0x030c0000
     cause = PyErr_GetRaisedException();
 #else
     PyObject *exc_type, *exc_traceback;
     PyErr_Fetch(&exc_type, &cause, &exc_traceback);
@@ -1334,23 +1334,24 @@
 }
 
 // CBORDecoder.decode_epoch_date(self)
 static PyObject *
 CBORDecoder_decode_epoch_date(CBORDecoderObject *self)
 {
     // semantic type 100
-    PyObject *num, *tuple, *ret = NULL;
+    PyObject *num, *ordinal, *ret = NULL;
 
     num = decode(self, DECODE_NORMAL);
     if (num) {
         if (PyNumber_Check(num)) {
-            tuple = PyTuple_Pack(1, PyNumber_Multiply(num, PyLong_FromLong(24 * 60 * 60)));
-            if (tuple) {
-                ret = PyDate_FromTimestamp(tuple);
-                Py_DECREF(tuple);
+            ordinal = PyNumber_Add(num, _CBOR2_date_ordinal_offset);
+            if (ordinal) {
+                ret = PyObject_CallMethodObjArgs(
+                    (PyObject*) PyDateTimeAPI->DateType, _CBOR2_str_fromordinal, ordinal, NULL);
+                Py_DECREF(ordinal);
             }
         } else {
             PyErr_Format(
                 _CBOR2_CBORDecodeValueError, "invalid timestamp value %R", num);
         }
         Py_DECREF(num);
     }
```

### Comparing `cbor2-5.6.2/source/decoder.h` & `cbor2-5.6.3/source/decoder.h`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/source/encoder.c` & `cbor2-5.6.3/source/encoder.c`

 * *Files 0% similar despite different names*

```diff
@@ -1052,15 +1052,15 @@
         if (tmp)
             ret = CBOREncoder_encode_datetime(self, tmp);
     }
     else if (self->timestamp_format) {
         tmp = PyObject_CallMethodObjArgs(
                 value, _CBOR2_str_toordinal, NULL);
         if (tmp && fp_write(self, "\xD8\x64", 2) == 0) {
-            ret = CBOREncoder_encode_int(self, PyNumber_Subtract(tmp, PyLong_FromLong(719163)));
+            ret = CBOREncoder_encode_int(self, PyNumber_Subtract(tmp, _CBOR2_date_ordinal_offset));
         }
     } else {
         tmp = PyObject_CallMethodObjArgs(
                 value, _CBOR2_str_isoformat, NULL);
         if (tmp && fp_write(self, "\xD9\x03\xEC", 3) == 0) {
             ret = CBOREncoder_encode_string(self, tmp);
         }
```

### Comparing `cbor2-5.6.2/source/encoder.h` & `cbor2-5.6.3/source/encoder.h`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/source/halffloat.c` & `cbor2-5.6.3/source/halffloat.c`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/source/module.c` & `cbor2-5.6.3/source/module.c`

 * *Files 2% similar despite different names*

```diff
@@ -617,14 +617,15 @@
 }
 
 
 // Module definition /////////////////////////////////////////////////////////
 
 PyObject *_CBOR2_empty_bytes = NULL;
 PyObject *_CBOR2_empty_str = NULL;
+PyObject *_CBOR2_date_ordinal_offset = NULL;
 PyObject *_CBOR2_str_as_string = NULL;
 PyObject *_CBOR2_str_as_tuple = NULL;
 PyObject *_CBOR2_str_bit_length = NULL;
 PyObject *_CBOR2_str_bytes = NULL;
 PyObject *_CBOR2_str_BytesIO = NULL;
 PyObject *_CBOR2_str_canonical_encoders = NULL;
 PyObject *_CBOR2_str_compile = NULL;
@@ -634,14 +635,15 @@
 PyObject *_CBOR2_str_Decimal = NULL;
 PyObject *_CBOR2_str_default_encoders = NULL;
 PyObject *_CBOR2_str_denominator = NULL;
 PyObject *_CBOR2_str_encode_date = NULL;
 PyObject *_CBOR2_str_Fraction = NULL;
 PyObject *_CBOR2_str_fromtimestamp = NULL;
 PyObject *_CBOR2_str_FrozenDict = NULL;
+PyObject *_CBOR2_str_fromordinal = NULL;
 PyObject *_CBOR2_str_getvalue = NULL;
 PyObject *_CBOR2_str_groups = NULL;
 PyObject *_CBOR2_str_ip_address = NULL;
 PyObject *_CBOR2_str_ip_network = NULL;
 PyObject *_CBOR2_str_is_infinite = NULL;
 PyObject *_CBOR2_str_is_nan = NULL;
 PyObject *_CBOR2_str_isoformat = NULL;
@@ -967,14 +969,15 @@
     INTERN_STRING(Decimal);
     INTERN_STRING(default_encoders);
     INTERN_STRING(denominator);
     INTERN_STRING(encode_date);
     INTERN_STRING(Fraction);
     INTERN_STRING(fromtimestamp);
     INTERN_STRING(FrozenDict);
+    INTERN_STRING(fromordinal);
     INTERN_STRING(getvalue);
     INTERN_STRING(groups);
     INTERN_STRING(ip_address);
     INTERN_STRING(ip_network);
     INTERN_STRING(is_infinite);
     INTERN_STRING(is_nan);
     INTERN_STRING(isoformat);
@@ -996,14 +999,17 @@
     INTERN_STRING(update);
     INTERN_STRING(utc);
     INTERN_STRING(UUID);
     INTERN_STRING(write);
 
 #undef INTERN_STRING
 
+    if (!_CBOR2_date_ordinal_offset &&
+            !(_CBOR2_date_ordinal_offset = PyLong_FromLong(719163)))
+        goto error;
     if (!_CBOR2_str_utc_suffix &&
             !(_CBOR2_str_utc_suffix = PyUnicode_InternFromString("+00:00")))
         goto error;
     if (!_CBOR2_str_datetimestr_re &&
         !(_CBOR2_str_datetimestr_re = PyUnicode_InternFromString(
                     "^(\\d{4})-(\\d\\d)-(\\d\\d)T"     // Y-m-d
                     "(\\d\\d):(\\d\\d):(\\d\\d)"       // H:M:S
```

### Comparing `cbor2-5.6.2/source/module.h` & `cbor2-5.6.3/source/module.h`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 // CBORSimpleValue namedtuple type
 extern PyTypeObject CBORSimpleValueType;
 
 // Various interned strings
 extern PyObject *_CBOR2_empty_bytes;
 extern PyObject *_CBOR2_empty_str;
+extern PyObject *_CBOR2_date_ordinal_offset;
 extern PyObject *_CBOR2_str_as_string;
 extern PyObject *_CBOR2_str_as_tuple;
 extern PyObject *_CBOR2_str_bit_length;
 extern PyObject *_CBOR2_str_bytes;
 extern PyObject *_CBOR2_str_BytesIO;
 extern PyObject *_CBOR2_str_canonical_encoders;
 extern PyObject *_CBOR2_str_compile;
@@ -45,14 +46,15 @@
 extern PyObject *_CBOR2_str_Decimal;
 extern PyObject *_CBOR2_str_default_encoders;
 extern PyObject *_CBOR2_str_denominator;
 extern PyObject *_CBOR2_str_encode_date;
 extern PyObject *_CBOR2_str_Fraction;
 extern PyObject *_CBOR2_str_fromtimestamp;
 extern PyObject *_CBOR2_str_FrozenDict;
+extern PyObject *_CBOR2_str_fromordinal;
 extern PyObject *_CBOR2_str_getvalue;
 extern PyObject *_CBOR2_str_groups;
 extern PyObject *_CBOR2_str_ip_address;
 extern PyObject *_CBOR2_str_ip_network;
 extern PyObject *_CBOR2_str_is_infinite;
 extern PyObject *_CBOR2_str_is_nan;
 extern PyObject *_CBOR2_str_isoformat;
```

### Comparing `cbor2-5.6.2/source/tags.c` & `cbor2-5.6.3/source/tags.c`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/tests/conftest.py` & `cbor2-5.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/tests/examples.cbor.b64` & `cbor2-5.6.3/tests/examples.cbor.b64`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/tests/examples.json` & `cbor2-5.6.3/tests/examples.json`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/tests/hypothesis_strategies.py` & `cbor2-5.6.3/tests/hypothesis_strategies.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/tests/test_decoder.py` & `cbor2-5.6.3/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/tests/test_encoder.py` & `cbor2-5.6.3/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/tests/test_tool.py` & `cbor2-5.6.3/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `cbor2-5.6.2/tests/test_types.py` & `cbor2-5.6.3/tests/test_types.py`

 * *Files identical despite different names*

