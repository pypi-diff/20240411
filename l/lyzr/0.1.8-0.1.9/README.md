# Comparing `tmp/lyzr-0.1.8.tar.gz` & `tmp/lyzr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyzr-0.1.8.tar", last modified: Wed Nov 15 09:40:24 2023, max compression
+gzip compressed data, was "lyzr-0.1.9.tar", last modified: Thu Nov 16 07:35:45 2023, max compression
```

## Comparing `lyzr-0.1.8.tar` & `lyzr-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)       32 2023-11-13 20:12:06.000000 lyzr-0.1.8/MANIFEST.in
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     2751 2023-11-15 09:40:24.590011 lyzr-0.1.8/PKG-INFO
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     1915 2023-11-13 20:12:06.000000 lyzr-0.1.8/README.md
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.580011 lyzr-0.1.8/lyzr/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      601 2023-11-15 09:06:12.000000 lyzr-0.1.8/lyzr/__init__.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/lyzr/base/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      417 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/__init__.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      861 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/errors.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     2463 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/file_utils.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      279 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/llm.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     5303 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/llms.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/lyzr/base/prompts/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     1552 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/prompts/analysis_pt.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      765 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/prompts/dataset_description_pt.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      744 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/prompts/insights_pt.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     1471 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/prompts/make_analysis_query_pt.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      799 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/prompts/manual_input_pt.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      921 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/prompts/query_gen_pt.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     1194 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/prompts/recommendations_pt.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     1376 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/prompts/tasks_pt.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     1473 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/service.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     3201 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/base/vector_store.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/lyzr/chatqa/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      109 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/chatqa/__init__.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     6636 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/chatqa/chatbot.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     6624 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/chatqa/qa_bot.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/lyzr/data_analyzr/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)       81 2023-11-15 09:06:12.000000 lyzr-0.1.8/lyzr/data_analyzr/__init__.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     5260 2023-11-15 09:06:12.000000 lyzr-0.1.8/lyzr/data_analyzr/data_analyzr.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/lyzr/formula_generator/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)       90 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/formula_generator/__init__.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     9478 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/formula_generator/formula_generator.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/lyzr/generator/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)       73 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/generator/__init__.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     6729 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/generator/_generator.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/lyzr/utils/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      421 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/__init__.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     9746 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/chat_utils.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)        0 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/constants.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)        0 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/db_utils.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     3260 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/document_reading.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      722 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/docx_reader.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)        0 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/env_utils.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      209 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/llm_utils.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      721 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/pdf_reader.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     9516 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/rag_utils.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      602 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/templates.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      713 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/txt_reader.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     1580 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/webpage_reader.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      924 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/website_reader.py
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      452 2023-11-13 20:12:06.000000 lyzr-0.1.8/lyzr/utils/youtube_reader.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/lyzr.egg-info/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     2751 2023-11-15 09:40:24.000000 lyzr-0.1.8/lyzr.egg-info/PKG-INFO
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)     1308 2023-11-15 09:40:24.000000 lyzr-0.1.8/lyzr.egg-info/SOURCES.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)        1 2023-11-15 09:40:24.000000 lyzr-0.1.8/lyzr.egg-info/dependency_links.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      261 2023-11-15 09:40:24.000000 lyzr-0.1.8/lyzr.egg-info/requires.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)       11 2023-11-15 09:40:24.000000 lyzr-0.1.8/lyzr.egg-info/top_level.txt
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)       38 2023-11-15 09:40:24.590011 lyzr-0.1.8/setup.cfg
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)      964 2023-11-15 09:40:11.000000 lyzr-0.1.8/setup.py
-drwxr-xr-x   0 lyzr      (1000) lyzr      (1000)        0 2023-11-15 09:40:24.590011 lyzr-0.1.8/tests/
--rw-r--r--   0 lyzr      (1000) lyzr      (1000)        0 2023-11-13 20:12:06.000000 lyzr-0.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.128141 lyzr-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-11-16 07:35:32.000000 lyzr-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 07:35:32.000000 lyzr-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-11-16 07:35:45.128141 lyzr-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2023-11-16 07:35:32.000000 lyzr-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.124141 lyzr-0.1.9/lyzr/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.124141 lyzr-0.1.9/lyzr/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/llms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.124141 lyzr-0.1.9/lyzr/base/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/prompts/analysis_pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/prompts/dataset_description_pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/prompts/insights_pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/prompts/make_analysis_query_pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/prompts/manual_input_pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/prompts/query_gen_pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/prompts/recommendations_pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/prompts/tasks_pt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/base/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.124141 lyzr-0.1.9/lyzr/chatqa/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/chatqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/chatqa/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/chatqa/qa_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.124141 lyzr-0.1.9/lyzr/csv_analyzr/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/csv_analyzr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/csv_analyzr/csv_analyzr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.124141 lyzr-0.1.9/lyzr/formula_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/formula_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/formula_generator/formula_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.128141 lyzr-0.1.9/lyzr/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/generator/_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.128141 lyzr-0.1.9/lyzr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/chat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/document_reading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/docx_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/pdf_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/rag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/txt_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/webpage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/website_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-16 07:35:32.000000 lyzr-0.1.9/lyzr/utils/youtube_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.124141 lyzr-0.1.9/lyzr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-11-16 07:35:45.000000 lyzr-0.1.9/lyzr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-11-16 07:35:45.000000 lyzr-0.1.9/lyzr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 07:35:45.000000 lyzr-0.1.9/lyzr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2023-11-16 07:35:45.000000 lyzr-0.1.9/lyzr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-16 07:35:45.000000 lyzr-0.1.9/lyzr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 07:35:45.128141 lyzr-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2023-11-16 07:35:32.000000 lyzr-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:45.128141 lyzr-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 07:35:32.000000 lyzr-0.1.9/tests/__init__.py
```

### Comparing `lyzr-0.1.8/PKG-INFO` & `lyzr-0.1.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,59 @@
-Metadata-Version: 2.1
-Name: lyzr
-Version: 0.1.8
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: lyzr
-License: UNKNOWN
-Description: # lyzr
-        
-        Lyzr AI is a set of super abstracted LLM SDKs for rapid generative AI application development (RAD) that comes with Lyzr Enterprise Hub – a control center with an AI-only Data Lake and IAM for administering the AI applications built with Lyzr SDKs. Available both as open-source and enterprise SDKs.
-        
-        Lyzr SDKs helps you build all your favorite GenAI SaaS products as enterprise applications in minutes. It is the enterprise alternative to popular in-demand Generative AI SaaS products like Mendable, PDF.ai, Chatbase.co, SiteGPT.ai, Julius.ai and more.
-        
-        [![PyPI - Version](https://img.shields.io/pypi/v/lyzr.svg)](https://pypi.org/project/lyzr/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lyzr.svg)](https://pypi.org/project/lyzr)
-        
-        -----
-        
-        **Table of Contents**
-        
-        - [Installation](#installation)
-        - [Building from Source](#building-from-source)
-        - [License](#license)
-        
-        ## Installation
-        
-        You can install the `lyzr` package directly from PyPI:
-        
-        ```console
-        pip install lyzr
-        ```
-        
-        ## Building from Source
-        
-        If you prefer to build the `lyzr` package from source, you'll need to have Python installed along with `setuptools` and `wheel`. 
-        
-        ### Steps to Build:
-        
-        1. Clone the repository or download the source code.
-        2. Navigate to the root directory of the project (where `setup.py` is located).
-        3. Run the following commands:
-        
-        ```console
-        # Ensure setuptools and wheel are installed
-        pip install setuptools wheel
-        
-        # Build the package
-        python setup.py sdist bdist_wheel
-        ```
-        
-        This will generate a `dist` directory containing the built package files.
-        
-        ### Installing the Built Package:
-        
-        Once you've built the package, you can install it using pip:
-        
-        ```console
-        cd dist/
-        pip install lyzr-[version]-py3-none-any.whl
-        ```
-        
-        Replace `[version]` with the actual version of the package you have built.
-        
-        ## License
-        
-        `lyzr` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.1, <3.12
-Description-Content-Type: text/markdown
+# lyzr
+
+Lyzr AI is a set of super abstracted LLM SDKs for rapid generative AI application development (RAD) that comes with Lyzr Enterprise Hub – a control center with an AI-only Data Lake and IAM for administering the AI applications built with Lyzr SDKs. Available both as open-source and enterprise SDKs.
+
+Lyzr SDKs helps you build all your favorite GenAI SaaS products as enterprise applications in minutes. It is the enterprise alternative to popular in-demand Generative AI SaaS products like Mendable, PDF.ai, Chatbase.co, SiteGPT.ai, Julius.ai and more.
+
+[![PyPI - Version](https://img.shields.io/pypi/v/lyzr.svg)](https://pypi.org/project/lyzr/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lyzr.svg)](https://pypi.org/project/lyzr)
+
+-----
+
+**Table of Contents**
+
+- [Installation](#installation)
+- [Building from Source](#building-from-source)
+- [License](#license)
+
+## Installation
+
+You can install the `lyzr` package directly from PyPI:
+
+```console
+pip install lyzr
+```
+
+## Building from Source
+
+If you prefer to build the `lyzr` package from source, you'll need to have Python installed along with `setuptools` and `wheel`. 
+
+### Steps to Build:
+
+1. Clone the repository or download the source code.
+2. Navigate to the root directory of the project (where `setup.py` is located).
+3. Run the following commands:
+
+```console
+# Ensure setuptools and wheel are installed
+pip install setuptools wheel
+
+# Build the package
+python setup.py sdist bdist_wheel
+```
+
+This will generate a `dist` directory containing the built package files.
+
+### Installing the Built Package:
+
+Once you've built the package, you can install it using pip:
+
+```console
+cd dist/
+pip install lyzr-[version]-py3-none-any.whl
+```
+
+Replace `[version]` with the actual version of the package you have built.
+
+## License
+
+`lyzr` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `lyzr-0.1.8/README.md` & `lyzr-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: lyzr
+Version: 0.1.9
+Home-page: 
+Author: lyzr
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8.1, <3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # lyzr
 
 Lyzr AI is a set of super abstracted LLM SDKs for rapid generative AI application development (RAD) that comes with Lyzr Enterprise Hub – a control center with an AI-only Data Lake and IAM for administering the AI applications built with Lyzr SDKs. Available both as open-source and enterprise SDKs.
 
 Lyzr SDKs helps you build all your favorite GenAI SaaS products as enterprise applications in minutes. It is the enterprise alternative to popular in-demand Generative AI SaaS products like Mendable, PDF.ai, Chatbase.co, SiteGPT.ai, Julius.ai and more.
 
 [![PyPI - Version](https://img.shields.io/pypi/v/lyzr.svg)](https://pypi.org/project/lyzr/)
```

### Comparing `lyzr-0.1.8/lyzr/__init__.py` & `lyzr-0.1.9/lyzr/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from lyzr.generator import Generator
 from lyzr.chatqa.chatbot import ChatBot
 from lyzr.base.llm import LyzrLLMFactory
 from lyzr.chatqa.qa_bot import QABot
 from lyzr.base.service import LyzrService
 from lyzr.base.vector_store import LyzrVectorStoreIndex
 from lyzr.formula_generator import FormulaGen
-from lyzr.data_analyzr import DataAnalyzr
+from lyzr.csv_analyzr import CsvAnalyzr
 
 __all__ = [
     "LyzrLLMFactory",
     "LyzrService",
     "LyzrVectorStoreIndex",
     "QABot",
     "ChatBot",
     "FormulaGen",
     "Generator",
-    "DataAnalyzr"
+    "CsvAnalyzr"
 ]
```

### Comparing `lyzr-0.1.8/lyzr/base/errors.py` & `lyzr-0.1.9/lyzr/base/errors.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/file_utils.py` & `lyzr-0.1.9/lyzr/base/file_utils.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/llms.py` & `lyzr-0.1.9/lyzr/base/llms.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/prompts/analysis_pt.txt` & `lyzr-0.1.9/lyzr/base/prompts/analysis_pt.txt`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/prompts/dataset_description_pt.txt` & `lyzr-0.1.9/lyzr/base/prompts/dataset_description_pt.txt`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/prompts/insights_pt.txt` & `lyzr-0.1.9/lyzr/base/prompts/insights_pt.txt`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/prompts/make_analysis_query_pt.txt` & `lyzr-0.1.9/lyzr/base/prompts/make_analysis_query_pt.txt`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/prompts/manual_input_pt.txt` & `lyzr-0.1.9/lyzr/base/prompts/manual_input_pt.txt`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/prompts/query_gen_pt.txt` & `lyzr-0.1.9/lyzr/base/prompts/query_gen_pt.txt`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/prompts/recommendations_pt.txt` & `lyzr-0.1.9/lyzr/base/prompts/recommendations_pt.txt`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/prompts/tasks_pt.txt` & `lyzr-0.1.9/lyzr/base/prompts/tasks_pt.txt`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/service.py` & `lyzr-0.1.9/lyzr/base/service.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/base/vector_store.py` & `lyzr-0.1.9/lyzr/base/vector_store.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/chatqa/chatbot.py` & `lyzr-0.1.9/lyzr/chatqa/chatbot.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/chatqa/qa_bot.py` & `lyzr-0.1.9/lyzr/chatqa/qa_bot.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/data_analyzr/data_analyzr.py` & `lyzr-0.1.9/lyzr/csv_analyzr/csv_analyzr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pandas as pd
 import openai
-import time
 import re
 
-class DataAnalyzr:
-    def __init__(self, df, user_input, gpt_model="gpt-3.5-turbo"):
-        self.df = df
+class CsvAnalyzr:
+    def __init__(self, csv_path, user_input, gpt_model="gpt-3.5-turbo"):
+        self.csv_path = csv_path
+        self.df = pd.read_csv(csv_path)
         self.user_input = user_input
         self.gpt_model = gpt_model
-        self.df_columns = df.columns.tolist()
-        self.df_head = df.head(5)
+        self.df_columns = self.df.columns.tolist()
+        self.df_head = self.df.head(5)
 
 
     def getSteps(self):
 
         system_prompt = """You are a Senior Data Scientist with 10+ Years of Experience. This is a Critical Scenerio. The CEO has asked you a question on a given data, your job is to list down steps to Analyze the Data and answer the CEO's question. """
 
         user_prompt = f"""CEO: {self.user_input}
@@ -87,67 +87,71 @@
             corrected_python_code = python_code_blocks[0]
         except:
             corrected_python_code = model_response
 
         return corrected_python_code
 
 
-    def writeCode(self, instructions):
+    def getCode(self, instructions):
 
         system_prompt = """You Write Python Function. You are a Senior Data Analyst with 10+ Years of Experience. This is a Critical Scenerio. The CEO has asked you to write Python Function to answer a question on a given data, based on the instructions given by Senior Data Scientist"""
 
         user_prompt = f"""CEO: {self.user_input}
 
         Dataframe Head: 
         {self.df_head}
         
         Data Scientist's Instructions:{instructions}
 
         Here is a sample output for the Python Function:
         ```python
-        import <necessory_libraries>
+        import pandas as pd
+        import <necessory_libraries> # import ALL the necessory libraries
 
         def function_name(dataframe):
             # Write your Python Function here that does the required analysis and answer's CEO's Question
            
         if __name__ == "__main__":
-            function_name(df) 
-            # Call the function, Assume that the df (dataframe) is already defined
+            df = pandas.read_csv("{self.csv_path}") # Do NOT change this line
+            function_name(df) # Call the function that you wrote with the dataframe as the argument
         ```
 
         Now, Write down python function to answer the CEO's question: {self.user_input}
 
         Just Write the Python Function in markdown format, that's it.
         """
 
         messages=[
         {"role": "system", "content": system_prompt},
         {"role": "user", "content": user_prompt},
         ]
 
         completion = openai.ChatCompletion.create(model=self.gpt_model, temperature = 0, messages=messages)
 
-        python_code = completion.choices[0].message.content
-
-        return python_code
-
-
-    def getCode(self, data_scientist_instructions=None):
-        print("\n Getting Steps")
-        if data_scientist_instructions is None:
-            data_scientist_instructions = self.getSteps()
-
-        print("\n Steps: ", data_scientist_instructions)
-
-        print("\n Writing Code")
-        model_response = self.writeCode(instructions=data_scientist_instructions)
-        print("\n Code:\n ", model_response)
+        model_response = completion.choices[0].message.content
 
         pattern = r'```python\n(.*?)\n```'
         python_code_blocks = re.findall(pattern, model_response, re.DOTALL)
 
         try:
             python_code = python_code_blocks[0]
         except:
             python_code = model_response    
 
         return python_code
+
+
+
+    def run(self, data_scientist_instructions=None):
+        if data_scientist_instructions is None:
+            data_scientist_instructions = self.getSteps()
+
+        python_code = self.getCode(instructions=data_scientist_instructions)
+
+        try:
+            exec(python_code)
+            return python_code
+        except Exception as e:
+            print("Failed to Analyze CSV")
+            error_message = f"Error: {str(e)}"
+            print(error_message)
+            return ""
```

### Comparing `lyzr-0.1.8/lyzr/formula_generator/formula_generator.py` & `lyzr-0.1.9/lyzr/formula_generator/formula_generator.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/generator/_generator.py` & `lyzr-0.1.9/lyzr/generator/_generator.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/chat_utils.py` & `lyzr-0.1.9/lyzr/utils/chat_utils.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/document_reading.py` & `lyzr-0.1.9/lyzr/utils/document_reading.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/docx_reader.py` & `lyzr-0.1.9/lyzr/utils/docx_reader.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/pdf_reader.py` & `lyzr-0.1.9/lyzr/utils/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/rag_utils.py` & `lyzr-0.1.9/lyzr/utils/rag_utils.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/templates.py` & `lyzr-0.1.9/lyzr/utils/templates.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/txt_reader.py` & `lyzr-0.1.9/lyzr/utils/txt_reader.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/webpage_reader.py` & `lyzr-0.1.9/lyzr/utils/webpage_reader.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr/utils/website_reader.py` & `lyzr-0.1.9/lyzr/utils/website_reader.py`

 * *Files identical despite different names*

### Comparing `lyzr-0.1.8/lyzr.egg-info/SOURCES.txt` & `lyzr-0.1.9/lyzr.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
 lyzr/__init__.py
 lyzr.egg-info/PKG-INFO
 lyzr.egg-info/SOURCES.txt
 lyzr.egg-info/dependency_links.txt
@@ -21,16 +22,16 @@
 lyzr/base/prompts/manual_input_pt.txt
 lyzr/base/prompts/query_gen_pt.txt
 lyzr/base/prompts/recommendations_pt.txt
 lyzr/base/prompts/tasks_pt.txt
 lyzr/chatqa/__init__.py
 lyzr/chatqa/chatbot.py
 lyzr/chatqa/qa_bot.py
-lyzr/data_analyzr/__init__.py
-lyzr/data_analyzr/data_analyzr.py
+lyzr/csv_analyzr/__init__.py
+lyzr/csv_analyzr/csv_analyzr.py
 lyzr/formula_generator/__init__.py
 lyzr/formula_generator/formula_generator.py
 lyzr/generator/__init__.py
 lyzr/generator/_generator.py
 lyzr/utils/__init__.py
 lyzr/utils/chat_utils.py
 lyzr/utils/constants.py
```

### Comparing `lyzr-0.1.8/setup.py` & `lyzr-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="lyzr",
-    version="0.1.8",
+    version="0.1.9",
     author="lyzr",
     description="",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="",
     include_package_data=True,
     packages=find_packages(),
```

