# Comparing `tmp/rdt-1.9.2.dev0.tar.gz` & `tmp/rdt-1.9.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt-1.9.2.dev0.tar", last modified: Tue Feb 13 19:19:25 2024, max compression
+gzip compressed data, was "rdt-1.9.3.dev0.tar", last modified: Wed Mar 13 11:10:09 2024, max compression
```

## Comparing `rdt-1.9.2.dev0.tar` & `rdt-1.9.3.dev0.tar`

### file list

```diff
@@ -1,112 +1,48 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.825995 rdt-1.9.2.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22810 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52758 2024-01-10 22:43:42.000000 rdt-1.9.2.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60798 2024-02-13 19:19:25.826145 rdt-1.9.2.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7132 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6495 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.803882 rdt-1.9.2.dev0/rdt/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5342 2024-01-10 22:44:17.000000 rdt-1.9.2.dev0/rdt/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/rdt/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    36559 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/rdt/hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.805742 rdt-1.9.2.dev0/rdt/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/rdt/performance/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.808005 rdt-1.9.2.dev0/rdt/performance/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/rdt/performance/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/rdt/performance/datasets/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.9.2.dev0/rdt/performance/datasets/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-06-01 21:46:38.000000 rdt-1.9.2.dev0/rdt/performance/datasets/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/rdt/performance/datasets/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/rdt/performance/datasets/numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2023-06-01 21:46:38.000000 rdt-1.9.2.dev0/rdt/performance/datasets/pii.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/rdt/performance/datasets/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/rdt/performance/datasets/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3372 2023-06-01 21:46:38.000000 rdt-1.9.2.dev0/rdt/performance/performance.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.9.2.dev0/rdt/performance/profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.809948 rdt-1.9.2.dev0/rdt/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5190 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/rdt/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.810170 rdt-1.9.2.dev0/rdt/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3345 2023-07-12 20:34:31.000000 rdt-1.9.2.dev0/rdt/transformers/addons/addons_setup.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19851 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/rdt/transformers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3794 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/rdt/transformers/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    31684 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/rdt/transformers/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11367 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/rdt/transformers/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6460 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/rdt/transformers/null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22866 2024-02-13 19:11:19.000000 rdt-1.9.2.dev0/rdt/transformers/numerical.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.810963 rdt-1.9.2.dev0/rdt/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.9.2.dev0/rdt/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3048 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/rdt/transformers/pii/anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14644 2024-01-10 22:43:42.000000 rdt-1.9.2.dev0/rdt/transformers/pii/anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/rdt/transformers/pii/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7634 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/rdt/transformers/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7687 2024-02-13 19:11:19.000000 rdt-1.9.2.dev0/rdt/transformers/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.805070 rdt-1.9.2.dev0/rdt.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60798 2024-02-13 19:19:25.000000 rdt-1.9.2.dev0/rdt.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2980 2024-02-13 19:19:25.000000 rdt-1.9.2.dev0/rdt.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-02-13 19:19:25.000000 rdt-1.9.2.dev0/rdt.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-02-13 19:19:25.000000 rdt-1.9.2.dev0/rdt.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1437 2024-02-13 19:19:25.000000 rdt-1.9.2.dev0/rdt.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2024-02-13 19:19:25.000000 rdt-1.9.2.dev0/rdt.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2024-02-13 19:19:25.826517 rdt-1.9.2.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4124 2024-01-10 22:44:17.000000 rdt-1.9.2.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.811859 rdt-1.9.2.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18320 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.800246 rdt-1.9.2.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.813251 rdt-1.9.2.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.814400 rdt-1.9.2.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67719 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9535 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.816537 rdt-1.9.2.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.817387 rdt-1.9.2.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/tests/integration/transformers/pii/test_anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8080 2023-08-22 19:30:54.000000 rdt-1.9.2.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10206 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-07-12 20:34:31.000000 rdt-1.9.2.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19590 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7853 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15116 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11135 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.818221 rdt-1.9.2.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5171 2023-08-22 19:30:54.000000 rdt-1.9.2.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.818727 rdt-1.9.2.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.9.2.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.819682 rdt-1.9.2.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-07-12 20:34:31.000000 rdt-1.9.2.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   123777 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.823521 rdt-1.9.2.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.823756 rdt-1.9.2.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.824368 rdt-1.9.2.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-02-13 19:19:25.825792 rdt-1.9.2.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.9.2.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5307 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/tests/unit/transformers/pii/test_anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    33517 2024-01-10 22:43:42.000000 rdt-1.9.2.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.9.2.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3227 2023-08-22 19:30:54.000000 rdt-1.9.2.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    49566 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-10-27 17:15:14.000000 rdt-1.9.2.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    78145 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20563 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20799 2023-11-14 22:48:38.000000 rdt-1.9.2.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    55491 2024-02-13 19:11:19.000000 rdt-1.9.2.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18419 2024-02-12 22:51:07.000000 rdt-1.9.2.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6714 2024-02-13 19:11:19.000000 rdt-1.9.2.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-13 11:10:09.833370 rdt-1.9.3.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.9.3.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11463 2024-03-13 11:10:09.833252 rdt-1.9.3.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7132 2023-11-14 22:48:38.000000 rdt-1.9.3.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5137 2024-03-13 11:09:59.000000 rdt-1.9.3.dev0/pyproject.toml
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-13 11:10:09.819917 rdt-1.9.3.dev0/rdt/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5342 2024-02-13 21:05:17.000000 rdt-1.9.3.dev0/rdt/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.9.3.dev0/rdt/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    36559 2024-02-13 21:04:40.000000 rdt-1.9.3.dev0/rdt/hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-13 11:10:09.822147 rdt-1.9.3.dev0/rdt/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.9.3.dev0/rdt/performance/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-13 11:10:09.825629 rdt-1.9.3.dev0/rdt/performance/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.9.3.dev0/rdt/performance/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.9.3.dev0/rdt/performance/datasets/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.9.3.dev0/rdt/performance/datasets/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-06-01 21:46:38.000000 rdt-1.9.3.dev0/rdt/performance/datasets/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.9.3.dev0/rdt/performance/datasets/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.9.3.dev0/rdt/performance/datasets/numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2023-06-01 21:46:38.000000 rdt-1.9.3.dev0/rdt/performance/datasets/pii.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.9.3.dev0/rdt/performance/datasets/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.9.3.dev0/rdt/performance/datasets/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3372 2023-06-01 21:46:38.000000 rdt-1.9.3.dev0/rdt/performance/performance.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.9.3.dev0/rdt/performance/profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-13 11:10:09.828372 rdt-1.9.3.dev0/rdt/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4597 2024-03-13 10:39:00.000000 rdt-1.9.3.dev0/rdt/transformers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19851 2024-02-13 21:04:40.000000 rdt-1.9.3.dev0/rdt/transformers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3794 2023-11-14 22:48:38.000000 rdt-1.9.3.dev0/rdt/transformers/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    31684 2024-02-13 21:04:40.000000 rdt-1.9.3.dev0/rdt/transformers/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11367 2023-11-14 22:48:38.000000 rdt-1.9.3.dev0/rdt/transformers/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6460 2023-11-14 22:48:38.000000 rdt-1.9.3.dev0/rdt/transformers/null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22866 2024-02-13 21:04:40.000000 rdt-1.9.3.dev0/rdt/transformers/numerical.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-13 11:10:09.829573 rdt-1.9.3.dev0/rdt/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.9.3.dev0/rdt/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3048 2023-11-14 22:48:38.000000 rdt-1.9.3.dev0/rdt/transformers/pii/anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17279 2024-03-13 10:39:00.000000 rdt-1.9.3.dev0/rdt/transformers/pii/anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.9.3.dev0/rdt/transformers/pii/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7634 2024-02-13 21:04:40.000000 rdt-1.9.3.dev0/rdt/transformers/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7687 2024-02-13 21:04:40.000000 rdt-1.9.3.dev0/rdt/transformers/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-13 11:10:09.830184 rdt-1.9.3.dev0/rdt.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11463 2024-03-13 11:10:09.000000 rdt-1.9.3.dev0/rdt.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1074 2024-03-13 11:10:09.000000 rdt-1.9.3.dev0/rdt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2024-03-13 11:10:09.000000 rdt-1.9.3.dev0/rdt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       35 2024-03-13 11:10:09.000000 rdt-1.9.3.dev0/rdt.egg-info/entry_points.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1385 2024-03-13 11:10:09.000000 rdt-1.9.3.dev0/rdt.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2024-03-13 11:10:09.000000 rdt-1.9.3.dev0/rdt.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2024-03-13 11:10:09.833654 rdt-1.9.3.dev0/setup.cfg
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2024-03-13 11:10:09.829837 rdt-1.9.3.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1332 2024-03-13 10:39:00.000000 rdt-1.9.3.dev0/tests/test_tasks.py
```

### Comparing `rdt-1.9.2.dev0/LICENSE` & `rdt-1.9.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/README.md` & `rdt-1.9.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/__init__.py` & `rdt-1.9.3.dev0/rdt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for RDT."""
 
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.9.2.dev0'
+__version__ = '1.9.3.dev0'
 
 
 import sys
 import warnings
 from operator import attrgetter
 from types import ModuleType
```

### Comparing `rdt-1.9.2.dev0/rdt/errors.py` & `rdt-1.9.3.dev0/rdt/errors.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/hyper_transformer.py` & `rdt-1.9.3.dev0/rdt/hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/__init__.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/base.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/boolean.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/categorical.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/datetime.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/numerical.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/pii.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/pii.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/text.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/datasets/utils.py` & `rdt-1.9.3.dev0/rdt/performance/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/performance.py` & `rdt-1.9.3.dev0/rdt/performance/performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/performance/profiling.py` & `rdt-1.9.3.dev0/rdt/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/__init__.py` & `rdt-1.9.3.dev0/rdt/transformers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Transformers module."""
 
 import importlib
 import inspect
-import json
-import sys
 from collections import defaultdict
 from copy import deepcopy
 from functools import lru_cache
-from pathlib import Path
 
 from rdt.transformers.base import BaseMultiColumnTransformer, BaseTransformer
 from rdt.transformers.boolean import BinaryEncoder
 from rdt.transformers.categorical import (
     CustomLabelEncoder, FrequencyEncoder, LabelEncoder, OneHotEncoder, OrderedLabelEncoder,
     OrderedUniformEncoder, UniformEncoder)
 from rdt.transformers.datetime import OptimizedTimestampEncoder, UnixTimestampEncoder
@@ -45,29 +42,14 @@
     'get_default_transformers',
     'get_default_transformer',
     'UniformEncoder',
     'OrderedUniformEncoder',
 ]
 
 
-def _import_addons():
-    """Import all the addon modules."""
-    addons_path = Path(__file__).parent / 'addons'
-    for addon_json_path in addons_path.glob('*/*.json'):
-        with open(addon_json_path, 'r', encoding='utf-8') as addon_json_file:
-            transformers = json.load(addon_json_file).get('transformers', [])
-            for transformer in transformers:
-                module = transformer.rsplit('.', 1)[0]
-                if module not in sys.modules:
-                    importlib.import_module(module)
-
-
-_import_addons()
-
-
 def get_transformer_name(transformer):
     """Return the fully qualified path of the transformer.
 
     Args:
         transformer:
             A transformer class.
```

### Comparing `rdt-1.9.2.dev0/rdt/transformers/base.py` & `rdt-1.9.3.dev0/rdt/transformers/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/boolean.py` & `rdt-1.9.3.dev0/rdt/transformers/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/categorical.py` & `rdt-1.9.3.dev0/rdt/transformers/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/datetime.py` & `rdt-1.9.3.dev0/rdt/transformers/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/null.py` & `rdt-1.9.3.dev0/rdt/transformers/null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/numerical.py` & `rdt-1.9.3.dev0/rdt/transformers/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/pii/anonymization.py` & `rdt-1.9.3.dev0/rdt/transformers/pii/anonymization.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/pii/anonymizer.py` & `rdt-1.9.3.dev0/rdt/transformers/pii/anonymizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import warnings
 from collections.abc import Iterable
 from copy import deepcopy
 from operator import attrgetter
 
 import faker
 import numpy as np
+import pandas as pd
 
 from rdt.errors import TransformerInputError, TransformerProcessingError
 from rdt.transformers.base import BaseTransformer
 from rdt.transformers.categorical import LabelEncoder
 
 
 class AnonymizedFaker(BaseTransformer):
@@ -29,28 +30,36 @@
         function_name (str):
             The name of the function to use within the ``faker.provider``. Defaults to
             ``lexify``.
         function_kwargs (dict):
             Keyword args to pass into the ``function_name`` when being called.
         locales (list):
             List of localized providers to use instead of the global provider.
+        cardinality_rule (str):
+            If ``'unique'`` enforce that every created value is unique.
+            If ``'match'`` match the cardinality of the data seen during fit.
+            If ``None`` do not consider cardinality.
+            Defaults to ``None``.
         enforce_uniqueness (bool):
-            Whether or not to ensure that the new anonymized data is all unique. If it isn't
-            possible to create the requested number of rows, then an error will be raised.
+            **DEPRECATED** Whether or not to ensure that the new anonymized data is all unique.
+            If it isn't possible to create the requested number of rows, then an error will be
+            raised.
             Defaults to ``False``.
         missing_value_generation (str or None):
             The way missing values are being handled. There are two strategies:
 
                 * ``random``: Randomly generates missing values based on the percentage of
                   missing values.
                 * ``None``: Don't learn anything during fit. Then during reverse transform,
                   don't create any missing values.
 
     """
 
+    # pylint: disable=too-many-instance-attributes
+
     IS_GENERATOR = True
     INPUT_SDTYPE = 'pii'
 
     @staticmethod
     def check_provider_function(provider_name, function_name):
         """Check that the provider and the function exist.
 
@@ -94,18 +103,29 @@
                 f"Locales {missed_locales} do not support provider '{self.provider_name}' "
                 f"and function '{self.function_name}'.\nIn place of these locales, 'en_US' will "
                 'be used instead. Please refer to the localized provider docs for more '
                 'information: https://faker.readthedocs.io/en/master/locales.html'
             )
 
     def __init__(self, provider_name=None, function_name=None, function_kwargs=None,
-                 locales=None, enforce_uniqueness=False, missing_value_generation='random'):
+                 locales=None, cardinality_rule=None, enforce_uniqueness=False,
+                 missing_value_generation='random'):
         super().__init__()
+        self._data_cardinality = None
         self.data_length = None
-        self.enforce_uniqueness = enforce_uniqueness
+        self.cardinality_rule = cardinality_rule.lower() if cardinality_rule else None
+        if enforce_uniqueness:
+            warnings.warn(
+                "The 'enforce_uniqueness' parameter is no longer supported. "
+                "Please use the 'cardinality_rule' parameter instead.",
+                FutureWarning
+            )
+            if not self.cardinality_rule:
+                self.cardinality_rule = 'unique'
+
         self.provider_name = provider_name if provider_name else 'BaseProvider'
         if self.provider_name != 'BaseProvider' and function_name is None:
             raise TransformerInputError(
                 'Please specify the function name to use from the '
                 f"'{self.provider_name}' provider."
             )
 
@@ -152,15 +172,19 @@
         """Create a new ``Faker`` instance."""
         super().reset_randomization()
         self.faker = faker.Faker(self.locales)
         self.faker.seed_instance(self._faker_random_seed)
 
     def _function(self):
         """Return the result of calling the ``faker`` function."""
-        faker_attr = self.faker.unique if self.enforce_uniqueness else self.faker
+        if self.cardinality_rule in {'unique', 'match'}:
+            faker_attr = self.faker.unique
+        else:
+            faker_attr = self.faker
+
         result = getattr(faker_attr, self.function_name)(**self.function_kwargs)
 
         if isinstance(result, Iterable) and not isinstance(result, str):
             result = ', '.join(map(str, result))
 
         return result
 
@@ -181,18 +205,50 @@
                 Data to fit to.
         """
         self._set_faker_seed(data)
         self.data_length = len(data)
         if self.missing_value_generation == 'random':
             self._nan_frequency = data.isna().sum() / len(data)
 
+        if self.cardinality_rule == 'match':
+            # remove nans from data
+            self._data_cardinality = len(data.dropna().unique())
+
     def _transform(self, _data):
         """Drop the input column by returning ``None``."""
         return None
 
+    def _get_unique_categories(self, samples):
+        return np.array([self._function() for _ in range(samples)], dtype=object)
+
+    def _reverse_transform_cardinality_rule_match(self, sample_size):
+        """Reverse transform the data when the cardinality rule is 'match'."""
+        reverse_transformed = np.array([], dtype=object)
+        if self.missing_value_generation == 'random':
+            num_nans = int(self._nan_frequency * sample_size)
+            reverse_transformed = np.concatenate([reverse_transformed, np.full(num_nans, np.nan)])
+        else:
+            num_nans = 0
+
+        if sample_size <= num_nans:
+            return reverse_transformed
+
+        if sample_size < num_nans + self._data_cardinality:
+            unique_categories = self._get_unique_categories(sample_size - num_nans)
+            reverse_transformed = np.concatenate([reverse_transformed, unique_categories])
+        else:
+            unique_categories = self._get_unique_categories(self._data_cardinality)
+            num_copies = sample_size - self._data_cardinality - num_nans
+            copies = np.random.choice(unique_categories, num_copies)
+            reverse_transformed = np.concatenate([reverse_transformed, unique_categories, copies])
+
+        np.random.shuffle(reverse_transformed)
+
+        return reverse_transformed
+
     def _reverse_transform(self, data):
         """Generate new anonymized data using a ``faker.provider.function``.
 
         Args:
             data (pd.Series or numpy.ndarray):
                 Data to transform.
 
@@ -201,26 +257,30 @@
         """
         if data is not None and len(data):
             sample_size = len(data)
         else:
             sample_size = self.data_length
 
         try:
-            reverse_transformed = np.array([
-                self._function()
-                for _ in range(sample_size)
-            ], dtype=object)
+            if self.cardinality_rule == 'match':
+                reverse_transformed = self._reverse_transform_cardinality_rule_match(sample_size)
+            else:
+                reverse_transformed = np.array([
+                    self._function()
+                    for _ in range(sample_size)
+                ], dtype=object)
+
         except faker.exceptions.UniquenessException as exception:
             raise TransformerProcessingError(
                 f'The Faker function you specified is not able to generate {sample_size} unique '
                 'values. Please use a different Faker function for column '
                 f"('{self.get_input_column()}')."
             ) from exception
 
-        if self.missing_value_generation == 'random':
+        if self.missing_value_generation == 'random' and not pd.isna(reverse_transformed).any():
             num_nans = int(self._nan_frequency * sample_size)
             nan_indices = np.random.choice(sample_size, num_nans, replace=False)
             reverse_transformed[nan_indices] = np.nan
 
         return reverse_transformed
 
     def __repr__(self):
@@ -231,14 +291,15 @@
                 The name of the transformer followed by any non-default parameters.
         """
         class_name = self.__class__.get_name()
         custom_args = []
         args = inspect.getfullargspec(self.__init__)
         keys = args.args[1:]
         defaults = dict(zip(keys, args.defaults))
+        keys.remove('enforce_uniqueness')
         instanced = {key: getattr(self, key) for key in keys}
 
         defaults['function_name'] = None
         for arg, value in instanced.items():
             if value and defaults[arg] != value and value != 'BaseProvider':
                 value = f"'{value}'" if isinstance(value, str) else value
                 custom_args.append(f'{arg}={value}')
@@ -279,15 +340,15 @@
 
     def __init__(self, provider_name=None, function_name=None, function_kwargs=None, locales=None):
         super().__init__(
             provider_name=provider_name,
             function_name=function_name,
             function_kwargs=function_kwargs,
             locales=locales,
-            enforce_uniqueness=True
+            cardinality_rule='unique'
         )
         self._mapping_dict = {}
         self._reverse_mapping_dict = {}
         self.output_properties = {
             None: {'sdtype': 'categorical', 'next_transformer': LabelEncoder(add_noise=True)}
         }
```

### Comparing `rdt-1.9.2.dev0/rdt/transformers/pii/utils.py` & `rdt-1.9.3.dev0/rdt/transformers/pii/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/text.py` & `rdt-1.9.3.dev0/rdt/transformers/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt/transformers/utils.py` & `rdt-1.9.3.dev0/rdt/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.9.2.dev0/rdt.egg-info/requires.txt` & `rdt-1.9.3.dev0/rdt.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 pandas>=1.1.3
 scipy<2,>=1.5.4
 scikit-learn<2,>=0.24
 
 [:python_version >= "3.10"]
 numpy<2,>=1.23.3
 scipy<2,>=1.9.2
-scikit-learn<2,>=1.1.3
 
 [:python_version >= "3.10" and python_version < "3.11"]
 pandas>=1.3.4
+scikit-learn>=1.1.0
 
 [:python_version >= "3.11"]
 pandas>=1.5.0
+scikit-learn<2,>=1.1.3
 
 [copulas]
-copulas<0.10,>=0.9.0
+copulas<0.11,>=0.10.0
 
 [dev]
-bumpversion<0.6,>=0.5.3
+rdt[test]
+bump-my-version<1,>=0.18.3
 pip>=9.0.1
 watchdog<0.11,>=0.8.3
 pycodestyle<2.8.0,>=2.7.0
 pyflakes<2.4.0,>=2.3.0
 flake8<4,>=3.7.7
 flake8-absolute-import<2,>=1.0
 flake8-builtins<1.6,>=1.5.3
@@ -53,21 +55,17 @@
 autopep8<1.6,>=1.4.3
 twine<4,>=1.10.0
 wheel>=0.30.0
 coverage<6,>=4.5.1
 tox<4,>=2.9.1
 tabulate<1,>=0.8.9
 invoke
-pytest>=3.4.2
-pytest-cov>=2.6.0
-jupyter<2,>=1.0.0
-rundoc<0.5,>=0.4.3
-pytest-subtests<1.0,>=0.5
-copulas<0.10,>=0.9.0
 
 [test]
+rdt[copulas]
 pytest>=3.4.2
 pytest-cov>=2.6.0
 jupyter<2,>=1.0.0
 rundoc<0.5,>=0.4.3
 pytest-subtests<1.0,>=0.5
-copulas<0.10,>=0.9.0
+pytest-runner>=2.11.1
+tomli<3,>=2.0.0
```

