# Comparing `tmp/langfun-0.0.2.dev20240409.tar.gz` & `tmp/langfun-0.0.2.dev20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240409.tar", last modified: Tue Apr  9 08:03:33 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240410.tar", last modified: Wed Apr 10 08:03:52 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240409.tar` & `langfun-0.0.2.dev20240410.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.803562 langfun-0.0.2.dev20240409/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-09 08:03:33.803562 langfun-0.0.2.dev20240409/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.783563 langfun-0.0.2.dev20240409/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.791563 langfun-0.0.2.dev20240409/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.791563 langfun-0.0.2.dev20240409/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.791563 langfun-0.0.2.dev20240409/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.795563 langfun-0.0.2.dev20240409/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54551 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21083 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.795563 langfun-0.0.2.dev20240409/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.795563 langfun-0.0.2.dev20240409/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.795563 langfun-0.0.2.dev20240409/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.799563 langfun-0.0.2.dev20240409/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.799563 langfun-0.0.2.dev20240409/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19249 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19610 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.803562 langfun-0.0.2.dev20240409/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:03:33.803562 langfun-0.0.2.dev20240409/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-09 08:03:33.000000 langfun-0.0.2.dev20240409/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-09 08:03:33.000000 langfun-0.0.2.dev20240409/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:03:33.000000 langfun-0.0.2.dev20240409/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-09 08:03:33.000000 langfun-0.0.2.dev20240409/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 08:03:33.000000 langfun-0.0.2.dev20240409/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:03:33.803562 langfun-0.0.2.dev20240409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-09 08:03:13.000000 langfun-0.0.2.dev20240409/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.200279 langfun-0.0.2.dev20240410/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-10 08:03:52.200279 langfun-0.0.2.dev20240410/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.184279 langfun-0.0.2.dev20240410/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.188279 langfun-0.0.2.dev20240410/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.188279 langfun-0.0.2.dev20240410/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.192279 langfun-0.0.2.dev20240410/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.192279 langfun-0.0.2.dev20240410/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54551 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21083 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.196279 langfun-0.0.2.dev20240410/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.196279 langfun-0.0.2.dev20240410/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.196279 langfun-0.0.2.dev20240410/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.196279 langfun-0.0.2.dev20240410/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.200279 langfun-0.0.2.dev20240410/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19249 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20846 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19610 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.200279 langfun-0.0.2.dev20240410/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:03:52.200279 langfun-0.0.2.dev20240410/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-10 08:03:52.000000 langfun-0.0.2.dev20240410/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-10 08:03:52.000000 langfun-0.0.2.dev20240410/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:03:52.000000 langfun-0.0.2.dev20240410/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-10 08:03:52.000000 langfun-0.0.2.dev20240410/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 08:03:52.000000 langfun-0.0.2.dev20240410/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:03:52.200279 langfun-0.0.2.dev20240410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-10 08:03:26.000000 langfun-0.0.2.dev20240410/setup.py
```

### Comparing `langfun-0.0.2.dev20240409/LICENSE` & `langfun-0.0.2.dev20240410/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/PKG-INFO` & `langfun-0.0.2.dev20240410/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240409
+Version: 0.0.2.dev20240410
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240409/README.md` & `langfun-0.0.2.dev20240410/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/__init__.py` & `langfun-0.0.2.dev20240410/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240410/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/component.py` & `langfun-0.0.2.dev20240410/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/component_test.py` & `langfun-0.0.2.dev20240410/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240410/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240410/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/console.py` & `langfun-0.0.2.dev20240410/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/console_test.py` & `langfun-0.0.2.dev20240410/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240410/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240410/langfun/core/eval/base_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
   def test_basics(self):
     lm = fake.StaticSequence(['two', 'Solution(final_answer=2)'])
     s = eval_set('basic_test', 'call', schema_fn=answer_schema(), lm=lm)
 
     self.assertEqual(s.dir, os.path.join(s.root_dir, s.id))
     self.assertEqual(s.hash, s.clone().hash)
     # Test persistent hash.
-    self.assertEqual(s.hash, 'abc7c29a')
+    self.assertEqual(s.hash, '4a2f9694')
     self.assertEqual(
         s.hash, s.clone(override={'max_workers': 2, 'lm.timeout': 20}).hash
     )
     self.assertNotEqual(
         s.hash, s.clone(override={'prompt': 'Hello {{example.question}}'}).hash
     )
     self.assertIsNone(s.parent)
@@ -205,15 +205,15 @@
     ])
     s = eval_set('run_test', 'query', schema_fn=answer_schema(), lm=lm)
     s.run()
     self.assertEqual(
         s.result,
         dict(
             experiment_setup=dict(
-                id='Evaluation@17915dc6',
+                id='Evaluation@28030a68',
                 dir=s.dir,
                 model='StaticSequence',
                 prompt_template='{{example.question}}',
                 method='query',
                 schema_fn='answer_schema()',
             ),
             cache_stats=dict(
@@ -317,15 +317,15 @@
         max_workers=1,
     )
     self.assertEqual(s.children[0].id, f'{s.id}@{s.children[0].hash}')
     self.assertEqual(
         s.children[0].dir, os.path.join(s.root_dir, s.children[0].id)
     )
     # Test persistent hash.
-    self.assertEqual(s.hash, 'ca7f722b')
+    self.assertEqual(s.hash, 'e2a499d0')
 
     summary = s.run(verbose=True)
     self.assertEqual(len(summary.evaluations), 2)
 
     self.assertEqual(
         s.result,
         {
@@ -444,15 +444,15 @@
             eval_set('run_test_2',
                      pg.oneof(['call', 'query']),
                      schema_fn=pg.oneof([answer_schema(), answer_schema()])),
         ],
         lm=lm
     )
     # Test for persistent hash.
-    self.assertEqual(s.hash, '7285e52b')
+    self.assertEqual(s.hash, '8eb9e73f')
     s.run()
     expected = {
         s.children[0].id: dict(
             experiment_setup=dict(
                 id=s.children[0].id,
                 dir=s.children[0].dir,
                 model='StaticSequence',
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240410/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240410/langfun/core/eval/matching_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     s = eval_set('match_run_test', 'query', schema_fn=answer_schema(), lm=lm)
     s.run()
     self.assertEqual(
         s.result,
         dict(
             experiment_setup=dict(
-                id='MyTask@3d87f97f',
+                id='MyTask@9e3c5aa3',
                 dir=s.dir,
                 model='StaticSequence',
                 prompt_template='{{example.question}}',
                 method='query',
                 schema_fn='answer_schema()',
             ),
             cache_stats=dict(
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240410/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240410/langfun/core/eval/scoring_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,21 +71,22 @@
   def test_run(self):
     lm = fake.StaticSequence([
         '[0.5, 0.2, 0.3]',
         '[0.6, 0.7]',
     ])
 
     s = eval_set(lm=lm)
+    self.maxDiff = None
     self.assertEqual(s.avg_score, 0.0)
     s.run()
     self.assertEqual(
         s.result,
         dict(
             experiment_setup=dict(
-                id='ConstraintFollowing@9e51bb9e',
+                id='ConstraintFollowing@76285393',
                 dir=s.dir,
                 model='StaticSequence',
                 prompt_template='{{example}}',
                 method='query',
                 schema_fn='float_list()',
             ),
             cache_stats=dict(
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240410/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240410/langfun/core/langfunc_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     self.assertEqual(str(l), 'Hello')
     print(repr(l))
     self.assertEqual(
         repr(l),
         "LangFunc(template_str='Hello', clean=True,"
         ' lm=ExcitedEchoer(sampling_options=LMSamplingOptions(temperature=0.0,'
-        ' max_tokens=1024, n=1, top_k=40, top_p=None, stop=None,'
+        ' max_tokens=None, n=1, top_k=40, top_p=None, stop=None,'
         ' random_seed=None, logprobs=False, top_logprobs=None), cache=None,'
         ' max_concurrency=None, timeout=120.0, max_attempts=5,'
         ' retry_interval=(5, 60), exponential_backoff=True, debug=False))',
     )
 
     l = LangFunc('Hello')
     with component.context(lm=ExcitedEchoer()):
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/language_model.py` & `langfun-0.0.2.dev20240410/langfun/core/language_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,22 @@
   temperature: Annotated[
       float,
       (
           'Model temperature, which is usually between 0 and 1.0. '
           'OpenAI models have temperature range from 0.0 to 2.0.'
       )
   ] = 0.0
-  max_tokens: Annotated[int, 'Per example max tokens to generate.'] = 1024
+  max_tokens: Annotated[
+      int | None,
+      (
+          'Per example max tokens to generate. '
+          'If None, use the model default.'
+      )
+  ] = None
+
   n: Annotated[int | None, 'Max number of samples to return.'] = 1
   top_k: Annotated[
       int | None,
       (
           'Top k tokens to sample the next token. '
           'Not applicable to OpenAI models.'
       )
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240410/langfun/core/language_model_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,21 +69,21 @@
 
 class LMSamplingOptionsTest(unittest.TestCase):
   """Tests for LMSamplingOptions."""
 
   def test_cache_key(self):
     options = lm_lib.LMSamplingOptions()
     key1 = options.cache_key()
-    self.assertEqual(key1, (0.0, 1024, 1, 40, None, None))
+    self.assertEqual(key1, (0.0, None, 1, 40, None, None))
     with options.override(temperature=1.0, max_tokens=256):
       key2 = options.cache_key()
       self.assertEqual(key2, (1.0, 256, 1, 40, None, None))
 
       # Make sure key1 does not change upon override.
-      self.assertEqual(key1, (0.0, 1024, 1, 40, None, None))
+      self.assertEqual(key1, (0.0, None, 1, 40, None, None))
 
 
 class LanguageModelTest(unittest.TestCase):
   """Tests for LanguageModel."""
 
   def test_init(self):
     lm = MockModel(1, temperature=0.5, top_k=2, max_attempts=2)
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/cache/in_memory_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,27 +40,27 @@
     self.assertEqual(lm('a', cache_seed=None), '5')
     self.assertEqual(lm('a', cache_seed=None), '6')
 
     self.assertEqual(cache.model_ids(), ['StaticSequence'])
     self.assertEqual(
         list(cache.keys()),
         [
-            ('a', (0.0, 1024, 1, 40, None, None), 0),
-            ('a', (0.0, 1024, 1, 40, None, None), 1),
-            ('b', (0.0, 1024, 1, 40, None, None), 0),
-            ('c', (0.0, 1024, 1, 40, None, None), 0),
+            ('a', (0.0, None, 1, 40, None, None), 0),
+            ('a', (0.0, None, 1, 40, None, None), 1),
+            ('b', (0.0, None, 1, 40, None, None), 0),
+            ('c', (0.0, None, 1, 40, None, None), 0),
         ],
     )
     self.assertEqual(
         list(cache.keys('StaticSequence')),
         [
-            ('a', (0.0, 1024, 1, 40, None, None), 0),
-            ('a', (0.0, 1024, 1, 40, None, None), 1),
-            ('b', (0.0, 1024, 1, 40, None, None), 0),
-            ('c', (0.0, 1024, 1, 40, None, None), 0),
+            ('a', (0.0, None, 1, 40, None, None), 0),
+            ('a', (0.0, None, 1, 40, None, None), 1),
+            ('b', (0.0, None, 1, 40, None, None), 0),
+            ('c', (0.0, None, 1, 40, None, None), 0),
         ],
     )
 
     def cache_entry(response_text, cache_seed=0):
       return base.LMCacheEntry(
           lf.LMSamplingResult([
               lf.LMSample(
@@ -86,48 +86,48 @@
             cache_entry('4'),
         ],
     )
     self.assertEqual(
         list(cache.items()),
         [
             (
-                ('a', (0.0, 1024, 1, 40, None, None), 0),
+                ('a', (0.0, None, 1, 40, None, None), 0),
                 cache_entry('1'),
             ),
             (
-                ('a', (0.0, 1024, 1, 40, None, None), 1),
+                ('a', (0.0, None, 1, 40, None, None), 1),
                 cache_entry('2', 1),
             ),
             (
-                ('b', (0.0, 1024, 1, 40, None, None), 0),
+                ('b', (0.0, None, 1, 40, None, None), 0),
                 cache_entry('3'),
             ),
             (
-                ('c', (0.0, 1024, 1, 40, None, None), 0),
+                ('c', (0.0, None, 1, 40, None, None), 0),
                 cache_entry('4'),
             ),
         ],
     )
     self.assertEqual(
         list(cache.items('StaticSequence')),
         [
             (
-                ('a', (0.0, 1024, 1, 40, None, None), 0),
+                ('a', (0.0, None, 1, 40, None, None), 0),
                 cache_entry('1'),
             ),
             (
-                ('a', (0.0, 1024, 1, 40, None, None), 1),
+                ('a', (0.0, None, 1, 40, None, None), 1),
                 cache_entry('2', 1),
             ),
             (
-                ('b', (0.0, 1024, 1, 40, None, None), 0),
+                ('b', (0.0, None, 1, 40, None, None), 0),
                 cache_entry('3'),
             ),
             (
-                ('c', (0.0, 1024, 1, 40, None, None), 0),
+                ('c', (0.0, None, 1, 40, None, None), 0),
                 cache_entry('4'),
             ),
         ],
     )
 
     # Test clone/copy semantics.
     self.assertIs(cache.clone()._stats, cache._stats)
@@ -157,16 +157,16 @@
     lm = fake.StaticSequence(['1', '2', '3'], cache=cache)
     self.assertEqual(lm('a'), '1')
     self.assertEqual(lm('a'), '1')
     self.assertEqual(lm('a', temperature=1.0), '2')
     self.assertEqual(
         list(cache.keys()),
         [
-            ('a', (0.0, 1024, 1, 40, None, None), 0),
-            ('a', (1.0, 1024, 1, 40, None, None), 0),
+            ('a', (0.0, None, 1, 40, None, None), 0),
+            ('a', (1.0, None, 1, 40, None, None), 0),
         ],
     )
 
   def test_different_model(self):
     cache = in_memory.InMemory()
     lm1 = fake.StaticSequence(['1', '2', '3'], cache=cache)
     lm2 = fake.Echo(cache=cache)
@@ -176,23 +176,23 @@
     self.assertEqual(lm1('a'), '1')
     self.assertEqual(lm1('b'), '2')
     self.assertEqual(lm2('b'), 'b')
 
     self.assertEqual(
         list(cache.keys('StaticSequence')),
         [
-            ('a', (0.0, 1024, 1, 40, None, None), 0),
-            ('b', (0.0, 1024, 1, 40, None, None), 0),
+            ('a', (0.0, None, 1, 40, None, None), 0),
+            ('b', (0.0, None, 1, 40, None, None), 0),
         ],
     )
     self.assertEqual(
         list(cache.keys('Echo')),
         [
-            ('a', (0.0, 1024, 1, 40, None, None), 0),
-            ('b', (0.0, 1024, 1, 40, None, None), 0),
+            ('a', (0.0, None, 1, 40, None, None), 0),
+            ('b', (0.0, None, 1, 40, None, None), 0),
         ],
     )
     self.assertEqual(len(cache), 4)
     cache.reset('Echo')
     self.assertEqual(list(cache.keys('Echo')), [])
     cache.reset()
     self.assertEqual(list(cache.keys()), [])
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/google_genai_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       orig_get_model = genai.get_model
       genai.get_model = mock_get_model
       mock_generate.side_effect = mock_generate_content
 
       lm = google_genai.GeminiPro(api_key='test_key')
       self.maxDiff = None
       self.assertEqual(
-          lm('hello', temperature=2.0, top_k=20).text,
+          lm('hello', temperature=2.0, top_k=20, max_tokens=1024).text,
           (
               'This is a response to hello with n=1, temperature=2.0, '
               'top_p=None, top_k=20, max_tokens=1024, stop=None.'
           ),
       )
       genai.get_model = orig_get_model
 
@@ -193,15 +193,15 @@
     lm = google_genai.Palm2(api_key='test_key')
     self.maxDiff = None
     self.assertEqual(
         lm('hello', temperature=2.0, top_k=20).text,
         (
             "hello to models/text-bison-001 with {'temperature': 2.0, "
             "'top_k': 20, 'top_p': None, 'candidate_count': 1, "
-            "'max_output_tokens': 1024, 'stop_sequences': None}"
+            "'max_output_tokens': None, 'stop_sequences': None}"
         ),
     )
     genai.get_model = orig_get_model
     genai.generate_text = orig_generate_text
 
   def test_call_with_legacy_chat_model(self):
     orig_get_model = genai.get_model
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,23 +160,24 @@
       self, options: lf.LMSamplingOptions) -> dict[str, Any]:
     # Reference:
     # https://platform.openai.com/docs/api-reference/completions/create
     # NOTE(daiyip): options.top_k is not applicable.
     args = dict(
         n=options.n,
         temperature=options.temperature,
-        max_tokens=options.max_tokens,
         stream=False,
         timeout=self.timeout,
         logprobs=options.logprobs,
         top_logprobs=options.top_logprobs,
     )
     # Completion and ChatCompletion uses different parameter name for model.
     args['model' if self.is_chat_model else 'engine'] = self.model
 
+    if options.max_tokens is not None:
+      args['max_tokens'] = options.max_tokens
     if options.top_p is not None:
       args['top_p'] = options.top_p
     if options.stop:
       args['stop'] = options.stop
     return args
 
   def _sample(self, prompts: list[lf.Message]) -> list[LMSamplingResult]:
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240410/langfun/core/llms/openai_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
         ),
         dict(
             model='gpt-4',
             logprobs=False,
             top_logprobs=None,
             n=1,
             temperature=1.0,
-            max_tokens=1024,
             stream=False,
             timeout=120.0,
             stop=['\n'],
         ),
     )
 
   def test_call_completion(self):
```

### Comparing `langfun-0.0.2.dev20240409/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240410/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240410/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/memory.py` & `langfun-0.0.2.dev20240410/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/message.py` & `langfun-0.0.2.dev20240410/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/message_test.py` & `langfun-0.0.2.dev20240410/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240410/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240410/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240410/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240410/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240410/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240410/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modality.py` & `langfun-0.0.2.dev20240410/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240410/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240410/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240410/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/sampling.py` & `langfun-0.0.2.dev20240410/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240410/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240410/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/subscription.py` & `langfun-0.0.2.dev20240410/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240410/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/template.py` & `langfun-0.0.2.dev20240410/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/template_test.py` & `langfun-0.0.2.dev20240410/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240410/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240410/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240410/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240410/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240409
+Version: 0.0.2.dev20240410
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240409/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240410/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240409/setup.py` & `langfun-0.0.2.dev20240410/setup.py`

 * *Files identical despite different names*

