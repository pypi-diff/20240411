# Comparing `tmp/openparse-0.5.1.tar.gz` & `tmp/openparse-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openparse-0.5.1.tar", last modified: Mon Apr  8 21:08:37 2024, max compression
+gzip compressed data, was "openparse-0.5.2.tar", last modified: Thu Apr 11 14:23:20 2024, max compression
```

## Comparing `openparse-0.5.1.tar` & `openparse-0.5.2.tar`

### file list

```diff
@@ -1,90 +1,89 @@
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.558946 openparse-0.5.1/
--rw-r--r--   0 sergey     (501) staff       (20)     1072 2024-03-26 18:50:21.000000 openparse-0.5.1/LICENSE
--rw-r--r--   0 sergey     (501) staff       (20)     7961 2024-04-08 21:08:37.558677 openparse-0.5.1/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     7259 2024-04-08 14:44:49.000000 openparse-0.5.1/README.md
--rw-r--r--   0 sergey     (501) staff       (20)       38 2024-04-08 21:08:37.559000 openparse-0.5.1/setup.cfg
--rw-r--r--   0 sergey     (501) staff       (20)      917 2024-04-08 20:56:22.000000 openparse-0.5.1/setup.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.537869 openparse-0.5.1/src/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.539330 openparse-0.5.1/src/evals/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-25 03:59:07.000000 openparse-0.5.1/src/evals/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      684 2024-03-31 16:14:48.000000 openparse-0.5.1/src/evals/run_evals.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.539965 openparse-0.5.1/src/notebooks/
--rw-r--r--   0 sergey     (501) staff       (20)       68 2024-03-25 18:09:44.000000 openparse-0.5.1/src/notebooks/config.py
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 21:37:35.000000 openparse-0.5.1/src/notebooks/trash.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.542848 openparse-0.5.1/src/openparse/
--rw-r--r--   0 sergey     (501) staff       (20)      404 2024-04-08 02:54:44.000000 openparse-0.5.1/src/openparse/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1814 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/cli.py
--rw-r--r--   0 sergey     (501) staff       (20)      225 2024-04-05 01:50:40.000000 openparse-0.5.1/src/openparse/consts.py
--rw-r--r--   0 sergey     (501) staff       (20)     4416 2024-04-08 01:37:39.000000 openparse-0.5.1/src/openparse/doc_parser.py
--rw-r--r--   0 sergey     (501) staff       (20)     7089 2024-04-07 21:00:47.000000 openparse-0.5.1/src/openparse/pdf.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.544941 openparse-0.5.1/src/openparse/processing/
--rw-r--r--   0 sergey     (501) staff       (20)      931 2024-04-08 02:55:39.000000 openparse-0.5.1/src/openparse/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     9199 2024-04-08 02:55:46.000000 openparse-0.5.1/src/openparse/processing/basic_transforms.py
--rw-r--r--   0 sergey     (501) staff       (20)     4301 2024-04-08 20:05:45.000000 openparse-0.5.1/src/openparse/processing/ingest.py
--rw-r--r--   0 sergey     (501) staff       (20)     3796 2024-04-08 20:10:30.000000 openparse-0.5.1/src/openparse/processing/semantic_transforms.py
--rw-r--r--   0 sergey     (501) staff       (20)    17879 2024-04-08 03:22:10.000000 openparse-0.5.1/src/openparse/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.546605 openparse-0.5.1/src/openparse/tables/
--rw-r--r--   0 sergey     (501) staff       (20)      154 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     7686 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.547181 openparse-0.5.1/src/openparse/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)      174 2024-03-27 17:19:41.000000 openparse-0.5.1/src/openparse/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1199 2024-03-27 05:08:58.000000 openparse-0.5.1/src/openparse/tables/pymupdf/parse.py
--rw-r--r--   0 sergey     (501) staff       (20)      195 2024-04-05 15:33:41.000000 openparse-0.5.1/src/openparse/tables/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.548315 openparse-0.5.1/src/openparse/tables/table_transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-27 16:25:28.000000 openparse-0.5.1/src/openparse/tables/table_transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1343 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/table_transformers/geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10575 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/table_transformers/ml.py
--rw-r--r--   0 sergey     (501) staff       (20)     8546 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/table_transformers/schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.550312 openparse-0.5.1/src/openparse/tables/unitable/
--rw-r--r--   0 sergey     (501) staff       (20)       69 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1938 2024-04-05 19:13:16.000000 openparse-0.5.1/src/openparse/tables/unitable/config.py
--rw-r--r--   0 sergey     (501) staff       (20)     6288 2024-04-05 19:15:08.000000 openparse-0.5.1/src/openparse/tables/unitable/core.py
--rw-r--r--   0 sergey     (501) staff       (20)     2976 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/schemas.py
--rw-r--r--   0 sergey     (501) staff       (20)     6164 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/tabular_transformer.py
--rw-r--r--   0 sergey     (501) staff       (20)     1629 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/tokens.py
--rw-r--r--   0 sergey     (501) staff       (20)     2215 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/unitable_model.py
--rw-r--r--   0 sergey     (501) staff       (20)     4212 2024-04-05 04:51:26.000000 openparse-0.5.1/src/openparse/tables/unitable/utils.py
--rw-r--r--   0 sergey     (501) staff       (20)     6189 2024-04-05 04:51:27.000000 openparse-0.5.1/src/openparse/tables/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.550725 openparse-0.5.1/src/openparse/text/
--rw-r--r--   0 sergey     (501) staff       (20)       48 2024-03-27 17:16:27.000000 openparse-0.5.1/src/openparse/text/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)      743 2024-03-27 17:19:41.000000 openparse-0.5.1/src/openparse/text/parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.551345 openparse-0.5.1/src/openparse/text/pdfminer/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:16:32.000000 openparse-0.5.1/src/openparse/text/pdfminer/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     4491 2024-04-05 18:56:46.000000 openparse-0.5.1/src/openparse/text/pdfminer/core.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.552001 openparse-0.5.1/src/openparse/text/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)       47 2024-03-27 17:19:41.000000 openparse-0.5.1/src/openparse/text/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2967 2024-04-05 22:10:00.000000 openparse-0.5.1/src/openparse/text/pymupdf/core.py
--rw-r--r--   0 sergey     (501) staff       (20)      839 2024-04-05 04:51:27.000000 openparse-0.5.1/src/openparse/types.py
--rw-r--r--   0 sergey     (501) staff       (20)      221 2024-03-27 17:19:41.000000 openparse-0.5.1/src/openparse/utils.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.558071 openparse-0.5.1/src/openparse.egg-info/
--rw-r--r--   0 sergey     (501) staff       (20)     7961 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/PKG-INFO
--rw-r--r--   0 sergey     (501) staff       (20)     2268 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/SOURCES.txt
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/dependency_links.txt
--rw-r--r--   0 sergey     (501) staff       (20)       79 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/entry_points.txt
--rw-r--r--   0 sergey     (501) staff       (20)      160 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/requires.txt
--rw-r--r--   0 sergey     (501) staff       (20)       42 2024-04-08 21:08:37.000000 openparse-0.5.1/src/openparse.egg-info/top_level.txt
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.553374 openparse-0.5.1/src/tests/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-23 00:56:45.000000 openparse-0.5.1/src/tests/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.554659 openparse-0.5.1/src/tests/processing/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 01:35:13.000000 openparse-0.5.1/src/tests/processing/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     1085 2024-03-31 15:54:18.000000 openparse-0.5.1/src/tests/processing/test_pipeline.py
--rw-r--r--   0 sergey     (501) staff       (20)    16645 2024-04-08 02:57:13.000000 openparse-0.5.1/src/tests/processing/test_steps.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.555140 openparse-0.5.1/src/tests/tables/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-25 03:12:34.000000 openparse-0.5.1/src/tests/tables/__init__.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.555399 openparse-0.5.1/src/tests/tables/pymupdf/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 04:18:24.000000 openparse-0.5.1/src/tests/tables/pymupdf/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2765 2024-03-27 17:19:41.000000 openparse-0.5.1/src/tests/tables/pymupdf/test_parse.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.556158 openparse-0.5.1/src/tests/tables/transformers/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-03-27 03:41:31.000000 openparse-0.5.1/src/tests/tables/transformers/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)     2174 2024-03-29 00:46:39.000000 openparse-0.5.1/src/tests/tables/transformers/test_geometry.py
--rw-r--r--   0 sergey     (501) staff       (20)    10190 2024-03-27 17:17:26.000000 openparse-0.5.1/src/tests/tables/transformers/test_ml.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.557570 openparse-0.5.1/src/tests/tables/unitable/
--rw-r--r--   0 sergey     (501) staff       (20)        0 2024-04-05 04:51:27.000000 openparse-0.5.1/src/tests/tables/unitable/__init__.py
--rw-r--r--   0 sergey     (501) staff       (20)   190851 2024-04-05 04:51:27.000000 openparse-0.5.1/src/tests/tables/unitable/sample_pred_outputs.py
--rw-r--r--   0 sergey     (501) staff       (20)     1113 2024-04-05 04:51:27.000000 openparse-0.5.1/src/tests/tables/unitable/test_pred_to_schema.py
--rw-r--r--   0 sergey     (501) staff       (20)     1566 2024-04-08 03:15:57.000000 openparse-0.5.1/src/tests/test_doc_parser.py
--rw-r--r--   0 sergey     (501) staff       (20)        1 2024-03-28 23:19:06.000000 openparse-0.5.1/src/tests/test_main.py
--rw-r--r--   0 sergey     (501) staff       (20)    20672 2024-03-31 21:03:58.000000 openparse-0.5.1/src/tests/test_schemas.py
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.538400 openparse-0.5.1/src/tests/text/
-drwxr-xr-x   0 sergey     (501) staff       (20)        0 2024-04-08 21:08:37.557735 openparse-0.5.1/src/tests/text/pdf_miner/
--rw-r--r--   0 sergey     (501) staff       (20)     4002 2024-03-27 17:19:41.000000 openparse-0.5.1/src/tests/text/pdf_miner/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-11 14:23:14.000000 openparse-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-11 14:23:20.915871 openparse-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-11 14:23:14.000000 openparse-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-11 14:23:14.000000 openparse-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:23:20.915871 openparse-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.903871 openparse-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.907871 openparse-0.5.2/src/evals/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:23:14.000000 openparse-0.5.2/src/evals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-11 14:23:14.000000 openparse-0.5.2/src/evals/run_evals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.907871 openparse-0.5.2/src/openparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/doc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.907871 openparse-0.5.2/src/openparse/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/processing/basic_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/processing/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/processing/semantic_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/tables/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/pymupdf/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/tables/table_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/table_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/table_transformers/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/table_transformers/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/table_transformers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/tables/unitable/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/tabular_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/unitable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/unitable/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/tables/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/text/pdfminer/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/pdfminer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/pdfminer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/openparse/text/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/text/pymupdf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-11 14:23:14.000000 openparse-0.5.2/src/openparse/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/openparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 14:23:20.000000 openparse-0.5.2/src/openparse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.911872 openparse-0.5.2/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/processing/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/processing/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/tables/pymupdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/pymupdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/pymupdf/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/tables/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/transformers/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/transformers/test_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/tables/unitable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/unitable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190851 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/unitable/sample_pred_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/tables/unitable/test_pred_to_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/test_doc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.903871 openparse-0.5.2/src/tests/text/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:23:20.915871 openparse-0.5.2/src/tests/text/pdf_miner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-11 14:23:14.000000 openparse-0.5.2/src/tests/text/pdf_miner/test_core.py
```

### Comparing `openparse-0.5.1/LICENSE` & `openparse-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/PKG-INFO` & `openparse-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,498 +1,534 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6f70 656e  : 2.1.Name: open
 00000020: 7061 7273 650a 5665 7273 696f 6e3a 2030  parse.Version: 0
-00000030: 2e35 2e31 0a53 756d 6d61 7279 3a20 5374  .5.1.Summary: St
+00000030: 2e35 2e32 0a53 756d 6d61 7279 3a20 5374  .5.2.Summary: St
 00000040: 7265 616d 6c69 6e65 7320 7468 6520 7072  reamlines the pr
 00000050: 6f63 6573 7320 6f66 2070 7265 7061 7269  ocess of prepari
 00000060: 6e67 2064 6f63 756d 656e 7473 2066 6f72  ng documents for
-00000070: 204c 4c4d 2773 2e0a 486f 6d65 2d70 6167   LLM's..Home-pag
-00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-00000090: 622e 636f 6d2f 4669 6c69 6d6f 612f 6f70  b.com/Filimoa/op
-000000a0: 656e 2d70 6172 7365 2f0a 4175 7468 6f72  en-parse/.Author
-000000b0: 3a20 5365 7267 6579 2046 696c 696d 6f6e  : Sergey Filimon
-000000c0: 6f76 0a41 7574 686f 722d 656d 6169 6c3a  ov.Author-email:
-000000d0: 2068 656c 6c6f 4073 6572 6765 792e 6679   hello@sergey.fy
-000000e0: 690a 4465 7363 7269 7074 696f 6e2d 436f  i.Description-Co
-000000f0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000100: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
-00000110: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
-00000120: 5265 7175 6972 6573 2d44 6973 743a 2050  Requires-Dist: P
-00000130: 794d 7550 4446 3e3d 312e 3233 2e32 0a52  yMuPDF>=1.23.2.R
-00000140: 6571 7569 7265 732d 4469 7374 3a20 7069  equires-Dist: pi
-00000150: 6c6c 6f77 3e3d 382e 330a 5265 7175 6972  llow>=8.3.Requir
-00000160: 6573 2d44 6973 743a 2070 7964 616e 7469  es-Dist: pydanti
-00000170: 633e 3d32 2e30 0a52 6571 7569 7265 732d  c>=2.0.Requires-
-00000180: 4469 7374 3a20 7079 7064 663e 3d34 2e30  Dist: pypdf>=4.0
-00000190: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
-000001a0: 3a20 7064 666d 696e 6572 2e73 6978 3e3d  : pdfminer.six>=
-000001b0: 3230 3230 3034 3031 0a52 6571 7569 7265  20200401.Require
-000001c0: 732d 4469 7374 3a20 7469 6b74 6f6b 656e  s-Dist: tiktoken
-000001d0: 3e3d 302e 330a 5265 7175 6972 6573 2d44  >=0.3.Requires-D
-000001e0: 6973 743a 206f 7065 6e61 693e 3d31 2e30  ist: openai>=1.0
-000001f0: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
-00000200: 3a20 6e75 6d70 790a 5072 6f76 6964 6573  : numpy.Provides
-00000210: 2d45 7874 7261 3a20 6d6c 0a52 6571 7569  -Extra: ml.Requi
-00000220: 7265 732d 4469 7374 3a20 746f 7263 683b  res-Dist: torch;
-00000230: 2065 7874 7261 203d 3d20 226d 6c22 0a52   extra == "ml".R
-00000240: 6571 7569 7265 732d 4469 7374 3a20 746f  equires-Dist: to
-00000250: 7263 6876 6973 696f 6e3b 2065 7874 7261  rchvision; extra
-00000260: 203d 3d20 226d 6c22 0a52 6571 7569 7265   == "ml".Require
-00000270: 732d 4469 7374 3a20 7472 616e 7366 6f72  s-Dist: transfor
-00000280: 6d65 7273 3b20 6578 7472 6120 3d3d 2022  mers; extra == "
-00000290: 6d6c 220a 5265 7175 6972 6573 2d44 6973  ml".Requires-Dis
-000002a0: 743a 2074 6f6b 656e 697a 6572 733b 2065  t: tokenizers; e
-000002b0: 7874 7261 203d 3d20 226d 6c22 0a0a 3c70  xtra == "ml"..<p
-000002c0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000002d0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-000002e0: 7474 7073 3a2f 2f73 6572 6765 792d 6669  ttps://sergey-fi
-000002f0: 6c69 6d6f 6e6f 762e 6e79 6333 2e64 6967  limonov.nyc3.dig
-00000300: 6974 616c 6f63 6561 6e73 7061 6365 732e  italoceanspaces.
-00000310: 636f 6d2f 6f70 656e 2d70 6172 7365 2f6f  com/open-parse/o
-00000320: 7065 6e2d 7061 7273 652d 7769 7468 2d74  pen-parse-with-t
-00000330: 6578 742d 7470 2d6c 6f67 6f2e 7765 6270  ext-tp-logo.webp
-00000340: 2220 7769 6474 683d 2233 3530 2220 2f3e  " width="350" />
-00000350: 0a3c 2f70 3e0a 3c62 722f 3e0a 0a2a 2a45  .</p>.<br/>..**E
-00000360: 6173 696c 7920 6368 756e 6b20 636f 6d70  asily chunk comp
-00000370: 6c65 7820 646f 6375 6d65 6e74 7320 7468  lex documents th
-00000380: 6520 7361 6d65 2077 6179 2061 2068 756d  e same way a hum
-00000390: 616e 2077 6f75 6c64 2e2a 2a20 200a 0a43  an would.**  ..C
-000003a0: 6875 6e6b 696e 6720 646f 6375 6d65 6e74  hunking document
-000003b0: 7320 6973 2061 2063 6861 6c6c 656e 6769  s is a challengi
-000003c0: 6e67 2074 6173 6b20 7468 6174 2075 6e64  ng task that und
-000003d0: 6572 7069 6e73 2061 6e79 2052 4147 2073  erpins any RAG s
-000003e0: 7973 7465 6d2e 2020 4869 6768 2071 7561  ystem.  High qua
-000003f0: 6c69 7479 2072 6573 756c 7473 2061 7265  lity results are
-00000400: 2063 7269 7469 6361 6c20 746f 2061 2073   critical to a s
-00000410: 7563 6573 7366 756c 2041 4920 6170 706c  ucessful AI appl
-00000420: 6963 6174 696f 6e2c 2079 6574 206d 6f73  ication, yet mos
-00000430: 7420 6f70 656e 2d73 6f75 7263 6520 6c69  t open-source li
-00000440: 6272 6172 6965 7320 6172 6520 6c69 6d69  braries are limi
-00000450: 7465 6420 696e 2074 6865 6972 2061 6269  ted in their abi
-00000460: 6c69 7479 2074 6f20 6861 6e64 6c65 2063  lity to handle c
-00000470: 6f6d 706c 6578 2064 6f63 756d 656e 7473  omplex documents
-00000480: 2e20 200a 0a4f 7065 6e20 5061 7273 6520  .  ..Open Parse 
-00000490: 6973 2064 6573 6967 6e65 6420 746f 2066  is designed to f
-000004a0: 696c 6c20 7468 6973 2067 6170 2062 7920  ill this gap by 
-000004b0: 7072 6f76 6964 696e 6720 6120 666c 6578  providing a flex
-000004c0: 6962 6c65 2c20 6561 7379 2d74 6f2d 7573  ible, easy-to-us
-000004d0: 6520 6c69 6272 6172 7920 6361 7061 626c  e library capabl
-000004e0: 6520 6f66 2076 6973 7561 6c6c 7920 6469  e of visually di
-000004f0: 7363 6572 6e69 6e67 2064 6f63 756d 656e  scerning documen
-00000500: 7420 6c61 796f 7574 7320 616e 6420 6368  t layouts and ch
-00000510: 756e 6b69 6e67 2074 6865 6d20 6566 6665  unking them effe
-00000520: 6374 6976 656c 792e 0a0a 3c64 6574 6169  ctively...<detai
-00000530: 6c73 3e0a 2020 3c73 756d 6d61 7279 3e3c  ls>.  <summary><
-00000540: 623e 486f 7720 6973 2074 6869 7320 6469  b>How is this di
-00000550: 6666 6572 656e 7420 6672 6f6d 206f 7468  fferent from oth
-00000560: 6572 206c 6179 6f75 7420 7061 7273 6572  er layout parser
-00000570: 733f 3c2f 623e 3c2f 7375 6d6d 6172 793e  s?</b></summary>
-00000580: 0a0a 2020 2323 2323 20e2 9c82 efb8 8f20  ..  #### ...... 
-00000590: 5465 7874 2053 706c 6974 7469 6e67 0a20  Text Splitting. 
-000005a0: 2054 6578 7420 7370 6c69 7474 696e 6720   Text splitting 
-000005b0: 636f 6e76 6572 7473 2061 2066 696c 6520  converts a file 
-000005c0: 746f 2072 6177 2074 6578 7420 616e 6420  to raw text and 
-000005d0: 5b73 6c69 6365 7320 6974 2075 705d 2868  [slices it up](h
-000005e0: 7474 7073 3a2f 2f64 6f63 732e 6c6c 616d  ttps://docs.llam
-000005f0: 6169 6e64 6578 2e61 692f 656e 2f73 7461  aindex.ai/en/sta
-00000600: 626c 652f 6170 695f 7265 6665 7265 6e63  ble/api_referenc
-00000610: 652f 6e6f 6465 5f70 6172 7365 7273 2f74  e/node_parsers/t
-00000620: 6f6b 656e 5f74 6578 745f 7370 6c69 7474  oken_text_splitt
-00000630: 6572 2f29 2e0a 2020 0a20 202d 2059 6f75  er/)..  .  - You
-00000640: 206c 6f73 6520 7468 6520 6162 696c 6974   lose the abilit
-00000650: 7920 746f 2065 6173 696c 7920 6f76 6572  y to easily over
-00000660: 6c61 7920 7468 6520 6368 756e 6b20 6f6e  lay the chunk on
-00000670: 2074 6865 206f 7269 6769 6e61 6c20 7064   the original pd
-00000680: 660a 2020 2d20 596f 7520 6967 6e6f 7265  f.  - You ignore
-00000690: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-000006a0: 7365 6d61 6e74 6963 2073 7472 7563 7475  semantic structu
-000006b0: 7265 206f 6620 7468 6520 6669 6c65 202d  re of the file -
-000006c0: 2068 6561 6469 6e67 732c 2073 6563 7469   headings, secti
-000006d0: 6f6e 732c 2062 756c 6c65 7473 2072 6570  ons, bullets rep
-000006e0: 7265 7365 6e74 2076 616c 7561 626c 6520  resent valuable 
-000006f0: 696e 666f 726d 6174 696f 6e2e 0a20 202d  information..  -
-00000700: 204e 6f20 7375 7070 6f72 7420 666f 7220   No support for 
-00000710: 7461 626c 6573 2c20 696d 6167 6573 206f  tables, images o
-00000720: 7220 6d61 726b 646f 776e 2e0a 2020 0a20  r markdown..  . 
-00000730: 2023 2323 2320 f09f a496 204d 4c20 4c61   #### .... ML La
-00000740: 796f 7574 2050 6172 7365 7273 0a20 2054  yout Parsers.  T
-00000750: 6865 7265 2773 2073 6f6d 6520 6f66 2066  here's some of f
-00000760: 616e 7461 7374 6963 206c 6962 7261 7269  antastic librari
-00000770: 6573 206c 696b 6520 5b6c 6179 6f75 742d  es like [layout-
-00000780: 7061 7273 6572 5d28 6874 7470 733a 2f2f  parser](https://
-00000790: 6769 7468 7562 2e63 6f6d 2f4c 6179 6f75  github.com/Layou
-000007a0: 742d 5061 7273 6572 2f6c 6179 6f75 742d  t-Parser/layout-
-000007b0: 7061 7273 6572 292e 200a 2020 2d20 5768  parser). .  - Wh
-000007c0: 696c 6520 7468 6579 2063 616e 2069 6465  ile they can ide
-000007d0: 6e74 6966 7920 7661 7269 6f75 7320 656c  ntify various el
-000007e0: 656d 656e 7473 206c 696b 6520 7465 7874  ements like text
-000007f0: 2062 6c6f 636b 732c 2069 6d61 6765 732c   blocks, images,
-00000800: 2061 6e64 2074 6162 6c65 732c 2062 7574   and tables, but
-00000810: 2074 6865 7920 6172 6520 6e6f 7420 6275   they are not bu
-00000820: 696c 7420 746f 2067 726f 7570 2072 656c  ilt to group rel
-00000830: 6174 6564 2063 6f6e 7465 6e74 2065 6666  ated content eff
-00000840: 6563 7469 7665 6c79 2e0a 2020 2d20 5468  ectively..  - Th
-00000850: 6579 2073 7472 6963 746c 7920 666f 6375  ey strictly focu
-00000860: 7320 6f6e 206c 6179 6f75 7420 7061 7273  s on layout pars
-00000870: 696e 6720 2d20 796f 7520 7769 6c6c 206e  ing - you will n
-00000880: 6565 6420 746f 2061 6464 2061 6e6f 7468  eed to add anoth
-00000890: 6572 206d 6f64 656c 2074 6f20 6578 7472  er model to extr
-000008a0: 6163 7420 6d61 726b 646f 776e 2066 726f  act markdown fro
-000008b0: 6d20 7468 6520 696d 6167 6573 2c20 7061  m the images, pa
-000008c0: 7273 6520 7461 626c 6573 2c20 6772 6f75  rse tables, grou
-000008d0: 7020 6e6f 6465 732c 2065 7463 2e0a 2020  p nodes, etc..  
-000008e0: 2d20 5765 2776 6520 666f 756e 6420 7065  - We've found pe
-000008f0: 7266 6f72 6d61 6e63 6520 746f 2062 6520  rformance to be 
-00000900: 7375 622d 6f70 7469 6d61 6c20 6f6e 206d  sub-optimal on m
-00000910: 616e 7920 646f 6375 6d65 6e74 7320 7768  any documents wh
-00000920: 696c 6520 616c 736f 2062 6569 6e67 2063  ile also being c
-00000930: 6f6d 7075 7461 7469 6f6e 616c 6c79 2068  omputationally h
-00000940: 6561 7679 2e0a 0a20 2023 2323 2320 f09f  eavy...  #### ..
-00000950: 92bc 2043 6f6d 6d65 7263 6961 6c20 536f  .. Commercial So
-00000960: 6c75 7469 6f6e 730a 0a20 202d 2054 7970  lutions..  - Typ
-00000970: 6963 616c 6c79 2070 7269 6365 6420 6174  ically priced at
-00000980: 20e2 8988 2024 3130 202f 2031 6b20 7061   ... $10 / 1k pa
-00000990: 6765 732e 2053 6565 205b 6865 7265 5d28  ges. See [here](
-000009a0: 6874 7470 733a 2f2f 636c 6f75 642e 676f  https://cloud.go
-000009b0: 6f67 6c65 2e63 6f6d 2f64 6f63 756d 656e  ogle.com/documen
-000009c0: 742d 6169 292c 205b 6865 7265 5d28 6874  t-ai), [here](ht
-000009d0: 7470 733a 2f2f 6177 732e 616d 617a 6f6e  tps://aws.amazon
-000009e0: 2e63 6f6d 2f74 6578 7472 6163 742f 2920  .com/textract/) 
-000009f0: 616e 6420 5b68 6572 655d 2868 7474 7073  and [here](https
-00000a00: 3a2f 2f77 7777 2e72 6564 7563 746f 2e61  ://www.reducto.a
-00000a10: 692f 292e 0a20 202d 2052 6571 7569 7265  i/)..  - Require
-00000a20: 7320 7368 6172 696e 6720 796f 7572 2064  s sharing your d
-00000a30: 6174 6120 7769 7468 2061 2076 656e 646f  ata with a vendo
-00000a40: 720a 0a3c 2f64 6574 6169 6c73 3e0a 0a23  r..</details>..#
-00000a50: 2320 4869 6768 6c69 6768 7473 0a0a 2d20  # Highlights..- 
-00000a60: 2a2a f09f 948d 2056 6973 7561 6c6c 792d  **.... Visually-
-00000a70: 4472 6976 656e 3a2a 2a20 4f70 656e 2d50  Driven:** Open-P
-00000a80: 6172 7365 2076 6973 7561 6c6c 7920 616e  arse visually an
-00000a90: 616c 797a 6573 2064 6f63 756d 656e 7473  alyzes documents
-00000aa0: 2066 6f72 2073 7570 6572 696f 7220 4c4c   for superior LL
-00000ab0: 4d20 696e 7075 742c 2067 6f69 6e67 2062  M input, going b
-00000ac0: 6579 6f6e 6420 6e61 6976 6520 7465 7874  eyond naive text
-00000ad0: 2073 706c 6974 7469 6e67 2e0a 2d20 2a2a   splitting..- **
-00000ae0: e29c 8def b88f 204d 6172 6b64 6f77 6e20  ...... Markdown 
-00000af0: 5375 7070 6f72 743a 2a2a 2042 6173 6963  Support:** Basic
-00000b00: 206d 6172 6b64 6f77 6e20 7375 7070 6f72   markdown suppor
-00000b10: 7420 666f 7220 7061 7273 696e 6720 6865  t for parsing he
-00000b20: 6164 696e 6773 2c20 626f 6c64 2061 6e64  adings, bold and
-00000b30: 2069 7461 6c69 6373 2e0a 2d20 2a2a f09f   italics..- **..
-00000b40: 938a 2048 6967 682d 5072 6563 6973 696f  .. High-Precisio
-00000b50: 6e20 5461 626c 6520 5375 7070 6f72 743a  n Table Support:
-00000b60: 2a2a 2045 7874 7261 6374 2074 6162 6c65  ** Extract table
-00000b70: 7320 696e 746f 2063 6c65 616e 204d 6172  s into clean Mar
-00000b80: 6b64 6f77 6e20 666f 726d 6174 7320 7769  kdown formats wi
-00000b90: 7468 2061 6363 7572 6163 7920 7468 6174  th accuracy that
-00000ba0: 2073 7572 7061 7373 6573 2074 7261 6469   surpasses tradi
-00000bb0: 7469 6f6e 616c 2074 6f6f 6c73 2e0a 2020  tional tools..  
-00000bc0: 2020 3c64 6574 6169 6c73 3e0a 2020 3c73    <details>.  <s
-00000bd0: 756d 6d61 7279 3e3c 693e 4578 616d 706c  ummary><i>Exampl
-00000be0: 6573 3c2f 693e 3c2f 7375 6d6d 6172 793e  es</i></summary>
-00000bf0: 0a20 2054 6865 2066 6f6c 6c6f 7769 6e67  .  The following
-00000c00: 2065 7861 6d70 6c65 7320 7765 7265 2070   examples were p
-00000c10: 6172 7365 6420 7769 7468 2075 6e69 7461  arsed with unita
-00000c20: 626c 652e 0a20 2020 203c 6272 2f3e 0a20  ble..    <br/>. 
-00000c30: 2020 203c 7020 616c 6967 6e3d 2263 656e     <p align="cen
-00000c40: 7465 7222 3e0a 2020 2020 2020 2020 3c62  ter">.        <b
-00000c50: 722f 3e0a 2020 2020 2020 2020 3c69 6d67  r/>.        <img
-00000c60: 2073 7263 3d22 6874 7470 733a 2f2f 7365   src="https://se
-00000c70: 7267 6579 2d66 696c 696d 6f6e 6f76 2e6e  rgey-filimonov.n
-00000c80: 7963 332e 6469 6769 7461 6c6f 6365 616e  yc3.digitalocean
-00000c90: 7370 6163 6573 2e63 6f6d 2f6f 7065 6e2d  spaces.com/open-
-00000ca0: 7061 7273 652f 756e 6974 6162 6c65 2d70  parse/unitable-p
-00000cb0: 6172 7369 6e67 2d73 616d 706c 652e 7765  arsing-sample.we
-00000cc0: 6270 2220 7769 6474 683d 2236 3530 222f  bp" width="650"/
-00000cd0: 3e0a 2020 2020 3c2f 703e 0a20 2020 2020  >.    </p>.     
-00000ce0: 2020 2020 3c62 722f 3e0a 2020 2020 3c2f      <br/>.    </
-00000cf0: 6465 7461 696c 733e 0a0a 2d20 2a2a f09f  details>..- **..
-00000d00: 9ba0 efb8 8f20 4578 7465 6e73 6962 6c65  ..... Extensible
-00000d10: 3a2a 2a20 4561 7369 6c79 2069 6d70 6c65  :** Easily imple
-00000d20: 6d65 6e74 2079 6f75 7220 6f77 6e20 706f  ment your own po
-00000d30: 7374 2d70 726f 6365 7373 696e 6720 7374  st-processing st
-00000d40: 6570 732e 0a2d 202a 2af0 9f92 a149 6e74  eps..- **....Int
-00000d50: 7569 7469 7665 3a2a 2a20 4772 6561 7420  uitive:** Great 
-00000d60: 6564 6974 6f72 2073 7570 706f 7274 2e20  editor support. 
-00000d70: 436f 6d70 6c65 7469 6f6e 2065 7665 7279  Completion every
-00000d80: 7768 6572 652e 204c 6573 7320 7469 6d65  where. Less time
-00000d90: 2064 6562 7567 6769 6e67 2e0a 2d20 2a2a   debugging..- **
-00000da0: f09f 8eaf 2045 6173 793a 2a2a 2044 6573  .... Easy:** Des
-00000db0: 6967 6e65 6420 746f 2062 6520 6561 7379  igned to be easy
-00000dc0: 2074 6f20 7573 6520 616e 6420 6c65 6172   to use and lear
-00000dd0: 6e2e 204c 6573 7320 7469 6d65 2072 6561  n. Less time rea
-00000de0: 6469 6e67 2064 6f63 732e 0a0a 3c62 722f  ding docs...<br/
-00000df0: 3e0a 3c70 2061 6c69 676e 3d22 6365 6e74  >.<p align="cent
-00000e00: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
-00000e10: 633d 2268 7474 7073 3a2f 2f73 6572 6765  c="https://serge
-00000e20: 792d 6669 6c69 6d6f 6e6f 762e 6e79 6333  y-filimonov.nyc3
-00000e30: 2e64 6967 6974 616c 6f63 6561 6e73 7061  .digitaloceanspa
-00000e40: 6365 732e 636f 6d2f 6f70 656e 2d70 6172  ces.com/open-par
-00000e50: 7365 2f6d 6172 6b65 642d 7570 2d64 6f63  se/marked-up-doc
-00000e60: 2d32 2e77 6562 7022 2077 6964 7468 3d22  -2.webp" width="
-00000e70: 3235 3022 202f 3e0a 3c2f 703e 0a0a 2323  250" />.</p>..##
-00000e80: 2045 7861 6d70 6c65 0a0a 2323 2323 2042   Example..#### B
-00000e90: 6173 6963 2045 7861 6d70 6c65 0a0a 6060  asic Example..``
-00000ea0: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
-00000eb0: 7065 6e70 6172 7365 0a0a 6261 7369 635f  penparse..basic_
-00000ec0: 646f 635f 7061 7468 203d 2022 2e2f 7361  doc_path = "./sa
-00000ed0: 6d70 6c65 2d64 6f63 732f 6d6f 6269 6c65  mple-docs/mobile
-00000ee0: 2d68 6f6d 652d 6d61 6e75 616c 2e70 6466  -home-manual.pdf
-00000ef0: 220a 7061 7273 6572 203d 206f 7065 6e70  ".parser = openp
-00000f00: 6172 7365 2e44 6f63 756d 656e 7450 6172  arse.DocumentPar
-00000f10: 7365 7228 290a 7061 7273 6564 5f62 6173  ser().parsed_bas
-00000f20: 6963 5f64 6f63 203d 2070 6172 7365 722e  ic_doc = parser.
-00000f30: 7061 7273 6528 6261 7369 635f 646f 635f  parse(basic_doc_
-00000f40: 7061 7468 290a 0a66 6f72 206e 6f64 6520  path)..for node 
-00000f50: 696e 2070 6172 7365 645f 6261 7369 635f  in parsed_basic_
-00000f60: 646f 632e 6e6f 6465 733a 0a20 2020 2070  doc.nodes:.    p
-00000f70: 7269 6e74 286e 6f64 6529 0a60 6060 0a0a  rint(node).```..
-00000f80: 2a2a f09f 9393 2054 7279 2074 6865 2073  **.... Try the s
-00000f90: 616d 706c 6520 6e6f 7465 626f 6f6b 2a2a  ample notebook**
-00000fa0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000fb0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00000fc0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
-00000fd0: 652f 315a 3542 3567 736e 6d68 464b 4546  e/1Z5B5gsnmhFKEF
-00000fe0: 4c2d 3579 5949 636f 6f78 372d 6a51 616f  L-5yYIcoox7-jQao
-00000ff0: 3845 703f 7573 703d 7368 6172 696e 6722  8Ep?usp=sharing"
-00001000: 2063 6c61 7373 3d22 6578 7465 726e 616c   class="external
-00001010: 2d6c 696e 6b22 2074 6172 6765 743d 225f  -link" target="_
-00001020: 626c 616e 6b22 3e68 6572 653c 2f61 3e0a  blank">here</a>.
-00001030: 0a23 2323 2320 5365 6d61 6e74 6963 2050  .#### Semantic P
-00001040: 726f 6365 7373 696e 6720 4578 616d 706c  rocessing Exampl
-00001050: 650a 0a43 6875 6e6b 696e 6720 646f 6375  e..Chunking docu
-00001060: 6d65 6e74 7320 6973 2066 756e 6461 6d65  ments is fundame
-00001070: 6e74 616c 6c79 2061 626f 7574 2067 726f  ntally about gro
-00001080: 7570 696e 6720 7369 6d69 6c61 7220 7365  uping similar se
-00001090: 6d61 6e74 6963 206e 6f64 6573 2074 6f67  mantic nodes tog
-000010a0: 6574 6865 722e 2042 7920 656d 6265 6464  ether. By embedd
-000010b0: 696e 6720 7468 6520 7465 7874 206f 6620  ing the text of 
-000010c0: 6561 6368 206e 6f64 652c 2077 6520 6361  each node, we ca
-000010d0: 6e20 7468 656e 2063 6c75 7374 6572 2074  n then cluster t
-000010e0: 6865 6d20 746f 6765 7468 6572 2062 6173  hem together bas
-000010f0: 6564 206f 6e20 7468 6569 7220 7369 6d69  ed on their simi
-00001100: 6c61 7269 7479 2e0a 0a60 6060 7079 7468  larity...```pyth
-00001110: 6f6e 0a66 726f 6d20 6f70 656e 7061 7273  on.from openpars
-00001120: 6520 696d 706f 7274 2070 726f 6365 7373  e import process
-00001130: 696e 672c 2044 6f63 756d 656e 7450 6172  ing, DocumentPar
-00001140: 7365 720a 0a73 656d 616e 7469 635f 7069  ser..semantic_pi
-00001150: 7065 6c69 6e65 203d 2070 726f 6365 7373  peline = process
-00001160: 696e 672e 5365 6d61 6e74 6963 496e 6765  ing.SemanticInge
-00001170: 7374 696f 6e50 6970 656c 696e 6528 0a20  stionPipeline(. 
-00001180: 2020 206f 7065 6e61 695f 6170 695f 6b65     openai_api_ke
-00001190: 793d 4f50 454e 5f41 495f 4b45 592c 0a20  y=OPEN_AI_KEY,. 
-000011a0: 2020 206d 6f64 656c 3d22 7465 7874 2d65     model="text-e
-000011b0: 6d62 6564 6469 6e67 2d33 2d6c 6172 6765  mbedding-3-large
-000011c0: 222c 0a20 2020 206d 696e 5f74 6f6b 656e  ",.    min_token
-000011d0: 733d 3634 2c0a 2020 2020 6d61 785f 746f  s=64,.    max_to
-000011e0: 6b65 6e73 3d31 3032 342c 0a29 0a70 6172  kens=1024,.).par
-000011f0: 7365 7220 3d20 446f 6375 6d65 6e74 5061  ser = DocumentPa
-00001200: 7273 6572 280a 2020 2020 7072 6f63 6573  rser(.    proces
-00001210: 7369 6e67 5f70 6970 656c 696e 653d 7365  sing_pipeline=se
-00001220: 6d61 6e74 6963 5f70 6970 656c 696e 652c  mantic_pipeline,
-00001230: 0a29 0a70 6172 7365 645f 636f 6e74 656e  .).parsed_conten
-00001240: 7420 3d20 7061 7273 6572 2e70 6172 7365  t = parser.parse
-00001250: 2862 6173 6963 5f64 6f63 5f70 6174 6829  (basic_doc_path)
-00001260: 0a60 6060 0a0a 2a2a f09f 9393 2053 616d  .```..**.... Sam
-00001270: 706c 6520 6e6f 7465 626f 6f6b 2a2a 203c  ple notebook** <
-00001280: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001290: 6769 7468 7562 2e63 6f6d 2f46 696c 696d  github.com/Filim
-000012a0: 6f61 2f6f 7065 6e2d 7061 7273 652f 626c  oa/open-parse/bl
-000012b0: 6f62 2f6d 6169 6e2f 7372 632f 636f 6f6b  ob/main/src/cook
-000012c0: 626f 6f6b 732f 7365 6d61 6e74 6963 5f70  books/semantic_p
-000012d0: 726f 6365 7373 696e 672e 6970 796e 6222  rocessing.ipynb"
-000012e0: 2063 6c61 7373 3d22 6578 7465 726e 616c   class="external
-000012f0: 2d6c 696e 6b22 2074 6172 6765 743d 225f  -link" target="_
-00001300: 626c 616e 6b22 3e68 6572 653c 2f61 3e0a  blank">here</a>.
-00001310: 0a23 2323 2320 5365 7269 616c 697a 696e  .#### Serializin
-00001320: 6720 5265 7375 6c74 730a 5573 6573 2070  g Results.Uses p
-00001330: 7964 616e 7469 6320 756e 6465 7220 7468  ydantic under th
-00001340: 6520 686f 6f64 2073 6f20 796f 7520 6361  e hood so you ca
-00001350: 6e20 7365 7269 616c 697a 6520 7265 7375  n serialize resu
-00001360: 6c74 7320 7769 7468 200a 0a60 6060 7079  lts with ..```py
-00001370: 7468 6f6e 0a70 6172 7365 645f 636f 6e74  thon.parsed_cont
-00001380: 656e 742e 6469 6374 2829 0a23 206f 720a  ent.dict().# or.
-00001390: 7061 7273 6564 5f63 6f6e 7465 6e74 2e6a  parsed_content.j
-000013a0: 736f 6e28 290a 6060 600a 0a23 2320 5265  son().```..## Re
-000013b0: 7175 6972 656d 656e 7473 0a0a 5079 7468  quirements..Pyth
-000013c0: 6f6e 2033 2e38 2b0a 0a2a 2a44 6561 6c69  on 3.8+..**Deali
-000013d0: 6e67 2077 6974 6820 5044 4627 733a 2a2a  ng with PDF's:**
-000013e0: 0a0a 2d20 3c61 2068 7265 663d 2268 7474  ..- <a href="htt
-000013f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001400: 7064 666d 696e 6572 2f70 6466 6d69 6e65  pdfminer/pdfmine
-00001410: 722e 7369 7822 2063 6c61 7373 3d22 6578  r.six" class="ex
-00001420: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
-00001430: 6765 743d 225f 626c 616e 6b22 3e70 6466  get="_blank">pdf
-00001440: 6d69 6e65 722e 7369 783c 2f61 3e20 4675  miner.six</a> Fu
-00001450: 6c6c 7920 6f70 656e 2073 6f75 7263 652e  lly open source.
-00001460: 0a0a 2a2a 4578 7472 6163 7469 6e67 2054  ..**Extracting T
-00001470: 6162 6c65 733a 2a2a 0a0a 2d20 3c61 2068  ables:**..- <a h
-00001480: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001490: 6875 622e 636f 6d2f 7079 6d75 7064 662f  hub.com/pymupdf/
-000014a0: 5079 4d75 5044 4622 2063 6c61 7373 3d22  PyMuPDF" class="
-000014b0: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
-000014c0: 6172 6765 743d 225f 626c 616e 6b22 3e50  arget="_blank">P
-000014d0: 794d 7550 4446 3c2f 613e 2068 6173 2073  yMuPDF</a> has s
-000014e0: 6f6d 6520 7461 626c 6520 6465 7465 6374  ome table detect
-000014f0: 696f 6e20 6675 6e63 7469 6f6e 616c 6974  ion functionalit
-00001500: 792e 2050 6c65 6173 6520 7365 6520 7468  y. Please see th
-00001510: 6569 7220 3c61 2068 7265 663d 2268 7474  eir <a href="htt
-00001520: 7073 3a2f 2f6d 7570 6466 2e63 6f6d 2f6c  ps://mupdf.com/l
-00001530: 6963 656e 7369 6e67 2f69 6e64 6578 2e68  icensing/index.h
-00001540: 746d 6c23 636f 6d6d 6572 6369 616c 2220  tml#commercial" 
-00001550: 636c 6173 733d 2265 7874 6572 6e61 6c2d  class="external-
-00001560: 6c69 6e6b 2220 7461 7267 6574 3d22 5f62  link" target="_b
-00001570: 6c61 6e6b 223e 6c69 6365 6e73 653c 2f61  lank">license</a
-00001580: 3e2e 0a2d 203c 6120 6872 6566 3d22 6874  >..- <a href="ht
-00001590: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-000015a0: 652e 636f 2f6d 6963 726f 736f 6674 2f74  e.co/microsoft/t
-000015b0: 6162 6c65 2d74 7261 6e73 666f 726d 6572  able-transformer
-000015c0: 2d64 6574 6563 7469 6f6e 2220 636c 6173  -detection" clas
-000015d0: 733d 2265 7874 6572 6e61 6c2d 6c69 6e6b  s="external-link
-000015e0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-000015f0: 223e 5461 626c 6520 5472 616e 7366 6f72  ">Table Transfor
-00001600: 6d65 723c 2f61 3e20 6973 2061 2064 6565  mer</a> is a dee
-00001610: 7020 6c65 6172 6e69 6e67 2061 7070 726f  p learning appro
-00001620: 6163 682e 0a2d 203c 6120 6872 6566 3d22  ach..- <a href="
-00001630: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001640: 6f6d 2f70 6f6c 6f63 6c75 622f 756e 6974  om/poloclub/unit
-00001650: 6162 6c65 2220 636c 6173 733d 2265 7874  able" class="ext
-00001660: 6572 6e61 6c2d 6c69 6e6b 2220 7461 7267  ernal-link" targ
-00001670: 6574 3d22 5f62 6c61 6e6b 223e 756e 6974  et="_blank">unit
-00001680: 6162 6c65 3c2f 613e 2069 7320 616e 6f74  able</a> is anot
-00001690: 6865 7220 7472 616e 7366 6f72 6d65 7273  her transformers
-000016a0: 2062 6173 6564 2061 7070 726f 6163 6820   based approach 
-000016b0: 7769 7468 202a 2a73 7461 7465 2d6f 662d  with **state-of-
-000016c0: 7468 652d 6172 742a 2a20 7065 7266 6f72  the-art** perfor
-000016d0: 6d61 6e63 652e 0a0a 2323 2049 6e73 7461  mance...## Insta
-000016e0: 6c6c 6174 696f 6e0a 0a23 2323 2320 312e  llation..#### 1.
-000016f0: 2043 6f72 6520 4c69 6272 6172 790a 0a60   Core Library..`
-00001700: 6060 636f 6e73 6f6c 650a 7069 7020 696e  ``console.pip in
-00001710: 7374 616c 6c20 6f70 656e 7061 7273 650a  stall openparse.
-00001720: 6060 600a 0a2a 2a45 6e61 626c 696e 6720  ```..**Enabling 
-00001730: 4f43 5220 5375 7070 6f72 742a 2a3a 0a0a  OCR Support**:..
-00001740: 5079 4d75 5044 4620 7769 6c6c 2061 6c72  PyMuPDF will alr
-00001750: 6561 6479 2063 6f6e 7461 696e 2061 6c6c  eady contain all
-00001760: 2074 6865 206c 6f67 6963 2074 6f20 7375   the logic to su
-00001770: 7070 6f72 7420 4f43 5220 6675 6e63 7469  pport OCR functi
-00001780: 6f6e 732e 2042 7574 2069 7420 6164 6469  ons. But it addi
-00001790: 7469 6f6e 616c 6c79 2064 6f65 7320 6e65  tionally does ne
-000017a0: 6564 2054 6573 7365 7261 6374 e280 9973  ed Tesseract...s
-000017b0: 206c 616e 6775 6167 6520 7375 7070 6f72   language suppor
-000017c0: 7420 6461 7461 2c20 736f 2069 6e73 7461  t data, so insta
-000017d0: 6c6c 6174 696f 6e20 6f66 2054 6573 7365  llation of Tesse
-000017e0: 7261 6374 2d4f 4352 2069 7320 7374 696c  ract-OCR is stil
-000017f0: 6c20 7265 7175 6972 6564 2e0a 0a54 6865  l required...The
-00001800: 206c 616e 6775 6167 6520 7375 7070 6f72   language suppor
-00001810: 7420 666f 6c64 6572 206c 6f63 6174 696f  t folder locatio
-00001820: 6e20 6d75 7374 2062 6520 636f 6d6d 756e  n must be commun
-00001830: 6963 6174 6564 2065 6974 6865 7220 7669  icated either vi
-00001840: 6120 7374 6f72 696e 6720 6974 2069 6e20  a storing it in 
-00001850: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
-00001860: 7661 7269 6162 6c65 2022 5445 5353 4441  variable "TESSDA
-00001870: 5441 5f50 5245 4649 5822 2c20 6f72 2061  TA_PREFIX", or a
-00001880: 7320 6120 7061 7261 6d65 7465 7220 696e  s a parameter in
-00001890: 2074 6865 2061 7070 6c69 6361 626c 6520   the applicable 
-000018a0: 6675 6e63 7469 6f6e 732e 0a0a 536f 2066  functions...So f
-000018b0: 6f72 2061 2077 6f72 6b69 6e67 204f 4352  or a working OCR
-000018c0: 2066 756e 6374 696f 6e61 6c69 7479 2c20   functionality, 
-000018d0: 6d61 6b65 2073 7572 6520 746f 2063 6f6d  make sure to com
-000018e0: 706c 6574 6520 7468 6973 2063 6865 636b  plete this check
-000018f0: 6c69 7374 3a0a 0a31 2e20 496e 7374 616c  list:..1. Instal
-00001900: 6c20 5465 7373 6572 6163 742e 0a0a 322e  l Tesseract...2.
-00001910: 204c 6f63 6174 6520 5465 7373 6572 6163   Locate Tesserac
-00001920: 74e2 8099 7320 6c61 6e67 7561 6765 2073  t...s language s
-00001930: 7570 706f 7274 2066 6f6c 6465 722e 2054  upport folder. T
-00001940: 7970 6963 616c 6c79 2079 6f75 2077 696c  ypically you wil
-00001950: 6c20 6669 6e64 2069 7420 6865 7265 3a0a  l find it here:.
-00001960: 0a20 2020 2d20 5769 6e64 6f77 733a 2060  .   - Windows: `
-00001970: 433a 2f50 726f 6772 616d 2046 696c 6573  C:/Program Files
-00001980: 2f54 6573 7365 7261 6374 2d4f 4352 2f74  /Tesseract-OCR/t
-00001990: 6573 7364 6174 6160 0a0a 2020 202d 2055  essdata`..   - U
-000019a0: 6e69 7820 7379 7374 656d 733a 2060 2f75  nix systems: `/u
-000019b0: 7372 2f73 6861 7265 2f74 6573 7365 7261  sr/share/tessera
-000019c0: 6374 2d6f 6372 2f35 2f74 6573 7364 6174  ct-ocr/5/tessdat
-000019d0: 6160 0a0a 332e 2053 6574 2074 6865 2065  a`..3. Set the e
-000019e0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-000019f0: 626c 6520 5445 5353 4441 5441 5f50 5245  ble TESSDATA_PRE
-00001a00: 4649 580a 0a20 2020 2d20 5769 6e64 6f77  FIX..   - Window
-00001a10: 733a 2060 7365 7478 2054 4553 5344 4154  s: `setx TESSDAT
-00001a20: 415f 5052 4546 4958 2022 433a 2f50 726f  A_PREFIX "C:/Pro
-00001a30: 6772 616d 2046 696c 6573 2f54 6573 7365  gram Files/Tesse
-00001a40: 7261 6374 2d4f 4352 2f74 6573 7364 6174  ract-OCR/tessdat
-00001a50: 6122 600a 0a20 2020 2d20 556e 6978 2073  a"`..   - Unix s
-00001a60: 7973 7465 6d73 3a20 6064 6563 6c61 7265  ystems: `declare
-00001a70: 202d 7820 5445 5353 4441 5441 5f50 5245   -x TESSDATA_PRE
-00001a80: 4649 583d 202f 7573 722f 7368 6172 652f  FIX= /usr/share/
-00001a90: 7465 7373 6572 6163 742d 6f63 722f 352f  tesseract-ocr/5/
-00001aa0: 7465 7373 6461 7461 600a 0a2a 2a4e 6f74  tessdata`..**Not
-00001ab0: 653a 2a2a 205f 4f6e 2057 696e 646f 7773  e:** _On Windows
-00001ac0: 2073 7973 7465 6d73 2c20 7468 6973 206d   systems, this m
-00001ad0: 7573 7420 6861 7070 656e 206f 7574 7369  ust happen outsi
-00001ae0: 6465 2050 7974 686f 6e20 e280 9320 6265  de Python ... be
-00001af0: 666f 7265 2073 7461 7274 696e 6720 796f  fore starting yo
-00001b00: 7572 2073 6372 6970 742e 204a 7573 7420  ur script. Just 
-00001b10: 6d61 6e69 7075 6c61 7469 6e67 206f 732e  manipulating os.
-00001b20: 656e 7669 726f 6e20 7769 6c6c 206e 6f74  environ will not
-00001b30: 2077 6f72 6b21 5f0a 0a23 2323 2320 322e   work!_..#### 2.
-00001b40: 204d 4c20 5461 626c 6520 4465 7465 6374   ML Table Detect
-00001b50: 696f 6e20 284f 7074 696f 6e61 6c29 0a0a  ion (Optional)..
-00001b60: 5468 6973 2072 6570 6f73 6974 6f72 7920  This repository 
-00001b70: 7072 6f76 6964 6573 2061 6e20 6f70 7469  provides an opti
-00001b80: 6f6e 616c 2066 6561 7475 7265 2074 6f20  onal feature to 
-00001b90: 7061 7273 6520 636f 6e74 656e 7420 6672  parse content fr
-00001ba0: 6f6d 2074 6162 6c65 7320 7573 696e 6720  om tables using 
-00001bb0: 6120 7661 7269 6574 7920 6f66 2064 6565  a variety of dee
-00001bc0: 7020 6c65 6172 6e69 6e67 206d 6f64 656c  p learning model
-00001bd0: 732e 0a0a 6060 6063 6f6e 736f 6c65 0a70  s...```console.p
-00001be0: 6970 2069 6e73 7461 6c6c 2022 6f70 656e  ip install "open
-00001bf0: 7061 7273 655b 6d6c 5d22 0a60 6060 0a0a  parse[ml]".```..
-00001c00: 5468 656e 2064 6f77 6e6c 6f61 6420 7468  Then download th
-00001c10: 6520 6d6f 6465 6c20 7765 6967 6874 7320  e model weights 
-00001c20: 7769 7468 0a0a 6060 6063 6f6e 736f 6c65  with..```console
-00001c30: 0a6f 7065 6e70 6172 7365 2d64 6f77 6e6c  .openparse-downl
-00001c40: 6f61 640a 6060 600a 0a59 6f75 2063 616e  oad.```..You can
-00001c50: 2072 756e 2074 6865 2070 6172 7369 6e67   run the parsing
-00001c60: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
-00001c70: 696e 672e 200a 0a60 6060 7079 7468 6f6e  ing. ..```python
-00001c80: 0a70 6172 7365 7220 3d20 6f70 656e 7061  .parser = openpa
-00001c90: 7273 652e 446f 6375 6d65 6e74 5061 7273  rse.DocumentPars
-00001ca0: 6572 280a 2020 2020 2020 2020 7461 626c  er(.        tabl
-00001cb0: 655f 6172 6773 3d7b 0a20 2020 2020 2020  e_args={.       
-00001cc0: 2020 2020 2022 7061 7273 696e 675f 616c       "parsing_al
-00001cd0: 676f 7269 7468 6d22 3a20 2275 6e69 7461  gorithm": "unita
-00001ce0: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
-00001cf0: 2020 226d 696e 5f74 6162 6c65 5f63 6f6e    "min_table_con
-00001d00: 6669 6465 6e63 6522 3a20 302e 382c 0a20  fidence": 0.8,. 
-00001d10: 2020 2020 2020 207d 2c0a 290a 7061 7273         },.).pars
-00001d20: 6564 5f6e 6f64 6573 203d 2070 6172 7365  ed_nodes = parse
-00001d30: 722e 7061 7273 6528 7064 665f 7061 7468  r.parse(pdf_path
-00001d40: 290a 6060 600a 0a4e 6f74 6520 7765 2063  ).```..Note we c
-00001d50: 7572 7265 6e74 6c79 2075 7365 205b 7461  urrently use [ta
-00001d60: 626c 652d 7472 616e 7366 6f72 6d65 7273  ble-transformers
-00001d70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001d80: 2e63 6f6d 2f6d 6963 726f 736f 6674 2f74  .com/microsoft/t
-00001d90: 6162 6c65 2d74 7261 6e73 666f 726d 6572  able-transformer
-00001da0: 2920 666f 7220 616c 6c20 7461 626c 6520  ) for all table 
-00001db0: 6465 7465 6374 696f 6e20 616e 6420 7765  detection and we
-00001dc0: 2066 696e 6420 6974 7320 7065 7266 6f72   find its perfor
-00001dd0: 6d61 6e63 6520 746f 2062 6520 7375 6270  mance to be subp
-00001de0: 6172 2e20 5468 6973 206e 6567 6174 6976  ar. This negativ
-00001df0: 656c 7920 6166 6665 6374 7320 7468 6520  ely affects the 
-00001e00: 646f 776e 7374 7265 616d 2072 6573 756c  downstream resul
-00001e10: 7473 206f 6620 756e 6974 6162 6c65 2e20  ts of unitable. 
-00001e20: 4966 2079 6f75 2772 6520 6177 6172 6520  If you're aware 
-00001e30: 6f66 2061 2062 6574 7465 7220 6d6f 6465  of a better mode
-00001e40: 6c20 706c 6561 7365 206f 7065 6e20 616e  l please open an
-00001e50: 2049 7373 7565 202d 2074 6865 2075 6e69   Issue - the uni
-00001e60: 7461 626c 6520 7465 616d 206d 656e 7469  table team menti
-00001e70: 6f6e 6564 2074 6865 7920 6d69 6768 7420  oned they might 
-00001e80: 6164 6420 7468 6973 2073 6f6f 6e20 746f  add this soon to
-00001e90: 6f2e 0a0a 2323 2043 6f6f 6b62 6f6f 6b73  o...## Cookbooks
-00001ea0: 0a0a 6874 7470 733a 2f2f 6769 7468 7562  ..https://github
-00001eb0: 2e63 6f6d 2f46 696c 696d 6f61 2f6f 7065  .com/Filimoa/ope
-00001ec0: 6e2d 7061 7273 652f 7472 6565 2f6d 6169  n-parse/tree/mai
-00001ed0: 6e2f 7372 632f 636f 6f6b 626f 6f6b 730a  n/src/cookbooks.
-00001ee0: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
-00001ef0: 6e0a 0a68 7474 7073 3a2f 2f66 696c 696d  n..https://filim
-00001f00: 6f61 2e67 6974 6875 622e 696f 2f6f 7065  oa.github.io/ope
-00001f10: 6e2d 7061 7273 652f 0a                   n-parse/.
+00000070: 204c 4c4d 2773 2e0a 4175 7468 6f72 2d65   LLM's..Author-e
+00000080: 6d61 696c 3a20 5365 7267 6579 2046 696c  mail: Sergey Fil
+00000090: 696d 6f6e 6f76 203c 6865 6c6c 6f40 7365  imonov <hello@se
+000000a0: 7267 6579 2e66 7969 3e0a 5072 6f6a 6563  rgey.fyi>.Projec
+000000b0: 742d 5552 4c3a 2068 6f6d 6570 6167 652c  t-URL: homepage,
+000000c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000d0: 636f 6d2f 4669 6c69 6d6f 612f 6f70 656e  com/Filimoa/open
+000000e0: 2d70 6172 7365 0a50 726f 6a65 6374 2d55  -parse.Project-U
+000000f0: 524c 3a20 7265 706f 7369 746f 7279 2c20  RL: repository, 
+00000100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000110: 6f6d 2f46 696c 696d 6f61 2f6f 7065 6e2d  om/Filimoa/open-
+00000120: 7061 7273 650a 5072 6f6a 6563 742d 5552  parse.Project-UR
+00000130: 4c3a 2064 6f63 756d 656e 7461 7469 6f6e  L: documentation
+00000140: 2c20 6874 7470 733a 2f2f 6669 6c69 6d6f  , https://filimo
+00000150: 612e 6769 7468 7562 2e69 6f2f 6f70 656e  a.github.io/open
+00000160: 2d70 6172 7365 0a52 6571 7569 7265 732d  -parse.Requires-
+00000170: 5079 7468 6f6e 3a20 3e3d 332e 380a 4465  Python: >=3.8.De
+00000180: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+00000190: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000001a0: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
+000001b0: 6c65 3a20 4c49 4345 4e53 450a 5265 7175  le: LICENSE.Requ
+000001c0: 6972 6573 2d44 6973 743a 2050 794d 7550  ires-Dist: PyMuP
+000001d0: 4446 3e3d 312e 3233 2e32 0a52 6571 7569  DF>=1.23.2.Requi
+000001e0: 7265 732d 4469 7374 3a20 7069 6c6c 6f77  res-Dist: pillow
+000001f0: 3e3d 382e 330a 5265 7175 6972 6573 2d44  >=8.3.Requires-D
+00000200: 6973 743a 2070 7964 616e 7469 633e 3d32  ist: pydantic>=2
+00000210: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
+00000220: 3a20 7079 7064 663e 3d34 2e30 2e30 0a52  : pypdf>=4.0.0.R
+00000230: 6571 7569 7265 732d 4469 7374 3a20 7064  equires-Dist: pd
+00000240: 666d 696e 6572 2e73 6978 3e3d 3230 3230  fminer.six>=2020
+00000250: 3034 3031 0a52 6571 7569 7265 732d 4469  0401.Requires-Di
+00000260: 7374 3a20 7469 6b74 6f6b 656e 3e3d 302e  st: tiktoken>=0.
+00000270: 330a 5265 7175 6972 6573 2d44 6973 743a  3.Requires-Dist:
+00000280: 206f 7065 6e61 693e 3d31 2e30 2e30 0a52   openai>=1.0.0.R
+00000290: 6571 7569 7265 732d 4469 7374 3a20 6e75  equires-Dist: nu
+000002a0: 6d70 790a 5072 6f76 6964 6573 2d45 7874  mpy.Provides-Ext
+000002b0: 7261 3a20 6d6c 0a52 6571 7569 7265 732d  ra: ml.Requires-
+000002c0: 4469 7374 3a20 746f 7263 683b 2065 7874  Dist: torch; ext
+000002d0: 7261 203d 3d20 226d 6c22 0a52 6571 7569  ra == "ml".Requi
+000002e0: 7265 732d 4469 7374 3a20 746f 7263 6876  res-Dist: torchv
+000002f0: 6973 696f 6e3b 2065 7874 7261 203d 3d20  ision; extra == 
+00000300: 226d 6c22 0a52 6571 7569 7265 732d 4469  "ml".Requires-Di
+00000310: 7374 3a20 7472 616e 7366 6f72 6d65 7273  st: transformers
+00000320: 3b20 6578 7472 6120 3d3d 2022 6d6c 220a  ; extra == "ml".
+00000330: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000340: 6f6b 656e 697a 6572 733b 2065 7874 7261  okenizers; extra
+00000350: 203d 3d20 226d 6c22 0a0a 3c70 2061 6c69   == "ml"..<p ali
+00000360: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000370: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000380: 3a2f 2f73 6572 6765 792d 6669 6c69 6d6f  ://sergey-filimo
+00000390: 6e6f 762e 6e79 6333 2e64 6967 6974 616c  nov.nyc3.digital
+000003a0: 6f63 6561 6e73 7061 6365 732e 636f 6d2f  oceanspaces.com/
+000003b0: 6f70 656e 2d70 6172 7365 2f6f 7065 6e2d  open-parse/open-
+000003c0: 7061 7273 652d 7769 7468 2d74 6578 742d  parse-with-text-
+000003d0: 7470 2d6c 6f67 6f2e 7765 6270 2220 7769  tp-logo.webp" wi
+000003e0: 6474 683d 2233 3530 2220 2f3e 0a3c 2f70  dth="350" />.</p
+000003f0: 3e0a 3c62 722f 3e0a 0a2a 2a45 6173 696c  >.<br/>..**Easil
+00000400: 7920 6368 756e 6b20 636f 6d70 6c65 7820  y chunk complex 
+00000410: 646f 6375 6d65 6e74 7320 7468 6520 7361  documents the sa
+00000420: 6d65 2077 6179 2061 2068 756d 616e 2077  me way a human w
+00000430: 6f75 6c64 2e2a 2a20 200a 0a43 6875 6e6b  ould.**  ..Chunk
+00000440: 696e 6720 646f 6375 6d65 6e74 7320 6973  ing documents is
+00000450: 2061 2063 6861 6c6c 656e 6769 6e67 2074   a challenging t
+00000460: 6173 6b20 7468 6174 2075 6e64 6572 7069  ask that underpi
+00000470: 6e73 2061 6e79 2052 4147 2073 7973 7465  ns any RAG syste
+00000480: 6d2e 2020 4869 6768 2071 7561 6c69 7479  m.  High quality
+00000490: 2072 6573 756c 7473 2061 7265 2063 7269   results are cri
+000004a0: 7469 6361 6c20 746f 2061 2073 7563 6573  tical to a suces
+000004b0: 7366 756c 2041 4920 6170 706c 6963 6174  sful AI applicat
+000004c0: 696f 6e2c 2079 6574 206d 6f73 7420 6f70  ion, yet most op
+000004d0: 656e 2d73 6f75 7263 6520 6c69 6272 6172  en-source librar
+000004e0: 6965 7320 6172 6520 6c69 6d69 7465 6420  ies are limited 
+000004f0: 696e 2074 6865 6972 2061 6269 6c69 7479  in their ability
+00000500: 2074 6f20 6861 6e64 6c65 2063 6f6d 706c   to handle compl
+00000510: 6578 2064 6f63 756d 656e 7473 2e20 200a  ex documents.  .
+00000520: 0a4f 7065 6e20 5061 7273 6520 6973 2064  .Open Parse is d
+00000530: 6573 6967 6e65 6420 746f 2066 696c 6c20  esigned to fill 
+00000540: 7468 6973 2067 6170 2062 7920 7072 6f76  this gap by prov
+00000550: 6964 696e 6720 6120 666c 6578 6962 6c65  iding a flexible
+00000560: 2c20 6561 7379 2d74 6f2d 7573 6520 6c69  , easy-to-use li
+00000570: 6272 6172 7920 6361 7061 626c 6520 6f66  brary capable of
+00000580: 2076 6973 7561 6c6c 7920 6469 7363 6572   visually discer
+00000590: 6e69 6e67 2064 6f63 756d 656e 7420 6c61  ning document la
+000005a0: 796f 7574 7320 616e 6420 6368 756e 6b69  youts and chunki
+000005b0: 6e67 2074 6865 6d20 6566 6665 6374 6976  ng them effectiv
+000005c0: 656c 792e 0a0a 3c64 6574 6169 6c73 3e0a  ely...<details>.
+000005d0: 2020 3c73 756d 6d61 7279 3e3c 623e 486f    <summary><b>Ho
+000005e0: 7720 6973 2074 6869 7320 6469 6666 6572  w is this differ
+000005f0: 656e 7420 6672 6f6d 206f 7468 6572 206c  ent from other l
+00000600: 6179 6f75 7420 7061 7273 6572 733f 3c2f  ayout parsers?</
+00000610: 623e 3c2f 7375 6d6d 6172 793e 0a0a 2020  b></summary>..  
+00000620: 2323 2323 20e2 9c82 efb8 8f20 5465 7874  #### ...... Text
+00000630: 2053 706c 6974 7469 6e67 0a20 2054 6578   Splitting.  Tex
+00000640: 7420 7370 6c69 7474 696e 6720 636f 6e76  t splitting conv
+00000650: 6572 7473 2061 2066 696c 6520 746f 2072  erts a file to r
+00000660: 6177 2074 6578 7420 616e 6420 5b73 6c69  aw text and [sli
+00000670: 6365 7320 6974 2075 705d 2868 7474 7073  ces it up](https
+00000680: 3a2f 2f64 6f63 732e 6c6c 616d 6169 6e64  ://docs.llamaind
+00000690: 6578 2e61 692f 656e 2f73 7461 626c 652f  ex.ai/en/stable/
+000006a0: 6170 695f 7265 6665 7265 6e63 652f 6e6f  api_reference/no
+000006b0: 6465 5f70 6172 7365 7273 2f74 6f6b 656e  de_parsers/token
+000006c0: 5f74 6578 745f 7370 6c69 7474 6572 2f29  _text_splitter/)
+000006d0: 2e0a 2020 0a20 202d 2059 6f75 206c 6f73  ..  .  - You los
+000006e0: 6520 7468 6520 6162 696c 6974 7920 746f  e the ability to
+000006f0: 2065 6173 696c 7920 6f76 6572 6c61 7920   easily overlay 
+00000700: 7468 6520 6368 756e 6b20 6f6e 2074 6865  the chunk on the
+00000710: 206f 7269 6769 6e61 6c20 7064 660a 2020   original pdf.  
+00000720: 2d20 596f 7520 6967 6e6f 7265 2074 6865  - You ignore the
+00000730: 2075 6e64 6572 6c79 696e 6720 7365 6d61   underlying sema
+00000740: 6e74 6963 2073 7472 7563 7475 7265 206f  ntic structure o
+00000750: 6620 7468 6520 6669 6c65 202d 2068 6561  f the file - hea
+00000760: 6469 6e67 732c 2073 6563 7469 6f6e 732c  dings, sections,
+00000770: 2062 756c 6c65 7473 2072 6570 7265 7365   bullets represe
+00000780: 6e74 2076 616c 7561 626c 6520 696e 666f  nt valuable info
+00000790: 726d 6174 696f 6e2e 0a20 202d 204e 6f20  rmation..  - No 
+000007a0: 7375 7070 6f72 7420 666f 7220 7461 626c  support for tabl
+000007b0: 6573 2c20 696d 6167 6573 206f 7220 6d61  es, images or ma
+000007c0: 726b 646f 776e 2e0a 2020 0a20 2023 2323  rkdown..  .  ###
+000007d0: 2320 f09f a496 204d 4c20 4c61 796f 7574  # .... ML Layout
+000007e0: 2050 6172 7365 7273 0a20 2054 6865 7265   Parsers.  There
+000007f0: 2773 2073 6f6d 6520 6f66 2066 616e 7461  's some of fanta
+00000800: 7374 6963 206c 6962 7261 7269 6573 206c  stic libraries l
+00000810: 696b 6520 5b6c 6179 6f75 742d 7061 7273  ike [layout-pars
+00000820: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
+00000830: 7562 2e63 6f6d 2f4c 6179 6f75 742d 5061  ub.com/Layout-Pa
+00000840: 7273 6572 2f6c 6179 6f75 742d 7061 7273  rser/layout-pars
+00000850: 6572 292e 200a 2020 2d20 5768 696c 6520  er). .  - While 
+00000860: 7468 6579 2063 616e 2069 6465 6e74 6966  they can identif
+00000870: 7920 7661 7269 6f75 7320 656c 656d 656e  y various elemen
+00000880: 7473 206c 696b 6520 7465 7874 2062 6c6f  ts like text blo
+00000890: 636b 732c 2069 6d61 6765 732c 2061 6e64  cks, images, and
+000008a0: 2074 6162 6c65 732c 2062 7574 2074 6865   tables, but the
+000008b0: 7920 6172 6520 6e6f 7420 6275 696c 7420  y are not built 
+000008c0: 746f 2067 726f 7570 2072 656c 6174 6564  to group related
+000008d0: 2063 6f6e 7465 6e74 2065 6666 6563 7469   content effecti
+000008e0: 7665 6c79 2e0a 2020 2d20 5468 6579 2073  vely..  - They s
+000008f0: 7472 6963 746c 7920 666f 6375 7320 6f6e  trictly focus on
+00000900: 206c 6179 6f75 7420 7061 7273 696e 6720   layout parsing 
+00000910: 2d20 796f 7520 7769 6c6c 206e 6565 6420  - you will need 
+00000920: 746f 2061 6464 2061 6e6f 7468 6572 206d  to add another m
+00000930: 6f64 656c 2074 6f20 6578 7472 6163 7420  odel to extract 
+00000940: 6d61 726b 646f 776e 2066 726f 6d20 7468  markdown from th
+00000950: 6520 696d 6167 6573 2c20 7061 7273 6520  e images, parse 
+00000960: 7461 626c 6573 2c20 6772 6f75 7020 6e6f  tables, group no
+00000970: 6465 732c 2065 7463 2e0a 2020 2d20 5765  des, etc..  - We
+00000980: 2776 6520 666f 756e 6420 7065 7266 6f72  've found perfor
+00000990: 6d61 6e63 6520 746f 2062 6520 7375 622d  mance to be sub-
+000009a0: 6f70 7469 6d61 6c20 6f6e 206d 616e 7920  optimal on many 
+000009b0: 646f 6375 6d65 6e74 7320 7768 696c 6520  documents while 
+000009c0: 616c 736f 2062 6569 6e67 2063 6f6d 7075  also being compu
+000009d0: 7461 7469 6f6e 616c 6c79 2068 6561 7679  tationally heavy
+000009e0: 2e0a 0a20 2023 2323 2320 f09f 92bc 2043  ...  #### .... C
+000009f0: 6f6d 6d65 7263 6961 6c20 536f 6c75 7469  ommercial Soluti
+00000a00: 6f6e 730a 0a20 202d 2054 7970 6963 616c  ons..  - Typical
+00000a10: 6c79 2070 7269 6365 6420 6174 20e2 8988  ly priced at ...
+00000a20: 2024 3130 202f 2031 6b20 7061 6765 732e   $10 / 1k pages.
+00000a30: 2053 6565 205b 6865 7265 5d28 6874 7470   See [here](http
+00000a40: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+00000a50: 2e63 6f6d 2f64 6f63 756d 656e 742d 6169  .com/document-ai
+00000a60: 292c 205b 6865 7265 5d28 6874 7470 733a  ), [here](https:
+00000a70: 2f2f 6177 732e 616d 617a 6f6e 2e63 6f6d  //aws.amazon.com
+00000a80: 2f74 6578 7472 6163 742f 2920 616e 6420  /textract/) and 
+00000a90: 5b68 6572 655d 2868 7474 7073 3a2f 2f77  [here](https://w
+00000aa0: 7777 2e72 6564 7563 746f 2e61 692f 292e  ww.reducto.ai/).
+00000ab0: 0a20 202d 2052 6571 7569 7265 7320 7368  .  - Requires sh
+00000ac0: 6172 696e 6720 796f 7572 2064 6174 6120  aring your data 
+00000ad0: 7769 7468 2061 2076 656e 646f 720a 0a3c  with a vendor..<
+00000ae0: 2f64 6574 6169 6c73 3e0a 0a23 2320 4869  /details>..## Hi
+00000af0: 6768 6c69 6768 7473 0a0a 2d20 2a2a f09f  ghlights..- **..
+00000b00: 948d 2056 6973 7561 6c6c 792d 4472 6976  .. Visually-Driv
+00000b10: 656e 3a2a 2a20 4f70 656e 2d50 6172 7365  en:** Open-Parse
+00000b20: 2076 6973 7561 6c6c 7920 616e 616c 797a   visually analyz
+00000b30: 6573 2064 6f63 756d 656e 7473 2066 6f72  es documents for
+00000b40: 2073 7570 6572 696f 7220 4c4c 4d20 696e   superior LLM in
+00000b50: 7075 742c 2067 6f69 6e67 2062 6579 6f6e  put, going beyon
+00000b60: 6420 6e61 6976 6520 7465 7874 2073 706c  d naive text spl
+00000b70: 6974 7469 6e67 2e0a 2d20 2a2a e29c 8def  itting..- **....
+00000b80: b88f 204d 6172 6b64 6f77 6e20 5375 7070  .. Markdown Supp
+00000b90: 6f72 743a 2a2a 2042 6173 6963 206d 6172  ort:** Basic mar
+00000ba0: 6b64 6f77 6e20 7375 7070 6f72 7420 666f  kdown support fo
+00000bb0: 7220 7061 7273 696e 6720 6865 6164 696e  r parsing headin
+00000bc0: 6773 2c20 626f 6c64 2061 6e64 2069 7461  gs, bold and ita
+00000bd0: 6c69 6373 2e0a 2d20 2a2a f09f 938a 2048  lics..- **.... H
+00000be0: 6967 682d 5072 6563 6973 696f 6e20 5461  igh-Precision Ta
+00000bf0: 626c 6520 5375 7070 6f72 743a 2a2a 2045  ble Support:** E
+00000c00: 7874 7261 6374 2074 6162 6c65 7320 696e  xtract tables in
+00000c10: 746f 2063 6c65 616e 204d 6172 6b64 6f77  to clean Markdow
+00000c20: 6e20 666f 726d 6174 7320 7769 7468 2061  n formats with a
+00000c30: 6363 7572 6163 7920 7468 6174 2073 7572  ccuracy that sur
+00000c40: 7061 7373 6573 2074 7261 6469 7469 6f6e  passes tradition
+00000c50: 616c 2074 6f6f 6c73 2e0a 2020 2020 3c64  al tools..    <d
+00000c60: 6574 6169 6c73 3e0a 2020 3c73 756d 6d61  etails>.  <summa
+00000c70: 7279 3e3c 693e 4578 616d 706c 6573 3c2f  ry><i>Examples</
+00000c80: 693e 3c2f 7375 6d6d 6172 793e 0a20 2054  i></summary>.  T
+00000c90: 6865 2066 6f6c 6c6f 7769 6e67 2065 7861  he following exa
+00000ca0: 6d70 6c65 7320 7765 7265 2070 6172 7365  mples were parse
+00000cb0: 6420 7769 7468 2075 6e69 7461 626c 652e  d with unitable.
+00000cc0: 0a20 2020 203c 6272 2f3e 0a20 2020 203c  .    <br/>.    <
+00000cd0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000ce0: 3e0a 2020 2020 2020 2020 3c62 722f 3e0a  >.        <br/>.
+00000cf0: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000d00: 3d22 6874 7470 733a 2f2f 7365 7267 6579  ="https://sergey
+00000d10: 2d66 696c 696d 6f6e 6f76 2e6e 7963 332e  -filimonov.nyc3.
+00000d20: 6469 6769 7461 6c6f 6365 616e 7370 6163  digitaloceanspac
+00000d30: 6573 2e63 6f6d 2f6f 7065 6e2d 7061 7273  es.com/open-pars
+00000d40: 652f 756e 6974 6162 6c65 2d70 6172 7369  e/unitable-parsi
+00000d50: 6e67 2d73 616d 706c 652e 7765 6270 2220  ng-sample.webp" 
+00000d60: 7769 6474 683d 2236 3530 222f 3e0a 2020  width="650"/>.  
+00000d70: 2020 3c2f 703e 0a20 2020 2020 2020 2020    </p>.         
+00000d80: 3c62 722f 3e0a 2020 2020 3c2f 6465 7461  <br/>.    </deta
+00000d90: 696c 733e 0a0a 2d20 2a2a f09f 9ba0 efb8  ils>..- **......
+00000da0: 8f20 4578 7465 6e73 6962 6c65 3a2a 2a20  . Extensible:** 
+00000db0: 4561 7369 6c79 2069 6d70 6c65 6d65 6e74  Easily implement
+00000dc0: 2079 6f75 7220 6f77 6e20 706f 7374 2d70   your own post-p
+00000dd0: 726f 6365 7373 696e 6720 7374 6570 732e  rocessing steps.
+00000de0: 0a2d 202a 2af0 9f92 a149 6e74 7569 7469  .- **....Intuiti
+00000df0: 7665 3a2a 2a20 4772 6561 7420 6564 6974  ve:** Great edit
+00000e00: 6f72 2073 7570 706f 7274 2e20 436f 6d70  or support. Comp
+00000e10: 6c65 7469 6f6e 2065 7665 7279 7768 6572  letion everywher
+00000e20: 652e 204c 6573 7320 7469 6d65 2064 6562  e. Less time deb
+00000e30: 7567 6769 6e67 2e0a 2d20 2a2a f09f 8eaf  ugging..- **....
+00000e40: 2045 6173 793a 2a2a 2044 6573 6967 6e65   Easy:** Designe
+00000e50: 6420 746f 2062 6520 6561 7379 2074 6f20  d to be easy to 
+00000e60: 7573 6520 616e 6420 6c65 6172 6e2e 204c  use and learn. L
+00000e70: 6573 7320 7469 6d65 2072 6561 6469 6e67  ess time reading
+00000e80: 2064 6f63 732e 0a0a 3c62 722f 3e0a 3c70   docs...<br/>.<p
+00000e90: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000ea0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000eb0: 7474 7073 3a2f 2f73 6572 6765 792d 6669  ttps://sergey-fi
+00000ec0: 6c69 6d6f 6e6f 762e 6e79 6333 2e64 6967  limonov.nyc3.dig
+00000ed0: 6974 616c 6f63 6561 6e73 7061 6365 732e  italoceanspaces.
+00000ee0: 636f 6d2f 6f70 656e 2d70 6172 7365 2f6d  com/open-parse/m
+00000ef0: 6172 6b65 642d 7570 2d64 6f63 2d32 2e77  arked-up-doc-2.w
+00000f00: 6562 7022 2077 6964 7468 3d22 3235 3022  ebp" width="250"
+00000f10: 202f 3e0a 3c2f 703e 0a0a 2323 2045 7861   />.</p>..## Exa
+00000f20: 6d70 6c65 0a0a 2323 2323 2042 6173 6963  mple..#### Basic
+00000f30: 2045 7861 6d70 6c65 0a0a 6060 6070 7974   Example..```pyt
+00000f40: 686f 6e0a 696d 706f 7274 206f 7065 6e70  hon.import openp
+00000f50: 6172 7365 0a0a 6261 7369 635f 646f 635f  arse..basic_doc_
+00000f60: 7061 7468 203d 2022 2e2f 7361 6d70 6c65  path = "./sample
+00000f70: 2d64 6f63 732f 6d6f 6269 6c65 2d68 6f6d  -docs/mobile-hom
+00000f80: 652d 6d61 6e75 616c 2e70 6466 220a 7061  e-manual.pdf".pa
+00000f90: 7273 6572 203d 206f 7065 6e70 6172 7365  rser = openparse
+00000fa0: 2e44 6f63 756d 656e 7450 6172 7365 7228  .DocumentParser(
+00000fb0: 290a 7061 7273 6564 5f62 6173 6963 5f64  ).parsed_basic_d
+00000fc0: 6f63 203d 2070 6172 7365 722e 7061 7273  oc = parser.pars
+00000fd0: 6528 6261 7369 635f 646f 635f 7061 7468  e(basic_doc_path
+00000fe0: 290a 0a66 6f72 206e 6f64 6520 696e 2070  )..for node in p
+00000ff0: 6172 7365 645f 6261 7369 635f 646f 632e  arsed_basic_doc.
+00001000: 6e6f 6465 733a 0a20 2020 2070 7269 6e74  nodes:.    print
+00001010: 286e 6f64 6529 0a60 6060 0a0a 2a2a f09f  (node).```..**..
+00001020: 9393 2054 7279 2074 6865 2073 616d 706c  .. Try the sampl
+00001030: 6520 6e6f 7465 626f 6f6b 2a2a 203c 6120  e notebook** <a 
+00001040: 6872 6566 3d22 6874 7470 733a 2f2f 636f  href="https://co
+00001050: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+00001060: 676c 652e 636f 6d2f 6472 6976 652f 315a  gle.com/drive/1Z
+00001070: 3542 3567 736e 6d68 464b 4546 4c2d 3579  5B5gsnmhFKEFL-5y
+00001080: 5949 636f 6f78 372d 6a51 616f 3845 703f  YIcoox7-jQao8Ep?
+00001090: 7573 703d 7368 6172 696e 6722 2063 6c61  usp=sharing" cla
+000010a0: 7373 3d22 6578 7465 726e 616c 2d6c 696e  ss="external-lin
+000010b0: 6b22 2074 6172 6765 743d 225f 626c 616e  k" target="_blan
+000010c0: 6b22 3e68 6572 653c 2f61 3e0a 0a23 2323  k">here</a>..###
+000010d0: 2320 5365 6d61 6e74 6963 2050 726f 6365  # Semantic Proce
+000010e0: 7373 696e 6720 4578 616d 706c 650a 0a43  ssing Example..C
+000010f0: 6875 6e6b 696e 6720 646f 6375 6d65 6e74  hunking document
+00001100: 7320 6973 2066 756e 6461 6d65 6e74 616c  s is fundamental
+00001110: 6c79 2061 626f 7574 2067 726f 7570 696e  ly about groupin
+00001120: 6720 7369 6d69 6c61 7220 7365 6d61 6e74  g similar semant
+00001130: 6963 206e 6f64 6573 2074 6f67 6574 6865  ic nodes togethe
+00001140: 722e 2042 7920 656d 6265 6464 696e 6720  r. By embedding 
+00001150: 7468 6520 7465 7874 206f 6620 6561 6368  the text of each
+00001160: 206e 6f64 652c 2077 6520 6361 6e20 7468   node, we can th
+00001170: 656e 2063 6c75 7374 6572 2074 6865 6d20  en cluster them 
+00001180: 746f 6765 7468 6572 2062 6173 6564 206f  together based o
+00001190: 6e20 7468 6569 7220 7369 6d69 6c61 7269  n their similari
+000011a0: 7479 2e0a 0a60 6060 7079 7468 6f6e 0a66  ty...```python.f
+000011b0: 726f 6d20 6f70 656e 7061 7273 6520 696d  rom openparse im
+000011c0: 706f 7274 2070 726f 6365 7373 696e 672c  port processing,
+000011d0: 2044 6f63 756d 656e 7450 6172 7365 720a   DocumentParser.
+000011e0: 0a73 656d 616e 7469 635f 7069 7065 6c69  .semantic_pipeli
+000011f0: 6e65 203d 2070 726f 6365 7373 696e 672e  ne = processing.
+00001200: 5365 6d61 6e74 6963 496e 6765 7374 696f  SemanticIngestio
+00001210: 6e50 6970 656c 696e 6528 0a20 2020 206f  nPipeline(.    o
+00001220: 7065 6e61 695f 6170 695f 6b65 793d 4f50  penai_api_key=OP
+00001230: 454e 5f41 495f 4b45 592c 0a20 2020 206d  EN_AI_KEY,.    m
+00001240: 6f64 656c 3d22 7465 7874 2d65 6d62 6564  odel="text-embed
+00001250: 6469 6e67 2d33 2d6c 6172 6765 222c 0a20  ding-3-large",. 
+00001260: 2020 206d 696e 5f74 6f6b 656e 733d 3634     min_tokens=64
+00001270: 2c0a 2020 2020 6d61 785f 746f 6b65 6e73  ,.    max_tokens
+00001280: 3d31 3032 342c 0a29 0a70 6172 7365 7220  =1024,.).parser 
+00001290: 3d20 446f 6375 6d65 6e74 5061 7273 6572  = DocumentParser
+000012a0: 280a 2020 2020 7072 6f63 6573 7369 6e67  (.    processing
+000012b0: 5f70 6970 656c 696e 653d 7365 6d61 6e74  _pipeline=semant
+000012c0: 6963 5f70 6970 656c 696e 652c 0a29 0a70  ic_pipeline,.).p
+000012d0: 6172 7365 645f 636f 6e74 656e 7420 3d20  arsed_content = 
+000012e0: 7061 7273 6572 2e70 6172 7365 2862 6173  parser.parse(bas
+000012f0: 6963 5f64 6f63 5f70 6174 6829 0a60 6060  ic_doc_path).```
+00001300: 0a0a 2a2a f09f 9393 2053 616d 706c 6520  ..**.... Sample 
+00001310: 6e6f 7465 626f 6f6b 2a2a 203c 6120 6872  notebook** <a hr
+00001320: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001330: 7562 2e63 6f6d 2f46 696c 696d 6f61 2f6f  ub.com/Filimoa/o
+00001340: 7065 6e2d 7061 7273 652f 626c 6f62 2f6d  pen-parse/blob/m
+00001350: 6169 6e2f 7372 632f 636f 6f6b 626f 6f6b  ain/src/cookbook
+00001360: 732f 7365 6d61 6e74 6963 5f70 726f 6365  s/semantic_proce
+00001370: 7373 696e 672e 6970 796e 6222 2063 6c61  ssing.ipynb" cla
+00001380: 7373 3d22 6578 7465 726e 616c 2d6c 696e  ss="external-lin
+00001390: 6b22 2074 6172 6765 743d 225f 626c 616e  k" target="_blan
+000013a0: 6b22 3e68 6572 653c 2f61 3e0a 0a23 2323  k">here</a>..###
+000013b0: 2320 5365 7269 616c 697a 696e 6720 5265  # Serializing Re
+000013c0: 7375 6c74 730a 5573 6573 2070 7964 616e  sults.Uses pydan
+000013d0: 7469 6320 756e 6465 7220 7468 6520 686f  tic under the ho
+000013e0: 6f64 2073 6f20 796f 7520 6361 6e20 7365  od so you can se
+000013f0: 7269 616c 697a 6520 7265 7375 6c74 7320  rialize results 
+00001400: 7769 7468 200a 0a60 6060 7079 7468 6f6e  with ..```python
+00001410: 0a70 6172 7365 645f 636f 6e74 656e 742e  .parsed_content.
+00001420: 6469 6374 2829 0a0a 2320 6f72 2074 6f20  dict()..# or to 
+00001430: 636f 6e76 6572 7420 746f 2061 2076 616c  convert to a val
+00001440: 6964 206a 736f 6e20 6469 6374 0a70 6172  id json dict.par
+00001450: 7365 645f 636f 6e74 656e 742e 6a73 6f6e  sed_content.json
+00001460: 2829 0a60 6060 0a0a 2323 2052 6571 7569  ().```..## Requi
+00001470: 7265 6d65 6e74 730a 0a50 7974 686f 6e20  rements..Python 
+00001480: 332e 382b 0a0a 2a2a 4465 616c 696e 6720  3.8+..**Dealing 
+00001490: 7769 7468 2050 4446 2773 3a2a 2a0a 0a2d  with PDF's:**..-
+000014a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000014b0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6466  //github.com/pdf
+000014c0: 6d69 6e65 722f 7064 666d 696e 6572 2e73  miner/pdfminer.s
+000014d0: 6978 2220 636c 6173 733d 2265 7874 6572  ix" class="exter
+000014e0: 6e61 6c2d 6c69 6e6b 2220 7461 7267 6574  nal-link" target
+000014f0: 3d22 5f62 6c61 6e6b 223e 7064 666d 696e  ="_blank">pdfmin
+00001500: 6572 2e73 6978 3c2f 613e 2046 756c 6c79  er.six</a> Fully
+00001510: 206f 7065 6e20 736f 7572 6365 2e0a 0a2a   open source...*
+00001520: 2a45 7874 7261 6374 696e 6720 5461 626c  *Extracting Tabl
+00001530: 6573 3a2a 2a0a 0a2d 203c 6120 6872 6566  es:**..- <a href
+00001540: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00001550: 2e63 6f6d 2f70 796d 7570 6466 2f50 794d  .com/pymupdf/PyM
+00001560: 7550 4446 2220 636c 6173 733d 2265 7874  uPDF" class="ext
+00001570: 6572 6e61 6c2d 6c69 6e6b 2220 7461 7267  ernal-link" targ
+00001580: 6574 3d22 5f62 6c61 6e6b 223e 5079 4d75  et="_blank">PyMu
+00001590: 5044 463c 2f61 3e20 6861 7320 736f 6d65  PDF</a> has some
+000015a0: 2074 6162 6c65 2064 6574 6563 7469 6f6e   table detection
+000015b0: 2066 756e 6374 696f 6e61 6c69 7479 2e20   functionality. 
+000015c0: 506c 6561 7365 2073 6565 2074 6865 6972  Please see their
+000015d0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000015e0: 2f2f 6d75 7064 662e 636f 6d2f 6c69 6365  //mupdf.com/lice
+000015f0: 6e73 696e 672f 696e 6465 782e 6874 6d6c  nsing/index.html
+00001600: 2363 6f6d 6d65 7263 6961 6c22 2063 6c61  #commercial" cla
+00001610: 7373 3d22 6578 7465 726e 616c 2d6c 696e  ss="external-lin
+00001620: 6b22 2074 6172 6765 743d 225f 626c 616e  k" target="_blan
+00001630: 6b22 3e6c 6963 656e 7365 3c2f 613e 2e0a  k">license</a>..
+00001640: 2d20 3c61 2068 7265 663d 2268 7474 7073  - <a href="https
+00001650: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00001660: 6f2f 6d69 6372 6f73 6f66 742f 7461 626c  o/microsoft/tabl
+00001670: 652d 7472 616e 7366 6f72 6d65 722d 6465  e-transformer-de
+00001680: 7465 6374 696f 6e22 2063 6c61 7373 3d22  tection" class="
+00001690: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
+000016a0: 6172 6765 743d 225f 626c 616e 6b22 3e54  arget="_blank">T
+000016b0: 6162 6c65 2054 7261 6e73 666f 726d 6572  able Transformer
+000016c0: 3c2f 613e 2069 7320 6120 6465 6570 206c  </a> is a deep l
+000016d0: 6561 726e 696e 6720 6170 7072 6f61 6368  earning approach
+000016e0: 2e0a 2d20 3c61 2068 7265 663d 2268 7474  ..- <a href="htt
+000016f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001700: 706f 6c6f 636c 7562 2f75 6e69 7461 626c  poloclub/unitabl
+00001710: 6522 2063 6c61 7373 3d22 6578 7465 726e  e" class="extern
+00001720: 616c 2d6c 696e 6b22 2074 6172 6765 743d  al-link" target=
+00001730: 225f 626c 616e 6b22 3e75 6e69 7461 626c  "_blank">unitabl
+00001740: 653c 2f61 3e20 6973 2061 6e6f 7468 6572  e</a> is another
+00001750: 2074 7261 6e73 666f 726d 6572 7320 6261   transformers ba
+00001760: 7365 6420 6170 7072 6f61 6368 2077 6974  sed approach wit
+00001770: 6820 2a2a 7374 6174 652d 6f66 2d74 6865  h **state-of-the
+00001780: 2d61 7274 2a2a 2070 6572 666f 726d 616e  -art** performan
+00001790: 6365 2e0a 0a23 2320 496e 7374 616c 6c61  ce...## Installa
+000017a0: 7469 6f6e 0a0a 2323 2323 2031 2e20 436f  tion..#### 1. Co
+000017b0: 7265 204c 6962 7261 7279 0a0a 6060 6063  re Library..```c
+000017c0: 6f6e 736f 6c65 0a70 6970 2069 6e73 7461  onsole.pip insta
+000017d0: 6c6c 206f 7065 6e70 6172 7365 0a60 6060  ll openparse.```
+000017e0: 0a0a 2a2a 456e 6162 6c69 6e67 204f 4352  ..**Enabling OCR
+000017f0: 2053 7570 706f 7274 2a2a 3a0a 0a50 794d   Support**:..PyM
+00001800: 7550 4446 2077 696c 6c20 616c 7265 6164  uPDF will alread
+00001810: 7920 636f 6e74 6169 6e20 616c 6c20 7468  y contain all th
+00001820: 6520 6c6f 6769 6320 746f 2073 7570 706f  e logic to suppo
+00001830: 7274 204f 4352 2066 756e 6374 696f 6e73  rt OCR functions
+00001840: 2e20 4275 7420 6974 2061 6464 6974 696f  . But it additio
+00001850: 6e61 6c6c 7920 646f 6573 206e 6565 6420  nally does need 
+00001860: 5465 7373 6572 6163 74e2 8099 7320 6c61  Tesseract...s la
+00001870: 6e67 7561 6765 2073 7570 706f 7274 2064  nguage support d
+00001880: 6174 612c 2073 6f20 696e 7374 616c 6c61  ata, so installa
+00001890: 7469 6f6e 206f 6620 5465 7373 6572 6163  tion of Tesserac
+000018a0: 742d 4f43 5220 6973 2073 7469 6c6c 2072  t-OCR is still r
+000018b0: 6571 7569 7265 642e 0a0a 5468 6520 6c61  equired...The la
+000018c0: 6e67 7561 6765 2073 7570 706f 7274 2066  nguage support f
+000018d0: 6f6c 6465 7220 6c6f 6361 7469 6f6e 206d  older location m
+000018e0: 7573 7420 6265 2063 6f6d 6d75 6e69 6361  ust be communica
+000018f0: 7465 6420 6569 7468 6572 2076 6961 2073  ted either via s
+00001900: 746f 7269 6e67 2069 7420 696e 2074 6865  toring it in the
+00001910: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00001920: 6961 626c 6520 2254 4553 5344 4154 415f  iable "TESSDATA_
+00001930: 5052 4546 4958 222c 206f 7220 6173 2061  PREFIX", or as a
+00001940: 2070 6172 616d 6574 6572 2069 6e20 7468   parameter in th
+00001950: 6520 6170 706c 6963 6162 6c65 2066 756e  e applicable fun
+00001960: 6374 696f 6e73 2e0a 0a53 6f20 666f 7220  ctions...So for 
+00001970: 6120 776f 726b 696e 6720 4f43 5220 6675  a working OCR fu
+00001980: 6e63 7469 6f6e 616c 6974 792c 206d 616b  nctionality, mak
+00001990: 6520 7375 7265 2074 6f20 636f 6d70 6c65  e sure to comple
+000019a0: 7465 2074 6869 7320 6368 6563 6b6c 6973  te this checklis
+000019b0: 743a 0a0a 312e 2049 6e73 7461 6c6c 2054  t:..1. Install T
+000019c0: 6573 7365 7261 6374 2e0a 0a32 2e20 4c6f  esseract...2. Lo
+000019d0: 6361 7465 2054 6573 7365 7261 6374 e280  cate Tesseract..
+000019e0: 9973 206c 616e 6775 6167 6520 7375 7070  .s language supp
+000019f0: 6f72 7420 666f 6c64 6572 2e20 5479 7069  ort folder. Typi
+00001a00: 6361 6c6c 7920 796f 7520 7769 6c6c 2066  cally you will f
+00001a10: 696e 6420 6974 2068 6572 653a 0a0a 2020  ind it here:..  
+00001a20: 202d 2057 696e 646f 7773 3a20 6043 3a2f   - Windows: `C:/
+00001a30: 5072 6f67 7261 6d20 4669 6c65 732f 5465  Program Files/Te
+00001a40: 7373 6572 6163 742d 4f43 522f 7465 7373  sseract-OCR/tess
+00001a50: 6461 7461 600a 0a20 2020 2d20 556e 6978  data`..   - Unix
+00001a60: 2073 7973 7465 6d73 3a20 602f 7573 722f   systems: `/usr/
+00001a70: 7368 6172 652f 7465 7373 6572 6163 742d  share/tesseract-
+00001a80: 6f63 722f 352f 7465 7373 6461 7461 600a  ocr/5/tessdata`.
+00001a90: 0a33 2e20 5365 7420 7468 6520 656e 7669  .3. Set the envi
+00001aa0: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00001ab0: 2054 4553 5344 4154 415f 5052 4546 4958   TESSDATA_PREFIX
+00001ac0: 0a0a 2020 202d 2057 696e 646f 7773 3a20  ..   - Windows: 
+00001ad0: 6073 6574 7820 5445 5353 4441 5441 5f50  `setx TESSDATA_P
+00001ae0: 5245 4649 5820 2243 3a2f 5072 6f67 7261  REFIX "C:/Progra
+00001af0: 6d20 4669 6c65 732f 5465 7373 6572 6163  m Files/Tesserac
+00001b00: 742d 4f43 522f 7465 7373 6461 7461 2260  t-OCR/tessdata"`
+00001b10: 0a0a 2020 202d 2055 6e69 7820 7379 7374  ..   - Unix syst
+00001b20: 656d 733a 2060 6465 636c 6172 6520 2d78  ems: `declare -x
+00001b30: 2054 4553 5344 4154 415f 5052 4546 4958   TESSDATA_PREFIX
+00001b40: 3d20 2f75 7372 2f73 6861 7265 2f74 6573  = /usr/share/tes
+00001b50: 7365 7261 6374 2d6f 6372 2f35 2f74 6573  seract-ocr/5/tes
+00001b60: 7364 6174 6160 0a0a 2a2a 4e6f 7465 3a2a  sdata`..**Note:*
+00001b70: 2a20 5f4f 6e20 5769 6e64 6f77 7320 7379  * _On Windows sy
+00001b80: 7374 656d 732c 2074 6869 7320 6d75 7374  stems, this must
+00001b90: 2068 6170 7065 6e20 6f75 7473 6964 6520   happen outside 
+00001ba0: 5079 7468 6f6e 20e2 8093 2062 6566 6f72  Python ... befor
+00001bb0: 6520 7374 6172 7469 6e67 2079 6f75 7220  e starting your 
+00001bc0: 7363 7269 7074 2e20 4a75 7374 206d 616e  script. Just man
+00001bd0: 6970 756c 6174 696e 6720 6f73 2e65 6e76  ipulating os.env
+00001be0: 6972 6f6e 2077 696c 6c20 6e6f 7420 776f  iron will not wo
+00001bf0: 726b 215f 0a0a 2323 2323 2032 2e20 4d4c  rk!_..#### 2. ML
+00001c00: 2054 6162 6c65 2044 6574 6563 7469 6f6e   Table Detection
+00001c10: 2028 4f70 7469 6f6e 616c 290a 0a54 6869   (Optional)..Thi
+00001c20: 7320 7265 706f 7369 746f 7279 2070 726f  s repository pro
+00001c30: 7669 6465 7320 616e 206f 7074 696f 6e61  vides an optiona
+00001c40: 6c20 6665 6174 7572 6520 746f 2070 6172  l feature to par
+00001c50: 7365 2063 6f6e 7465 6e74 2066 726f 6d20  se content from 
+00001c60: 7461 626c 6573 2075 7369 6e67 2061 2076  tables using a v
+00001c70: 6172 6965 7479 206f 6620 6465 6570 206c  ariety of deep l
+00001c80: 6561 726e 696e 6720 6d6f 6465 6c73 2e0a  earning models..
+00001c90: 0a60 6060 636f 6e73 6f6c 650a 7069 7020  .```console.pip 
+00001ca0: 696e 7374 616c 6c20 226f 7065 6e70 6172  install "openpar
+00001cb0: 7365 5b6d 6c5d 220a 6060 600a 0a54 6865  se[ml]".```..The
+00001cc0: 6e20 646f 776e 6c6f 6164 2074 6865 206d  n download the m
+00001cd0: 6f64 656c 2077 6569 6768 7473 2077 6974  odel weights wit
+00001ce0: 680a 0a60 6060 636f 6e73 6f6c 650a 6f70  h..```console.op
+00001cf0: 656e 7061 7273 652d 646f 776e 6c6f 6164  enparse-download
+00001d00: 0a60 6060 0a0a 596f 7520 6361 6e20 7275  .```..You can ru
+00001d10: 6e20 7468 6520 7061 7273 696e 6720 7769  n the parsing wi
+00001d20: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
+00001d30: 2e20 0a0a 6060 6070 7974 686f 6e0a 7061  . ..```python.pa
+00001d40: 7273 6572 203d 206f 7065 6e70 6172 7365  rser = openparse
+00001d50: 2e44 6f63 756d 656e 7450 6172 7365 7228  .DocumentParser(
+00001d60: 0a20 2020 2020 2020 2074 6162 6c65 5f61  .        table_a
+00001d70: 7267 733d 7b0a 2020 2020 2020 2020 2020  rgs={.          
+00001d80: 2020 2270 6172 7369 6e67 5f61 6c67 6f72    "parsing_algor
+00001d90: 6974 686d 223a 2022 756e 6974 6162 6c65  ithm": "unitable
+00001da0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00001db0: 6d69 6e5f 7461 626c 655f 636f 6e66 6964  min_table_confid
+00001dc0: 656e 6365 223a 2030 2e38 2c0a 2020 2020  ence": 0.8,.    
+00001dd0: 2020 2020 7d2c 0a29 0a70 6172 7365 645f      },.).parsed_
+00001de0: 6e6f 6465 7320 3d20 7061 7273 6572 2e70  nodes = parser.p
+00001df0: 6172 7365 2870 6466 5f70 6174 6829 0a60  arse(pdf_path).`
+00001e00: 6060 0a0a 4e6f 7465 2077 6520 6375 7272  ``..Note we curr
+00001e10: 656e 746c 7920 7573 6520 5b74 6162 6c65  ently use [table
+00001e20: 2d74 7261 6e73 666f 726d 6572 735d 2868  -transformers](h
+00001e30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001e40: 6d2f 6d69 6372 6f73 6f66 742f 7461 626c  m/microsoft/tabl
+00001e50: 652d 7472 616e 7366 6f72 6d65 7229 2066  e-transformer) f
+00001e60: 6f72 2061 6c6c 2074 6162 6c65 2064 6574  or all table det
+00001e70: 6563 7469 6f6e 2061 6e64 2077 6520 6669  ection and we fi
+00001e80: 6e64 2069 7473 2070 6572 666f 726d 616e  nd its performan
+00001e90: 6365 2074 6f20 6265 2073 7562 7061 722e  ce to be subpar.
+00001ea0: 2054 6869 7320 6e65 6761 7469 7665 6c79   This negatively
+00001eb0: 2061 6666 6563 7473 2074 6865 2064 6f77   affects the dow
+00001ec0: 6e73 7472 6561 6d20 7265 7375 6c74 7320  nstream results 
+00001ed0: 6f66 2075 6e69 7461 626c 652e 2049 6620  of unitable. If 
+00001ee0: 796f 7527 7265 2061 7761 7265 206f 6620  you're aware of 
+00001ef0: 6120 6265 7474 6572 206d 6f64 656c 2070  a better model p
+00001f00: 6c65 6173 6520 6f70 656e 2061 6e20 4973  lease open an Is
+00001f10: 7375 6520 2d20 7468 6520 756e 6974 6162  sue - the unitab
+00001f20: 6c65 2074 6561 6d20 6d65 6e74 696f 6e65  le team mentione
+00001f30: 6420 7468 6579 206d 6967 6874 2061 6464  d they might add
+00001f40: 2074 6869 7320 736f 6f6e 2074 6f6f 2e0a   this soon too..
+00001f50: 0a23 2320 436f 6f6b 626f 6f6b 730a 0a68  .## Cookbooks..h
+00001f60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001f70: 6d2f 4669 6c69 6d6f 612f 6f70 656e 2d70  m/Filimoa/open-p
+00001f80: 6172 7365 2f74 7265 652f 6d61 696e 2f73  arse/tree/main/s
+00001f90: 7263 2f63 6f6f 6b62 6f6f 6b73 0a0a 2323  rc/cookbooks..##
+00001fa0: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
+00001fb0: 6874 7470 733a 2f2f 6669 6c69 6d6f 612e  https://filimoa.
+00001fc0: 6769 7468 7562 2e69 6f2f 6f70 656e 2d70  github.io/open-p
+00001fd0: 6172 7365 2f0a 0a23 2320 5370 6f6e 736f  arse/..## Sponso
+00001fe0: 7273 0a0a 3c21 2d2d 2073 706f 6e73 6f72  rs..<!-- sponsor
+00001ff0: 7320 2d2d 3e0a 0a3c 6120 6872 6566 3d22  s -->..<a href="
+00002000: 6874 7470 733a 2f2f 7777 772e 6461 7461  https://www.data
+00002010: 2e74 6872 6565 7369 676d 612e 6169 2f66  .threesigma.ai/f
+00002020: 696c 696e 6773 2d61 6922 2074 6172 6765  ilings-ai" targe
+00002030: 743d 225f 626c 616e 6b22 2074 6974 6c65  t="_blank" title
+00002040: 3d22 5468 7265 6520 5369 676d 613a 2041  ="Three Sigma: A
+00002050: 4920 666f 7220 696e 7375 7261 6e63 6520  I for insurance 
+00002060: 6669 6c69 6e67 732e 223e 3c69 6d67 2073  filings."><img s
+00002070: 7263 3d22 6874 7470 733a 2f2f 7365 7267  rc="https://serg
+00002080: 6579 2d66 696c 696d 6f6e 6f76 2e6e 7963  ey-filimonov.nyc
+00002090: 332e 6469 6769 7461 6c6f 6365 616e 7370  3.digitaloceansp
+000020a0: 6163 6573 2e63 6f6d 2f6f 7065 6e2d 7061  aces.com/open-pa
+000020b0: 7273 652f 6d61 726b 6574 696e 672f 7468  rse/marketing/th
+000020c0: 7265 652d 7369 676d 612d 7769 6465 2e70  ree-sigma-wide.p
+000020d0: 6e67 2220 7769 6474 683d 2232 3530 223e  ng" width="250">
+000020e0: 3c2f 613e 0a0a 3c21 2d2d 202f 7370 6f6e  </a>..<!-- /spon
+000020f0: 736f 7273 202d 2d3e 0a0a 446f 6573 2079  sors -->..Does y
+00002100: 6f75 7220 7573 6520 6361 7365 206e 6565  our use case nee
+00002110: 6420 736f 6d65 7468 696e 6720 7370 6563  d something spec
+00002120: 6961 6c3f 2052 6561 6368 205b 6f75 745d  ial? Reach [out]
+00002130: 2868 7474 7073 3a2f 2f77 7777 2e6c 696e  (https://www.lin
+00002140: 6b65 6469 6e2e 636f 6d2f 696e 2f73 6572  kedin.com/in/ser
+00002150: 6765 792d 6f73 752f 292e 0a              gey-osu/)..
```

### Comparing `openparse-0.5.1/README.md` & `openparse-0.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -96,15 +96,16 @@
 **📓 Sample notebook** <a href="https://github.com/Filimoa/open-parse/blob/main/src/cookbooks/semantic_processing.ipynb" class="external-link" target="_blank">here</a>
 
 #### Serializing Results
 Uses pydantic under the hood so you can serialize results with 
 
 ```python
 parsed_content.dict()
-# or
+
+# or to convert to a valid json dict
 parsed_content.json()
 ```
 
 ## Requirements
 
 Python 3.8+
 
@@ -181,7 +182,17 @@
 ## Cookbooks
 
 https://github.com/Filimoa/open-parse/tree/main/src/cookbooks
 
 ## Documentation
 
 https://filimoa.github.io/open-parse/
+
+## Sponsors
+
+<!-- sponsors -->
+
+<a href="https://www.data.threesigma.ai/filings-ai" target="_blank" title="Three Sigma: AI for insurance filings."><img src="https://sergey-filimonov.nyc3.digitaloceanspaces.com/open-parse/marketing/three-sigma-wide.png" width="250"></a>
+
+<!-- /sponsors -->
+
+Does your use case need something special? Reach [out](https://www.linkedin.com/in/sergey-osu/).
```

#### html2text {}

```diff
@@ -48,39 +48,42 @@
 we can then cluster them together based on their similarity. ```python from
 openparse import processing, DocumentParser semantic_pipeline =
 processing.SemanticIngestionPipeline( openai_api_key=OPEN_AI_KEY, model="text-
 embedding-3-large", min_tokens=64, max_tokens=1024, ) parser = DocumentParser
 ( processing_pipeline=semantic_pipeline, ) parsed_content = parser.parse
 (basic_doc_path) ``` **ð Sample notebook** _h_e_r_e #### Serializing Results
 Uses pydantic under the hood so you can serialize results with ```python
-parsed_content.dict() # or parsed_content.json() ``` ## Requirements Python
-3.8+ **Dealing with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully open source. **Extracting
-Tables:** - _P_y_M_u_P_D_F has some table detection functionality. Please see their
-_l_i_c_e_n_s_e. - _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning approach. - _u_n_i_t_a_b_l_e is another
-transformers based approach with **state-of-the-art** performance. ##
-Installation #### 1. Core Library ```console pip install openparse ```
-**Enabling OCR Support**: PyMuPDF will already contain all the logic to support
-OCR functions. But it additionally does need Tesseractâs language support
-data, so installation of Tesseract-OCR is still required. The language support
-folder location must be communicated either via storing it in the environment
-variable "TESSDATA_PREFIX", or as a parameter in the applicable functions. So
-for a working OCR functionality, make sure to complete this checklist: 1.
-Install Tesseract. 2. Locate Tesseractâs language support folder. Typically
-you will find it here: - Windows: `C:/Program Files/Tesseract-OCR/tessdata` -
-Unix systems: `/usr/share/tesseract-ocr/5/tessdata` 3. Set the environment
-variable TESSDATA_PREFIX - Windows: `setx TESSDATA_PREFIX "C:/Program Files/
-Tesseract-OCR/tessdata"` - Unix systems: `declare -x TESSDATA_PREFIX= /usr/
-share/tesseract-ocr/5/tessdata` **Note:** _On Windows systems, this must happen
-outside Python â before starting your script. Just manipulating os.environ
-will not work!_ #### 2. ML Table Detection (Optional) This repository provides
-an optional feature to parse content from tables using a variety of deep
-learning models. ```console pip install "openparse[ml]" ``` Then download the
-model weights with ```console openparse-download ``` You can run the parsing
-with the following. ```python parser = openparse.DocumentParser( table_args=
-{ "parsing_algorithm": "unitable", "min_table_confidence": 0.8, }, )
-parsed_nodes = parser.parse(pdf_path) ``` Note we currently use [table-
-transformers](https://github.com/microsoft/table-transformer) for all table
-detection and we find its performance to be subpar. This negatively affects the
-downstream results of unitable. If you're aware of a better model please open
-an Issue - the unitable team mentioned they might add this soon too. ##
-Cookbooks https://github.com/Filimoa/open-parse/tree/main/src/cookbooks ##
-Documentation https://filimoa.github.io/open-parse/
+parsed_content.dict() # or to convert to a valid json dict parsed_content.json
+() ``` ## Requirements Python 3.8+ **Dealing with PDF's:** - _p_d_f_m_i_n_e_r_._s_i_x Fully
+open source. **Extracting Tables:** - _P_y_M_u_P_D_F has some table detection
+functionality. Please see their _l_i_c_e_n_s_e. - _T_a_b_l_e_ _T_r_a_n_s_f_o_r_m_e_r is a deep learning
+approach. - _u_n_i_t_a_b_l_e is another transformers based approach with **state-of-
+the-art** performance. ## Installation #### 1. Core Library ```console pip
+install openparse ``` **Enabling OCR Support**: PyMuPDF will already contain
+all the logic to support OCR functions. But it additionally does need
+Tesseractâs language support data, so installation of Tesseract-OCR is still
+required. The language support folder location must be communicated either via
+storing it in the environment variable "TESSDATA_PREFIX", or as a parameter in
+the applicable functions. So for a working OCR functionality, make sure to
+complete this checklist: 1. Install Tesseract. 2. Locate Tesseractâs language
+support folder. Typically you will find it here: - Windows: `C:/Program Files/
+Tesseract-OCR/tessdata` - Unix systems: `/usr/share/tesseract-ocr/5/tessdata`
+3. Set the environment variable TESSDATA_PREFIX - Windows: `setx
+TESSDATA_PREFIX "C:/Program Files/Tesseract-OCR/tessdata"` - Unix systems:
+`declare -x TESSDATA_PREFIX= /usr/share/tesseract-ocr/5/tessdata` **Note:** _On
+Windows systems, this must happen outside Python â before starting your
+script. Just manipulating os.environ will not work!_ #### 2. ML Table Detection
+(Optional) This repository provides an optional feature to parse content from
+tables using a variety of deep learning models. ```console pip install
+"openparse[ml]" ``` Then download the model weights with ```console openparse-
+download ``` You can run the parsing with the following. ```python parser =
+openparse.DocumentParser( table_args={ "parsing_algorithm": "unitable",
+"min_table_confidence": 0.8, }, ) parsed_nodes = parser.parse(pdf_path) ```
+Note we currently use [table-transformers](https://github.com/microsoft/table-
+transformer) for all table detection and we find its performance to be subpar.
+This negatively affects the downstream results of unitable. If you're aware of
+a better model please open an Issue - the unitable team mentioned they might
+add this soon too. ## Cookbooks https://github.com/Filimoa/open-parse/tree/
+main/src/cookbooks ## Documentation https://filimoa.github.io/open-parse/ ##
+Sponsors _[_h_t_t_p_s_:_/_/_s_e_r_g_e_y_-_f_i_l_i_m_o_n_o_v_._n_y_c_3_._d_i_g_i_t_a_l_o_c_e_a_n_s_p_a_c_e_s_._c_o_m_/_o_p_e_n_-_p_a_r_s_e_/
+_m_a_r_k_e_t_i_n_g_/_t_h_r_e_e_-_s_i_g_m_a_-_w_i_d_e_._p_n_g_]Does your use case need something special? Reach
+[out](https://www.linkedin.com/in/sergey-osu/).
```

### Comparing `openparse-0.5.1/src/evals/run_evals.py` & `openparse-0.5.2/src/evals/run_evals.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/cli.py` & `openparse-0.5.2/src/openparse/cli.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/doc_parser.py` & `openparse-0.5.2/src/openparse/doc_parser.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/pdf.py` & `openparse-0.5.2/src/openparse/pdf.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/processing/__init__.py` & `openparse-0.5.2/src/openparse/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/processing/basic_transforms.py` & `openparse-0.5.2/src/openparse/processing/basic_transforms.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/processing/ingest.py` & `openparse-0.5.2/src/openparse/processing/ingest.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/processing/semantic_transforms.py` & `openparse-0.5.2/src/openparse/processing/semantic_transforms.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/schemas.py` & `openparse-0.5.2/src/openparse/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/parse.py` & `openparse-0.5.2/src/openparse/tables/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/pymupdf/parse.py` & `openparse-0.5.2/src/openparse/tables/pymupdf/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/table_transformers/geometry.py` & `openparse-0.5.2/src/openparse/tables/table_transformers/geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/table_transformers/ml.py` & `openparse-0.5.2/src/openparse/tables/table_transformers/ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from PIL import Image  # type: ignore
 from torchvision import transforms  # type: ignore
 from transformers import (
     AutoModelForObjectDetection,  # type: ignore
     TableTransformerForObjectDetection,  # type: ignore
 )  # type: ignore
 
+from openparse.config import config
 from ..schemas import (
     BBox,
     Size,
 )
 from ..utils import (
     display_cells_on_img,
     crop_img_with_padding,
@@ -30,20 +31,15 @@
     _TableDataCell,
     _TableHeader,
     _TableHeaderCell,
     _TableRow,
 )
 
 t0 = time.time()
-
-cuda_available = torch.cuda.is_available()
-user_preferred_device = "cuda"
-device = torch.device(
-    "cuda" if cuda_available and user_preferred_device != "cpu" else "cpu"
-)
+device = config.get_device()
 
 
 class MaxResize:
     def __init__(self, max_size=800):
         self.max_size = max_size
 
     def __call__(self, image):
@@ -182,15 +178,15 @@
         )
     return tables
 
 
 def find_table_bboxes(
     image: Image.Image, min_table_confidence: float
 ) -> List[_TableModelOutput]:
-    pixel_values = detection_transform(image).unsqueeze(0).to("cpu")
+    pixel_values = detection_transform(image).unsqueeze(0).to(device)
     with torch.no_grad():
         outputs = detection_model(pixel_values)
 
     detection_id2label = {
         **detection_model.config.id2label,
         len(detection_model.config.id2label): "no object",
     }
@@ -330,15 +326,15 @@
     OFFSET = 0.05
     table_img = crop_img_with_padding(page_img, table_bbox, padding_pct=OFFSET)
     structure_id2label = {
         **structure_model.config.id2label,
         len(structure_model.config.id2label): "no object",
     }
 
-    pixel_values_st = structure_transform(table_img).unsqueeze(0).to("cpu")
+    pixel_values_st = structure_transform(table_img).unsqueeze(0).to(device)
     with torch.no_grad():
         outputs_st = structure_model(pixel_values_st)
 
     cells = _cell_outputs_to_objs(outputs_st, table_img.size, structure_id2label)
 
     for cell in cells:
         cell.bbox = convert_croppped_cords_to_full_img_cords(
```

### Comparing `openparse-0.5.1/src/openparse/tables/table_transformers/schemas.py` & `openparse-0.5.2/src/openparse/tables/table_transformers/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/unitable/config.py` & `openparse-0.5.2/src/openparse/tables/unitable/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import torch
 from pydantic import BaseModel
 from pathlib import Path
 import sys
 from openparse import consts
 
-device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 root = Path(consts.__file__).parent
 
 
 class StructureModelConfig(BaseModel):
     weights_path: Path = root / "weights/unitable/unitable_large_structure.pt"
     vocab_path: Path = root / "weights/unitable/vocab_html.json"
     max_seq_len: int = 784
```

### Comparing `openparse-0.5.1/src/openparse/tables/unitable/core.py` & `openparse-0.5.2/src/openparse/tables/unitable/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import re
 
 from PIL import Image  # type: ignore
 import torch  # type: ignore
 from torchvision import transforms  # type: ignore
 from torch import nn, Tensor  # type: ignore
 
-from .config import device
 from .tokens import VALID_HTML_TOKEN, VALID_BBOX_TOKEN, INVALID_CELL_TOKEN
 from .utils import (
     subsequent_mask,
     pred_token_within_range,
     greedy_sampling,
     html_str_to_token_list,
     bbox_str_to_token_list,
@@ -23,18 +22,21 @@
     structure_model,
     bbox_vocab,
     bbox_model,
     cell_vocab,
     cell_model,
     EncoderDecoder,
 )
+from openparse.config import config
 
 Size = Tuple[int, int]
 BBox = Tuple[int, int, int, int]
 
+device = config.get_device()
+
 
 def _image_to_tensor(image: Image, size: Size) -> Tensor:
     T = transforms.Compose(
         [
             transforms.Resize(size),
             transforms.ToTensor(),
             transforms.Normalize(
```

### Comparing `openparse-0.5.1/src/openparse/tables/unitable/schemas.py` & `openparse-0.5.2/src/openparse/tables/unitable/schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/unitable/tabular_transformer.py` & `openparse-0.5.2/src/openparse/tables/unitable/tabular_transformer.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/unitable/tokens.py` & `openparse-0.5.2/src/openparse/tables/unitable/tokens.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/unitable/unitable_model.py` & `openparse-0.5.2/src/openparse/tables/unitable/unitable_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 import torch  # type: ignore
 import tokenizers as tk  # type: ignore
 import warnings
 
 from torch import nn
 from functools import partial
 
-from .config import device, config
+from .config import config
 from .tabular_transformer import (
     EncoderDecoder,
     ImgLinearBackbone,
     Encoder,
     Decoder,
 )
+from openparse.config import config as global_config
 
+device = global_config.get_device()
 warnings.filterwarnings("ignore")
 
 
 def load_vocab_and_model(
     vocab_path: Union[str, Path],
     max_seq_len: int,
     model_weights: Union[str, Path],
```

### Comparing `openparse-0.5.1/src/openparse/tables/unitable/utils.py` & `openparse-0.5.2/src/openparse/tables/unitable/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/tables/utils.py` & `openparse-0.5.2/src/openparse/tables/utils.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/text/parse.py` & `openparse-0.5.2/src/openparse/text/parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/text/pdfminer/core.py` & `openparse-0.5.2/src/openparse/text/pdfminer/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/text/pymupdf/core.py` & `openparse-0.5.2/src/openparse/text/pymupdf/core.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse/types.py` & `openparse-0.5.2/src/openparse/types.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/openparse.egg-info/PKG-INFO` & `openparse-0.5.2/src/openparse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,498 +1,534 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6f70 656e  : 2.1.Name: open
 00000020: 7061 7273 650a 5665 7273 696f 6e3a 2030  parse.Version: 0
-00000030: 2e35 2e31 0a53 756d 6d61 7279 3a20 5374  .5.1.Summary: St
+00000030: 2e35 2e32 0a53 756d 6d61 7279 3a20 5374  .5.2.Summary: St
 00000040: 7265 616d 6c69 6e65 7320 7468 6520 7072  reamlines the pr
 00000050: 6f63 6573 7320 6f66 2070 7265 7061 7269  ocess of prepari
 00000060: 6e67 2064 6f63 756d 656e 7473 2066 6f72  ng documents for
-00000070: 204c 4c4d 2773 2e0a 486f 6d65 2d70 6167   LLM's..Home-pag
-00000080: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-00000090: 622e 636f 6d2f 4669 6c69 6d6f 612f 6f70  b.com/Filimoa/op
-000000a0: 656e 2d70 6172 7365 2f0a 4175 7468 6f72  en-parse/.Author
-000000b0: 3a20 5365 7267 6579 2046 696c 696d 6f6e  : Sergey Filimon
-000000c0: 6f76 0a41 7574 686f 722d 656d 6169 6c3a  ov.Author-email:
-000000d0: 2068 656c 6c6f 4073 6572 6765 792e 6679   hello@sergey.fy
-000000e0: 690a 4465 7363 7269 7074 696f 6e2d 436f  i.Description-Co
-000000f0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000100: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
-00000110: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
-00000120: 5265 7175 6972 6573 2d44 6973 743a 2050  Requires-Dist: P
-00000130: 794d 7550 4446 3e3d 312e 3233 2e32 0a52  yMuPDF>=1.23.2.R
-00000140: 6571 7569 7265 732d 4469 7374 3a20 7069  equires-Dist: pi
-00000150: 6c6c 6f77 3e3d 382e 330a 5265 7175 6972  llow>=8.3.Requir
-00000160: 6573 2d44 6973 743a 2070 7964 616e 7469  es-Dist: pydanti
-00000170: 633e 3d32 2e30 0a52 6571 7569 7265 732d  c>=2.0.Requires-
-00000180: 4469 7374 3a20 7079 7064 663e 3d34 2e30  Dist: pypdf>=4.0
-00000190: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
-000001a0: 3a20 7064 666d 696e 6572 2e73 6978 3e3d  : pdfminer.six>=
-000001b0: 3230 3230 3034 3031 0a52 6571 7569 7265  20200401.Require
-000001c0: 732d 4469 7374 3a20 7469 6b74 6f6b 656e  s-Dist: tiktoken
-000001d0: 3e3d 302e 330a 5265 7175 6972 6573 2d44  >=0.3.Requires-D
-000001e0: 6973 743a 206f 7065 6e61 693e 3d31 2e30  ist: openai>=1.0
-000001f0: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
-00000200: 3a20 6e75 6d70 790a 5072 6f76 6964 6573  : numpy.Provides
-00000210: 2d45 7874 7261 3a20 6d6c 0a52 6571 7569  -Extra: ml.Requi
-00000220: 7265 732d 4469 7374 3a20 746f 7263 683b  res-Dist: torch;
-00000230: 2065 7874 7261 203d 3d20 226d 6c22 0a52   extra == "ml".R
-00000240: 6571 7569 7265 732d 4469 7374 3a20 746f  equires-Dist: to
-00000250: 7263 6876 6973 696f 6e3b 2065 7874 7261  rchvision; extra
-00000260: 203d 3d20 226d 6c22 0a52 6571 7569 7265   == "ml".Require
-00000270: 732d 4469 7374 3a20 7472 616e 7366 6f72  s-Dist: transfor
-00000280: 6d65 7273 3b20 6578 7472 6120 3d3d 2022  mers; extra == "
-00000290: 6d6c 220a 5265 7175 6972 6573 2d44 6973  ml".Requires-Dis
-000002a0: 743a 2074 6f6b 656e 697a 6572 733b 2065  t: tokenizers; e
-000002b0: 7874 7261 203d 3d20 226d 6c22 0a0a 3c70  xtra == "ml"..<p
-000002c0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000002d0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-000002e0: 7474 7073 3a2f 2f73 6572 6765 792d 6669  ttps://sergey-fi
-000002f0: 6c69 6d6f 6e6f 762e 6e79 6333 2e64 6967  limonov.nyc3.dig
-00000300: 6974 616c 6f63 6561 6e73 7061 6365 732e  italoceanspaces.
-00000310: 636f 6d2f 6f70 656e 2d70 6172 7365 2f6f  com/open-parse/o
-00000320: 7065 6e2d 7061 7273 652d 7769 7468 2d74  pen-parse-with-t
-00000330: 6578 742d 7470 2d6c 6f67 6f2e 7765 6270  ext-tp-logo.webp
-00000340: 2220 7769 6474 683d 2233 3530 2220 2f3e  " width="350" />
-00000350: 0a3c 2f70 3e0a 3c62 722f 3e0a 0a2a 2a45  .</p>.<br/>..**E
-00000360: 6173 696c 7920 6368 756e 6b20 636f 6d70  asily chunk comp
-00000370: 6c65 7820 646f 6375 6d65 6e74 7320 7468  lex documents th
-00000380: 6520 7361 6d65 2077 6179 2061 2068 756d  e same way a hum
-00000390: 616e 2077 6f75 6c64 2e2a 2a20 200a 0a43  an would.**  ..C
-000003a0: 6875 6e6b 696e 6720 646f 6375 6d65 6e74  hunking document
-000003b0: 7320 6973 2061 2063 6861 6c6c 656e 6769  s is a challengi
-000003c0: 6e67 2074 6173 6b20 7468 6174 2075 6e64  ng task that und
-000003d0: 6572 7069 6e73 2061 6e79 2052 4147 2073  erpins any RAG s
-000003e0: 7973 7465 6d2e 2020 4869 6768 2071 7561  ystem.  High qua
-000003f0: 6c69 7479 2072 6573 756c 7473 2061 7265  lity results are
-00000400: 2063 7269 7469 6361 6c20 746f 2061 2073   critical to a s
-00000410: 7563 6573 7366 756c 2041 4920 6170 706c  ucessful AI appl
-00000420: 6963 6174 696f 6e2c 2079 6574 206d 6f73  ication, yet mos
-00000430: 7420 6f70 656e 2d73 6f75 7263 6520 6c69  t open-source li
-00000440: 6272 6172 6965 7320 6172 6520 6c69 6d69  braries are limi
-00000450: 7465 6420 696e 2074 6865 6972 2061 6269  ted in their abi
-00000460: 6c69 7479 2074 6f20 6861 6e64 6c65 2063  lity to handle c
-00000470: 6f6d 706c 6578 2064 6f63 756d 656e 7473  omplex documents
-00000480: 2e20 200a 0a4f 7065 6e20 5061 7273 6520  .  ..Open Parse 
-00000490: 6973 2064 6573 6967 6e65 6420 746f 2066  is designed to f
-000004a0: 696c 6c20 7468 6973 2067 6170 2062 7920  ill this gap by 
-000004b0: 7072 6f76 6964 696e 6720 6120 666c 6578  providing a flex
-000004c0: 6962 6c65 2c20 6561 7379 2d74 6f2d 7573  ible, easy-to-us
-000004d0: 6520 6c69 6272 6172 7920 6361 7061 626c  e library capabl
-000004e0: 6520 6f66 2076 6973 7561 6c6c 7920 6469  e of visually di
-000004f0: 7363 6572 6e69 6e67 2064 6f63 756d 656e  scerning documen
-00000500: 7420 6c61 796f 7574 7320 616e 6420 6368  t layouts and ch
-00000510: 756e 6b69 6e67 2074 6865 6d20 6566 6665  unking them effe
-00000520: 6374 6976 656c 792e 0a0a 3c64 6574 6169  ctively...<detai
-00000530: 6c73 3e0a 2020 3c73 756d 6d61 7279 3e3c  ls>.  <summary><
-00000540: 623e 486f 7720 6973 2074 6869 7320 6469  b>How is this di
-00000550: 6666 6572 656e 7420 6672 6f6d 206f 7468  fferent from oth
-00000560: 6572 206c 6179 6f75 7420 7061 7273 6572  er layout parser
-00000570: 733f 3c2f 623e 3c2f 7375 6d6d 6172 793e  s?</b></summary>
-00000580: 0a0a 2020 2323 2323 20e2 9c82 efb8 8f20  ..  #### ...... 
-00000590: 5465 7874 2053 706c 6974 7469 6e67 0a20  Text Splitting. 
-000005a0: 2054 6578 7420 7370 6c69 7474 696e 6720   Text splitting 
-000005b0: 636f 6e76 6572 7473 2061 2066 696c 6520  converts a file 
-000005c0: 746f 2072 6177 2074 6578 7420 616e 6420  to raw text and 
-000005d0: 5b73 6c69 6365 7320 6974 2075 705d 2868  [slices it up](h
-000005e0: 7474 7073 3a2f 2f64 6f63 732e 6c6c 616d  ttps://docs.llam
-000005f0: 6169 6e64 6578 2e61 692f 656e 2f73 7461  aindex.ai/en/sta
-00000600: 626c 652f 6170 695f 7265 6665 7265 6e63  ble/api_referenc
-00000610: 652f 6e6f 6465 5f70 6172 7365 7273 2f74  e/node_parsers/t
-00000620: 6f6b 656e 5f74 6578 745f 7370 6c69 7474  oken_text_splitt
-00000630: 6572 2f29 2e0a 2020 0a20 202d 2059 6f75  er/)..  .  - You
-00000640: 206c 6f73 6520 7468 6520 6162 696c 6974   lose the abilit
-00000650: 7920 746f 2065 6173 696c 7920 6f76 6572  y to easily over
-00000660: 6c61 7920 7468 6520 6368 756e 6b20 6f6e  lay the chunk on
-00000670: 2074 6865 206f 7269 6769 6e61 6c20 7064   the original pd
-00000680: 660a 2020 2d20 596f 7520 6967 6e6f 7265  f.  - You ignore
-00000690: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-000006a0: 7365 6d61 6e74 6963 2073 7472 7563 7475  semantic structu
-000006b0: 7265 206f 6620 7468 6520 6669 6c65 202d  re of the file -
-000006c0: 2068 6561 6469 6e67 732c 2073 6563 7469   headings, secti
-000006d0: 6f6e 732c 2062 756c 6c65 7473 2072 6570  ons, bullets rep
-000006e0: 7265 7365 6e74 2076 616c 7561 626c 6520  resent valuable 
-000006f0: 696e 666f 726d 6174 696f 6e2e 0a20 202d  information..  -
-00000700: 204e 6f20 7375 7070 6f72 7420 666f 7220   No support for 
-00000710: 7461 626c 6573 2c20 696d 6167 6573 206f  tables, images o
-00000720: 7220 6d61 726b 646f 776e 2e0a 2020 0a20  r markdown..  . 
-00000730: 2023 2323 2320 f09f a496 204d 4c20 4c61   #### .... ML La
-00000740: 796f 7574 2050 6172 7365 7273 0a20 2054  yout Parsers.  T
-00000750: 6865 7265 2773 2073 6f6d 6520 6f66 2066  here's some of f
-00000760: 616e 7461 7374 6963 206c 6962 7261 7269  antastic librari
-00000770: 6573 206c 696b 6520 5b6c 6179 6f75 742d  es like [layout-
-00000780: 7061 7273 6572 5d28 6874 7470 733a 2f2f  parser](https://
-00000790: 6769 7468 7562 2e63 6f6d 2f4c 6179 6f75  github.com/Layou
-000007a0: 742d 5061 7273 6572 2f6c 6179 6f75 742d  t-Parser/layout-
-000007b0: 7061 7273 6572 292e 200a 2020 2d20 5768  parser). .  - Wh
-000007c0: 696c 6520 7468 6579 2063 616e 2069 6465  ile they can ide
-000007d0: 6e74 6966 7920 7661 7269 6f75 7320 656c  ntify various el
-000007e0: 656d 656e 7473 206c 696b 6520 7465 7874  ements like text
-000007f0: 2062 6c6f 636b 732c 2069 6d61 6765 732c   blocks, images,
-00000800: 2061 6e64 2074 6162 6c65 732c 2062 7574   and tables, but
-00000810: 2074 6865 7920 6172 6520 6e6f 7420 6275   they are not bu
-00000820: 696c 7420 746f 2067 726f 7570 2072 656c  ilt to group rel
-00000830: 6174 6564 2063 6f6e 7465 6e74 2065 6666  ated content eff
-00000840: 6563 7469 7665 6c79 2e0a 2020 2d20 5468  ectively..  - Th
-00000850: 6579 2073 7472 6963 746c 7920 666f 6375  ey strictly focu
-00000860: 7320 6f6e 206c 6179 6f75 7420 7061 7273  s on layout pars
-00000870: 696e 6720 2d20 796f 7520 7769 6c6c 206e  ing - you will n
-00000880: 6565 6420 746f 2061 6464 2061 6e6f 7468  eed to add anoth
-00000890: 6572 206d 6f64 656c 2074 6f20 6578 7472  er model to extr
-000008a0: 6163 7420 6d61 726b 646f 776e 2066 726f  act markdown fro
-000008b0: 6d20 7468 6520 696d 6167 6573 2c20 7061  m the images, pa
-000008c0: 7273 6520 7461 626c 6573 2c20 6772 6f75  rse tables, grou
-000008d0: 7020 6e6f 6465 732c 2065 7463 2e0a 2020  p nodes, etc..  
-000008e0: 2d20 5765 2776 6520 666f 756e 6420 7065  - We've found pe
-000008f0: 7266 6f72 6d61 6e63 6520 746f 2062 6520  rformance to be 
-00000900: 7375 622d 6f70 7469 6d61 6c20 6f6e 206d  sub-optimal on m
-00000910: 616e 7920 646f 6375 6d65 6e74 7320 7768  any documents wh
-00000920: 696c 6520 616c 736f 2062 6569 6e67 2063  ile also being c
-00000930: 6f6d 7075 7461 7469 6f6e 616c 6c79 2068  omputationally h
-00000940: 6561 7679 2e0a 0a20 2023 2323 2320 f09f  eavy...  #### ..
-00000950: 92bc 2043 6f6d 6d65 7263 6961 6c20 536f  .. Commercial So
-00000960: 6c75 7469 6f6e 730a 0a20 202d 2054 7970  lutions..  - Typ
-00000970: 6963 616c 6c79 2070 7269 6365 6420 6174  ically priced at
-00000980: 20e2 8988 2024 3130 202f 2031 6b20 7061   ... $10 / 1k pa
-00000990: 6765 732e 2053 6565 205b 6865 7265 5d28  ges. See [here](
-000009a0: 6874 7470 733a 2f2f 636c 6f75 642e 676f  https://cloud.go
-000009b0: 6f67 6c65 2e63 6f6d 2f64 6f63 756d 656e  ogle.com/documen
-000009c0: 742d 6169 292c 205b 6865 7265 5d28 6874  t-ai), [here](ht
-000009d0: 7470 733a 2f2f 6177 732e 616d 617a 6f6e  tps://aws.amazon
-000009e0: 2e63 6f6d 2f74 6578 7472 6163 742f 2920  .com/textract/) 
-000009f0: 616e 6420 5b68 6572 655d 2868 7474 7073  and [here](https
-00000a00: 3a2f 2f77 7777 2e72 6564 7563 746f 2e61  ://www.reducto.a
-00000a10: 692f 292e 0a20 202d 2052 6571 7569 7265  i/)..  - Require
-00000a20: 7320 7368 6172 696e 6720 796f 7572 2064  s sharing your d
-00000a30: 6174 6120 7769 7468 2061 2076 656e 646f  ata with a vendo
-00000a40: 720a 0a3c 2f64 6574 6169 6c73 3e0a 0a23  r..</details>..#
-00000a50: 2320 4869 6768 6c69 6768 7473 0a0a 2d20  # Highlights..- 
-00000a60: 2a2a f09f 948d 2056 6973 7561 6c6c 792d  **.... Visually-
-00000a70: 4472 6976 656e 3a2a 2a20 4f70 656e 2d50  Driven:** Open-P
-00000a80: 6172 7365 2076 6973 7561 6c6c 7920 616e  arse visually an
-00000a90: 616c 797a 6573 2064 6f63 756d 656e 7473  alyzes documents
-00000aa0: 2066 6f72 2073 7570 6572 696f 7220 4c4c   for superior LL
-00000ab0: 4d20 696e 7075 742c 2067 6f69 6e67 2062  M input, going b
-00000ac0: 6579 6f6e 6420 6e61 6976 6520 7465 7874  eyond naive text
-00000ad0: 2073 706c 6974 7469 6e67 2e0a 2d20 2a2a   splitting..- **
-00000ae0: e29c 8def b88f 204d 6172 6b64 6f77 6e20  ...... Markdown 
-00000af0: 5375 7070 6f72 743a 2a2a 2042 6173 6963  Support:** Basic
-00000b00: 206d 6172 6b64 6f77 6e20 7375 7070 6f72   markdown suppor
-00000b10: 7420 666f 7220 7061 7273 696e 6720 6865  t for parsing he
-00000b20: 6164 696e 6773 2c20 626f 6c64 2061 6e64  adings, bold and
-00000b30: 2069 7461 6c69 6373 2e0a 2d20 2a2a f09f   italics..- **..
-00000b40: 938a 2048 6967 682d 5072 6563 6973 696f  .. High-Precisio
-00000b50: 6e20 5461 626c 6520 5375 7070 6f72 743a  n Table Support:
-00000b60: 2a2a 2045 7874 7261 6374 2074 6162 6c65  ** Extract table
-00000b70: 7320 696e 746f 2063 6c65 616e 204d 6172  s into clean Mar
-00000b80: 6b64 6f77 6e20 666f 726d 6174 7320 7769  kdown formats wi
-00000b90: 7468 2061 6363 7572 6163 7920 7468 6174  th accuracy that
-00000ba0: 2073 7572 7061 7373 6573 2074 7261 6469   surpasses tradi
-00000bb0: 7469 6f6e 616c 2074 6f6f 6c73 2e0a 2020  tional tools..  
-00000bc0: 2020 3c64 6574 6169 6c73 3e0a 2020 3c73    <details>.  <s
-00000bd0: 756d 6d61 7279 3e3c 693e 4578 616d 706c  ummary><i>Exampl
-00000be0: 6573 3c2f 693e 3c2f 7375 6d6d 6172 793e  es</i></summary>
-00000bf0: 0a20 2054 6865 2066 6f6c 6c6f 7769 6e67  .  The following
-00000c00: 2065 7861 6d70 6c65 7320 7765 7265 2070   examples were p
-00000c10: 6172 7365 6420 7769 7468 2075 6e69 7461  arsed with unita
-00000c20: 626c 652e 0a20 2020 203c 6272 2f3e 0a20  ble..    <br/>. 
-00000c30: 2020 203c 7020 616c 6967 6e3d 2263 656e     <p align="cen
-00000c40: 7465 7222 3e0a 2020 2020 2020 2020 3c62  ter">.        <b
-00000c50: 722f 3e0a 2020 2020 2020 2020 3c69 6d67  r/>.        <img
-00000c60: 2073 7263 3d22 6874 7470 733a 2f2f 7365   src="https://se
-00000c70: 7267 6579 2d66 696c 696d 6f6e 6f76 2e6e  rgey-filimonov.n
-00000c80: 7963 332e 6469 6769 7461 6c6f 6365 616e  yc3.digitalocean
-00000c90: 7370 6163 6573 2e63 6f6d 2f6f 7065 6e2d  spaces.com/open-
-00000ca0: 7061 7273 652f 756e 6974 6162 6c65 2d70  parse/unitable-p
-00000cb0: 6172 7369 6e67 2d73 616d 706c 652e 7765  arsing-sample.we
-00000cc0: 6270 2220 7769 6474 683d 2236 3530 222f  bp" width="650"/
-00000cd0: 3e0a 2020 2020 3c2f 703e 0a20 2020 2020  >.    </p>.     
-00000ce0: 2020 2020 3c62 722f 3e0a 2020 2020 3c2f      <br/>.    </
-00000cf0: 6465 7461 696c 733e 0a0a 2d20 2a2a f09f  details>..- **..
-00000d00: 9ba0 efb8 8f20 4578 7465 6e73 6962 6c65  ..... Extensible
-00000d10: 3a2a 2a20 4561 7369 6c79 2069 6d70 6c65  :** Easily imple
-00000d20: 6d65 6e74 2079 6f75 7220 6f77 6e20 706f  ment your own po
-00000d30: 7374 2d70 726f 6365 7373 696e 6720 7374  st-processing st
-00000d40: 6570 732e 0a2d 202a 2af0 9f92 a149 6e74  eps..- **....Int
-00000d50: 7569 7469 7665 3a2a 2a20 4772 6561 7420  uitive:** Great 
-00000d60: 6564 6974 6f72 2073 7570 706f 7274 2e20  editor support. 
-00000d70: 436f 6d70 6c65 7469 6f6e 2065 7665 7279  Completion every
-00000d80: 7768 6572 652e 204c 6573 7320 7469 6d65  where. Less time
-00000d90: 2064 6562 7567 6769 6e67 2e0a 2d20 2a2a   debugging..- **
-00000da0: f09f 8eaf 2045 6173 793a 2a2a 2044 6573  .... Easy:** Des
-00000db0: 6967 6e65 6420 746f 2062 6520 6561 7379  igned to be easy
-00000dc0: 2074 6f20 7573 6520 616e 6420 6c65 6172   to use and lear
-00000dd0: 6e2e 204c 6573 7320 7469 6d65 2072 6561  n. Less time rea
-00000de0: 6469 6e67 2064 6f63 732e 0a0a 3c62 722f  ding docs...<br/
-00000df0: 3e0a 3c70 2061 6c69 676e 3d22 6365 6e74  >.<p align="cent
-00000e00: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
-00000e10: 633d 2268 7474 7073 3a2f 2f73 6572 6765  c="https://serge
-00000e20: 792d 6669 6c69 6d6f 6e6f 762e 6e79 6333  y-filimonov.nyc3
-00000e30: 2e64 6967 6974 616c 6f63 6561 6e73 7061  .digitaloceanspa
-00000e40: 6365 732e 636f 6d2f 6f70 656e 2d70 6172  ces.com/open-par
-00000e50: 7365 2f6d 6172 6b65 642d 7570 2d64 6f63  se/marked-up-doc
-00000e60: 2d32 2e77 6562 7022 2077 6964 7468 3d22  -2.webp" width="
-00000e70: 3235 3022 202f 3e0a 3c2f 703e 0a0a 2323  250" />.</p>..##
-00000e80: 2045 7861 6d70 6c65 0a0a 2323 2323 2042   Example..#### B
-00000e90: 6173 6963 2045 7861 6d70 6c65 0a0a 6060  asic Example..``
-00000ea0: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
-00000eb0: 7065 6e70 6172 7365 0a0a 6261 7369 635f  penparse..basic_
-00000ec0: 646f 635f 7061 7468 203d 2022 2e2f 7361  doc_path = "./sa
-00000ed0: 6d70 6c65 2d64 6f63 732f 6d6f 6269 6c65  mple-docs/mobile
-00000ee0: 2d68 6f6d 652d 6d61 6e75 616c 2e70 6466  -home-manual.pdf
-00000ef0: 220a 7061 7273 6572 203d 206f 7065 6e70  ".parser = openp
-00000f00: 6172 7365 2e44 6f63 756d 656e 7450 6172  arse.DocumentPar
-00000f10: 7365 7228 290a 7061 7273 6564 5f62 6173  ser().parsed_bas
-00000f20: 6963 5f64 6f63 203d 2070 6172 7365 722e  ic_doc = parser.
-00000f30: 7061 7273 6528 6261 7369 635f 646f 635f  parse(basic_doc_
-00000f40: 7061 7468 290a 0a66 6f72 206e 6f64 6520  path)..for node 
-00000f50: 696e 2070 6172 7365 645f 6261 7369 635f  in parsed_basic_
-00000f60: 646f 632e 6e6f 6465 733a 0a20 2020 2070  doc.nodes:.    p
-00000f70: 7269 6e74 286e 6f64 6529 0a60 6060 0a0a  rint(node).```..
-00000f80: 2a2a f09f 9393 2054 7279 2074 6865 2073  **.... Try the s
-00000f90: 616d 706c 6520 6e6f 7465 626f 6f6b 2a2a  ample notebook**
-00000fa0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000fb0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00000fc0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
-00000fd0: 652f 315a 3542 3567 736e 6d68 464b 4546  e/1Z5B5gsnmhFKEF
-00000fe0: 4c2d 3579 5949 636f 6f78 372d 6a51 616f  L-5yYIcoox7-jQao
-00000ff0: 3845 703f 7573 703d 7368 6172 696e 6722  8Ep?usp=sharing"
-00001000: 2063 6c61 7373 3d22 6578 7465 726e 616c   class="external
-00001010: 2d6c 696e 6b22 2074 6172 6765 743d 225f  -link" target="_
-00001020: 626c 616e 6b22 3e68 6572 653c 2f61 3e0a  blank">here</a>.
-00001030: 0a23 2323 2320 5365 6d61 6e74 6963 2050  .#### Semantic P
-00001040: 726f 6365 7373 696e 6720 4578 616d 706c  rocessing Exampl
-00001050: 650a 0a43 6875 6e6b 696e 6720 646f 6375  e..Chunking docu
-00001060: 6d65 6e74 7320 6973 2066 756e 6461 6d65  ments is fundame
-00001070: 6e74 616c 6c79 2061 626f 7574 2067 726f  ntally about gro
-00001080: 7570 696e 6720 7369 6d69 6c61 7220 7365  uping similar se
-00001090: 6d61 6e74 6963 206e 6f64 6573 2074 6f67  mantic nodes tog
-000010a0: 6574 6865 722e 2042 7920 656d 6265 6464  ether. By embedd
-000010b0: 696e 6720 7468 6520 7465 7874 206f 6620  ing the text of 
-000010c0: 6561 6368 206e 6f64 652c 2077 6520 6361  each node, we ca
-000010d0: 6e20 7468 656e 2063 6c75 7374 6572 2074  n then cluster t
-000010e0: 6865 6d20 746f 6765 7468 6572 2062 6173  hem together bas
-000010f0: 6564 206f 6e20 7468 6569 7220 7369 6d69  ed on their simi
-00001100: 6c61 7269 7479 2e0a 0a60 6060 7079 7468  larity...```pyth
-00001110: 6f6e 0a66 726f 6d20 6f70 656e 7061 7273  on.from openpars
-00001120: 6520 696d 706f 7274 2070 726f 6365 7373  e import process
-00001130: 696e 672c 2044 6f63 756d 656e 7450 6172  ing, DocumentPar
-00001140: 7365 720a 0a73 656d 616e 7469 635f 7069  ser..semantic_pi
-00001150: 7065 6c69 6e65 203d 2070 726f 6365 7373  peline = process
-00001160: 696e 672e 5365 6d61 6e74 6963 496e 6765  ing.SemanticInge
-00001170: 7374 696f 6e50 6970 656c 696e 6528 0a20  stionPipeline(. 
-00001180: 2020 206f 7065 6e61 695f 6170 695f 6b65     openai_api_ke
-00001190: 793d 4f50 454e 5f41 495f 4b45 592c 0a20  y=OPEN_AI_KEY,. 
-000011a0: 2020 206d 6f64 656c 3d22 7465 7874 2d65     model="text-e
-000011b0: 6d62 6564 6469 6e67 2d33 2d6c 6172 6765  mbedding-3-large
-000011c0: 222c 0a20 2020 206d 696e 5f74 6f6b 656e  ",.    min_token
-000011d0: 733d 3634 2c0a 2020 2020 6d61 785f 746f  s=64,.    max_to
-000011e0: 6b65 6e73 3d31 3032 342c 0a29 0a70 6172  kens=1024,.).par
-000011f0: 7365 7220 3d20 446f 6375 6d65 6e74 5061  ser = DocumentPa
-00001200: 7273 6572 280a 2020 2020 7072 6f63 6573  rser(.    proces
-00001210: 7369 6e67 5f70 6970 656c 696e 653d 7365  sing_pipeline=se
-00001220: 6d61 6e74 6963 5f70 6970 656c 696e 652c  mantic_pipeline,
-00001230: 0a29 0a70 6172 7365 645f 636f 6e74 656e  .).parsed_conten
-00001240: 7420 3d20 7061 7273 6572 2e70 6172 7365  t = parser.parse
-00001250: 2862 6173 6963 5f64 6f63 5f70 6174 6829  (basic_doc_path)
-00001260: 0a60 6060 0a0a 2a2a f09f 9393 2053 616d  .```..**.... Sam
-00001270: 706c 6520 6e6f 7465 626f 6f6b 2a2a 203c  ple notebook** <
-00001280: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001290: 6769 7468 7562 2e63 6f6d 2f46 696c 696d  github.com/Filim
-000012a0: 6f61 2f6f 7065 6e2d 7061 7273 652f 626c  oa/open-parse/bl
-000012b0: 6f62 2f6d 6169 6e2f 7372 632f 636f 6f6b  ob/main/src/cook
-000012c0: 626f 6f6b 732f 7365 6d61 6e74 6963 5f70  books/semantic_p
-000012d0: 726f 6365 7373 696e 672e 6970 796e 6222  rocessing.ipynb"
-000012e0: 2063 6c61 7373 3d22 6578 7465 726e 616c   class="external
-000012f0: 2d6c 696e 6b22 2074 6172 6765 743d 225f  -link" target="_
-00001300: 626c 616e 6b22 3e68 6572 653c 2f61 3e0a  blank">here</a>.
-00001310: 0a23 2323 2320 5365 7269 616c 697a 696e  .#### Serializin
-00001320: 6720 5265 7375 6c74 730a 5573 6573 2070  g Results.Uses p
-00001330: 7964 616e 7469 6320 756e 6465 7220 7468  ydantic under th
-00001340: 6520 686f 6f64 2073 6f20 796f 7520 6361  e hood so you ca
-00001350: 6e20 7365 7269 616c 697a 6520 7265 7375  n serialize resu
-00001360: 6c74 7320 7769 7468 200a 0a60 6060 7079  lts with ..```py
-00001370: 7468 6f6e 0a70 6172 7365 645f 636f 6e74  thon.parsed_cont
-00001380: 656e 742e 6469 6374 2829 0a23 206f 720a  ent.dict().# or.
-00001390: 7061 7273 6564 5f63 6f6e 7465 6e74 2e6a  parsed_content.j
-000013a0: 736f 6e28 290a 6060 600a 0a23 2320 5265  son().```..## Re
-000013b0: 7175 6972 656d 656e 7473 0a0a 5079 7468  quirements..Pyth
-000013c0: 6f6e 2033 2e38 2b0a 0a2a 2a44 6561 6c69  on 3.8+..**Deali
-000013d0: 6e67 2077 6974 6820 5044 4627 733a 2a2a  ng with PDF's:**
-000013e0: 0a0a 2d20 3c61 2068 7265 663d 2268 7474  ..- <a href="htt
-000013f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001400: 7064 666d 696e 6572 2f70 6466 6d69 6e65  pdfminer/pdfmine
-00001410: 722e 7369 7822 2063 6c61 7373 3d22 6578  r.six" class="ex
-00001420: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
-00001430: 6765 743d 225f 626c 616e 6b22 3e70 6466  get="_blank">pdf
-00001440: 6d69 6e65 722e 7369 783c 2f61 3e20 4675  miner.six</a> Fu
-00001450: 6c6c 7920 6f70 656e 2073 6f75 7263 652e  lly open source.
-00001460: 0a0a 2a2a 4578 7472 6163 7469 6e67 2054  ..**Extracting T
-00001470: 6162 6c65 733a 2a2a 0a0a 2d20 3c61 2068  ables:**..- <a h
-00001480: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001490: 6875 622e 636f 6d2f 7079 6d75 7064 662f  hub.com/pymupdf/
-000014a0: 5079 4d75 5044 4622 2063 6c61 7373 3d22  PyMuPDF" class="
-000014b0: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
-000014c0: 6172 6765 743d 225f 626c 616e 6b22 3e50  arget="_blank">P
-000014d0: 794d 7550 4446 3c2f 613e 2068 6173 2073  yMuPDF</a> has s
-000014e0: 6f6d 6520 7461 626c 6520 6465 7465 6374  ome table detect
-000014f0: 696f 6e20 6675 6e63 7469 6f6e 616c 6974  ion functionalit
-00001500: 792e 2050 6c65 6173 6520 7365 6520 7468  y. Please see th
-00001510: 6569 7220 3c61 2068 7265 663d 2268 7474  eir <a href="htt
-00001520: 7073 3a2f 2f6d 7570 6466 2e63 6f6d 2f6c  ps://mupdf.com/l
-00001530: 6963 656e 7369 6e67 2f69 6e64 6578 2e68  icensing/index.h
-00001540: 746d 6c23 636f 6d6d 6572 6369 616c 2220  tml#commercial" 
-00001550: 636c 6173 733d 2265 7874 6572 6e61 6c2d  class="external-
-00001560: 6c69 6e6b 2220 7461 7267 6574 3d22 5f62  link" target="_b
-00001570: 6c61 6e6b 223e 6c69 6365 6e73 653c 2f61  lank">license</a
-00001580: 3e2e 0a2d 203c 6120 6872 6566 3d22 6874  >..- <a href="ht
-00001590: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-000015a0: 652e 636f 2f6d 6963 726f 736f 6674 2f74  e.co/microsoft/t
-000015b0: 6162 6c65 2d74 7261 6e73 666f 726d 6572  able-transformer
-000015c0: 2d64 6574 6563 7469 6f6e 2220 636c 6173  -detection" clas
-000015d0: 733d 2265 7874 6572 6e61 6c2d 6c69 6e6b  s="external-link
-000015e0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-000015f0: 223e 5461 626c 6520 5472 616e 7366 6f72  ">Table Transfor
-00001600: 6d65 723c 2f61 3e20 6973 2061 2064 6565  mer</a> is a dee
-00001610: 7020 6c65 6172 6e69 6e67 2061 7070 726f  p learning appro
-00001620: 6163 682e 0a2d 203c 6120 6872 6566 3d22  ach..- <a href="
-00001630: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001640: 6f6d 2f70 6f6c 6f63 6c75 622f 756e 6974  om/poloclub/unit
-00001650: 6162 6c65 2220 636c 6173 733d 2265 7874  able" class="ext
-00001660: 6572 6e61 6c2d 6c69 6e6b 2220 7461 7267  ernal-link" targ
-00001670: 6574 3d22 5f62 6c61 6e6b 223e 756e 6974  et="_blank">unit
-00001680: 6162 6c65 3c2f 613e 2069 7320 616e 6f74  able</a> is anot
-00001690: 6865 7220 7472 616e 7366 6f72 6d65 7273  her transformers
-000016a0: 2062 6173 6564 2061 7070 726f 6163 6820   based approach 
-000016b0: 7769 7468 202a 2a73 7461 7465 2d6f 662d  with **state-of-
-000016c0: 7468 652d 6172 742a 2a20 7065 7266 6f72  the-art** perfor
-000016d0: 6d61 6e63 652e 0a0a 2323 2049 6e73 7461  mance...## Insta
-000016e0: 6c6c 6174 696f 6e0a 0a23 2323 2320 312e  llation..#### 1.
-000016f0: 2043 6f72 6520 4c69 6272 6172 790a 0a60   Core Library..`
-00001700: 6060 636f 6e73 6f6c 650a 7069 7020 696e  ``console.pip in
-00001710: 7374 616c 6c20 6f70 656e 7061 7273 650a  stall openparse.
-00001720: 6060 600a 0a2a 2a45 6e61 626c 696e 6720  ```..**Enabling 
-00001730: 4f43 5220 5375 7070 6f72 742a 2a3a 0a0a  OCR Support**:..
-00001740: 5079 4d75 5044 4620 7769 6c6c 2061 6c72  PyMuPDF will alr
-00001750: 6561 6479 2063 6f6e 7461 696e 2061 6c6c  eady contain all
-00001760: 2074 6865 206c 6f67 6963 2074 6f20 7375   the logic to su
-00001770: 7070 6f72 7420 4f43 5220 6675 6e63 7469  pport OCR functi
-00001780: 6f6e 732e 2042 7574 2069 7420 6164 6469  ons. But it addi
-00001790: 7469 6f6e 616c 6c79 2064 6f65 7320 6e65  tionally does ne
-000017a0: 6564 2054 6573 7365 7261 6374 e280 9973  ed Tesseract...s
-000017b0: 206c 616e 6775 6167 6520 7375 7070 6f72   language suppor
-000017c0: 7420 6461 7461 2c20 736f 2069 6e73 7461  t data, so insta
-000017d0: 6c6c 6174 696f 6e20 6f66 2054 6573 7365  llation of Tesse
-000017e0: 7261 6374 2d4f 4352 2069 7320 7374 696c  ract-OCR is stil
-000017f0: 6c20 7265 7175 6972 6564 2e0a 0a54 6865  l required...The
-00001800: 206c 616e 6775 6167 6520 7375 7070 6f72   language suppor
-00001810: 7420 666f 6c64 6572 206c 6f63 6174 696f  t folder locatio
-00001820: 6e20 6d75 7374 2062 6520 636f 6d6d 756e  n must be commun
-00001830: 6963 6174 6564 2065 6974 6865 7220 7669  icated either vi
-00001840: 6120 7374 6f72 696e 6720 6974 2069 6e20  a storing it in 
-00001850: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
-00001860: 7661 7269 6162 6c65 2022 5445 5353 4441  variable "TESSDA
-00001870: 5441 5f50 5245 4649 5822 2c20 6f72 2061  TA_PREFIX", or a
-00001880: 7320 6120 7061 7261 6d65 7465 7220 696e  s a parameter in
-00001890: 2074 6865 2061 7070 6c69 6361 626c 6520   the applicable 
-000018a0: 6675 6e63 7469 6f6e 732e 0a0a 536f 2066  functions...So f
-000018b0: 6f72 2061 2077 6f72 6b69 6e67 204f 4352  or a working OCR
-000018c0: 2066 756e 6374 696f 6e61 6c69 7479 2c20   functionality, 
-000018d0: 6d61 6b65 2073 7572 6520 746f 2063 6f6d  make sure to com
-000018e0: 706c 6574 6520 7468 6973 2063 6865 636b  plete this check
-000018f0: 6c69 7374 3a0a 0a31 2e20 496e 7374 616c  list:..1. Instal
-00001900: 6c20 5465 7373 6572 6163 742e 0a0a 322e  l Tesseract...2.
-00001910: 204c 6f63 6174 6520 5465 7373 6572 6163   Locate Tesserac
-00001920: 74e2 8099 7320 6c61 6e67 7561 6765 2073  t...s language s
-00001930: 7570 706f 7274 2066 6f6c 6465 722e 2054  upport folder. T
-00001940: 7970 6963 616c 6c79 2079 6f75 2077 696c  ypically you wil
-00001950: 6c20 6669 6e64 2069 7420 6865 7265 3a0a  l find it here:.
-00001960: 0a20 2020 2d20 5769 6e64 6f77 733a 2060  .   - Windows: `
-00001970: 433a 2f50 726f 6772 616d 2046 696c 6573  C:/Program Files
-00001980: 2f54 6573 7365 7261 6374 2d4f 4352 2f74  /Tesseract-OCR/t
-00001990: 6573 7364 6174 6160 0a0a 2020 202d 2055  essdata`..   - U
-000019a0: 6e69 7820 7379 7374 656d 733a 2060 2f75  nix systems: `/u
-000019b0: 7372 2f73 6861 7265 2f74 6573 7365 7261  sr/share/tessera
-000019c0: 6374 2d6f 6372 2f35 2f74 6573 7364 6174  ct-ocr/5/tessdat
-000019d0: 6160 0a0a 332e 2053 6574 2074 6865 2065  a`..3. Set the e
-000019e0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-000019f0: 626c 6520 5445 5353 4441 5441 5f50 5245  ble TESSDATA_PRE
-00001a00: 4649 580a 0a20 2020 2d20 5769 6e64 6f77  FIX..   - Window
-00001a10: 733a 2060 7365 7478 2054 4553 5344 4154  s: `setx TESSDAT
-00001a20: 415f 5052 4546 4958 2022 433a 2f50 726f  A_PREFIX "C:/Pro
-00001a30: 6772 616d 2046 696c 6573 2f54 6573 7365  gram Files/Tesse
-00001a40: 7261 6374 2d4f 4352 2f74 6573 7364 6174  ract-OCR/tessdat
-00001a50: 6122 600a 0a20 2020 2d20 556e 6978 2073  a"`..   - Unix s
-00001a60: 7973 7465 6d73 3a20 6064 6563 6c61 7265  ystems: `declare
-00001a70: 202d 7820 5445 5353 4441 5441 5f50 5245   -x TESSDATA_PRE
-00001a80: 4649 583d 202f 7573 722f 7368 6172 652f  FIX= /usr/share/
-00001a90: 7465 7373 6572 6163 742d 6f63 722f 352f  tesseract-ocr/5/
-00001aa0: 7465 7373 6461 7461 600a 0a2a 2a4e 6f74  tessdata`..**Not
-00001ab0: 653a 2a2a 205f 4f6e 2057 696e 646f 7773  e:** _On Windows
-00001ac0: 2073 7973 7465 6d73 2c20 7468 6973 206d   systems, this m
-00001ad0: 7573 7420 6861 7070 656e 206f 7574 7369  ust happen outsi
-00001ae0: 6465 2050 7974 686f 6e20 e280 9320 6265  de Python ... be
-00001af0: 666f 7265 2073 7461 7274 696e 6720 796f  fore starting yo
-00001b00: 7572 2073 6372 6970 742e 204a 7573 7420  ur script. Just 
-00001b10: 6d61 6e69 7075 6c61 7469 6e67 206f 732e  manipulating os.
-00001b20: 656e 7669 726f 6e20 7769 6c6c 206e 6f74  environ will not
-00001b30: 2077 6f72 6b21 5f0a 0a23 2323 2320 322e   work!_..#### 2.
-00001b40: 204d 4c20 5461 626c 6520 4465 7465 6374   ML Table Detect
-00001b50: 696f 6e20 284f 7074 696f 6e61 6c29 0a0a  ion (Optional)..
-00001b60: 5468 6973 2072 6570 6f73 6974 6f72 7920  This repository 
-00001b70: 7072 6f76 6964 6573 2061 6e20 6f70 7469  provides an opti
-00001b80: 6f6e 616c 2066 6561 7475 7265 2074 6f20  onal feature to 
-00001b90: 7061 7273 6520 636f 6e74 656e 7420 6672  parse content fr
-00001ba0: 6f6d 2074 6162 6c65 7320 7573 696e 6720  om tables using 
-00001bb0: 6120 7661 7269 6574 7920 6f66 2064 6565  a variety of dee
-00001bc0: 7020 6c65 6172 6e69 6e67 206d 6f64 656c  p learning model
-00001bd0: 732e 0a0a 6060 6063 6f6e 736f 6c65 0a70  s...```console.p
-00001be0: 6970 2069 6e73 7461 6c6c 2022 6f70 656e  ip install "open
-00001bf0: 7061 7273 655b 6d6c 5d22 0a60 6060 0a0a  parse[ml]".```..
-00001c00: 5468 656e 2064 6f77 6e6c 6f61 6420 7468  Then download th
-00001c10: 6520 6d6f 6465 6c20 7765 6967 6874 7320  e model weights 
-00001c20: 7769 7468 0a0a 6060 6063 6f6e 736f 6c65  with..```console
-00001c30: 0a6f 7065 6e70 6172 7365 2d64 6f77 6e6c  .openparse-downl
-00001c40: 6f61 640a 6060 600a 0a59 6f75 2063 616e  oad.```..You can
-00001c50: 2072 756e 2074 6865 2070 6172 7369 6e67   run the parsing
-00001c60: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
-00001c70: 696e 672e 200a 0a60 6060 7079 7468 6f6e  ing. ..```python
-00001c80: 0a70 6172 7365 7220 3d20 6f70 656e 7061  .parser = openpa
-00001c90: 7273 652e 446f 6375 6d65 6e74 5061 7273  rse.DocumentPars
-00001ca0: 6572 280a 2020 2020 2020 2020 7461 626c  er(.        tabl
-00001cb0: 655f 6172 6773 3d7b 0a20 2020 2020 2020  e_args={.       
-00001cc0: 2020 2020 2022 7061 7273 696e 675f 616c       "parsing_al
-00001cd0: 676f 7269 7468 6d22 3a20 2275 6e69 7461  gorithm": "unita
-00001ce0: 626c 6522 2c0a 2020 2020 2020 2020 2020  ble",.          
-00001cf0: 2020 226d 696e 5f74 6162 6c65 5f63 6f6e    "min_table_con
-00001d00: 6669 6465 6e63 6522 3a20 302e 382c 0a20  fidence": 0.8,. 
-00001d10: 2020 2020 2020 207d 2c0a 290a 7061 7273         },.).pars
-00001d20: 6564 5f6e 6f64 6573 203d 2070 6172 7365  ed_nodes = parse
-00001d30: 722e 7061 7273 6528 7064 665f 7061 7468  r.parse(pdf_path
-00001d40: 290a 6060 600a 0a4e 6f74 6520 7765 2063  ).```..Note we c
-00001d50: 7572 7265 6e74 6c79 2075 7365 205b 7461  urrently use [ta
-00001d60: 626c 652d 7472 616e 7366 6f72 6d65 7273  ble-transformers
-00001d70: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001d80: 2e63 6f6d 2f6d 6963 726f 736f 6674 2f74  .com/microsoft/t
-00001d90: 6162 6c65 2d74 7261 6e73 666f 726d 6572  able-transformer
-00001da0: 2920 666f 7220 616c 6c20 7461 626c 6520  ) for all table 
-00001db0: 6465 7465 6374 696f 6e20 616e 6420 7765  detection and we
-00001dc0: 2066 696e 6420 6974 7320 7065 7266 6f72   find its perfor
-00001dd0: 6d61 6e63 6520 746f 2062 6520 7375 6270  mance to be subp
-00001de0: 6172 2e20 5468 6973 206e 6567 6174 6976  ar. This negativ
-00001df0: 656c 7920 6166 6665 6374 7320 7468 6520  ely affects the 
-00001e00: 646f 776e 7374 7265 616d 2072 6573 756c  downstream resul
-00001e10: 7473 206f 6620 756e 6974 6162 6c65 2e20  ts of unitable. 
-00001e20: 4966 2079 6f75 2772 6520 6177 6172 6520  If you're aware 
-00001e30: 6f66 2061 2062 6574 7465 7220 6d6f 6465  of a better mode
-00001e40: 6c20 706c 6561 7365 206f 7065 6e20 616e  l please open an
-00001e50: 2049 7373 7565 202d 2074 6865 2075 6e69   Issue - the uni
-00001e60: 7461 626c 6520 7465 616d 206d 656e 7469  table team menti
-00001e70: 6f6e 6564 2074 6865 7920 6d69 6768 7420  oned they might 
-00001e80: 6164 6420 7468 6973 2073 6f6f 6e20 746f  add this soon to
-00001e90: 6f2e 0a0a 2323 2043 6f6f 6b62 6f6f 6b73  o...## Cookbooks
-00001ea0: 0a0a 6874 7470 733a 2f2f 6769 7468 7562  ..https://github
-00001eb0: 2e63 6f6d 2f46 696c 696d 6f61 2f6f 7065  .com/Filimoa/ope
-00001ec0: 6e2d 7061 7273 652f 7472 6565 2f6d 6169  n-parse/tree/mai
-00001ed0: 6e2f 7372 632f 636f 6f6b 626f 6f6b 730a  n/src/cookbooks.
-00001ee0: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
-00001ef0: 6e0a 0a68 7474 7073 3a2f 2f66 696c 696d  n..https://filim
-00001f00: 6f61 2e67 6974 6875 622e 696f 2f6f 7065  oa.github.io/ope
-00001f10: 6e2d 7061 7273 652f 0a                   n-parse/.
+00000070: 204c 4c4d 2773 2e0a 4175 7468 6f72 2d65   LLM's..Author-e
+00000080: 6d61 696c 3a20 5365 7267 6579 2046 696c  mail: Sergey Fil
+00000090: 696d 6f6e 6f76 203c 6865 6c6c 6f40 7365  imonov <hello@se
+000000a0: 7267 6579 2e66 7969 3e0a 5072 6f6a 6563  rgey.fyi>.Projec
+000000b0: 742d 5552 4c3a 2068 6f6d 6570 6167 652c  t-URL: homepage,
+000000c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000d0: 636f 6d2f 4669 6c69 6d6f 612f 6f70 656e  com/Filimoa/open
+000000e0: 2d70 6172 7365 0a50 726f 6a65 6374 2d55  -parse.Project-U
+000000f0: 524c 3a20 7265 706f 7369 746f 7279 2c20  RL: repository, 
+00000100: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000110: 6f6d 2f46 696c 696d 6f61 2f6f 7065 6e2d  om/Filimoa/open-
+00000120: 7061 7273 650a 5072 6f6a 6563 742d 5552  parse.Project-UR
+00000130: 4c3a 2064 6f63 756d 656e 7461 7469 6f6e  L: documentation
+00000140: 2c20 6874 7470 733a 2f2f 6669 6c69 6d6f  , https://filimo
+00000150: 612e 6769 7468 7562 2e69 6f2f 6f70 656e  a.github.io/open
+00000160: 2d70 6172 7365 0a52 6571 7569 7265 732d  -parse.Requires-
+00000170: 5079 7468 6f6e 3a20 3e3d 332e 380a 4465  Python: >=3.8.De
+00000180: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+00000190: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000001a0: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
+000001b0: 6c65 3a20 4c49 4345 4e53 450a 5265 7175  le: LICENSE.Requ
+000001c0: 6972 6573 2d44 6973 743a 2050 794d 7550  ires-Dist: PyMuP
+000001d0: 4446 3e3d 312e 3233 2e32 0a52 6571 7569  DF>=1.23.2.Requi
+000001e0: 7265 732d 4469 7374 3a20 7069 6c6c 6f77  res-Dist: pillow
+000001f0: 3e3d 382e 330a 5265 7175 6972 6573 2d44  >=8.3.Requires-D
+00000200: 6973 743a 2070 7964 616e 7469 633e 3d32  ist: pydantic>=2
+00000210: 2e30 0a52 6571 7569 7265 732d 4469 7374  .0.Requires-Dist
+00000220: 3a20 7079 7064 663e 3d34 2e30 2e30 0a52  : pypdf>=4.0.0.R
+00000230: 6571 7569 7265 732d 4469 7374 3a20 7064  equires-Dist: pd
+00000240: 666d 696e 6572 2e73 6978 3e3d 3230 3230  fminer.six>=2020
+00000250: 3034 3031 0a52 6571 7569 7265 732d 4469  0401.Requires-Di
+00000260: 7374 3a20 7469 6b74 6f6b 656e 3e3d 302e  st: tiktoken>=0.
+00000270: 330a 5265 7175 6972 6573 2d44 6973 743a  3.Requires-Dist:
+00000280: 206f 7065 6e61 693e 3d31 2e30 2e30 0a52   openai>=1.0.0.R
+00000290: 6571 7569 7265 732d 4469 7374 3a20 6e75  equires-Dist: nu
+000002a0: 6d70 790a 5072 6f76 6964 6573 2d45 7874  mpy.Provides-Ext
+000002b0: 7261 3a20 6d6c 0a52 6571 7569 7265 732d  ra: ml.Requires-
+000002c0: 4469 7374 3a20 746f 7263 683b 2065 7874  Dist: torch; ext
+000002d0: 7261 203d 3d20 226d 6c22 0a52 6571 7569  ra == "ml".Requi
+000002e0: 7265 732d 4469 7374 3a20 746f 7263 6876  res-Dist: torchv
+000002f0: 6973 696f 6e3b 2065 7874 7261 203d 3d20  ision; extra == 
+00000300: 226d 6c22 0a52 6571 7569 7265 732d 4469  "ml".Requires-Di
+00000310: 7374 3a20 7472 616e 7366 6f72 6d65 7273  st: transformers
+00000320: 3b20 6578 7472 6120 3d3d 2022 6d6c 220a  ; extra == "ml".
+00000330: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000340: 6f6b 656e 697a 6572 733b 2065 7874 7261  okenizers; extra
+00000350: 203d 3d20 226d 6c22 0a0a 3c70 2061 6c69   == "ml"..<p ali
+00000360: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000370: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000380: 3a2f 2f73 6572 6765 792d 6669 6c69 6d6f  ://sergey-filimo
+00000390: 6e6f 762e 6e79 6333 2e64 6967 6974 616c  nov.nyc3.digital
+000003a0: 6f63 6561 6e73 7061 6365 732e 636f 6d2f  oceanspaces.com/
+000003b0: 6f70 656e 2d70 6172 7365 2f6f 7065 6e2d  open-parse/open-
+000003c0: 7061 7273 652d 7769 7468 2d74 6578 742d  parse-with-text-
+000003d0: 7470 2d6c 6f67 6f2e 7765 6270 2220 7769  tp-logo.webp" wi
+000003e0: 6474 683d 2233 3530 2220 2f3e 0a3c 2f70  dth="350" />.</p
+000003f0: 3e0a 3c62 722f 3e0a 0a2a 2a45 6173 696c  >.<br/>..**Easil
+00000400: 7920 6368 756e 6b20 636f 6d70 6c65 7820  y chunk complex 
+00000410: 646f 6375 6d65 6e74 7320 7468 6520 7361  documents the sa
+00000420: 6d65 2077 6179 2061 2068 756d 616e 2077  me way a human w
+00000430: 6f75 6c64 2e2a 2a20 200a 0a43 6875 6e6b  ould.**  ..Chunk
+00000440: 696e 6720 646f 6375 6d65 6e74 7320 6973  ing documents is
+00000450: 2061 2063 6861 6c6c 656e 6769 6e67 2074   a challenging t
+00000460: 6173 6b20 7468 6174 2075 6e64 6572 7069  ask that underpi
+00000470: 6e73 2061 6e79 2052 4147 2073 7973 7465  ns any RAG syste
+00000480: 6d2e 2020 4869 6768 2071 7561 6c69 7479  m.  High quality
+00000490: 2072 6573 756c 7473 2061 7265 2063 7269   results are cri
+000004a0: 7469 6361 6c20 746f 2061 2073 7563 6573  tical to a suces
+000004b0: 7366 756c 2041 4920 6170 706c 6963 6174  sful AI applicat
+000004c0: 696f 6e2c 2079 6574 206d 6f73 7420 6f70  ion, yet most op
+000004d0: 656e 2d73 6f75 7263 6520 6c69 6272 6172  en-source librar
+000004e0: 6965 7320 6172 6520 6c69 6d69 7465 6420  ies are limited 
+000004f0: 696e 2074 6865 6972 2061 6269 6c69 7479  in their ability
+00000500: 2074 6f20 6861 6e64 6c65 2063 6f6d 706c   to handle compl
+00000510: 6578 2064 6f63 756d 656e 7473 2e20 200a  ex documents.  .
+00000520: 0a4f 7065 6e20 5061 7273 6520 6973 2064  .Open Parse is d
+00000530: 6573 6967 6e65 6420 746f 2066 696c 6c20  esigned to fill 
+00000540: 7468 6973 2067 6170 2062 7920 7072 6f76  this gap by prov
+00000550: 6964 696e 6720 6120 666c 6578 6962 6c65  iding a flexible
+00000560: 2c20 6561 7379 2d74 6f2d 7573 6520 6c69  , easy-to-use li
+00000570: 6272 6172 7920 6361 7061 626c 6520 6f66  brary capable of
+00000580: 2076 6973 7561 6c6c 7920 6469 7363 6572   visually discer
+00000590: 6e69 6e67 2064 6f63 756d 656e 7420 6c61  ning document la
+000005a0: 796f 7574 7320 616e 6420 6368 756e 6b69  youts and chunki
+000005b0: 6e67 2074 6865 6d20 6566 6665 6374 6976  ng them effectiv
+000005c0: 656c 792e 0a0a 3c64 6574 6169 6c73 3e0a  ely...<details>.
+000005d0: 2020 3c73 756d 6d61 7279 3e3c 623e 486f    <summary><b>Ho
+000005e0: 7720 6973 2074 6869 7320 6469 6666 6572  w is this differ
+000005f0: 656e 7420 6672 6f6d 206f 7468 6572 206c  ent from other l
+00000600: 6179 6f75 7420 7061 7273 6572 733f 3c2f  ayout parsers?</
+00000610: 623e 3c2f 7375 6d6d 6172 793e 0a0a 2020  b></summary>..  
+00000620: 2323 2323 20e2 9c82 efb8 8f20 5465 7874  #### ...... Text
+00000630: 2053 706c 6974 7469 6e67 0a20 2054 6578   Splitting.  Tex
+00000640: 7420 7370 6c69 7474 696e 6720 636f 6e76  t splitting conv
+00000650: 6572 7473 2061 2066 696c 6520 746f 2072  erts a file to r
+00000660: 6177 2074 6578 7420 616e 6420 5b73 6c69  aw text and [sli
+00000670: 6365 7320 6974 2075 705d 2868 7474 7073  ces it up](https
+00000680: 3a2f 2f64 6f63 732e 6c6c 616d 6169 6e64  ://docs.llamaind
+00000690: 6578 2e61 692f 656e 2f73 7461 626c 652f  ex.ai/en/stable/
+000006a0: 6170 695f 7265 6665 7265 6e63 652f 6e6f  api_reference/no
+000006b0: 6465 5f70 6172 7365 7273 2f74 6f6b 656e  de_parsers/token
+000006c0: 5f74 6578 745f 7370 6c69 7474 6572 2f29  _text_splitter/)
+000006d0: 2e0a 2020 0a20 202d 2059 6f75 206c 6f73  ..  .  - You los
+000006e0: 6520 7468 6520 6162 696c 6974 7920 746f  e the ability to
+000006f0: 2065 6173 696c 7920 6f76 6572 6c61 7920   easily overlay 
+00000700: 7468 6520 6368 756e 6b20 6f6e 2074 6865  the chunk on the
+00000710: 206f 7269 6769 6e61 6c20 7064 660a 2020   original pdf.  
+00000720: 2d20 596f 7520 6967 6e6f 7265 2074 6865  - You ignore the
+00000730: 2075 6e64 6572 6c79 696e 6720 7365 6d61   underlying sema
+00000740: 6e74 6963 2073 7472 7563 7475 7265 206f  ntic structure o
+00000750: 6620 7468 6520 6669 6c65 202d 2068 6561  f the file - hea
+00000760: 6469 6e67 732c 2073 6563 7469 6f6e 732c  dings, sections,
+00000770: 2062 756c 6c65 7473 2072 6570 7265 7365   bullets represe
+00000780: 6e74 2076 616c 7561 626c 6520 696e 666f  nt valuable info
+00000790: 726d 6174 696f 6e2e 0a20 202d 204e 6f20  rmation..  - No 
+000007a0: 7375 7070 6f72 7420 666f 7220 7461 626c  support for tabl
+000007b0: 6573 2c20 696d 6167 6573 206f 7220 6d61  es, images or ma
+000007c0: 726b 646f 776e 2e0a 2020 0a20 2023 2323  rkdown..  .  ###
+000007d0: 2320 f09f a496 204d 4c20 4c61 796f 7574  # .... ML Layout
+000007e0: 2050 6172 7365 7273 0a20 2054 6865 7265   Parsers.  There
+000007f0: 2773 2073 6f6d 6520 6f66 2066 616e 7461  's some of fanta
+00000800: 7374 6963 206c 6962 7261 7269 6573 206c  stic libraries l
+00000810: 696b 6520 5b6c 6179 6f75 742d 7061 7273  ike [layout-pars
+00000820: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
+00000830: 7562 2e63 6f6d 2f4c 6179 6f75 742d 5061  ub.com/Layout-Pa
+00000840: 7273 6572 2f6c 6179 6f75 742d 7061 7273  rser/layout-pars
+00000850: 6572 292e 200a 2020 2d20 5768 696c 6520  er). .  - While 
+00000860: 7468 6579 2063 616e 2069 6465 6e74 6966  they can identif
+00000870: 7920 7661 7269 6f75 7320 656c 656d 656e  y various elemen
+00000880: 7473 206c 696b 6520 7465 7874 2062 6c6f  ts like text blo
+00000890: 636b 732c 2069 6d61 6765 732c 2061 6e64  cks, images, and
+000008a0: 2074 6162 6c65 732c 2062 7574 2074 6865   tables, but the
+000008b0: 7920 6172 6520 6e6f 7420 6275 696c 7420  y are not built 
+000008c0: 746f 2067 726f 7570 2072 656c 6174 6564  to group related
+000008d0: 2063 6f6e 7465 6e74 2065 6666 6563 7469   content effecti
+000008e0: 7665 6c79 2e0a 2020 2d20 5468 6579 2073  vely..  - They s
+000008f0: 7472 6963 746c 7920 666f 6375 7320 6f6e  trictly focus on
+00000900: 206c 6179 6f75 7420 7061 7273 696e 6720   layout parsing 
+00000910: 2d20 796f 7520 7769 6c6c 206e 6565 6420  - you will need 
+00000920: 746f 2061 6464 2061 6e6f 7468 6572 206d  to add another m
+00000930: 6f64 656c 2074 6f20 6578 7472 6163 7420  odel to extract 
+00000940: 6d61 726b 646f 776e 2066 726f 6d20 7468  markdown from th
+00000950: 6520 696d 6167 6573 2c20 7061 7273 6520  e images, parse 
+00000960: 7461 626c 6573 2c20 6772 6f75 7020 6e6f  tables, group no
+00000970: 6465 732c 2065 7463 2e0a 2020 2d20 5765  des, etc..  - We
+00000980: 2776 6520 666f 756e 6420 7065 7266 6f72  've found perfor
+00000990: 6d61 6e63 6520 746f 2062 6520 7375 622d  mance to be sub-
+000009a0: 6f70 7469 6d61 6c20 6f6e 206d 616e 7920  optimal on many 
+000009b0: 646f 6375 6d65 6e74 7320 7768 696c 6520  documents while 
+000009c0: 616c 736f 2062 6569 6e67 2063 6f6d 7075  also being compu
+000009d0: 7461 7469 6f6e 616c 6c79 2068 6561 7679  tationally heavy
+000009e0: 2e0a 0a20 2023 2323 2320 f09f 92bc 2043  ...  #### .... C
+000009f0: 6f6d 6d65 7263 6961 6c20 536f 6c75 7469  ommercial Soluti
+00000a00: 6f6e 730a 0a20 202d 2054 7970 6963 616c  ons..  - Typical
+00000a10: 6c79 2070 7269 6365 6420 6174 20e2 8988  ly priced at ...
+00000a20: 2024 3130 202f 2031 6b20 7061 6765 732e   $10 / 1k pages.
+00000a30: 2053 6565 205b 6865 7265 5d28 6874 7470   See [here](http
+00000a40: 733a 2f2f 636c 6f75 642e 676f 6f67 6c65  s://cloud.google
+00000a50: 2e63 6f6d 2f64 6f63 756d 656e 742d 6169  .com/document-ai
+00000a60: 292c 205b 6865 7265 5d28 6874 7470 733a  ), [here](https:
+00000a70: 2f2f 6177 732e 616d 617a 6f6e 2e63 6f6d  //aws.amazon.com
+00000a80: 2f74 6578 7472 6163 742f 2920 616e 6420  /textract/) and 
+00000a90: 5b68 6572 655d 2868 7474 7073 3a2f 2f77  [here](https://w
+00000aa0: 7777 2e72 6564 7563 746f 2e61 692f 292e  ww.reducto.ai/).
+00000ab0: 0a20 202d 2052 6571 7569 7265 7320 7368  .  - Requires sh
+00000ac0: 6172 696e 6720 796f 7572 2064 6174 6120  aring your data 
+00000ad0: 7769 7468 2061 2076 656e 646f 720a 0a3c  with a vendor..<
+00000ae0: 2f64 6574 6169 6c73 3e0a 0a23 2320 4869  /details>..## Hi
+00000af0: 6768 6c69 6768 7473 0a0a 2d20 2a2a f09f  ghlights..- **..
+00000b00: 948d 2056 6973 7561 6c6c 792d 4472 6976  .. Visually-Driv
+00000b10: 656e 3a2a 2a20 4f70 656e 2d50 6172 7365  en:** Open-Parse
+00000b20: 2076 6973 7561 6c6c 7920 616e 616c 797a   visually analyz
+00000b30: 6573 2064 6f63 756d 656e 7473 2066 6f72  es documents for
+00000b40: 2073 7570 6572 696f 7220 4c4c 4d20 696e   superior LLM in
+00000b50: 7075 742c 2067 6f69 6e67 2062 6579 6f6e  put, going beyon
+00000b60: 6420 6e61 6976 6520 7465 7874 2073 706c  d naive text spl
+00000b70: 6974 7469 6e67 2e0a 2d20 2a2a e29c 8def  itting..- **....
+00000b80: b88f 204d 6172 6b64 6f77 6e20 5375 7070  .. Markdown Supp
+00000b90: 6f72 743a 2a2a 2042 6173 6963 206d 6172  ort:** Basic mar
+00000ba0: 6b64 6f77 6e20 7375 7070 6f72 7420 666f  kdown support fo
+00000bb0: 7220 7061 7273 696e 6720 6865 6164 696e  r parsing headin
+00000bc0: 6773 2c20 626f 6c64 2061 6e64 2069 7461  gs, bold and ita
+00000bd0: 6c69 6373 2e0a 2d20 2a2a f09f 938a 2048  lics..- **.... H
+00000be0: 6967 682d 5072 6563 6973 696f 6e20 5461  igh-Precision Ta
+00000bf0: 626c 6520 5375 7070 6f72 743a 2a2a 2045  ble Support:** E
+00000c00: 7874 7261 6374 2074 6162 6c65 7320 696e  xtract tables in
+00000c10: 746f 2063 6c65 616e 204d 6172 6b64 6f77  to clean Markdow
+00000c20: 6e20 666f 726d 6174 7320 7769 7468 2061  n formats with a
+00000c30: 6363 7572 6163 7920 7468 6174 2073 7572  ccuracy that sur
+00000c40: 7061 7373 6573 2074 7261 6469 7469 6f6e  passes tradition
+00000c50: 616c 2074 6f6f 6c73 2e0a 2020 2020 3c64  al tools..    <d
+00000c60: 6574 6169 6c73 3e0a 2020 3c73 756d 6d61  etails>.  <summa
+00000c70: 7279 3e3c 693e 4578 616d 706c 6573 3c2f  ry><i>Examples</
+00000c80: 693e 3c2f 7375 6d6d 6172 793e 0a20 2054  i></summary>.  T
+00000c90: 6865 2066 6f6c 6c6f 7769 6e67 2065 7861  he following exa
+00000ca0: 6d70 6c65 7320 7765 7265 2070 6172 7365  mples were parse
+00000cb0: 6420 7769 7468 2075 6e69 7461 626c 652e  d with unitable.
+00000cc0: 0a20 2020 203c 6272 2f3e 0a20 2020 203c  .    <br/>.    <
+00000cd0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000ce0: 3e0a 2020 2020 2020 2020 3c62 722f 3e0a  >.        <br/>.
+00000cf0: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000d00: 3d22 6874 7470 733a 2f2f 7365 7267 6579  ="https://sergey
+00000d10: 2d66 696c 696d 6f6e 6f76 2e6e 7963 332e  -filimonov.nyc3.
+00000d20: 6469 6769 7461 6c6f 6365 616e 7370 6163  digitaloceanspac
+00000d30: 6573 2e63 6f6d 2f6f 7065 6e2d 7061 7273  es.com/open-pars
+00000d40: 652f 756e 6974 6162 6c65 2d70 6172 7369  e/unitable-parsi
+00000d50: 6e67 2d73 616d 706c 652e 7765 6270 2220  ng-sample.webp" 
+00000d60: 7769 6474 683d 2236 3530 222f 3e0a 2020  width="650"/>.  
+00000d70: 2020 3c2f 703e 0a20 2020 2020 2020 2020    </p>.         
+00000d80: 3c62 722f 3e0a 2020 2020 3c2f 6465 7461  <br/>.    </deta
+00000d90: 696c 733e 0a0a 2d20 2a2a f09f 9ba0 efb8  ils>..- **......
+00000da0: 8f20 4578 7465 6e73 6962 6c65 3a2a 2a20  . Extensible:** 
+00000db0: 4561 7369 6c79 2069 6d70 6c65 6d65 6e74  Easily implement
+00000dc0: 2079 6f75 7220 6f77 6e20 706f 7374 2d70   your own post-p
+00000dd0: 726f 6365 7373 696e 6720 7374 6570 732e  rocessing steps.
+00000de0: 0a2d 202a 2af0 9f92 a149 6e74 7569 7469  .- **....Intuiti
+00000df0: 7665 3a2a 2a20 4772 6561 7420 6564 6974  ve:** Great edit
+00000e00: 6f72 2073 7570 706f 7274 2e20 436f 6d70  or support. Comp
+00000e10: 6c65 7469 6f6e 2065 7665 7279 7768 6572  letion everywher
+00000e20: 652e 204c 6573 7320 7469 6d65 2064 6562  e. Less time deb
+00000e30: 7567 6769 6e67 2e0a 2d20 2a2a f09f 8eaf  ugging..- **....
+00000e40: 2045 6173 793a 2a2a 2044 6573 6967 6e65   Easy:** Designe
+00000e50: 6420 746f 2062 6520 6561 7379 2074 6f20  d to be easy to 
+00000e60: 7573 6520 616e 6420 6c65 6172 6e2e 204c  use and learn. L
+00000e70: 6573 7320 7469 6d65 2072 6561 6469 6e67  ess time reading
+00000e80: 2064 6f63 732e 0a0a 3c62 722f 3e0a 3c70   docs...<br/>.<p
+00000e90: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000ea0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000eb0: 7474 7073 3a2f 2f73 6572 6765 792d 6669  ttps://sergey-fi
+00000ec0: 6c69 6d6f 6e6f 762e 6e79 6333 2e64 6967  limonov.nyc3.dig
+00000ed0: 6974 616c 6f63 6561 6e73 7061 6365 732e  italoceanspaces.
+00000ee0: 636f 6d2f 6f70 656e 2d70 6172 7365 2f6d  com/open-parse/m
+00000ef0: 6172 6b65 642d 7570 2d64 6f63 2d32 2e77  arked-up-doc-2.w
+00000f00: 6562 7022 2077 6964 7468 3d22 3235 3022  ebp" width="250"
+00000f10: 202f 3e0a 3c2f 703e 0a0a 2323 2045 7861   />.</p>..## Exa
+00000f20: 6d70 6c65 0a0a 2323 2323 2042 6173 6963  mple..#### Basic
+00000f30: 2045 7861 6d70 6c65 0a0a 6060 6070 7974   Example..```pyt
+00000f40: 686f 6e0a 696d 706f 7274 206f 7065 6e70  hon.import openp
+00000f50: 6172 7365 0a0a 6261 7369 635f 646f 635f  arse..basic_doc_
+00000f60: 7061 7468 203d 2022 2e2f 7361 6d70 6c65  path = "./sample
+00000f70: 2d64 6f63 732f 6d6f 6269 6c65 2d68 6f6d  -docs/mobile-hom
+00000f80: 652d 6d61 6e75 616c 2e70 6466 220a 7061  e-manual.pdf".pa
+00000f90: 7273 6572 203d 206f 7065 6e70 6172 7365  rser = openparse
+00000fa0: 2e44 6f63 756d 656e 7450 6172 7365 7228  .DocumentParser(
+00000fb0: 290a 7061 7273 6564 5f62 6173 6963 5f64  ).parsed_basic_d
+00000fc0: 6f63 203d 2070 6172 7365 722e 7061 7273  oc = parser.pars
+00000fd0: 6528 6261 7369 635f 646f 635f 7061 7468  e(basic_doc_path
+00000fe0: 290a 0a66 6f72 206e 6f64 6520 696e 2070  )..for node in p
+00000ff0: 6172 7365 645f 6261 7369 635f 646f 632e  arsed_basic_doc.
+00001000: 6e6f 6465 733a 0a20 2020 2070 7269 6e74  nodes:.    print
+00001010: 286e 6f64 6529 0a60 6060 0a0a 2a2a f09f  (node).```..**..
+00001020: 9393 2054 7279 2074 6865 2073 616d 706c  .. Try the sampl
+00001030: 6520 6e6f 7465 626f 6f6b 2a2a 203c 6120  e notebook** <a 
+00001040: 6872 6566 3d22 6874 7470 733a 2f2f 636f  href="https://co
+00001050: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+00001060: 676c 652e 636f 6d2f 6472 6976 652f 315a  gle.com/drive/1Z
+00001070: 3542 3567 736e 6d68 464b 4546 4c2d 3579  5B5gsnmhFKEFL-5y
+00001080: 5949 636f 6f78 372d 6a51 616f 3845 703f  YIcoox7-jQao8Ep?
+00001090: 7573 703d 7368 6172 696e 6722 2063 6c61  usp=sharing" cla
+000010a0: 7373 3d22 6578 7465 726e 616c 2d6c 696e  ss="external-lin
+000010b0: 6b22 2074 6172 6765 743d 225f 626c 616e  k" target="_blan
+000010c0: 6b22 3e68 6572 653c 2f61 3e0a 0a23 2323  k">here</a>..###
+000010d0: 2320 5365 6d61 6e74 6963 2050 726f 6365  # Semantic Proce
+000010e0: 7373 696e 6720 4578 616d 706c 650a 0a43  ssing Example..C
+000010f0: 6875 6e6b 696e 6720 646f 6375 6d65 6e74  hunking document
+00001100: 7320 6973 2066 756e 6461 6d65 6e74 616c  s is fundamental
+00001110: 6c79 2061 626f 7574 2067 726f 7570 696e  ly about groupin
+00001120: 6720 7369 6d69 6c61 7220 7365 6d61 6e74  g similar semant
+00001130: 6963 206e 6f64 6573 2074 6f67 6574 6865  ic nodes togethe
+00001140: 722e 2042 7920 656d 6265 6464 696e 6720  r. By embedding 
+00001150: 7468 6520 7465 7874 206f 6620 6561 6368  the text of each
+00001160: 206e 6f64 652c 2077 6520 6361 6e20 7468   node, we can th
+00001170: 656e 2063 6c75 7374 6572 2074 6865 6d20  en cluster them 
+00001180: 746f 6765 7468 6572 2062 6173 6564 206f  together based o
+00001190: 6e20 7468 6569 7220 7369 6d69 6c61 7269  n their similari
+000011a0: 7479 2e0a 0a60 6060 7079 7468 6f6e 0a66  ty...```python.f
+000011b0: 726f 6d20 6f70 656e 7061 7273 6520 696d  rom openparse im
+000011c0: 706f 7274 2070 726f 6365 7373 696e 672c  port processing,
+000011d0: 2044 6f63 756d 656e 7450 6172 7365 720a   DocumentParser.
+000011e0: 0a73 656d 616e 7469 635f 7069 7065 6c69  .semantic_pipeli
+000011f0: 6e65 203d 2070 726f 6365 7373 696e 672e  ne = processing.
+00001200: 5365 6d61 6e74 6963 496e 6765 7374 696f  SemanticIngestio
+00001210: 6e50 6970 656c 696e 6528 0a20 2020 206f  nPipeline(.    o
+00001220: 7065 6e61 695f 6170 695f 6b65 793d 4f50  penai_api_key=OP
+00001230: 454e 5f41 495f 4b45 592c 0a20 2020 206d  EN_AI_KEY,.    m
+00001240: 6f64 656c 3d22 7465 7874 2d65 6d62 6564  odel="text-embed
+00001250: 6469 6e67 2d33 2d6c 6172 6765 222c 0a20  ding-3-large",. 
+00001260: 2020 206d 696e 5f74 6f6b 656e 733d 3634     min_tokens=64
+00001270: 2c0a 2020 2020 6d61 785f 746f 6b65 6e73  ,.    max_tokens
+00001280: 3d31 3032 342c 0a29 0a70 6172 7365 7220  =1024,.).parser 
+00001290: 3d20 446f 6375 6d65 6e74 5061 7273 6572  = DocumentParser
+000012a0: 280a 2020 2020 7072 6f63 6573 7369 6e67  (.    processing
+000012b0: 5f70 6970 656c 696e 653d 7365 6d61 6e74  _pipeline=semant
+000012c0: 6963 5f70 6970 656c 696e 652c 0a29 0a70  ic_pipeline,.).p
+000012d0: 6172 7365 645f 636f 6e74 656e 7420 3d20  arsed_content = 
+000012e0: 7061 7273 6572 2e70 6172 7365 2862 6173  parser.parse(bas
+000012f0: 6963 5f64 6f63 5f70 6174 6829 0a60 6060  ic_doc_path).```
+00001300: 0a0a 2a2a f09f 9393 2053 616d 706c 6520  ..**.... Sample 
+00001310: 6e6f 7465 626f 6f6b 2a2a 203c 6120 6872  notebook** <a hr
+00001320: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001330: 7562 2e63 6f6d 2f46 696c 696d 6f61 2f6f  ub.com/Filimoa/o
+00001340: 7065 6e2d 7061 7273 652f 626c 6f62 2f6d  pen-parse/blob/m
+00001350: 6169 6e2f 7372 632f 636f 6f6b 626f 6f6b  ain/src/cookbook
+00001360: 732f 7365 6d61 6e74 6963 5f70 726f 6365  s/semantic_proce
+00001370: 7373 696e 672e 6970 796e 6222 2063 6c61  ssing.ipynb" cla
+00001380: 7373 3d22 6578 7465 726e 616c 2d6c 696e  ss="external-lin
+00001390: 6b22 2074 6172 6765 743d 225f 626c 616e  k" target="_blan
+000013a0: 6b22 3e68 6572 653c 2f61 3e0a 0a23 2323  k">here</a>..###
+000013b0: 2320 5365 7269 616c 697a 696e 6720 5265  # Serializing Re
+000013c0: 7375 6c74 730a 5573 6573 2070 7964 616e  sults.Uses pydan
+000013d0: 7469 6320 756e 6465 7220 7468 6520 686f  tic under the ho
+000013e0: 6f64 2073 6f20 796f 7520 6361 6e20 7365  od so you can se
+000013f0: 7269 616c 697a 6520 7265 7375 6c74 7320  rialize results 
+00001400: 7769 7468 200a 0a60 6060 7079 7468 6f6e  with ..```python
+00001410: 0a70 6172 7365 645f 636f 6e74 656e 742e  .parsed_content.
+00001420: 6469 6374 2829 0a0a 2320 6f72 2074 6f20  dict()..# or to 
+00001430: 636f 6e76 6572 7420 746f 2061 2076 616c  convert to a val
+00001440: 6964 206a 736f 6e20 6469 6374 0a70 6172  id json dict.par
+00001450: 7365 645f 636f 6e74 656e 742e 6a73 6f6e  sed_content.json
+00001460: 2829 0a60 6060 0a0a 2323 2052 6571 7569  ().```..## Requi
+00001470: 7265 6d65 6e74 730a 0a50 7974 686f 6e20  rements..Python 
+00001480: 332e 382b 0a0a 2a2a 4465 616c 696e 6720  3.8+..**Dealing 
+00001490: 7769 7468 2050 4446 2773 3a2a 2a0a 0a2d  with PDF's:**..-
+000014a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000014b0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6466  //github.com/pdf
+000014c0: 6d69 6e65 722f 7064 666d 696e 6572 2e73  miner/pdfminer.s
+000014d0: 6978 2220 636c 6173 733d 2265 7874 6572  ix" class="exter
+000014e0: 6e61 6c2d 6c69 6e6b 2220 7461 7267 6574  nal-link" target
+000014f0: 3d22 5f62 6c61 6e6b 223e 7064 666d 696e  ="_blank">pdfmin
+00001500: 6572 2e73 6978 3c2f 613e 2046 756c 6c79  er.six</a> Fully
+00001510: 206f 7065 6e20 736f 7572 6365 2e0a 0a2a   open source...*
+00001520: 2a45 7874 7261 6374 696e 6720 5461 626c  *Extracting Tabl
+00001530: 6573 3a2a 2a0a 0a2d 203c 6120 6872 6566  es:**..- <a href
+00001540: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00001550: 2e63 6f6d 2f70 796d 7570 6466 2f50 794d  .com/pymupdf/PyM
+00001560: 7550 4446 2220 636c 6173 733d 2265 7874  uPDF" class="ext
+00001570: 6572 6e61 6c2d 6c69 6e6b 2220 7461 7267  ernal-link" targ
+00001580: 6574 3d22 5f62 6c61 6e6b 223e 5079 4d75  et="_blank">PyMu
+00001590: 5044 463c 2f61 3e20 6861 7320 736f 6d65  PDF</a> has some
+000015a0: 2074 6162 6c65 2064 6574 6563 7469 6f6e   table detection
+000015b0: 2066 756e 6374 696f 6e61 6c69 7479 2e20   functionality. 
+000015c0: 506c 6561 7365 2073 6565 2074 6865 6972  Please see their
+000015d0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000015e0: 2f2f 6d75 7064 662e 636f 6d2f 6c69 6365  //mupdf.com/lice
+000015f0: 6e73 696e 672f 696e 6465 782e 6874 6d6c  nsing/index.html
+00001600: 2363 6f6d 6d65 7263 6961 6c22 2063 6c61  #commercial" cla
+00001610: 7373 3d22 6578 7465 726e 616c 2d6c 696e  ss="external-lin
+00001620: 6b22 2074 6172 6765 743d 225f 626c 616e  k" target="_blan
+00001630: 6b22 3e6c 6963 656e 7365 3c2f 613e 2e0a  k">license</a>..
+00001640: 2d20 3c61 2068 7265 663d 2268 7474 7073  - <a href="https
+00001650: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00001660: 6f2f 6d69 6372 6f73 6f66 742f 7461 626c  o/microsoft/tabl
+00001670: 652d 7472 616e 7366 6f72 6d65 722d 6465  e-transformer-de
+00001680: 7465 6374 696f 6e22 2063 6c61 7373 3d22  tection" class="
+00001690: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
+000016a0: 6172 6765 743d 225f 626c 616e 6b22 3e54  arget="_blank">T
+000016b0: 6162 6c65 2054 7261 6e73 666f 726d 6572  able Transformer
+000016c0: 3c2f 613e 2069 7320 6120 6465 6570 206c  </a> is a deep l
+000016d0: 6561 726e 696e 6720 6170 7072 6f61 6368  earning approach
+000016e0: 2e0a 2d20 3c61 2068 7265 663d 2268 7474  ..- <a href="htt
+000016f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001700: 706f 6c6f 636c 7562 2f75 6e69 7461 626c  poloclub/unitabl
+00001710: 6522 2063 6c61 7373 3d22 6578 7465 726e  e" class="extern
+00001720: 616c 2d6c 696e 6b22 2074 6172 6765 743d  al-link" target=
+00001730: 225f 626c 616e 6b22 3e75 6e69 7461 626c  "_blank">unitabl
+00001740: 653c 2f61 3e20 6973 2061 6e6f 7468 6572  e</a> is another
+00001750: 2074 7261 6e73 666f 726d 6572 7320 6261   transformers ba
+00001760: 7365 6420 6170 7072 6f61 6368 2077 6974  sed approach wit
+00001770: 6820 2a2a 7374 6174 652d 6f66 2d74 6865  h **state-of-the
+00001780: 2d61 7274 2a2a 2070 6572 666f 726d 616e  -art** performan
+00001790: 6365 2e0a 0a23 2320 496e 7374 616c 6c61  ce...## Installa
+000017a0: 7469 6f6e 0a0a 2323 2323 2031 2e20 436f  tion..#### 1. Co
+000017b0: 7265 204c 6962 7261 7279 0a0a 6060 6063  re Library..```c
+000017c0: 6f6e 736f 6c65 0a70 6970 2069 6e73 7461  onsole.pip insta
+000017d0: 6c6c 206f 7065 6e70 6172 7365 0a60 6060  ll openparse.```
+000017e0: 0a0a 2a2a 456e 6162 6c69 6e67 204f 4352  ..**Enabling OCR
+000017f0: 2053 7570 706f 7274 2a2a 3a0a 0a50 794d   Support**:..PyM
+00001800: 7550 4446 2077 696c 6c20 616c 7265 6164  uPDF will alread
+00001810: 7920 636f 6e74 6169 6e20 616c 6c20 7468  y contain all th
+00001820: 6520 6c6f 6769 6320 746f 2073 7570 706f  e logic to suppo
+00001830: 7274 204f 4352 2066 756e 6374 696f 6e73  rt OCR functions
+00001840: 2e20 4275 7420 6974 2061 6464 6974 696f  . But it additio
+00001850: 6e61 6c6c 7920 646f 6573 206e 6565 6420  nally does need 
+00001860: 5465 7373 6572 6163 74e2 8099 7320 6c61  Tesseract...s la
+00001870: 6e67 7561 6765 2073 7570 706f 7274 2064  nguage support d
+00001880: 6174 612c 2073 6f20 696e 7374 616c 6c61  ata, so installa
+00001890: 7469 6f6e 206f 6620 5465 7373 6572 6163  tion of Tesserac
+000018a0: 742d 4f43 5220 6973 2073 7469 6c6c 2072  t-OCR is still r
+000018b0: 6571 7569 7265 642e 0a0a 5468 6520 6c61  equired...The la
+000018c0: 6e67 7561 6765 2073 7570 706f 7274 2066  nguage support f
+000018d0: 6f6c 6465 7220 6c6f 6361 7469 6f6e 206d  older location m
+000018e0: 7573 7420 6265 2063 6f6d 6d75 6e69 6361  ust be communica
+000018f0: 7465 6420 6569 7468 6572 2076 6961 2073  ted either via s
+00001900: 746f 7269 6e67 2069 7420 696e 2074 6865  toring it in the
+00001910: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00001920: 6961 626c 6520 2254 4553 5344 4154 415f  iable "TESSDATA_
+00001930: 5052 4546 4958 222c 206f 7220 6173 2061  PREFIX", or as a
+00001940: 2070 6172 616d 6574 6572 2069 6e20 7468   parameter in th
+00001950: 6520 6170 706c 6963 6162 6c65 2066 756e  e applicable fun
+00001960: 6374 696f 6e73 2e0a 0a53 6f20 666f 7220  ctions...So for 
+00001970: 6120 776f 726b 696e 6720 4f43 5220 6675  a working OCR fu
+00001980: 6e63 7469 6f6e 616c 6974 792c 206d 616b  nctionality, mak
+00001990: 6520 7375 7265 2074 6f20 636f 6d70 6c65  e sure to comple
+000019a0: 7465 2074 6869 7320 6368 6563 6b6c 6973  te this checklis
+000019b0: 743a 0a0a 312e 2049 6e73 7461 6c6c 2054  t:..1. Install T
+000019c0: 6573 7365 7261 6374 2e0a 0a32 2e20 4c6f  esseract...2. Lo
+000019d0: 6361 7465 2054 6573 7365 7261 6374 e280  cate Tesseract..
+000019e0: 9973 206c 616e 6775 6167 6520 7375 7070  .s language supp
+000019f0: 6f72 7420 666f 6c64 6572 2e20 5479 7069  ort folder. Typi
+00001a00: 6361 6c6c 7920 796f 7520 7769 6c6c 2066  cally you will f
+00001a10: 696e 6420 6974 2068 6572 653a 0a0a 2020  ind it here:..  
+00001a20: 202d 2057 696e 646f 7773 3a20 6043 3a2f   - Windows: `C:/
+00001a30: 5072 6f67 7261 6d20 4669 6c65 732f 5465  Program Files/Te
+00001a40: 7373 6572 6163 742d 4f43 522f 7465 7373  sseract-OCR/tess
+00001a50: 6461 7461 600a 0a20 2020 2d20 556e 6978  data`..   - Unix
+00001a60: 2073 7973 7465 6d73 3a20 602f 7573 722f   systems: `/usr/
+00001a70: 7368 6172 652f 7465 7373 6572 6163 742d  share/tesseract-
+00001a80: 6f63 722f 352f 7465 7373 6461 7461 600a  ocr/5/tessdata`.
+00001a90: 0a33 2e20 5365 7420 7468 6520 656e 7669  .3. Set the envi
+00001aa0: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00001ab0: 2054 4553 5344 4154 415f 5052 4546 4958   TESSDATA_PREFIX
+00001ac0: 0a0a 2020 202d 2057 696e 646f 7773 3a20  ..   - Windows: 
+00001ad0: 6073 6574 7820 5445 5353 4441 5441 5f50  `setx TESSDATA_P
+00001ae0: 5245 4649 5820 2243 3a2f 5072 6f67 7261  REFIX "C:/Progra
+00001af0: 6d20 4669 6c65 732f 5465 7373 6572 6163  m Files/Tesserac
+00001b00: 742d 4f43 522f 7465 7373 6461 7461 2260  t-OCR/tessdata"`
+00001b10: 0a0a 2020 202d 2055 6e69 7820 7379 7374  ..   - Unix syst
+00001b20: 656d 733a 2060 6465 636c 6172 6520 2d78  ems: `declare -x
+00001b30: 2054 4553 5344 4154 415f 5052 4546 4958   TESSDATA_PREFIX
+00001b40: 3d20 2f75 7372 2f73 6861 7265 2f74 6573  = /usr/share/tes
+00001b50: 7365 7261 6374 2d6f 6372 2f35 2f74 6573  seract-ocr/5/tes
+00001b60: 7364 6174 6160 0a0a 2a2a 4e6f 7465 3a2a  sdata`..**Note:*
+00001b70: 2a20 5f4f 6e20 5769 6e64 6f77 7320 7379  * _On Windows sy
+00001b80: 7374 656d 732c 2074 6869 7320 6d75 7374  stems, this must
+00001b90: 2068 6170 7065 6e20 6f75 7473 6964 6520   happen outside 
+00001ba0: 5079 7468 6f6e 20e2 8093 2062 6566 6f72  Python ... befor
+00001bb0: 6520 7374 6172 7469 6e67 2079 6f75 7220  e starting your 
+00001bc0: 7363 7269 7074 2e20 4a75 7374 206d 616e  script. Just man
+00001bd0: 6970 756c 6174 696e 6720 6f73 2e65 6e76  ipulating os.env
+00001be0: 6972 6f6e 2077 696c 6c20 6e6f 7420 776f  iron will not wo
+00001bf0: 726b 215f 0a0a 2323 2323 2032 2e20 4d4c  rk!_..#### 2. ML
+00001c00: 2054 6162 6c65 2044 6574 6563 7469 6f6e   Table Detection
+00001c10: 2028 4f70 7469 6f6e 616c 290a 0a54 6869   (Optional)..Thi
+00001c20: 7320 7265 706f 7369 746f 7279 2070 726f  s repository pro
+00001c30: 7669 6465 7320 616e 206f 7074 696f 6e61  vides an optiona
+00001c40: 6c20 6665 6174 7572 6520 746f 2070 6172  l feature to par
+00001c50: 7365 2063 6f6e 7465 6e74 2066 726f 6d20  se content from 
+00001c60: 7461 626c 6573 2075 7369 6e67 2061 2076  tables using a v
+00001c70: 6172 6965 7479 206f 6620 6465 6570 206c  ariety of deep l
+00001c80: 6561 726e 696e 6720 6d6f 6465 6c73 2e0a  earning models..
+00001c90: 0a60 6060 636f 6e73 6f6c 650a 7069 7020  .```console.pip 
+00001ca0: 696e 7374 616c 6c20 226f 7065 6e70 6172  install "openpar
+00001cb0: 7365 5b6d 6c5d 220a 6060 600a 0a54 6865  se[ml]".```..The
+00001cc0: 6e20 646f 776e 6c6f 6164 2074 6865 206d  n download the m
+00001cd0: 6f64 656c 2077 6569 6768 7473 2077 6974  odel weights wit
+00001ce0: 680a 0a60 6060 636f 6e73 6f6c 650a 6f70  h..```console.op
+00001cf0: 656e 7061 7273 652d 646f 776e 6c6f 6164  enparse-download
+00001d00: 0a60 6060 0a0a 596f 7520 6361 6e20 7275  .```..You can ru
+00001d10: 6e20 7468 6520 7061 7273 696e 6720 7769  n the parsing wi
+00001d20: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
+00001d30: 2e20 0a0a 6060 6070 7974 686f 6e0a 7061  . ..```python.pa
+00001d40: 7273 6572 203d 206f 7065 6e70 6172 7365  rser = openparse
+00001d50: 2e44 6f63 756d 656e 7450 6172 7365 7228  .DocumentParser(
+00001d60: 0a20 2020 2020 2020 2074 6162 6c65 5f61  .        table_a
+00001d70: 7267 733d 7b0a 2020 2020 2020 2020 2020  rgs={.          
+00001d80: 2020 2270 6172 7369 6e67 5f61 6c67 6f72    "parsing_algor
+00001d90: 6974 686d 223a 2022 756e 6974 6162 6c65  ithm": "unitable
+00001da0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00001db0: 6d69 6e5f 7461 626c 655f 636f 6e66 6964  min_table_confid
+00001dc0: 656e 6365 223a 2030 2e38 2c0a 2020 2020  ence": 0.8,.    
+00001dd0: 2020 2020 7d2c 0a29 0a70 6172 7365 645f      },.).parsed_
+00001de0: 6e6f 6465 7320 3d20 7061 7273 6572 2e70  nodes = parser.p
+00001df0: 6172 7365 2870 6466 5f70 6174 6829 0a60  arse(pdf_path).`
+00001e00: 6060 0a0a 4e6f 7465 2077 6520 6375 7272  ``..Note we curr
+00001e10: 656e 746c 7920 7573 6520 5b74 6162 6c65  ently use [table
+00001e20: 2d74 7261 6e73 666f 726d 6572 735d 2868  -transformers](h
+00001e30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001e40: 6d2f 6d69 6372 6f73 6f66 742f 7461 626c  m/microsoft/tabl
+00001e50: 652d 7472 616e 7366 6f72 6d65 7229 2066  e-transformer) f
+00001e60: 6f72 2061 6c6c 2074 6162 6c65 2064 6574  or all table det
+00001e70: 6563 7469 6f6e 2061 6e64 2077 6520 6669  ection and we fi
+00001e80: 6e64 2069 7473 2070 6572 666f 726d 616e  nd its performan
+00001e90: 6365 2074 6f20 6265 2073 7562 7061 722e  ce to be subpar.
+00001ea0: 2054 6869 7320 6e65 6761 7469 7665 6c79   This negatively
+00001eb0: 2061 6666 6563 7473 2074 6865 2064 6f77   affects the dow
+00001ec0: 6e73 7472 6561 6d20 7265 7375 6c74 7320  nstream results 
+00001ed0: 6f66 2075 6e69 7461 626c 652e 2049 6620  of unitable. If 
+00001ee0: 796f 7527 7265 2061 7761 7265 206f 6620  you're aware of 
+00001ef0: 6120 6265 7474 6572 206d 6f64 656c 2070  a better model p
+00001f00: 6c65 6173 6520 6f70 656e 2061 6e20 4973  lease open an Is
+00001f10: 7375 6520 2d20 7468 6520 756e 6974 6162  sue - the unitab
+00001f20: 6c65 2074 6561 6d20 6d65 6e74 696f 6e65  le team mentione
+00001f30: 6420 7468 6579 206d 6967 6874 2061 6464  d they might add
+00001f40: 2074 6869 7320 736f 6f6e 2074 6f6f 2e0a   this soon too..
+00001f50: 0a23 2320 436f 6f6b 626f 6f6b 730a 0a68  .## Cookbooks..h
+00001f60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001f70: 6d2f 4669 6c69 6d6f 612f 6f70 656e 2d70  m/Filimoa/open-p
+00001f80: 6172 7365 2f74 7265 652f 6d61 696e 2f73  arse/tree/main/s
+00001f90: 7263 2f63 6f6f 6b62 6f6f 6b73 0a0a 2323  rc/cookbooks..##
+00001fa0: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
+00001fb0: 6874 7470 733a 2f2f 6669 6c69 6d6f 612e  https://filimoa.
+00001fc0: 6769 7468 7562 2e69 6f2f 6f70 656e 2d70  github.io/open-p
+00001fd0: 6172 7365 2f0a 0a23 2320 5370 6f6e 736f  arse/..## Sponso
+00001fe0: 7273 0a0a 3c21 2d2d 2073 706f 6e73 6f72  rs..<!-- sponsor
+00001ff0: 7320 2d2d 3e0a 0a3c 6120 6872 6566 3d22  s -->..<a href="
+00002000: 6874 7470 733a 2f2f 7777 772e 6461 7461  https://www.data
+00002010: 2e74 6872 6565 7369 676d 612e 6169 2f66  .threesigma.ai/f
+00002020: 696c 696e 6773 2d61 6922 2074 6172 6765  ilings-ai" targe
+00002030: 743d 225f 626c 616e 6b22 2074 6974 6c65  t="_blank" title
+00002040: 3d22 5468 7265 6520 5369 676d 613a 2041  ="Three Sigma: A
+00002050: 4920 666f 7220 696e 7375 7261 6e63 6520  I for insurance 
+00002060: 6669 6c69 6e67 732e 223e 3c69 6d67 2073  filings."><img s
+00002070: 7263 3d22 6874 7470 733a 2f2f 7365 7267  rc="https://serg
+00002080: 6579 2d66 696c 696d 6f6e 6f76 2e6e 7963  ey-filimonov.nyc
+00002090: 332e 6469 6769 7461 6c6f 6365 616e 7370  3.digitaloceansp
+000020a0: 6163 6573 2e63 6f6d 2f6f 7065 6e2d 7061  aces.com/open-pa
+000020b0: 7273 652f 6d61 726b 6574 696e 672f 7468  rse/marketing/th
+000020c0: 7265 652d 7369 676d 612d 7769 6465 2e70  ree-sigma-wide.p
+000020d0: 6e67 2220 7769 6474 683d 2232 3530 223e  ng" width="250">
+000020e0: 3c2f 613e 0a0a 3c21 2d2d 202f 7370 6f6e  </a>..<!-- /spon
+000020f0: 736f 7273 202d 2d3e 0a0a 446f 6573 2079  sors -->..Does y
+00002100: 6f75 7220 7573 6520 6361 7365 206e 6565  our use case nee
+00002110: 6420 736f 6d65 7468 696e 6720 7370 6563  d something spec
+00002120: 6961 6c3f 2052 6561 6368 205b 6f75 745d  ial? Reach [out]
+00002130: 2868 7474 7073 3a2f 2f77 7777 2e6c 696e  (https://www.lin
+00002140: 6b65 6469 6e2e 636f 6d2f 696e 2f73 6572  kedin.com/in/ser
+00002150: 6765 792d 6f73 752f 292e 0a              gey-osu/)..
```

### Comparing `openparse-0.5.1/src/openparse.egg-info/SOURCES.txt` & `openparse-0.5.2/src/openparse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 src/evals/__init__.py
 src/evals/run_evals.py
-src/notebooks/config.py
-src/notebooks/trash.py
 src/openparse/__init__.py
 src/openparse/cli.py
+src/openparse/config.py
 src/openparse/consts.py
 src/openparse/doc_parser.py
 src/openparse/pdf.py
 src/openparse/schemas.py
 src/openparse/types.py
 src/openparse/utils.py
+src/openparse/version.py
 src/openparse.egg-info/PKG-INFO
 src/openparse.egg-info/SOURCES.txt
 src/openparse.egg-info/dependency_links.txt
 src/openparse.egg-info/entry_points.txt
 src/openparse.egg-info/requires.txt
 src/openparse.egg-info/top_level.txt
 src/openparse/processing/__init__.py
```

### Comparing `openparse-0.5.1/src/tests/processing/test_pipeline.py` & `openparse-0.5.2/src/tests/processing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/processing/test_steps.py` & `openparse-0.5.2/src/tests/processing/test_steps.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/tables/pymupdf/test_parse.py` & `openparse-0.5.2/src/tests/tables/pymupdf/test_parse.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/tables/transformers/test_geometry.py` & `openparse-0.5.2/src/tests/tables/transformers/test_geometry.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/tables/transformers/test_ml.py` & `openparse-0.5.2/src/tests/tables/transformers/test_ml.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/tables/unitable/sample_pred_outputs.py` & `openparse-0.5.2/src/tests/tables/unitable/sample_pred_outputs.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/tables/unitable/test_pred_to_schema.py` & `openparse-0.5.2/src/tests/tables/unitable/test_pred_to_schema.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/test_doc_parser.py` & `openparse-0.5.2/src/tests/test_doc_parser.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/test_schemas.py` & `openparse-0.5.2/src/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openparse-0.5.1/src/tests/text/pdf_miner/test_core.py` & `openparse-0.5.2/src/tests/text/pdf_miner/test_core.py`

 * *Files identical despite different names*

