# Comparing `tmp/parsee_core-0.1.3.9.tar.gz` & `tmp/parsee_core-0.1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsee_core-0.1.3.9.tar", max compression
+gzip compressed data, was "parsee_core-0.1.4.0.tar", max compression
```

## Comparing `parsee_core-0.1.3.9.tar` & `parsee_core-0.1.4.0.tar`

### file list

```diff
@@ -1,70 +1,74 @@
--rw-r--r--   0        0        0      485 2024-02-14 17:01:39.100086 parsee_core-0.1.3.9/parsee/__init__.py
--rw-r--r--   0        0        0     2768 2024-03-13 08:58:10.546792 parsee_core-0.1.3.9/parsee/cloud/api.py
--rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.3.9/parsee/converters/__init__.py
--rw-r--r--   0        0        0     6035 2024-02-14 15:27:25.505875 parsee_core-0.1.3.9/parsee/converters/html_extraction.py
--rw-r--r--   0        0        0      344 2024-02-14 09:53:17.700535 parsee_core-0.1.3.9/parsee/converters/interfaces.py
--rw-r--r--   0        0        0     1800 2024-02-14 11:04:57.276847 parsee_core-0.1.3.9/parsee/converters/json_to_raw.py
--rw-r--r--   0        0        0     1063 2024-03-12 10:43:02.953449 parsee_core-0.1.3.9/parsee/converters/langchain.py
--rw-r--r--   0        0        0     2512 2024-03-14 12:40:05.729568 parsee_core-0.1.3.9/parsee/converters/main.py
--rw-r--r--   0        0        0     4339 2024-03-07 12:02:27.214681 parsee_core-0.1.3.9/parsee/converters/pdf_extraction.py
--rw-r--r--   0        0        0     6706 2024-02-28 09:39:54.651652 parsee_core-0.1.3.9/parsee/datasets/dataset_dataclasses.py
--rw-r--r--   0        0        0     6419 2024-03-11 17:39:35.687707 parsee_core-0.1.3.9/parsee/datasets/evaluation/main.py
--rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.3.9/parsee/datasets/main.py
--rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.3.9/parsee/datasets/readers/disk_reader.py
--rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.3.9/parsee/datasets/readers/interfaces.py
--rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.3.9/parsee/datasets/writers/disk_writer.py
--rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.3.9/parsee/datasets/writers/interfaces.py
--rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.3.9/parsee/extraction/__init__.py
--rw-r--r--   0        0        0     4072 2024-03-13 08:33:25.399204 parsee_core-0.1.3.9/parsee/extraction/extractor_dataclasses.py
--rw-r--r--   0        0        0    26486 2024-03-12 10:43:02.953830 parsee_core-0.1.3.9/parsee/extraction/extractor_elements.py
--rw-r--r--   0        0        0     9405 2024-02-14 09:53:17.695285 parsee_core-0.1.3.9/parsee/extraction/final_structuring.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.3.9/parsee/extraction/models/__init__.py
--rw-r--r--   0        0        0     1390 2024-03-15 10:50:04.142839 parsee_core-0.1.3.9/parsee/extraction/models/helpers.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/__init__.py
--rw-r--r--   0        0        0     1995 2024-03-15 12:24:39.438997 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/anthropic_model.py
--rw-r--r--   0        0        0     2107 2024-03-15 10:50:04.143625 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/chatgpt_model.py
--rw-r--r--   0        0        0      787 2024-02-22 09:42:26.224225 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/llm_base_model.py
--rw-r--r--   0        0        0      785 2024-02-19 16:48:56.158120 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/prompts.py
--rw-r--r--   0        0        0     1936 2024-03-15 10:50:04.143967 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/replicate_model.py
--rw-r--r--   0        0        0     7759 2024-03-12 16:24:07.618641 parsee_core-0.1.3.9/parsee/extraction/models/llm_models/structuring_schema.py
--rw-r--r--   0        0        0      882 2024-02-14 09:53:17.731629 parsee_core-0.1.3.9/parsee/extraction/models/model_dataclasses.py
--rw-r--r--   0        0        0     8011 2024-03-15 10:50:04.144186 parsee_core-0.1.3.9/parsee/extraction/models/model_loader.py
--rw-r--r--   0        0        0     3508 2024-02-22 09:49:50.419488 parsee_core-0.1.3.9/parsee/extraction/run.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.9/parsee/extraction/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/__init__.py
--rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/element_model.py
--rw-r--r--   0        0        0     2207 2024-02-22 09:52:47.321926 parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/element_model_llm.py
--rw-r--r--   0        0        0     7994 2024-03-08 10:22:59.229776 parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/features.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/__init__.py
--rw-r--r--   0        0        0     4811 2024-03-01 11:50:42.255522 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/features.py
--rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/mapping_model.py
--rw-r--r--   0        0        0     1944 2024-02-22 09:52:47.320729 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/mapping_model_llm.py
--rw-r--r--   0        0        0      928 2024-02-14 09:52:23.276265 parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/utils.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/__init__.py
--rw-r--r--   0        0        0    13012 2024-03-01 12:05:20.644356 parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/features.py
--rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/meta_info.py
--rw-r--r--   0        0        0     2619 2024-02-22 09:52:47.325111 parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/__init__.py
--rw-r--r--   0        0        0     5600 2024-03-15 10:50:04.144602 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/features.py
--rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/question_model.py
--rw-r--r--   0        0        0     3941 2024-03-12 16:27:29.550990 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/question_model_llm.py
--rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.3.9/parsee/extraction/tasks/questions/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.3.9/parsee/storage/__init__.py
--rw-r--r--   0        0        0     2284 2024-02-22 09:42:26.247730 parsee_core-0.1.3.9/parsee/storage/in_memory_storage.py
--rw-r--r--   0        0        0      989 2024-03-04 17:06:27.482788 parsee_core-0.1.3.9/parsee/storage/interfaces.py
--rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.3.9/parsee/storage/vector_stores/interfaces.py
--rw-r--r--   0        0        0     3005 2024-02-21 09:37:29.119873 parsee_core-0.1.3.9/parsee/storage/vector_stores/simple_faiss.py
--rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.3.9/parsee/templates/__init__.py
--rw-r--r--   0        0        0     1293 2024-02-22 09:42:26.225885 parsee_core-0.1.3.9/parsee/templates/element_schema.py
--rw-r--r--   0        0        0      238 2024-01-26 09:00:34.050000 parsee_core-0.1.3.9/parsee/templates/export_schema.py
--rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.3.9/parsee/templates/general_structuring_schema.py
--rw-r--r--   0        0        0     3740 2024-02-22 09:42:26.221745 parsee_core-0.1.3.9/parsee/templates/helpers.py
--rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.3.9/parsee/templates/job_template.py
--rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.3.9/parsee/templates/mappings.py
--rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.3.9/parsee/templates/template_from_json.py
--rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.3.9/parsee/utils/__init__.py
--rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.3.9/parsee/utils/constants.py
--rw-r--r--   0        0        0      741 2024-03-15 10:50:04.144816 parsee_core-0.1.3.9/parsee/utils/enums.py
--rw-r--r--   0        0        0     5552 2024-03-14 12:47:20.873826 parsee_core-0.1.3.9/parsee/utils/helper.py
--rw-r--r--   0        0        0      781 2024-03-15 12:24:39.443961 parsee_core-0.1.3.9/pyproject.toml
--rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 parsee_core-0.1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-21 12:33:53.103983 parsee_core-0.1.4.0/LICENSE
+-rw-r--r--   0        0        0      529 2024-03-27 13:19:30.023928 parsee_core-0.1.4.0/parsee/__init__.py
+-rw-r--r--   0        0        0     2768 2024-03-13 08:58:10.546792 parsee_core-0.1.4.0/parsee/cloud/api.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.4.0/parsee/converters/__init__.py
+-rw-r--r--   0        0        0     6063 2024-03-29 10:54:00.293459 parsee_core-0.1.4.0/parsee/converters/html_extraction.py
+-rw-r--r--   0        0        0     3117 2024-04-10 14:57:20.431510 parsee_core-0.1.4.0/parsee/converters/image_creation.py
+-rw-r--r--   0        0        0      399 2024-03-27 13:22:36.894150 parsee_core-0.1.4.0/parsee/converters/interfaces.py
+-rw-r--r--   0        0        0     1806 2024-04-10 14:57:20.432097 parsee_core-0.1.4.0/parsee/converters/json_to_raw.py
+-rw-r--r--   0        0        0     1069 2024-04-10 14:57:20.432511 parsee_core-0.1.4.0/parsee/converters/langchain.py
+-rw-r--r--   0        0        0     3015 2024-04-10 14:57:20.432769 parsee_core-0.1.4.0/parsee/converters/main.py
+-rw-r--r--   0        0        0     4324 2024-03-27 13:19:30.029388 parsee_core-0.1.4.0/parsee/converters/pdf_extraction.py
+-rw-r--r--   0        0        0      491 2024-03-27 13:22:36.895882 parsee_core-0.1.4.0/parsee/converters/simple_text.py
+-rw-r--r--   0        0        0     6680 2024-03-25 10:47:46.831244 parsee_core-0.1.4.0/parsee/datasets/dataset_dataclasses.py
+-rw-r--r--   0        0        0     7820 2024-03-20 10:51:40.783264 parsee_core-0.1.4.0/parsee/datasets/evaluation/main.py
+-rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.4.0/parsee/datasets/main.py
+-rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.4.0/parsee/datasets/readers/disk_reader.py
+-rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.4.0/parsee/datasets/readers/interfaces.py
+-rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.4.0/parsee/datasets/writers/disk_writer.py
+-rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.4.0/parsee/datasets/writers/interfaces.py
+-rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.4.0/parsee/extraction/__init__.py
+-rw-r--r--   0        0        0     4138 2024-04-10 14:57:20.433043 parsee_core-0.1.4.0/parsee/extraction/extractor_dataclasses.py
+-rw-r--r--   0        0        0    29531 2024-04-10 14:57:20.433583 parsee_core-0.1.4.0/parsee/extraction/extractor_elements.py
+-rw-r--r--   0        0        0     9472 2024-04-05 15:38:22.487342 parsee_core-0.1.4.0/parsee/extraction/final_structuring.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.0/parsee/extraction/models/__init__.py
+-rw-r--r--   0        0        0     2062 2024-04-10 14:57:20.433864 parsee_core-0.1.4.0/parsee/extraction/models/helpers.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.0/parsee/extraction/models/llm_models/__init__.py
+-rw-r--r--   0        0        0     2882 2024-04-10 14:57:20.434116 parsee_core-0.1.4.0/parsee/extraction/models/llm_models/anthropic_model.py
+-rw-r--r--   0        0        0     2866 2024-04-10 14:57:20.434321 parsee_core-0.1.4.0/parsee/extraction/models/llm_models/chatgpt_model.py
+-rw-r--r--   0        0        0      888 2024-04-10 14:57:20.434563 parsee_core-0.1.4.0/parsee/extraction/models/llm_models/llm_base_model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 14:57:20.434940 parsee_core-0.1.4.0/parsee/extraction/models/llm_models/ollama_model.py
+-rw-r--r--   0        0        0      875 2024-04-10 14:57:20.435213 parsee_core-0.1.4.0/parsee/extraction/models/llm_models/prompts.py
+-rw-r--r--   0        0        0     1971 2024-04-10 14:57:20.435485 parsee_core-0.1.4.0/parsee/extraction/models/llm_models/replicate_model.py
+-rw-r--r--   0        0        0     7875 2024-03-19 14:15:12.265884 parsee_core-0.1.4.0/parsee/extraction/models/llm_models/structuring_schema.py
+-rw-r--r--   0        0        0      985 2024-04-10 14:57:20.435851 parsee_core-0.1.4.0/parsee/extraction/models/model_dataclasses.py
+-rw-r--r--   0        0        0     8163 2024-03-20 12:24:18.192932 parsee_core-0.1.4.0/parsee/extraction/models/model_loader.py
+-rw-r--r--   0        0        0     3358 2024-04-09 11:54:32.370368 parsee_core-0.1.4.0/parsee/extraction/run.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.0/parsee/extraction/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.0/parsee/extraction/tasks/element_classification/__init__.py
+-rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.4.0/parsee/extraction/tasks/element_classification/element_model.py
+-rw-r--r--   0        0        0     2199 2024-04-10 14:57:20.436266 parsee_core-0.1.4.0/parsee/extraction/tasks/element_classification/element_model_llm.py
+-rw-r--r--   0        0        0     8051 2024-04-10 14:57:20.436667 parsee_core-0.1.4.0/parsee/extraction/tasks/element_classification/features.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.0/parsee/extraction/tasks/mappings/__init__.py
+-rw-r--r--   0        0        0     6108 2024-04-04 15:01:44.484913 parsee_core-0.1.4.0/parsee/extraction/tasks/mappings/features.py
+-rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.4.0/parsee/extraction/tasks/mappings/mapping_model.py
+-rw-r--r--   0        0        0     2519 2024-04-10 14:57:20.436928 parsee_core-0.1.4.0/parsee/extraction/tasks/mappings/mapping_model_llm.py
+-rw-r--r--   0        0        0      894 2024-03-28 20:25:58.634238 parsee_core-0.1.4.0/parsee/extraction/tasks/mappings/utils.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.0/parsee/extraction/tasks/meta_info_structuring/__init__.py
+-rw-r--r--   0        0        0    13073 2024-04-10 14:57:20.437207 parsee_core-0.1.4.0/parsee/extraction/tasks/meta_info_structuring/features.py
+-rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.4.0/parsee/extraction/tasks/meta_info_structuring/meta_info.py
+-rw-r--r--   0        0        0     2641 2024-04-10 14:57:20.437514 parsee_core-0.1.4.0/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.0/parsee/extraction/tasks/questions/__init__.py
+-rw-r--r--   0        0        0     6136 2024-04-10 14:57:20.437823 parsee_core-0.1.4.0/parsee/extraction/tasks/questions/features.py
+-rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.4.0/parsee/extraction/tasks/questions/question_model.py
+-rw-r--r--   0        0        0     4031 2024-04-10 14:57:20.438067 parsee_core-0.1.4.0/parsee/extraction/tasks/questions/question_model_llm.py
+-rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.4.0/parsee/extraction/tasks/questions/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.4.0/parsee/storage/__init__.py
+-rw-r--r--   0        0        0     2366 2024-04-10 14:57:20.438310 parsee_core-0.1.4.0/parsee/storage/in_memory_storage.py
+-rw-r--r--   0        0        0     1212 2024-04-10 14:57:20.438565 parsee_core-0.1.4.0/parsee/storage/interfaces.py
+-rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.4.0/parsee/storage/vector_stores/interfaces.py
+-rw-r--r--   0        0        0     3204 2024-03-22 17:12:35.963569 parsee_core-0.1.4.0/parsee/storage/vector_stores/simple_faiss.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.4.0/parsee/templates/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-05 15:38:22.487748 parsee_core-0.1.4.0/parsee/templates/element_schema.py
+-rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.4.0/parsee/templates/general_structuring_schema.py
+-rw-r--r--   0        0        0     4019 2024-04-05 15:38:22.488067 parsee_core-0.1.4.0/parsee/templates/helpers.py
+-rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.4.0/parsee/templates/job_template.py
+-rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.4.0/parsee/templates/mappings.py
+-rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.4.0/parsee/templates/template_from_json.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.4.0/parsee/utils/__init__.py
+-rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.4.0/parsee/utils/constants.py
+-rw-r--r--   0        0        0      781 2024-03-27 13:19:30.038637 parsee_core-0.1.4.0/parsee/utils/enums.py
+-rw-r--r--   0        0        0     6632 2024-04-08 08:51:44.149915 parsee_core-0.1.4.0/parsee/utils/helper.py
+-rw-r--r--   0        0        0     2030 2024-03-26 12:40:38.547700 parsee_core-0.1.4.0/parsee/utils/sample_items.py
+-rw-r--r--   0        0        0      827 2024-04-10 14:57:26.181350 parsee_core-0.1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 parsee_core-0.1.4.0/PKG-INFO
```

### Comparing `parsee_core-0.1.3.9/parsee/cloud/api.py` & `parsee_core-0.1.4.0/parsee/cloud/api.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/converters/html_extraction.py` & `parsee_core-0.1.4.0/parsee/converters/html_extraction.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     return get_element_sibling_xpath(parent, xpath)
 
 
 class HtmlConverter(RawToJsonConverter):
 
     def __init__(self):
         super().__init__(DocumentType.HTML)
-        self.service_name = "simfin_html"
+        self.service_name = "parsee_html"
 
-    def convert(self, file_path: str) -> Tuple[List[ExtractedEl], Decimal]:
-        with open(file_path) as html_file:
+    def convert(self, file_path_or_content: str) -> Tuple[List[ExtractedEl], Decimal]:
+        with open(file_path_or_content, 'rb') as html_file:
             html_content = html_file.read()
             return self._extract_elements_from_html_data(html_content), PRICING_HTML_CONVERSION
 
     def _extract_elements_from_html_data(self, html_data) -> List[ExtractedEl]:
 
         soup = BeautifulSoup(html_data, 'lxml')
```

### Comparing `parsee_core-0.1.3.9/parsee/converters/json_to_raw.py` & `parsee_core-0.1.4.0/parsee/converters/json_to_raw.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 
 def load_document_from_json(json_contents) -> StandardDocumentFormat:
 
     source_type = DocumentType(json_contents["source_type"])
     source_identifier = json_contents["source_identifier"]
     elements = load_elements_from_json(json_contents["elements"])
 
-    return StandardDocumentFormat(source_type, source_identifier, elements)
+    return StandardDocumentFormat(source_type, source_identifier, elements, None)
```

### Comparing `parsee_core-0.1.3.9/parsee/converters/langchain.py` & `parsee_core-0.1.4.0/parsee/converters/langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 def langchain_loader_to_sdf(loader: BaseLoader, document_type: DocumentType, source_identifier: str) -> StandardDocumentFormat:
 
     pages = loader.load_and_split()
 
     elements = documents_to_extracted_elements(pages, document_type)
 
-    return StandardDocumentFormat(document_type, source_identifier, elements)
+    return StandardDocumentFormat(document_type, source_identifier, elements, None)
```

### Comparing `parsee_core-0.1.3.9/parsee/converters/main.py` & `parsee_core-0.1.4.0/parsee/converters/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 from parsee.utils.enums import DocumentType
 from parsee.extraction.extractor_elements import StandardDocumentFormat
 from parsee.converters.json_to_raw import load_document_from_json
 from parsee.converters.interfaces import RawToJsonConverter
 from parsee.converters.html_extraction import HtmlConverter
 from parsee.converters.pdf_extraction import PdfConverter
-from parsee.utils.helper import get_source_identifier
+from parsee.converters.simple_text import SimpleTextConverter
+from parsee.utils.helper import get_source_identifier, get_source_identifier_simple
 
 
 def determine_document_type(file_path: str) -> DocumentType:
     file_path = file_path.lower()
     if file_path.endswith(".pdf") or file_path.endswith(".png") or file_path.endswith(".jpg") or file_path.endswith(".jpeg"):
         return DocumentType.PDF
     elif file_path.endswith(".html") or file_path.endswith(".xml"):
@@ -34,23 +35,32 @@
 def load_document(file_path: str) -> StandardDocumentFormat:
     doc_type = determine_document_type(file_path)
     source_identifier = get_source_identifier(file_path)
     doc, _ = doc_to_standard_format(source_identifier, doc_type, choose_converter(doc_type), file_path)
     return doc
 
 
+def from_text(text: str) -> StandardDocumentFormat:
+    source_identifier = get_source_identifier_simple(text)
+    converter = SimpleTextConverter(DocumentType.TEXT)
+    doc, _ = doc_to_standard_format(source_identifier, DocumentType.TEXT, converter, text)
+    return doc
+
+
 def doc_to_standard_format(source_identifier: str, source_type: DocumentType, converter: RawToJsonConverter,
-                           file_path: str) -> Tuple[StandardDocumentFormat, Decimal]:
-    elements, amount = converter.convert(file_path)
-    return StandardDocumentFormat(source_type, source_identifier, elements), amount
+                           file_path_or_content: str) -> Tuple[StandardDocumentFormat, Decimal]:
+    elements, amount = converter.convert(file_path_or_content)
+    return StandardDocumentFormat(source_type, source_identifier, elements, None if source_type == DocumentType.TEXT else file_path_or_content), amount
 
 
 def save_doc_in_standard_format(source_identifier: str, source_type: DocumentType, converter: RawToJsonConverter, file_path: str) -> \
         Tuple[any, StandardDocumentFormat, Decimal]:
     doc, amount = doc_to_standard_format(source_identifier, source_type, converter, file_path)
+    # unset file path
+    doc.file_path = None
     json_string = json.dumps(doc.to_json_dict())
     tmp = tempfile.NamedTemporaryFile(delete=True)
     tmp.write(str.encode(json_string, 'utf-8'))
     return tmp, doc, amount
 
 
 def load_standard_document_from_file(json_file_path: str) -> StandardDocumentFormat:
```

### Comparing `parsee_core-0.1.3.9/parsee/converters/pdf_extraction.py` & `parsee_core-0.1.4.0/parsee/converters/pdf_extraction.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 PRICING_PDF_CONVERSION = Decimal(os.getenv("PRICING_CONVERSION")) if os.getenv("PRICING_CONVERSION") is not None else Decimal(0)
 
 
 class PdfConverter(RawToJsonConverter):
 
     def __init__(self, predicted_areas: Union[None, Dict[int, List[RelativeAreaPrediction]]]):
         super().__init__(DocumentType.PDF)
-        self.service_name = "simfin_pdf"
+        self.service_name = "parsee_pdf"
         self.areas = predicted_areas
 
     def pages_to_extracted_el(self, pages: List[ExtractedPage]) -> List[ExtractedEl]:
         elements: List[ExtractedEl] = []
         for page_num, page in enumerate(pages):
             for idx, el in enumerate(page.paragraphs):
                 if isinstance(el, ExtractedTable):
@@ -40,31 +40,31 @@
                                                                             {"page_idx": page_num,
                                                                              "page_size": [page.size.x0, page.size.y0, page.size.x1, page.size.y1]}), el.get_text())
                 else:
                     raise Exception("element not recognized")
                 elements.append(element)
         return elements
 
-    def convert(self, file_path: str, **kwargs) -> Tuple[List[ExtractedEl], Decimal]:
+    def convert(self, file_path_or_content: str, **kwargs) -> Tuple[List[ExtractedEl], Decimal]:
 
-        pages = get_elements_from_pdf(file_path, self.areas, **kwargs)
+        pages = get_elements_from_pdf(file_path_or_content, self.areas, **kwargs)
 
         return self.pages_to_extracted_el(pages), PRICING_PDF_CONVERSION
 
     def _make_structured_table(self, source: ExtractedSource, table: ExtractedTable) -> StructuredTable:
 
         rows_structured: List[StructuredRow] = []
 
         # determine header end
         header_end_idx = 0
         for k, line_item in enumerate(table.items):
-            found_valid = False if line_item.caption == '' else True
+            found_valid = False
             for v in line_item.values:
-                if not is_number_cell(v.val) or is_year_cell(v.val):
-                    found_valid = False
+                if is_number_cell(v.val) and not is_year_cell(v.val):
+                    found_valid = True
                     break
             if found_valid:
                 header_end_idx = k
                 break
 
         # add value rows
         for k, row in enumerate(table.items):
```

### Comparing `parsee_core-0.1.3.9/parsee/datasets/dataset_dataclasses.py` & `parsee_core-0.1.4.0/parsee/datasets/dataset_dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 class CategoricalTransformation:
     categories: List[str]
 
 
 @dataclass
 class WordVectorTransformation:
     tokenizer: any
-    matrix: Optional[any]
     max_words: int
     col_index: int
     vocab_size: Optional[int]
 
 
 @dataclass
 class Transformation:
```

### Comparing `parsee_core-0.1.3.9/parsee/datasets/evaluation/main.py` & `parsee_core-0.1.4.0/parsee/datasets/evaluation/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,36 +31,46 @@
 
     def evaluate(self) -> Dict:
         scores_by_source = {}
         for source, sc_dict in self.answers.items():
             scores_by_source[source] = {}
             reference_item = sc_dict["assigned"]
             for model, by_class in sc_dict.items():
-                scores_by_source[source][model] = {"error_log": []}
+                scores_by_source[source][model] = {"error_log": [], "missing_answers": 0}
                 # check that all questions have been answered
                 scores_by_source[source][model]["completion"] = len(by_class.keys()) / len(reference_item.keys())
                 # check each question
                 score = 0
                 score_meta = 0
                 for class_id, assigned_values in reference_item.items():
                     if class_id not in by_class:
                         continue
                     predicted_values = by_class[class_id]
+                    # check if some answers are missing from the result
+                    scores_by_source[source][model]["missing_answers"] = max(len(assigned_values.keys()) - len(predicted_values.keys()), 0)
                     for meta_key, correct_value in assigned_values.items():
                         if meta_key in predicted_values:
                             if meta_key != "":
                                 score_meta += 1
                             predicted_value = predicted_values[meta_key]
                             # check if values match
                             if correct_value.class_value == predicted_value.class_value:
                                 score += 1
                             else:
                                 scores_by_source[source][model]["error_log"].append({"doc": source, "class_id": class_id, "type": "main question", "expected": correct_value.class_value, "actual": predicted_value.class_value})
-                        elif len(assigned_values.keys()) == 1 and len(predicted_values.keys()) == 1:
-                            predicted_value = predicted_values[list(predicted_values.keys())[0]]
+                        else:
+                            if len(assigned_values.keys()) == 1 and len(predicted_values.keys()) == 1:
+                                predicted_value = predicted_values[list(predicted_values.keys())[0]]
+                            else:
+                                # try to find main answer
+                                filtered_answers = [x for x in predicted_values.values() if x.class_value == correct_value.class_value]
+                                if len(filtered_answers) > 0:
+                                    predicted_value = filtered_answers[0]
+                                else:
+                                    continue
                             # meta mismatch
                             scores_by_source[source][model]["error_log"].append({"doc": source, "class_id": class_id, "type": "meta", "expected": correct_value.meta_key(), "actual": predicted_value.meta_key()})
                             # check if values match
                             if correct_value.class_value == predicted_value.class_value:
                                 score += 1
                             else:
                                 scores_by_source[source][model]["error_log"].append({"doc": source, "class_id": class_id, "type": "main question", "expected": correct_value.class_value, "actual": predicted_value.class_value})
@@ -68,28 +78,29 @@
                 scores_by_source[source][model]["total_correct"] = score
                 scores_by_source[source][model]["total_correct_meta_found"] = score_meta
 
         total_scores = {}
         for source, by_source in scores_by_source.items():
             for model, scores in by_source.items():
                 if model not in total_scores:
-                    total_scores[model] = {"completion": 0, "total_correct": 0, "total_correct_meta_found": 0, "error_log": []}
+                    total_scores[model] = {"completion": 0, "total_correct": 0, "total_correct_meta_found": 0, "missing_answers": 0, "error_log": []}
                 for score_key, score_value in scores.items():
                     total_scores[model][score_key] += score_value
         reference_scores = total_scores["assigned"]
         for model, scores_dict in total_scores.items():
             scores_dict_final = {**scores_dict}
-            for score_key, score_value in scores_dict.items():
-                if score_key == "completion":
-                    scores_dict_final[score_key] = scores_dict[score_key] / len(scores_by_source.keys())
-                elif score_key == "error_log":
-                    pass
-                else:
-                    rel_key = score_key+"_percent"
-                    scores_dict_final[rel_key] = score_value / reference_scores[score_key]
+            scores_dict_final["completion"] = scores_dict["completion"] / len(scores_by_source.keys())
+            # calculate completeness: how many items are not "missing" entirely
+            scores_dict_final["completeness"] = (reference_scores["total_correct"] - scores_dict_final["missing_answers"])/reference_scores["total_correct"]
+            # scores INCLUDING missing answers
+            scores_dict_final["total_correct_percent"] = scores_dict_final["total_correct"] / reference_scores["total_correct"]
+            scores_dict_final["total_correct_meta_found_percent"] = scores_dict_final["total_correct_meta_found"] / reference_scores["total_correct_meta_found"]
+            # scores EXCLUDING missing answers
+            scores_dict_final["total_correct_percent_ex_missing"] = scores_dict_final["total_correct"] / (reference_scores["total_correct"]-scores_dict_final["missing_answers"])
+            scores_dict_final["total_correct_meta_found_percent_ex_missing"] = scores_dict_final["total_correct_meta_found"] / (reference_scores["total_correct_meta_found"]-scores_dict_final["missing_answers"])
             total_scores[model] = scores_dict_final
         return total_scores
 
 
 def evaluate_llm_performance(template: JobTemplate, reader: DatasetReader, models: List[MlModelSpecification], storage: Optional[StorageManager] = None) -> Dict:
 
     storage = InMemoryStorageManager(models) if storage is None else storage
```

### Comparing `parsee_core-0.1.3.9/parsee/datasets/main.py` & `parsee_core-0.1.4.0/parsee/datasets/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/datasets/readers/disk_reader.py` & `parsee_core-0.1.4.0/parsee/datasets/readers/disk_reader.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/datasets/readers/interfaces.py` & `parsee_core-0.1.4.0/parsee/datasets/readers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/datasets/writers/disk_writer.py` & `parsee_core-0.1.4.0/parsee/datasets/writers/disk_writer.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/datasets/writers/interfaces.py` & `parsee_core-0.1.4.0/parsee/datasets/writers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/extraction/extractor_dataclasses.py` & `parsee_core-0.1.4.0/parsee/extraction/extractor_dataclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,7 +137,13 @@
 
 @dataclass
 class AssignedAnswer:
     class_id: str
     class_value: str
     meta: List[AssignedMeta]
     sources: List[ExtractedSource]
+
+
+@dataclass
+class Base64Image:
+    media_type: str
+    data: str
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/extractor_elements.py` & `parsee_core-0.1.4.0/parsee/extraction/extractor_elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,47 +29,40 @@
 
 class FinalOutputTableColumn:
     detected_class: str
     col_idx: int
     li_identifier: Union[str, None]
     kv_identifier: str
     key_value_pairs: List[Tuple[str, any]]
-    fully_structured: Dict[str, any]
     sources: List[ExtractedSource]
     meta: List[ParseeMeta]
     model: str
     locations: List[ParseeLocation]
 
     def __init__(self, location: ParseeLocation, element: StructuredTable, col_idx: int, col_idx_local: int, col_idx_org: int):
         self.col_idx = col_idx
         self.detected_class = location.detected_class
         self.key_value_pairs = []
         self.sources = []
         self.meta = []
         self.model = location.model
-        self.fully_structured = {}
         self.li_identifier = None
         self.set_identifiers()
         self.locations = [location]
         self._elements = [element]
         self._local_col_indices = [col_idx_local]
         self.org_col_indices = [col_idx_org]
         self.build()
 
     def __str__(self):
         return str(self.dict_json())
 
     def __repr__(self):
         return str(self)
 
-    def apply_mappings(self, mappings: List[ParseeBucket], schema: MappingSchema):
-        buckets = calc_buckets(self.key_value_pairs, mappings, schema)
-        for key, value in buckets.items():
-            self.fully_structured[key] = value
-
     def key_value_pairs_json(self):
         return [{str(key): (str(value) if value is not None else None)} for key, value in self.key_value_pairs]
 
     def set_identifiers(self):
         self.kv_identifier = sha256(str(self.key_value_pairs_json()).encode('utf-8')).hexdigest()
         self.li_identifier = sha256(str(get_table_signature(self.key_value_pairs)).encode('utf-8')).hexdigest()
 
@@ -84,44 +77,70 @@
             el = self._elements[k]
             kv_pairs += [(x.clean_caption(), x.value_elements[self._local_col_indices[k]].numeric_value_cleaned) for li_idx, x in enumerate(el.line_items)]
             sources.append(loc.source)
         self.key_value_pairs = kv_pairs
         self.sources = sources
         self.set_identifiers()
 
+    def add_empty_line_items(self, insert_idx: int, line_items: List[str]):
+        new_kv = self.key_value_pairs[0:insert_idx]+[(x, None) for x in line_items]+self.key_value_pairs[insert_idx:]
+        self.key_value_pairs = new_kv
+        self.set_identifiers()
+
     def add_location(self, location: ParseeLocation, element: StructuredTable, local_col_idx: int, org_col_idx: int):
         self.locations.append(location)
         self._elements.append(element)
         self._local_col_indices.append(local_col_idx)
         self.org_col_indices.append(org_col_idx)
         self.build()
 
+    def can_be_merged(self, col: FinalOutputTableColumn) -> bool:
+        if len(col.key_value_pairs) != len(self.key_value_pairs) or col.li_identifier != self.li_identifier:
+            return False
+        for k, (li, val) in enumerate(self.key_value_pairs):
+            check_li, check_val = col.key_value_pairs[k]
+            if val is not None and check_val is not None:
+                return False
+        return True
+
+    def merge_kv(self, col: FinalOutputTableColumn):
+        # merges key value pairs with key value pairs of other column
+        for k, (li, val) in enumerate(self.key_value_pairs):
+            if val is None:
+                self.key_value_pairs[k] = (li, col.key_value_pairs[k][1])
+        self.set_identifiers()
 
-@dataclass
 class FinalOutputTable:
     detected_class: str
     columns: List[FinalOutputTableColumn]
     li_identifier: str
     line_items: List[str]
 
+    def __init__(self, detected_class: str, columns: List[FinalOutputTableColumn], li_identifier: str):
+        self.detected_class = detected_class
+        self.columns = columns
+        self.li_identifier = li_identifier
+        self.line_items = [x[0] for x in columns[0].key_value_pairs]
+
     def li_number_matching(self) -> List[Tuple[str, Set[int]]]:
         output = []
         for k, li in enumerate(self.line_items):
             values = [clean_number_for_matching(col.key_value_pairs[k][1]) for col in self.columns]
             output.append((li, set(values)))
         return output
 
 
 class ElementGroup:
     detected_class: str
     components: List[ParseeLocation]
 
-    def __init__(self, detected_class: str, base_component: ParseeLocation):
+    def __init__(self, detected_class: str, base_component: ParseeLocation, collapse_columns: bool = False):
         self.detected_class = detected_class
         self.components = [base_component]
+        self.collapse_columns = collapse_columns
 
     def prob_combined(self) -> float:
         return float(np.mean([x.prob for x in self.components])) if len(self.components) > 0 else 0
 
     def closest_el(self, other: ElementGroup) -> ParseeLocation:
         el_sorted = list(sorted(self.components, key=lambda x: abs(x.source.element_index - other.components[0].source.element_index)))
         return el_sorted[0]
@@ -131,22 +150,32 @@
 
     def merge_with(self, other: ElementGroup):
         # merge elements
         self.components += other.components
 
     def structured_values(self, elements: List[ExtractedEl]) -> List[FinalOutputTableColumn]:
 
+        # sort by element index
+        components_sorted = list(sorted(self.components, key=lambda x: x.source.element_index))
+
         # collect all relevant elements
         elements_by_idx = {}
-        for comp in self.components:
+        for comp in components_sorted:
             el = elements[comp.source.element_index]
             elements_by_idx[comp.source.element_index] = el
 
+        # build / update reference line items
+        li_reference_list: Dict[int, List[str]] = {}
+        li_placed_by_col: Dict[int, Set[int]] = {}
+        for loc_k, location in enumerate(components_sorted):
+            current_element: StructuredTable = elements_by_idx[location.source.element_index]
+            li_reference_list[loc_k] = [x.clean_caption() for x in current_element.line_items]
+
         submissions_by_col = {}
-        for loc_k, location in enumerate(self.components):
+        for loc_k, location in enumerate(components_sorted):
             # check that element is really a table
             if elements_by_idx[location.source.element_index].el_type == ElementType.TEXT:
                 continue
             # index of last placed column from the current table
             placed_previous_index: Union[None, int] = None
             current_element: StructuredTable = elements_by_idx[location.source.element_index]
             current_numeric_col_indices = current_element.numeric_cols_indices
@@ -194,16 +223,38 @@
                     col_index_final = col_index_local
                 # update placed previous
                 placed_previous_index = col_index_final
                 if col_index_final not in submissions_by_col:
                     submissions_by_col[col_index_final] = FinalOutputTableColumn(location, current_element, col_index_final, col_index_local, col_index_org)
                 else:
                     submissions_by_col[col_index_final].add_location(location, current_element, col_index_local, col_index_org)
-
-        return list(submissions_by_col.values())
+                # update li placed dict
+                if col_index_final not in li_placed_by_col:
+                    li_placed_by_col[col_index_final] = set()
+                li_placed_by_col[col_index_final].add(loc_k)
+
+        # add missing line items to make sure that all columns have the same "length"
+        for col_idx, col in submissions_by_col.items():
+            if len(li_placed_by_col[col_idx]) < len(components_sorted):
+                # add missing items
+                for el_idx, li_values in li_reference_list.items():
+                    if el_idx not in li_placed_by_col[col_idx]:
+                        start_idx = sum([len(li_reference_list[x]) for x in range(0, el_idx)]) if el_idx > 0 else 0
+                        col.add_empty_line_items(start_idx, li_values)
+
+        # collapse columns from right to left if required and possible
+        to_del = set()
+        if self.collapse_columns:
+            for key_idx in range(len(submissions_by_col.keys())-1,-1,-1):
+                key = list(submissions_by_col.keys())[key_idx]
+                # check if columns can be merged
+                if key_idx > 0 and submissions_by_col[key].can_be_merged(submissions_by_col[list(submissions_by_col.keys())[key_idx-1]]):
+                    submissions_by_col[list(submissions_by_col.keys())[key_idx - 1]].merge_kv(submissions_by_col[key])
+                    to_del.add(key)
+        return [x for k, x in submissions_by_col.items() if k not in to_del]
 
 
 class StructuredLineItem:
     caption = None
     caption_elements = None
     value_elements = None
     row_index = None
@@ -558,15 +609,15 @@
         # determine numeric columns
         numeric_cols = []
         for col_index in range(0, self.num_columns_final()):
             col_value_types = [self.rows[x].final_values[col_index].cell_type for x in range(0, len(self.rows))]
 
             num_numeric = len([x for x in col_value_types if x == "numeric"])
             num_text = len([x for x in col_value_types if x == "text"])
-            if num_numeric > min_numeric and num_numeric > num_text:
+            if num_numeric >= min_numeric and num_numeric > num_text:
                 numeric_cols.append(col_index)
             if len(set(col_value_types)) == 1 and col_value_types[0] == "null":
                 self.empty_columns.append(col_index)
 
         # check if numeric columns can be consolidated because of duplicates
         numeric_cols = list(sorted(numeric_cols))
         if len(numeric_cols) > 1:
@@ -643,10 +694,11 @@
 
 
 @dataclass
 class StandardDocumentFormat:
     source_type: DocumentType
     source_identifier: str
     elements: List[ExtractedEl]
+    file_path: Optional[str]
 
     def to_json_dict(self):
         return {"source_type": self.source_type.value, "source_identifier": self.source_identifier, "elements": [x.to_json_dict() for x in self.elements]}
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/final_structuring.py` & `parsee_core-0.1.4.0/parsee/extraction/final_structuring.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     # transform predictions slightly
     candidates_by_class: Dict[str, List[ElementGroup]] = {}
     for k, prediction in enumerate(locations):
         class_value = prediction.detected_class
         if class_value is not None:
             if class_value not in candidates_by_class:
                 candidates_by_class[class_value] = []
-            candidates_by_class[class_value].append(ElementGroup(class_value, prediction))
+            # find detection item
+            candidates_by_class[class_value].append(ElementGroup(class_value, prediction, detection_schema_by_class[prediction.detected_class].collapseColumns))
 
     predictions_by_element_index = {}
     for pred in locations:
         predictions_by_element_index[pred.source.element_index] = pred
 
     # decide which partial matches to merge
     for class_value, structured_elements in candidates_by_class.items():
@@ -182,12 +183,12 @@
 def final_tables_from_columns(columns: List[FinalOutputTableColumn]) -> List[FinalOutputTable]:
 
     by_identifier = {}
 
     for col in columns:
         table_id = (col.li_identifier, col.detected_class)
         if table_id not in by_identifier:
-            by_identifier[table_id] = FinalOutputTable(col.detected_class, [col], col.li_identifier, [x[0] for x in col.key_value_pairs])
+            by_identifier[table_id] = FinalOutputTable(col.detected_class, [col], col.li_identifier)
         else:
             by_identifier[table_id].columns.append(col)
 
     return list(by_identifier.values())
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/anthropic_model.py` & `parsee_core-0.1.4.0/parsee/extraction/models/llm_models/chatgpt_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,75 @@
 import os
 import time
 from typing import List, Tuple
 from dataclasses import dataclass
 from decimal import Decimal
 import math
 
-import anthropic
+import openai
 import tiktoken
 
-from parsee.extraction.models.llm_models.llm_base_model import LLMBaseModel, truncate_prompt
+from parsee.extraction.models.llm_models.llm_base_model import LLMBaseModel, get_tokens_encoded, truncate_prompt
 from parsee.extraction.models.model_dataclasses import MlModelSpecification
+from parsee.extraction.models.llm_models.prompts import Prompt
+from parsee.extraction.extractor_dataclasses import Base64Image
 
 
-class AnthropicModel(LLMBaseModel):
+class ChatGPTModel(LLMBaseModel):
 
     def __init__(self, model: MlModelSpecification):
-        super().__init__(model.name)
-        self.model = model
+        super().__init__(model)
         self.max_retries = 5
         self.encoding = tiktoken.get_encoding("cl100k_base")
         self.max_tokens_answer = 1024
-        self.max_tokens_question = self.model.max_tokens - self.max_tokens_answer
-        self.client = anthropic.Anthropic(api_key=model.api_key if model.api_key is not None else os.getenv("ANTHROPIC_API_KEY"))
+        self.max_tokens_question = self.spec.max_tokens - self.max_tokens_answer
+        openai.api_key = model.api_key if model.api_key is not None else os.getenv("OPENAI_KEY")
 
-    def _call_api(self, prompt: str, retries: int = 0, wait: int = 5) -> Tuple[str, Decimal]:
+    def _call_api(self, prompt: str, images: List[Base64Image], retries: int = 0, wait: int = 5) -> Tuple[str, Decimal]:
+        user_message_content = [
+            {
+                "type": "text",
+                "text": prompt
+            }
+        ]
+        if len(images) > 0:
+            user_message_content += [
+                {
+                    "type": "text",
+                    "text": "These are the images:"
+                }
+            ]
+            user_message_content += [
+                {
+                    "type": "image_url",
+                    "image_url": {
+                        "url": f"data:{x.media_type};base64,{x.data}"
+                    }
+                }
+                for x in images
+            ]
         try:
-            message = self.client.messages.create(
-                model=self.model.internal_name,
-                max_tokens=self.max_tokens_answer,
-                temperature=0,
+            response = openai.ChatCompletion.create(
+                model=self.spec.internal_name,
                 messages=[
-                    {"role": "user", "content": prompt}
-                ]
+                    {"role": "user", "content": user_message_content}
+                ],
+                temperature=0,
+                max_tokens=self.max_tokens_answer,
+                top_p=1,
+                frequency_penalty=0,
+                presence_penalty=0
             )
 
-            answer = message.content[0].text if len(message.content) > 0 else ""
-            final_cost = (Decimal(message.usage.input_tokens+message.usage.output_tokens) * Decimal(self.model.price_per_1k_tokens/1000)) if self.model.price_per_1k_tokens is not None else Decimal(0)
+            answer = response['choices'][0]["message"]["content"]
+            final_cost = Decimal(int(response["usage"]['total_tokens']) * (self.spec.price_per_1k_tokens/1000)) if self.spec.price_per_1k_tokens is not None else Decimal(0)
             return answer, final_cost
         except Exception as e:
             if retries < self.max_retries:
                 time.sleep(wait * 2 ** retries)
-                return self._call_api(prompt, retries + 1)
+                return self._call_api(prompt, images, retries + 1)
             else:
                 return "", Decimal(0)
 
-    def make_prompt_request(self, prompt: str) -> Tuple[str, Decimal]:
-        final_prompt, _ = truncate_prompt(prompt, self.encoding, self.max_tokens_question)
-        return self._call_api(final_prompt)
+    def make_prompt_request(self, prompt: Prompt) -> Tuple[str, Decimal]:
+        final_prompt, _ = truncate_prompt(str(prompt), self.encoding, self.max_tokens_question)
+        return self._call_api(final_prompt, prompt.available_data if self.spec.multimodal else [])
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/chatgpt_model.py` & `parsee_core-0.1.4.0/parsee/extraction/models/llm_models/replicate_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 import os
 import time
 from typing import List, Tuple
 from dataclasses import dataclass
 from decimal import Decimal
 import math
 
-import openai
 import tiktoken
+import replicate
 
 from parsee.extraction.models.llm_models.llm_base_model import LLMBaseModel, get_tokens_encoded, truncate_prompt
 from parsee.extraction.models.model_dataclasses import MlModelSpecification
+from parsee.extraction.models.llm_models.prompts import Prompt
 
 
-class ChatGPTModel(LLMBaseModel):
+class ReplicateModel(LLMBaseModel):
 
     def __init__(self, model: MlModelSpecification):
-        super().__init__(model.name)
-        self.model = model
+        super().__init__(model)
         self.max_retries = 5
         self.encoding = tiktoken.get_encoding("cl100k_base")
         self.max_tokens_answer = 1024
-        self.max_tokens_question = self.model.max_tokens - self.max_tokens_answer
-        openai.api_key = model.api_key if model.api_key is not None else os.getenv("OPENAI_KEY")
+        self.max_tokens_question = self.spec.max_tokens - self.max_tokens_answer
 
-    def _call_api(self, prompt: str, retries: int = 0, wait: int = 5) -> Tuple[str, Decimal]:
+    def _call_api(self, prompt: str, retries: int = 0, wait: int = 5) -> str:
         try:
-            response = openai.ChatCompletion.create(
-                model=self.model.internal_name,
-                messages=[
-                    {
-                        "role": "user",
-                        "content": prompt
-                    }
-                ],
-                temperature=0,
-                max_tokens=self.max_tokens_answer,
-                top_p=1,
-                frequency_penalty=0,
-                presence_penalty=0
-            )
-
-            answer = response['choices'][0]["message"]["content"]
-            final_cost = Decimal(int(response["usage"]['total_tokens']) * (self.model.price_per_1k_tokens/1000)) if self.model.price_per_1k_tokens is not None else Decimal(0)
-            return answer, final_cost
+            response = replicate.run(self.spec.internal_name, input={
+                "prompt": prompt,
+                "top_k": 50,
+                "top_p": 0.9,
+                "temperature": 0,
+                "max_new_tokens": 1024,
+                "presence_penalty": 0,
+                "frequency_penalty": 0
+            })
+            answer = "".join(response)
+            return answer
         except Exception as e:
             if retries < self.max_retries:
                 time.sleep(wait * 2 ** retries)
                 return self._call_api(prompt, retries + 1)
             else:
-                return "", Decimal(0)
+                return ""
 
-    def make_prompt_request(self, prompt: str) -> Tuple[str, Decimal]:
-        final_prompt, _ = truncate_prompt(prompt, self.encoding, self.max_tokens_question)
-        return self._call_api(final_prompt)
+    def make_prompt_request(self, prompt: Prompt) -> Tuple[str, Decimal]:
+        final_prompt, num_tokens_input = truncate_prompt(str(prompt), self.encoding, self.max_tokens_question)
+        response = self._call_api(final_prompt)
+        tokens_response = len(get_tokens_encoded(response, self.encoding))
+        final_cost = Decimal((tokens_response + num_tokens_input) * (self.spec.price_per_1k_tokens/1000)) if self.spec.price_per_1k_tokens is not None else Decimal(0)
+        return response, final_cost
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/replicate_model.py` & `parsee_core-0.1.4.0/parsee/extraction/models/llm_models/ollama_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,49 +2,45 @@
 import time
 from typing import List, Tuple
 from dataclasses import dataclass
 from decimal import Decimal
 import math
 
 import tiktoken
-import replicate
+import ollama
+from ollama import Client
 
 from parsee.extraction.models.llm_models.llm_base_model import LLMBaseModel, get_tokens_encoded, truncate_prompt
 from parsee.extraction.models.model_dataclasses import MlModelSpecification
+from parsee.extraction.models.llm_models.prompts import Prompt
 
 
-class ReplicateModel(LLMBaseModel):
+class OllamaModel(LLMBaseModel):
 
     def __init__(self, model: MlModelSpecification):
-        super().__init__(model.name)
-        self.model = model
-        self.max_retries = 5
+        super().__init__(model)
+        self.max_retries = 0
         self.encoding = tiktoken.get_encoding("cl100k_base")
         self.max_tokens_answer = 1024
-        self.max_tokens_question = self.model.max_tokens - self.max_tokens_answer
+        self.max_tokens_question = self.spec.max_tokens - self.max_tokens_answer
+
+        self.client = Client(host='http://localhost:11434' if model.file_path is None else model.file_path)
 
     def _call_api(self, prompt: str, retries: int = 0, wait: int = 5) -> str:
         try:
-            response = replicate.run(self.model.internal_name, input={
-                "prompt": prompt,
-                "top_k": 50,
-                "top_p": 0.9,
-                "temperature": 0,
-                "max_new_tokens": 1024,
-                "presence_penalty": 0,
-                "frequency_penalty": 0
-            })
-            answer = "".join(response)
-            return answer
+            response = self.client.chat(model=self.spec.internal_name, messages=[
+                {
+                    'role': 'user',
+                    'content': prompt,
+                },
+            ])
+            return response["message"]["content"]
         except Exception as e:
             if retries < self.max_retries:
                 time.sleep(wait * 2 ** retries)
                 return self._call_api(prompt, retries + 1)
             else:
                 return ""
 
-    def make_prompt_request(self, prompt: str) -> Tuple[str, Decimal]:
-        final_prompt, num_tokens_input = truncate_prompt(prompt, self.encoding, self.max_tokens_question)
-        response = self._call_api(final_prompt)
-        tokens_response = len(get_tokens_encoded(response, self.encoding))
-        final_cost = Decimal((tokens_response + num_tokens_input) * (self.model.price_per_1k_tokens/1000)) if self.model.price_per_1k_tokens is not None else Decimal(0)
-        return response, final_cost
+    def make_prompt_request(self, prompt: Prompt) -> Tuple[str, Decimal]:
+        final_prompt, num_tokens_input = truncate_prompt(str(prompt), self.encoding, self.max_tokens_question)
+        return self._call_api(final_prompt), Decimal(0)
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/models/llm_models/structuring_schema.py` & `parsee_core-0.1.4.0/parsee/extraction/models/llm_models/structuring_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     def __init__(self, example: Optional[str] = None, default_value: Optional[str] = None):
         super().__init__([], example, default_value)
 
     def get_example(self, clean_value: bool = False) -> str:
         return self.example if self.is_valid_input(self.example) else "answer to question"
 
     def get_possible_values_str(self) -> str:
-        return "possible values: any text"
+        return "possible values: any text, but please only provide the 'entity' (e.g. a thing, company or person, depending on the question) and nothing else"
 
     def get_value(self, value: str) -> Tuple[str, bool]:
         val = get_entity_value(value)
         if val is None:
             return value.strip().rstrip(".").strip(), True
         return val.strip().rstrip(".").strip(), True
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/models/model_dataclasses.py` & `parsee_core-0.1.4.0/parsee/extraction/models/model_dataclasses.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,17 +16,21 @@
     max_tokens: Optional[int]
     api_key: Optional[str]
     only_questions: Optional[List[str]]
     only_elements: Optional[List[str]]
     only_meta: Optional[List[str]]
     only_mappings: Optional[List[str]]
     stats: Optional[Dict]
+    multimodal: bool
+    max_images: Optional[int]
+    max_image_pixels: Optional[int]
 
     def model_path(self) -> Union[None, str]:
         if self.file_path is None:
             return None
-        return os.path.join(self.file_path, "best_model.h5")
+        return self.file_path
 
     def settings_path(self) -> Union[None, str]:
         if self.file_path is None:
             return None
-        return os.path.join(self.file_path, "settings.pkl")
+        model_dir = os.path.dirname(self.file_path)
+        return os.path.join(model_dir, "settings.pkl")
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/models/model_loader.py` & `parsee_core-0.1.4.0/parsee/extraction/models/model_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from parsee.templates.element_schema import ElementDetectionSchema, ElementSchema
 from parsee.templates.general_structuring_schema import StructuringItemSchema, GeneralQuerySchema, GeneralQueryItemSchema
 from parsee.extraction.tasks.element_classification.element_model import ElementModel, AssignedElementModel
 from parsee.extraction.tasks.questions.question_model import QuestionModel, AssignedQuestionModel
 from parsee.extraction.models.llm_models.chatgpt_model import ChatGPTModel
 from parsee.extraction.models.llm_models.replicate_model import ReplicateModel
 from parsee.extraction.models.llm_models.anthropic_model import AnthropicModel
+from parsee.extraction.models.llm_models.ollama_model import OllamaModel
 from parsee.extraction.tasks.questions.question_model_llm import LLMQuestionModel
 from parsee.extraction.tasks.meta_info_structuring.meta_info import MetaInfoModel
 from parsee.extraction.tasks.meta_info_structuring.meta_info_llm import MetaLLMModel
 from parsee.extraction.tasks.element_classification.element_model_llm import ElementModelLLM
 from parsee.extraction.tasks.mappings.mapping_model import MappingModel
 from parsee.extraction.tasks.mappings.mapping_model_llm import MappingModelLLM
 from parsee.storage.interfaces import StorageManager
@@ -22,14 +23,16 @@
 def get_llm_base_model(spec: MlModelSpecification) -> LLMBaseModel:
     if spec.model_type == ModelType.GPT:
         return ChatGPTModel(spec)
     elif spec.model_type == ModelType.REPLICATE:
         return ReplicateModel(spec)
     elif spec.model_type == ModelType.ANTHROPIC:
         return AnthropicModel(spec)
+    elif spec.model_type == ModelType.OLLAMA:
+        return OllamaModel(spec)
     else:
         raise Exception("llm base model not found")
 
 
 class ModelLoader:
 
     def __init__(self, storage: StorageManager):
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/run.py` & `parsee_core-0.1.4.0/parsee/extraction/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,10 @@
     # run mapping
     all_mappings: List[ParseeBucket] = []
     tables = final_tables_from_columns(output_values)
     mapping_models = mapping_models_from_schema(job_template.detection, model_loader, params)
     for model_mapping in mapping_models:
         for table in tables:
             mappings, mapping_schema = model_mapping.classify_elements(table)
-            if mapping_schema is not None:
-                for col in table.columns:
-                    col.apply_mappings(mappings, mapping_schema)
             all_mappings += mappings
 
     return all_mappings, output_values, answers
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/element_model.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/element_classification/element_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/element_model_llm.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/element_classification/element_model_llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from typing import *
 import re
 
 from parsee.extraction.tasks.element_classification.element_model import ElementModel, ElementSchema, StandardDocumentFormat, ParseeLocation
 from parsee.storage.interfaces import StorageManager
-from parsee.utils.helper import is_number_cell, clean_numeric_value
+from parsee.utils.helper import is_number_cell, clean_numeric_value, parse_json_array
 from parsee.extraction.models.llm_models.llm_base_model import LLMBaseModel
 from parsee.extraction.tasks.element_classification.features import LLMLocationFeatureBuilder
 
 
 class ElementModelLLM(ElementModel):
 
     def __init__(self, items: List[ElementSchema], storage: StorageManager, llm: LLMBaseModel, **kwargs):
         super().__init__(items)
-        self.model_name = llm.model_name
+        self.model_name = llm.spec.internal_name
         self.llm = llm
         self.max_search_items = 10
         self.storage = storage
         self.prob = 0.8
         self.feature_builder: LLMLocationFeatureBuilder = LLMLocationFeatureBuilder()
 
-    def parse_prompt_answer(self, prompt_answer: str) -> Union[int, None]:
+    def parse_prompt_answer(self, prompt_answer: str) -> List[int]:
         answers = prompt_answer.splitlines()
+        output = []
         for k, answer in enumerate(answers):
-            result = re.search(r'(\[|)(\d+)(\]|)', answer)
-            if result is not None and len(result.groups()) > 2:
-                value_predicted = result.group(2)
-                clean_value = int(clean_numeric_value(value_predicted))
-                if is_number_cell(value_predicted) and clean_value >= 0:
-                    return clean_value
-        return None
+            values_predicted = parse_json_array(answer)
+            if values_predicted is not None:
+                for val in values_predicted:
+                    if isinstance(val, int):
+                        output.append(val)
+        return output
 
     def classify_elements(self, document: StandardDocumentFormat) -> List[ParseeLocation]:
 
         output: List[ParseeLocation] = []
-        PARTIAL_PROB = 0
 
         for item in self.items:
 
             prompt = self.feature_builder.make_prompt(item, document, self.storage)
 
-            answer, amount = self.llm.make_prompt_request(str(prompt))
+            answer, amount = self.llm.make_prompt_request(prompt)
             self.storage.log_expense(self.llm.model_name, amount, item.id)
 
-            best_idx = self.parse_prompt_answer(answer)
+            best_indexes = self.parse_prompt_answer(answer)
+
+            partial_prob = 0.0 if len(best_indexes) <= 1 else 0.6
 
-            if best_idx is not None and 0 <= best_idx < len(document.elements):
-                el = document.elements[best_idx]
-                location = ParseeLocation(self.model_name, PARTIAL_PROB, item.id, self.prob, el.source, [])
-                output.append(location)
+            for best_idx in best_indexes:
+                if 0 <= best_idx < len(document.elements):
+                    el = document.elements[best_idx]
+                    location = ParseeLocation(self.model_name, partial_prob, item.id, self.prob, el.source, [])
+                    output.append(location)
         return output
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/element_classification/features.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/element_classification/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,22 @@
         return temp_features
 
 
 class LLMLocationFeatureBuilder(LocationFeatureBuilder):
 
     def __init__(self):
         super().__init__()
-        self.number_replacement = "[number]"
+        self.number_replacement = "NUMBER"
 
     def build_raw_answer(self, locations: List[ParseeLocation]) -> str:
         sorted_ids = list(sorted([x.source.element_index for x in locations]))
         return f"[{','.join([str(x) for x in sorted_ids])}]"
 
     def get_elements_text(self, features: List[DatasetRow]):
-        llm_text = ""
+        llm_text = "This is the data to answer the question:\n"
         for feature_entry in features:
             llm_text += f"[{feature_entry.element_identifier}] text before table: {feature_entry.get_feature('text_before')}; line items in table: {feature_entry.get_feature('text')} [end of item] \n"
         return llm_text
 
     def make_prompt(self, item: ElementSchema, document: StandardDocumentFormat, storage: StorageManager) -> Prompt:
 
         if item.searchStrategy == SearchStrategy.VECTOR:
@@ -166,11 +166,11 @@
 
         additional_info_str = f" Additional info: {item.additionalInfo}" if item.additionalInfo.strip() != "" else ""
         all_element_indices = [x.source.element_index for x in closest_elements]
 
         features = self.make_features(None, None, all_element_indices, document.elements, False)
 
         prompt = Prompt("", f'we want to find an item labeled "{item.title}".{additional_info_str}', f"""We are providing data in the following with the element_index and the text, such as [ELEMENT_INDEX] "TEXT" [end of item].
-                Using the text, identify "{item.title}" and return the elements which you think are most likely representing "{item.title}" (it can be one item or several together).
-                It is very important that you only return the element_index and nothing else.""", "Your response could be for example: [10] or [241],[1204] ", self.get_elements_text(features))
+                Using the provided text, identify "{item.title}" and return the tables which you think are most likely representing "{item.title}" (it can be one item alone or several together that form the searched item).
+                Return the ELEMENT_INDEX of all items in a JSON array.""", "Your response could be for example: [10] or [241, 1204] ", self.get_elements_text(features))
 
         return prompt
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/mapping_model.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/mappings/mapping_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/mapping_model_llm.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/mappings/mapping_model_llm.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,34 +3,46 @@
 
 from parsee.extraction.tasks.mappings.mapping_model import MappingModel, ElementSchema, MappingSchema, ParseeBucket
 from parsee.storage.interfaces import StorageManager
 from parsee.extraction.models.llm_models.llm_base_model import LLMBaseModel
 from parsee.extraction.tasks.mappings.features import LLMMappingFeatureBuilder
 from parsee.extraction.extractor_elements import FinalOutputTable
 from parsee.utils.constants import ID_NOT_AVAILABLE
+from parsee.utils.helper import parse_json_dict, parse_int_simple
 
 
 class MappingModelLLM(MappingModel):
 
     def __init__(self, items: List[ElementSchema], storage: StorageManager, llm: LLMBaseModel, **kwargs):
         super().__init__(items)
-        self.model_name = llm.model_name
+        self.model_name = llm.spec.internal_name
         self.llm = llm
         self.storage = storage
         self.prob = 0.8
         self.feature_builder: LLMMappingFeatureBuilder = LLMMappingFeatureBuilder()
 
-    def parse_answer(self, answer: str, schema: MappingSchema, kv_idx: int, li_identifier: str) -> Union[None, ParseeBucket]:
+    def parse_answer(self, table: FinalOutputTable, answer: str, schema: MappingSchema, li_identifier: str) -> List[ParseeBucket]:
+        answer_dict = parse_json_dict(answer)
+        if answer_dict is None or not isinstance(answer_dict, Dict):
+            return []
+        output = []
+        handled = set()
         for bucket in schema.buckets:
-            if self.feature_builder.item_id_string(bucket).lower() in answer.lower() or bucket.id.lower() in answer.lower():
-                return ParseeBucket(schema.id, bucket.id, li_identifier, self.model_name, self.prob, kv_idx, 0, Decimal(1))
-        return ParseeBucket(schema.id, ID_NOT_AVAILABLE, li_identifier, self.model_name, self.prob, kv_idx, 0, Decimal(1))
+            if bucket.id in answer_dict and isinstance(answer_dict[bucket.id], List):
+                for answer in answer_dict[bucket.id]:
+                    line_item_idx = parse_int_simple(answer)
+                    if line_item_idx is not None:
+                        item = ParseeBucket(schema.id, bucket.id, li_identifier, self.model_name, self.prob, line_item_idx, 0, Decimal(1))
+                        output.append(item)
+                        handled.add(line_item_idx)
+        # handle items that have not been classified
+        for line_item_idx, _ in enumerate(table.line_items):
+            if line_item_idx not in handled:
+                output.append(ParseeBucket(schema.id, ID_NOT_AVAILABLE, li_identifier, self.model_name, self.prob, line_item_idx, 0, Decimal(1)))
+        return output
 
     def classify_with_schema(self, table: FinalOutputTable, schema: MappingSchema) -> List[ParseeBucket]:
 
-        output = []
-        for idx, _ in enumerate(table.line_items):
-            prompt = self.feature_builder.make_prompt(table, schema, idx)
-            answer, amount = self.llm.make_prompt_request(str(prompt))
-            self.storage.log_expense(self.llm.model_name, amount, f"mapping:{table.detected_class}")
-            output.append(self.parse_answer(answer, schema, idx, table.li_identifier))
-        return output
+        prompt = self.feature_builder.make_prompt(table, schema)
+        answer, amount = self.llm.make_prompt_request(prompt)
+        self.storage.log_expense(self.llm.model_name, amount, f"mapping:{table.detected_class}")
+        return self.parse_answer(table, answer, schema, table.li_identifier)
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/mappings/utils.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/mappings/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from parsee.extraction.extractor_dataclasses import ParseeBucket
 from parsee.templates.mappings import MappingSchema
 
 
 def calc_buckets(key_value_pairs: List[Tuple[str, any]], mappings: List[ParseeBucket], mapping_schema: MappingSchema) -> Dict[str, Decimal]:
 
     if len(mappings) != len(key_value_pairs):
-        raise Exception("mappings not same length")
+        return {}
 
     output = {}
 
     # TODO: improve
 
     for k, mapping in enumerate(mappings):
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/features.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/meta_info_structuring/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,14 +241,15 @@
             output += f"{k + 1}) {get_prompt_schema_item(item).get_example()}\n"
 
         return output
 
     def build_prompt(self, features: DatasetRow, col_idx: int, items: List[StructuringItemSchema]) -> Prompt:
 
         available_data = f'''
+                This is the information that is available:\n
                 The current column index is: {col_idx}. \n
                 On top of the column (in the header part), there is this text: "{features.get_feature('top_column_all')}"\n
                 The content of the table is the following (excluding any numbers): {features.get_feature('li_and_values')}\n
                 On top of the line items, there is this text: "{features.get_feature('top_li_reworked')}\n"
 
                 Before the table starts, there is this text: "{features.get_feature('before')}"\n
                 '''
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/meta_info.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/meta_info_structuring/meta_info.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,40 +12,40 @@
 
 
 class MetaLLMModel(MetaInfoModel):
 
     def __init__(self, items: List[StructuringItemSchema], llm: LLMBaseModel, storage: StorageManager, **kwargs):
         super().__init__(items)
         self.storage = storage
-        self.model_name = llm.model_name if llm is not None else "llm"
+        self.model_name = llm.spec.internal_name if llm is not None else "llm"
         self.default_prob_answer = 0.8
         self.elements = []
         self.llm = llm
         self.feature_builder: LLMMetaFeatureBuilder = LLMMetaFeatureBuilder()
 
     def parse_prompt_answer(self, prompt_answer: str) -> Dict[str, Tuple[str, bool]]:
         answers = prompt_answer.splitlines()
         output = {}
         for k, answer in enumerate(answers):
             result = re.search(r'((\d+)\) *)(.+)', answer)
             if result is not None and len(result.groups()) > 2:
                 number = result.group(2)
                 value_predicted = result.group(3)
-                number_check = (int(number) == k + 1) if number.isdigit() else False
-                if number_check:
-                    output[self.items[k].id] = get_prompt_schema_item(self.items[k]).get_value(value_predicted)
+                if number.isdigit() and 0 <= int(number)-1 < len(self.items):
+                    item_idx = int(number)-1
+                    output[self.items[item_idx].id] = get_prompt_schema_item(self.items[item_idx]).get_value(value_predicted)
         return output
 
     def predict_meta(self, columns: List[FinalOutputTableColumn], elements: List[ExtractedEl]) -> List[List[ParseeMeta]]:
 
         all_output = []
         for column in columns:
             prompt = self.feature_builder.make_prompt(column, elements, self.items)
 
-            prompt_answer, amount = self.llm.make_prompt_request(str(prompt))
+            prompt_answer, amount = self.llm.make_prompt_request(prompt)
 
             self.storage.log_expense(self.llm.model_name, amount, "meta LLM")
 
             prediction_dict = self.parse_prompt_answer(prompt_answer)
 
             output: List[ParseeMeta] = []
             for key, values in prediction_dict.items():
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/questions/features.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/questions/features.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,72 +14,75 @@
 class GeneralQueriesPromptBuilder:
 
     storage: StorageManager
 
     def __init__(self, storage: StorageManager):
         self.storage = storage
 
-    def build_raw_value(self, main_value: any, meta: List[ParseeMeta], sources: List[ExtractedSource], item: GeneralQueryItemSchema, meta_items: List[StructuringItemSchema]):
+    def build_raw_value(self, main_value: any, meta: List[ParseeMeta], sources: List[ExtractedSource], item: GeneralQueryItemSchema, meta_items: List[StructuringItemSchema], add_sources: bool = True):
         schema_item = get_prompt_schema_item(item)
         if len(meta_items) > 0:
             output = f"{MAIN_QUESTION_STR}: {main_value}"
             for meta_item in meta_items:
                 meta_schema_item = get_prompt_schema_item(meta_item)
                 meta_answers = [x for x in meta if x.class_id == meta_item.id]
                 answer_chosen = meta_answers[0].class_value if len(meta_answers) > 0 else "n/a"
                 output += f"\n({meta_item.id}): {meta_schema_item.parsed_to_raw(answer_chosen)}"
         else:
             output = f"{schema_item.parsed_to_raw(main_value)}"
-        output += "\nSources: " + ",".join(f"[{x.element_index}]" for x in sources)
+        if add_sources:
+            output += "\nSources: " + ",".join(f"[{x.element_index}]" for x in sources)
         return output
 
     def get_relevant_elements(self, schema_item: GeneralQueryItemSchema, document: StandardDocumentFormat) -> List[ExtractedEl]:
 
         if schema_item.searchStrategy == SearchStrategy.VECTOR:
             return self.storage.vector_store.find_closest_elements(document, schema_item.title, schema_item.keywords, False)
         elif schema_item.searchStrategy == SearchStrategy.START:
             return document.elements
         else:
             raise NotImplemented
 
     def get_elements_text(self, elements: List[ExtractedEl]):
-        llm_text = " (For the following data, if tables have empty cells, they are omitted)\n"
+        llm_text = "This is the available data to answer the question (in the following, if tables have empty cells, they are omitted):\n"
         for el in elements:
             llm_text += f"[{el.source.element_index}]: {el.get_text_llm(True)}\n"
         return llm_text
 
-    def build_prompt(self, structuring_item: GeneralQueryItemSchema, meta_items: List[StructuringItemSchema], document: StandardDocumentFormat, relevant_elements_custom: Optional[List[ExtractedEl]] = None) -> Prompt:
+    def build_prompt(self, structuring_item: GeneralQueryItemSchema, meta_items: List[StructuringItemSchema], document: StandardDocumentFormat, relevant_elements_custom: Optional[List[ExtractedEl]] = None, multimodal: bool = False, max_images: Optional[int] = None, max_image_size: Optional[int] = None) -> Prompt:
 
         elements = self.get_relevant_elements(structuring_item, document) if relevant_elements_custom is None else relevant_elements_custom
 
-        general_info = "You are supposed to answer a question based on text fragments that are provided. " \
-                       "The fragments start with a number and then the actual text. The lower the number of the fragment, " \
-                       "the earlier the fragment appeared in the document (reading from left to right, top to bottom). " \
-                       "Please respond as concise as possible."
+        if not multimodal:
+            general_info = "You are supposed to answer a question based on text fragments that are provided. " \
+                           "The fragments start with a number and then the actual text. The lower the number of the fragment, " \
+                           "the earlier the fragment appeared in the document (reading from left to right, top to bottom). " \
+                           "Please respond as concise as possible."
+        else:
+            general_info = "You are supposed to answer a question based on one or several images that are provided below."
 
         prompt_schema_item = get_prompt_schema_item(structuring_item)
 
         additional_info_str = f" Additional info: {structuring_item.additionalInfo}" if structuring_item.additionalInfo.strip() != "" else ""
         main_question = f'The question is: {structuring_item.title} {additional_info_str} {prompt_schema_item.get_possible_values_str()}'
 
         relevant_meta_items = [x for x in meta_items if structuring_item.metaInfoIds is not None and x.id in structuring_item.metaInfoIds]
 
         # build full example
         source_examples = [ExtractedSource(DocumentType.PDF, None, None, 241, None), ExtractedSource(DocumentType.PDF, None, None, 423, None)]
         meta_examples = [ParseeMeta("test", 0, source_examples, x.id, get_prompt_schema_item(x).get_example(True), 0.8) for x in relevant_meta_items]
-        example_output = self.build_raw_value(prompt_schema_item.get_example(), meta_examples, source_examples, structuring_item, meta_items)
+        example_output = self.build_raw_value(prompt_schema_item.get_example(), meta_examples, source_examples, structuring_item, relevant_meta_items, not multimodal)
 
         full_example = f"Your answer could look like this: {example_output}" if len(relevant_meta_items) == 0 else f"One possible answer block could be (there can be more than one in your response): {example_output}"
 
         # add prompting for meta
         if len(relevant_meta_items) > 0:
             main_question += "\n We also want to retrieve some meta information. In the following we will present the meta item ID and then the additional question to be answered, format: (META_ID): QUESTION. In the answer please first provide the meta ID (for the main question use 'main question' instead) in brackets and then the answer. If there are several possible answers to the question (with different meta values), structure your answer into multiple answer blocks of the same format, one after the other separated by new lines."
             for meta_item in relevant_meta_items:
                 meta_prompt_item = get_prompt_schema_item(meta_item)
                 main_question += f"\n({meta_item.id}): {meta_item.title} {meta_item.additionalInfo} {meta_prompt_item.get_possible_values_str()}"
 
         prompt = Prompt(general_info, main_question,
-                        'Please at the end of each answer also provide the numbers of the text fragments you used to answer in square brackets.',
+                        'Please at the end of each answer also provide the numbers of the text fragments you used to answer in square brackets.' if not multimodal else "",
                         full_example,
-                        self.get_elements_text(elements))
-
-        return prompt
+                        self.get_elements_text(elements) if not multimodal else self.storage.image_creator.get_images(document, elements, max_images, max_image_size))
+        return prompt
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/questions/question_model.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/questions/question_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/questions/question_model_llm.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/questions/question_model_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import *
 
-from parsee.extraction.extractor_elements import StandardDocumentFormat, ExtractedEl
+from parsee.extraction.extractor_elements import StandardDocumentFormat
 from parsee.extraction.tasks.questions.question_model import QuestionModel
 from parsee.extraction.tasks.questions.features import GeneralQueriesPromptBuilder
 from parsee.extraction.extractor_dataclasses import ParseeAnswer, ParseeMeta
 from parsee.storage.interfaces import StorageManager
 from parsee.extraction.models.llm_models.llm_base_model import LLMBaseModel
 from parsee.extraction.tasks.questions.utils import parse_sources, parse_answer_blocks, parse_main_and_meta, MAIN_QUESTION_STR
 from parsee.templates.general_structuring_schema import StructuringItemSchema, GeneralQueryItemSchema
 from parsee.extraction.models.llm_models.structuring_schema import get_prompt_schema_item
-from parsee.datasets.dataset_dataclasses import DatasetRow
+from parsee.extraction.models.llm_models.prompts import Prompt
 
 
 class LLMQuestionModel(QuestionModel):
 
     def __init__(self, items: List[GeneralQueryItemSchema], meta_items: List[StructuringItemSchema], storage: StorageManager, llm: LLMBaseModel, **kwargs):
         super().__init__(items, meta_items)
         self.storage = storage
         self.llm = llm
-        self.model_name = llm.model_name
+        self.model_name = llm.spec.internal_name
         self.prompt_builder = GeneralQueriesPromptBuilder(storage)
 
     def parse_prompt_answer(self, item: GeneralQueryItemSchema, prompt_answer: str, total_elements: Optional[int], document: Optional[StandardDocumentFormat]) -> List[ParseeAnswer]:
 
         multi_block = item.metaInfoIds is not None and len(item.metaInfoIds) > 0
 
         answer_blocks = parse_answer_blocks(prompt_answer) if multi_block else [prompt_answer]
@@ -57,20 +57,20 @@
 
             if main_answer is not None:
 
                 output.append(ParseeAnswer(self.model_name, sources_full, item.id, main_answer, answer_block, parse_successful, detected_meta))
 
         return output
 
-    def predict_for_prompt(self, prompt: str, schema_item: GeneralQueryItemSchema, max_element_index: Optional[int], document: Optional[StandardDocumentFormat]) -> List[ParseeAnswer]:
-        prompt_answer, amount = self.llm.make_prompt_request(str(prompt))
-        self.storage.log_expense(self.llm.model_name, amount, schema_item.id)
+    def predict_for_prompt(self, prompt: Prompt, schema_item: GeneralQueryItemSchema, max_element_index: Optional[int], document: Optional[StandardDocumentFormat]) -> List[ParseeAnswer]:
+        prompt_answer, amount = self.llm.make_prompt_request(prompt)
+        self.storage.log_expense(self.llm.spec.internal_name, amount, schema_item.id)
         return self.parse_prompt_answer(schema_item, prompt_answer, max_element_index, document)
 
     def predict_answers(self, document: StandardDocumentFormat) -> List[ParseeAnswer]:
 
         answers: List[ParseeAnswer] = []
         for schema_item in self.items:
-            prompt = self.prompt_builder.build_prompt(schema_item, self.meta, document)
-            answers += self.predict_for_prompt(str(prompt), schema_item, len(document.elements), document)
+            prompt = self.prompt_builder.build_prompt(schema_item, self.meta, document, None, self.llm.spec.multimodal, self.llm.spec.max_images, self.llm.spec.max_image_pixels)
+            answers += self.predict_for_prompt(prompt, schema_item, len(document.elements), document)
 
         return answers
```

### Comparing `parsee_core-0.1.3.9/parsee/extraction/tasks/questions/utils.py` & `parsee_core-0.1.4.0/parsee/extraction/tasks/questions/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/storage/in_memory_storage.py` & `parsee_core-0.1.4.0/parsee/storage/in_memory_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from copy import deepcopy
 
 from parsee.storage.interfaces import StorageManager
 from parsee.storage.vector_stores.simple_faiss import SimpleFaissStore
 from parsee.extraction.models.model_dataclasses import MlModelSpecification
 from parsee.templates.job_template import JobTemplate
 from parsee.extraction.extractor_dataclasses import AssignedMeta, AssignedLocation, AssignedAnswer, AssignedBucket
+from parsee.converters.image_creation import DiskImageCreator
 
 
 class InMemoryStorageManager(StorageManager):
     
     truth_questions: List[AssignedAnswer]
     truth_locations: List[AssignedLocation]
     truth_meta: List[AssignedMeta]
     truth_mappings: List[AssignedBucket]
 
     def __init__(self, available_models: Optional[List[MlModelSpecification]]):
-        super().__init__(SimpleFaissStore())
+        super().__init__(SimpleFaissStore(), DiskImageCreator())
         self.models = available_models if available_models is not None else []
         self.truth_questions = []
         self.truth_locations = []
 
     def get_available_models(self) -> List[MlModelSpecification]:
         return self.models if self.models is not None else []
```

### Comparing `parsee_core-0.1.3.9/parsee/storage/interfaces.py` & `parsee_core-0.1.4.0/parsee/storage/interfaces.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 from parsee.extraction.extractor_elements import StandardDocumentFormat, FinalOutputTableColumn, ParseeAnswer
 from parsee.utils.enums import DocumentType
 from parsee.templates.job_template import JobTemplate
 from parsee.extraction.extractor_dataclasses import ParseeBucket
 from parsee.extraction.models.model_dataclasses import MlModelSpecification
 from parsee.datasets.readers.interfaces import ModelReader
 from parsee.storage.vector_stores.interfaces import VectorStore
+from parsee.extraction.extractor_elements import ExtractedEl
+from parsee.converters.image_creation import ImageCreator
 
 
 class StorageManager:
 
     vector_store: VectorStore
+    image_creator: ImageCreator
 
-    def __init__(self, vector_store: VectorStore):
+    def __init__(self, vector_store: VectorStore, image_creator: ImageCreator):
         self.vector_store = vector_store
+        self.image_creator = image_creator
 
     def db_values_template(self, job_template: JobTemplate, strict: bool) -> JobTemplate:
         raise NotImplemented
 
     def log_expense(self, service: str, amount: Decimal, class_id: str):
         raise NotImplemented
```

### Comparing `parsee_core-0.1.3.9/parsee/storage/vector_stores/simple_faiss.py` & `parsee_core-0.1.4.0/parsee/storage/vector_stores/simple_faiss.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class SimpleFaissStore(VectorStore):
 
     def __init__(self):
         self.encoder = SentenceTransformer('all-MiniLM-L6-v2')
         self.min_chunk_size_characters = 1000
         self.k = 100
+        self.indexes = {}
 
     def make_index(self, document: StandardDocumentFormat, tables_only: bool) -> Tuple[List[List[int]], any]:
         data = []
         current_batch = {"chars": 0, "element_indices": [], "text": ""}
         for k, el in enumerate(document.elements):
             if el.el_type == ElementType.TABLE:
                 data.append(
@@ -51,16 +52,19 @@
 
         d = sentence_embeddings.shape[1]
         index = faiss.IndexFlatL2(d)
         index.add(sentence_embeddings)
 
         return [x["element_indices"] for x in data], index
 
-    def get_index(self, document: StandardDocumentFormat, tables_only: bool):
-        return self.make_index(document, tables_only)
+    def get_index(self, document: StandardDocumentFormat, tables_only: bool) -> Tuple[List[List[int]], any]:
+        key = (document.source_identifier, tables_only)
+        if key not in self.indexes:
+            self.indexes[key] = self.make_index(document, tables_only)
+        return self.indexes[key]
 
     def find_closest_elements(self, document: StandardDocumentFormat, search_element_title: str, keywords: Optional[str], tables_only: bool = True) -> List[ExtractedEl]:
 
         element_indices, index = self.get_index(document, tables_only)
 
         query = f"{search_element_title}" + (f"; {keywords}" if keywords is not None else "")
```

### Comparing `parsee_core-0.1.3.9/parsee/templates/element_schema.py` & `parsee_core-0.1.4.0/parsee/templates/element_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 @dataclass
 class ElementSchema:
     id: str
     title: str
     additionalInfo: str
     keywords: str
     takeBestInProximity: bool
+    collapseColumns: bool
     model: Optional[str]
     searchStrategy: SearchStrategy
     mapRows: Union[None, MappingSchema]
     mappingModel: Optional[str]
     metaInfoIds: List[str]
 
     def to_json_dict(self) -> Dict:
         return {"id": self.id, "title": self.title, "additionalInfo": self.additionalInfo, "keywords": self.keywords,
-                "takeBestInProximity": self.takeBestInProximity, "model": self.model, "searchStrategy": self.searchStrategy.value,
+                "takeBestInProximity": self.takeBestInProximity, "collapseColumns": self.collapseColumns, "model": self.model, "searchStrategy": self.searchStrategy.value,
                 "mapRows": self.mapRows.to_json_dict() if self.mapRows is not None else None,
                 "mappingModel": self.mappingModel,
                 "metaInfoIds": self.metaInfoIds
                 }
 
 
 @dataclass
```

### Comparing `parsee_core-0.1.3.9/parsee/templates/general_structuring_schema.py` & `parsee_core-0.1.4.0/parsee/templates/general_structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/templates/helpers.py` & `parsee_core-0.1.4.0/parsee/templates/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,45 +16,45 @@
         id_store[category] = 0
     id_store[category] += 1
     return f"{category}{id_store[category]}"
 
 
 class MetaItem(StructuringItemSchema):
 
-    def __init__(self, question: str, output_type: OutputType, list_values: Optional[List[str]] = None, assigned_id: Optional[str] = None):
+    def __init__(self, question: str, output_type: OutputType, list_values: Optional[List[str]] = None, assigned_id: Optional[str] = None, example: Optional[str] = None, additional_info: Optional[str] = None):
 
         self.model = None
         self.type = output_type
         self.context = ContextType.QUESTIONS
         self.id = simple_id("meta") if assigned_id is None else assigned_id
         self.title = question
-        self.additionalInfo = ""
+        self.additionalInfo = "" if additional_info is None else additional_info
         self.searchStrategy = SearchStrategy.VECTOR
         self.valuesList = list_values
-        self.example = None
+        self.example = example
         self.keywords = None
         self.defaultValue = None
         self.customArgsJson = None
 
 
 class StructuringItem(GeneralQueryItemSchema):
 
-    def __init__(self, question: str, output_type: OutputType, list_values: Optional[List[str]] = None, meta_info: Optional[List[MetaItem]] = None, assigned_id: Optional[str] = None):
+    def __init__(self, question: str, output_type: OutputType, list_values: Optional[List[str]] = None, meta_info: Optional[List[MetaItem]] = None, assigned_id: Optional[str] = None, example: Optional[str] = None, additional_info: Optional[str] = None):
 
         self.model = None
         self.type = output_type
         self.context = ContextType.QUESTIONS
         self.id = simple_id("question") if assigned_id is None else assigned_id
         self.title = question
-        self.additionalInfo = ""
+        self.additionalInfo = "" if additional_info is None else additional_info
         self.searchStrategy = SearchStrategy.VECTOR
         self.valuesList = list_values
         self.metaInfoIds = [] if meta_info is None else [x.id for x in meta_info]
         self.meta_info = meta_info
-        self.example = None
+        self.example = example
         self.keywords = None
         self.valuesList = None
         self.defaultValue = None
         self.customArgsJson = None
 
 
 class RowMapping:
@@ -68,14 +68,15 @@
     def __init__(self, item_title: str, keywords: str, meta_info: Optional[List[MetaItem]] = None, row_mapping: Optional[RowMapping] = None, item_description: str = "", assigned_id: Optional[str] = None):
 
         self.id = simple_id("table") if assigned_id is None else assigned_id
         self.title = item_title
         self.additionalInfo = item_description
         self.keywords = keywords
         self.takeBestInProximity = False
+        self.collapseColumns = False
         self.model = None
         self.searchStrategy = SearchStrategy.VECTOR
         self.mapRows = row_mapping
         self.mappingModel = None
         self.metaInfoIds = [] if meta_info is None else [x.id for x in meta_info]
         self.meta_info = meta_info
```

### Comparing `parsee_core-0.1.3.9/parsee/templates/job_template.py` & `parsee_core-0.1.4.0/parsee/templates/job_template.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/templates/mappings.py` & `parsee_core-0.1.4.0/parsee/templates/mappings.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.3.9/parsee/utils/enums.py` & `parsee_core-0.1.4.0/parsee/utils/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 
 
 class DocumentType(Enum):
     HTML = "html"
     PDF = "pdf"
+    TEXT = "text"
 
 
 class ElementType(Enum):
     TEXT = "text"
     TABLE = "table"
     FIGURE = "figure"
 
@@ -43,7 +44,8 @@
 
 
 class ModelType(Enum):
     GPT = "gpt"
     CUSTOM = "custom"
     REPLICATE = "replicate"
     ANTHROPIC = "anthropic"
+    OLLAMA = "ollama"
```

### Comparing `parsee_core-0.1.3.9/parsee/utils/helper.py` & `parsee_core-0.1.4.0/parsee/utils/helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import *
 import re
 from decimal import Decimal
 import time
 import hashlib
+import json
 
 import numpy as np
 
 
 def clean_numeric_value_llm(string_val) -> Union[float, None]:
     matches = re.findall(r'(\d+(\d|,|\.|)*\d|\d)', string_val)
     last_numeric = None
@@ -30,37 +31,37 @@
     match = re.search(r'(\d\d\d\d\-\d\d\-\d\d)', string_val)
     if match:
         return match.group(1)
     else:
         return None
 
 
-def is_negative(cell_str):
+def is_negative(cell_str) -> bool:
     # minus
-    if re.search(r'(-|—|–|‒|―|–|−)( | |)*\d', cell_str.strip()):
+    if re.search(r'(-|—|–|‒|―|–|−)', cell_str):
         return True
     # brackets
     if re.search(r'\([\d ,.%]+(\)|\b)', cell_str.strip()):
         return True
     return False
 
 
-def comma_separator_thousands(cell_str):
+def comma_separator_thousands(cell_str) -> bool:
     if re.search(r'\b[0-9]{1,3}[,][0-9]{3}\b', cell_str):
         return True
     return False
 
 
-def dot_separator_thousands(cell_str):
+def dot_separator_thousands(cell_str) -> bool:
     if re.search(r'\b[0-9]{1,3}[.][0-9]{3}\b', cell_str):
         return True
     return False
 
 
-def clean_numeric_value(cell_str: str):
+def clean_numeric_value(cell_str: str) -> Union[None, Decimal]:
     if cell_str.strip() == "":
         return None
     mult = 1
     if is_negative(cell_str):
         mult = -1
 
     cell_str = re.sub(r'[^0-9,.]', '', cell_str)
@@ -193,20 +194,57 @@
 
     # delete trailing zeros
     num = delete_trailing_zeros(num)
 
     return num
 
 
+def get_source_identifier_simple(text: str) -> str:
+    sha = hashlib.sha256()
+    sha.update(str.encode(text, 'utf-8'))
+    return sha.hexdigest()
+
+
 def get_source_identifier(file_path: str) -> str:
     BUF_SIZE = 65536
 
     sha = hashlib.sha256()
 
     with open(file_path, 'rb') as f:
         while True:
             data = f.read(BUF_SIZE)
             if not data:
                 break
             sha.update(data)
 
-    return sha.hexdigest()
+    return sha.hexdigest()
+
+
+def parse_int_simple(string_val: str) -> Union[None, int]:
+    num = re.sub(r'[^0-9]', '', str(string_val))
+    if num.isdigit():
+        return int(num)
+    return None
+
+
+def parse_json_dict(string_val: str) -> Union[None, Dict[str, any]]:
+    match = re.search(r'({[\s\S]+})', string_val)
+    if match:
+        try:
+            parsed = json.loads(match.group(1))
+            return parsed
+        except Exception as e:
+            return None
+    else:
+        return None
+
+
+def parse_json_array(string_val: str) -> Union[None, List[any]]:
+    result = re.search(r'(\[[^\]]*\])', string_val)
+    if result is not None and len(result.groups()) > 0:
+        try:
+            values_predicted = json.loads(result.group(1))
+            if isinstance(values_predicted, list):
+                return values_predicted
+        except Exception as e:
+            return None
+    return None
```

### Comparing `parsee_core-0.1.3.9/pyproject.toml` & `parsee_core-0.1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsee-core"
-version = "0.1.3.9"
+version = "0.1.4.0"
 description = ""
 authors = ["Parsee.ai <info@parsee.ai>"]
 homepage = "https://parsee.ai"
 packages = [{include = "parsee"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
@@ -13,18 +13,20 @@
 numpy = "^1.23.1"
 tiktoken = "^0.4.0"
 openai = "^0.27.8"
 pydantic = "^1.6.2"
 faiss-cpu = [{version = "<1.7.1", platform = "darwin"}, {version = "^1.7.1", platform = "linux"}]
 replicate = "^0.23.1"
 beautifulsoup4 = "^4.11.1"
-parsee-pdf-reader = "^0.1.5.2"
+parsee-pdf-reader = "^0.1.5.7"
 sentence-transformers = "^2.2.2"
 lxml = "^4.9.1"
 anthropic = "^0.20.0"
+ollama = "^0.1.7"
+opencv-python = "^4.9.0.80"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.extras.dependencies]
 langchain = "^0.1.11"
 
 [build-system]
```

### Comparing `parsee_core-0.1.3.9/PKG-INFO` & `parsee_core-0.1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: parsee-core
-Version: 0.1.3.9
+Version: 0.1.4.0
 Summary: 
 Home-page: https://parsee.ai
 Author: Parsee.ai
 Author-email: info@parsee.ai
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: anthropic (>=0.20.0,<0.21.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: faiss-cpu (<1.7.1) ; sys_platform == "darwin"
 Requires-Dist: faiss-cpu (>=1.7.1,<2.0.0) ; sys_platform == "linux"
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
+Requires-Dist: ollama (>=0.1.7,<0.2.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: parsee-pdf-reader (>=0.1.5.2,<0.2.0.0)
+Requires-Dist: parsee-pdf-reader (>=0.1.5.7,<0.2.0.0)
 Requires-Dist: pydantic (>=1.6.2,<2.0.0)
 Requires-Dist: replicate (>=0.23.1,<0.24.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
```

