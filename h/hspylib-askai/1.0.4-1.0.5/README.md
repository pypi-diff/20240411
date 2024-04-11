# Comparing `tmp/hspylib-askai-1.0.4.tar.gz` & `tmp/hspylib-askai-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-askai-1.0.4.tar", last modified: Sun Mar 31 01:05:29 2024, max compression
+gzip compressed data, was "hspylib-askai-1.0.5.tar", last modified: Thu Apr 11 00:23:25 2024, max compression
```

## Comparing `hspylib-askai-1.0.4.tar` & `hspylib-askai-1.0.5.tar`

### file list

```diff
@@ -1,82 +1,80 @@
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.364548 hspylib-askai-1.0.4/
--rw-r--r--   0 hugo       (503) staff       (20)       49 2024-02-16 01:49:09.000000 hspylib-askai-1.0.4/MANIFEST.in
--rw-r--r--   0 hugo       (503) staff       (20)     7938 2024-03-31 01:05:29.363706 hspylib-askai-1.0.4/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)     5933 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/README.md
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.319059 hspylib-askai-1.0.4/askai/
--rw-r--r--   0 hugo       (503) staff       (20)        6 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/.version
--rw-r--r--   0 hugo       (503) staff       (20)      800 2024-03-23 00:45:13.000000 hspylib-askai-1.0.4/askai/__classpath__.py
--rw-r--r--   0 hugo       (503) staff       (20)      180 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/__init__.py
--rwxr-xr-x   0 hugo       (503) staff       (20)     3831 2024-03-30 18:49:26.000000 hspylib-askai-1.0.4/askai/__main__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.323905 hspylib-askai-1.0.4/askai/core/
--rw-r--r--   0 hugo       (503) staff       (20)      319 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/core/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     9680 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/askai.py
--rw-r--r--   0 hugo       (503) staff       (20)     2254 2024-03-29 20:22:15.000000 hspylib-askai-1.0.4/askai/core/askai_configs.py
--rw-r--r--   0 hugo       (503) staff       (20)     1976 2024-03-30 18:49:26.000000 hspylib-askai-1.0.4/askai/core/askai_events.py
--rw-r--r--   0 hugo       (503) staff       (20)     4591 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/askai_messages.py
--rw-r--r--   0 hugo       (503) staff       (20)     1719 2024-03-30 18:49:26.000000 hspylib-askai-1.0.4/askai/core/askai_prompt.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.329168 hspylib-askai-1.0.4/askai/core/component/
--rw-r--r--   0 hugo       (503) staff       (20)      272 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/core/component/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3618 2024-03-23 00:45:13.000000 hspylib-askai-1.0.4/askai/core/component/audio_player.py
--rw-r--r--   0 hugo       (503) staff       (20)     3788 2024-03-23 00:45:13.000000 hspylib-askai-1.0.4/askai/core/component/cache_service.py
--rw-r--r--   0 hugo       (503) staff       (20)     3001 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/component/geo_location.py
--rw-r--r--   0 hugo       (503) staff       (20)     6110 2024-03-30 21:57:34.000000 hspylib-askai-1.0.4/askai/core/component/internet_service.py
--rw-r--r--   0 hugo       (503) staff       (20)     7901 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/component/recorder.py
--rw-r--r--   0 hugo       (503) staff       (20)     5736 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/component/summarizer.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.331450 hspylib-askai-1.0.4/askai/core/engine/
--rw-r--r--   0 hugo       (503) staff       (20)      200 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/core/engine/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2441 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/engine/ai_engine.py
--rw-r--r--   0 hugo       (503) staff       (20)     1613 2024-03-14 00:29:25.000000 hspylib-askai-1.0.4/askai/core/engine/engine_factory.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.334971 hspylib-askai-1.0.4/askai/core/engine/openai/
--rw-r--r--   0 hugo       (503) staff       (20)      238 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/core/engine/openai/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     2316 2024-03-14 00:29:25.000000 hspylib-askai-1.0.4/askai/core/engine/openai/openai_configs.py
--rw-r--r--   0 hugo       (503) staff       (20)     5755 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/engine/openai/openai_engine.py
--rw-r--r--   0 hugo       (503) staff       (20)     2553 2024-03-30 18:49:26.000000 hspylib-askai-1.0.4/askai/core/engine/openai/openai_model.py
--rw-r--r--   0 hugo       (503) staff       (20)     2266 2024-03-15 02:46:13.000000 hspylib-askai-1.0.4/askai/core/engine/openai/temperatures.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.341814 hspylib-askai-1.0.4/askai/core/model/
--rw-r--r--   0 hugo       (503) staff       (20)      314 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/core/model/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)      669 2024-03-03 20:58:12.000000 hspylib-askai-1.0.4/askai/core/model/ai_model.py
--rw-r--r--   0 hugo       (503) staff       (20)      648 2024-03-26 00:19:30.000000 hspylib-askai-1.0.4/askai/core/model/ai_reply.py
--rw-r--r--   0 hugo       (503) staff       (20)     3608 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/model/chat_context.py
--rw-r--r--   0 hugo       (503) staff       (20)      936 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/model/processor_response.py
--rw-r--r--   0 hugo       (503) staff       (20)      479 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/model/query_type.py
--rw-r--r--   0 hugo       (503) staff       (20)      854 2024-03-30 18:49:26.000000 hspylib-askai-1.0.4/askai/core/model/search_result.py
--rw-r--r--   0 hugo       (503) staff       (20)      740 2024-03-23 00:45:13.000000 hspylib-askai-1.0.4/askai/core/model/summary_result.py
--rw-r--r--   0 hugo       (503) staff       (20)     1383 2024-03-23 00:45:13.000000 hspylib-askai-1.0.4/askai/core/model/terminal_command.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.344399 hspylib-askai-1.0.4/askai/core/processor/
--rw-r--r--   0 hugo       (503) staff       (20)      238 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/core/processor/__init__.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.349397 hspylib-askai-1.0.4/askai/core/processor/instances/
--rw-r--r--   0 hugo       (503) staff       (20)      314 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/core/processor/instances/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3867 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/processor/instances/analysis_processor.py
--rw-r--r--   0 hugo       (503) staff       (20)     6457 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/processor/instances/command_processor.py
--rw-r--r--   0 hugo       (503) staff       (20)     4155 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/processor/instances/generic_processor.py
--rw-r--r--   0 hugo       (503) staff       (20)     4008 2024-03-30 22:24:50.000000 hspylib-askai-1.0.4/askai/core/processor/instances/internet_processor.py
--rw-r--r--   0 hugo       (503) staff       (20)     3173 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/processor/instances/output_processor.py
--rw-r--r--   0 hugo       (503) staff       (20)     5299 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/processor/instances/summary_processor.py
--rw-r--r--   0 hugo       (503) staff       (20)     1481 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/processor/processor_base.py
--rw-r--r--   0 hugo       (503) staff       (20)     2698 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/processor/processor_factory.py
--rw-r--r--   0 hugo       (503) staff       (20)     2746 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/processor/processor_proxy.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.355073 hspylib-askai-1.0.4/askai/core/support/
--rw-r--r--   0 hugo       (503) staff       (20)      292 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/core/support/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1755 2024-03-23 00:45:13.000000 hspylib-askai-1.0.4/askai/core/support/langchain_support.py
--rw-r--r--   0 hugo       (503) staff       (20)     4407 2024-03-23 00:45:13.000000 hspylib-askai-1.0.4/askai/core/support/object_mapper.py
--rw-r--r--   0 hugo       (503) staff       (20)     4945 2024-03-03 20:58:12.000000 hspylib-askai-1.0.4/askai/core/support/presets.py
--rw-r--r--   0 hugo       (503) staff       (20)     1679 2024-03-14 00:29:25.000000 hspylib-askai-1.0.4/askai/core/support/settings.py
--rw-r--r--   0 hugo       (503) staff       (20)     2954 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/core/support/shared_instances.py
--rw-r--r--   0 hugo       (503) staff       (20)     2655 2024-03-30 22:32:50.000000 hspylib-askai-1.0.4/askai/core/support/text_formatter.py
--rw-r--r--   0 hugo       (503) staff       (20)     6936 2024-03-30 22:09:49.000000 hspylib-askai-1.0.4/askai/core/support/utilities.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.356127 hspylib-askai-1.0.4/askai/exception/
--rw-r--r--   0 hugo       (503) staff       (20)      161 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/exception/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     1602 2024-03-14 05:01:33.000000 hspylib-askai-1.0.4/askai/exception/exceptions.py
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.358042 hspylib-askai-1.0.4/askai/language/
--rw-r--r--   0 hugo       (503) staff       (20)      183 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/askai/language/__init__.py
--rw-r--r--   0 hugo       (503) staff       (20)     3338 2024-03-30 18:49:29.000000 hspylib-askai-1.0.4/askai/language/argos_translator.py
--rw-r--r--   0 hugo       (503) staff       (20)     8910 2024-03-30 18:49:26.000000 hspylib-askai-1.0.4/askai/language/language.py
--rw-r--r--   0 hugo       (503) staff       (20)      240 2024-03-03 20:58:12.000000 hspylib-askai-1.0.4/askai/welcome.txt
-drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-03-31 01:05:29.362265 hspylib-askai-1.0.4/hspylib_askai.egg-info/
--rw-r--r--   0 hugo       (503) staff       (20)     7938 2024-03-31 01:05:29.000000 hspylib-askai-1.0.4/hspylib_askai.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (503) staff       (20)     2244 2024-03-31 01:05:29.000000 hspylib-askai-1.0.4/hspylib_askai.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (503) staff       (20)        1 2024-03-31 01:05:29.000000 hspylib-askai-1.0.4/hspylib_askai.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (503) staff       (20)      614 2024-03-31 01:05:29.000000 hspylib-askai-1.0.4/hspylib_askai.egg-info/requires.txt
--rw-r--r--   0 hugo       (503) staff       (20)       11 2024-03-31 01:05:29.000000 hspylib-askai-1.0.4/hspylib_askai.egg-info/top_level.txt
--rw-r--r--   0 hugo       (503) staff       (20)       38 2024-03-31 01:05:29.364678 hspylib-askai-1.0.4/setup.cfg
--rw-r--r--   0 hugo       (503) staff       (20)     1991 2024-03-31 01:05:26.000000 hspylib-askai-1.0.4/setup.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.749843 hspylib-askai-1.0.5/
+-rw-r--r--   0 hjunior    (501) staff       (20)       49 2024-02-15 22:15:40.000000 hspylib-askai-1.0.5/MANIFEST.in
+-rw-r--r--   0 hjunior    (501) staff       (20)     7970 2024-04-11 00:23:25.747825 hspylib-askai-1.0.5/PKG-INFO
+-rw-r--r--   0 hjunior    (501) staff       (20)     5933 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/README.md
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.648781 hspylib-askai-1.0.5/askai/
+-rw-r--r--   0 hjunior    (501) staff       (20)        6 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/.version
+-rw-r--r--   0 hjunior    (501) staff       (20)      800 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/__classpath__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)      180 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/__init__.py
+-rwxr-xr-x   0 hjunior    (501) staff       (20)     4838 2024-04-09 23:04:09.000000 hspylib-askai-1.0.5/askai/__main__.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.660801 hspylib-askai-1.0.5/askai/core/
+-rw-r--r--   0 hjunior    (501) staff       (20)      318 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)    10474 2024-04-10 23:50:17.000000 hspylib-askai-1.0.5/askai/core/askai.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2787 2024-04-08 23:25:38.000000 hspylib-askai-1.0.5/askai/core/askai_configs.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1996 2024-04-04 15:23:06.000000 hspylib-askai-1.0.5/askai/core/askai_events.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     5057 2024-04-09 18:31:51.000000 hspylib-askai-1.0.5/askai/core/askai_messages.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1757 2024-04-10 00:17:24.000000 hspylib-askai-1.0.5/askai/core/askai_prompt.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.669932 hspylib-askai-1.0.5/askai/core/component/
+-rw-r--r--   0 hjunior    (501) staff       (20)      272 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/component/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3617 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/component/audio_player.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3788 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/component/cache_service.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3001 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/component/geo_location.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     6231 2024-04-08 16:43:58.000000 hspylib-askai-1.0.5/askai/core/component/internet_service.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     7876 2024-04-10 22:09:33.000000 hspylib-askai-1.0.5/askai/core/component/recorder.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     5736 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/component/summarizer.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.673660 hspylib-askai-1.0.5/askai/core/engine/
+-rw-r--r--   0 hjunior    (501) staff       (20)      200 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/engine/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2441 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/engine/ai_engine.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1613 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/engine/engine_factory.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.682593 hspylib-askai-1.0.5/askai/core/engine/openai/
+-rw-r--r--   0 hjunior    (501) staff       (20)      237 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/engine/openai/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2316 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/engine/openai/openai_configs.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     5755 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/engine/openai/openai_engine.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2553 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/engine/openai/openai_model.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2413 2024-04-09 18:52:10.000000 hspylib-askai-1.0.5/askai/core/engine/openai/temperature.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.687202 hspylib-askai-1.0.5/askai/core/features/
+-rw-r--r--   0 hjunior    (501) staff       (20)      191 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/features/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     6854 2024-04-09 19:09:30.000000 hspylib-askai-1.0.5/askai/core/features/actions.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     5214 2024-04-09 19:26:07.000000 hspylib-askai-1.0.5/askai/core/features/router.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.698101 hspylib-askai-1.0.5/askai/core/features/tools/
+-rw-r--r--   0 hjunior    (501) staff       (20)      240 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/features/tools/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2209 2024-04-09 15:46:53.000000 hspylib-askai-1.0.5/askai/core/features/tools/analysis.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2198 2024-04-09 00:47:29.000000 hspylib-askai-1.0.5/askai/core/features/tools/browser.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2076 2024-04-09 23:15:03.000000 hspylib-askai-1.0.5/askai/core/features/tools/general.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2024 2024-04-08 16:43:58.000000 hspylib-askai-1.0.5/askai/core/features/tools/summarization.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     4169 2024-04-09 19:37:59.000000 hspylib-askai-1.0.5/askai/core/features/tools/terminal.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.712287 hspylib-askai-1.0.5/askai/core/model/
+-rw-r--r--   0 hjunior    (501) staff       (20)      308 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/model/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)      669 2024-03-03 22:13:26.000000 hspylib-askai-1.0.5/askai/core/model/ai_model.py
+-rw-r--r--   0 hjunior    (501) staff       (20)      648 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/model/ai_reply.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     4173 2024-04-09 00:40:44.000000 hspylib-askai-1.0.5/askai/core/model/chat_context.py
+-rw-r--r--   0 hjunior    (501) staff       (20)      479 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/model/query_type.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1020 2024-04-08 16:43:58.000000 hspylib-askai-1.0.5/askai/core/model/rag_response.py
+-rw-r--r--   0 hjunior    (501) staff       (20)      854 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/model/search_result.py
+-rw-r--r--   0 hjunior    (501) staff       (20)      740 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/model/summary_result.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1383 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/model/terminal_command.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.723591 hspylib-askai-1.0.5/askai/core/support/
+-rw-r--r--   0 hjunior    (501) staff       (20)      292 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/support/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1755 2024-03-25 16:24:18.000000 hspylib-askai-1.0.5/askai/core/support/langchain_support.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     4407 2024-03-25 16:24:18.000000 hspylib-askai-1.0.5/askai/core/support/object_mapper.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     4943 2024-04-10 15:24:30.000000 hspylib-askai-1.0.5/askai/core/support/presets.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     1679 2024-03-25 16:24:18.000000 hspylib-askai-1.0.5/askai/core/support/settings.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3423 2024-04-10 23:54:31.000000 hspylib-askai-1.0.5/askai/core/support/shared_instances.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2992 2024-04-09 15:57:17.000000 hspylib-askai-1.0.5/askai/core/support/text_formatter.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     7453 2024-04-09 18:08:30.000000 hspylib-askai-1.0.5/askai/core/support/utilities.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.728358 hspylib-askai-1.0.5/askai/exception/
+-rw-r--r--   0 hjunior    (501) staff       (20)      161 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/exception/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     2159 2024-04-05 23:07:33.000000 hspylib-askai-1.0.5/askai/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.735265 hspylib-askai-1.0.5/askai/language/
+-rw-r--r--   0 hjunior    (501) staff       (20)      183 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/language/__init__.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     3338 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/language/argos_translator.py
+-rw-r--r--   0 hjunior    (501) staff       (20)     8910 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/language/language.py
+-rw-r--r--   0 hjunior    (501) staff       (20)      240 2024-03-03 22:13:26.000000 hspylib-askai-1.0.5/askai/welcome.txt
+drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.745001 hspylib-askai-1.0.5/hspylib_askai.egg-info/
+-rw-r--r--   0 hjunior    (501) staff       (20)     7970 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (501) staff       (20)     2051 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (501) staff       (20)        1 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (501) staff       (20)      631 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (501) staff       (20)       11 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (501) staff       (20)       38 2024-04-11 00:23:25.750298 hspylib-askai-1.0.5/setup.cfg
+-rw-r--r--   0 hjunior    (501) staff       (20)     1991 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/setup.py
```

### Comparing `hspylib-askai-1.0.4/PKG-INFO` & `hspylib-askai-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-askai
-Version: 1.0.4
+Version: 1.0.5
 Summary: HomeSetup - AskAI
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-askai/
@@ -20,21 +20,21 @@
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Terminals
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: hspylib>=1.12.35
-Requires-Dist: hspylib-clitt>=0.9.117
-Requires-Dist: retry==0.9.2
+Requires-Dist: hspylib-clitt>=0.9.119
+Requires-Dist: retry2==0.9.5
 Requires-Dist: pause==0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: argostranslate==1.9.1
 Requires-Dist: protobuf==4.22.1
-Requires-Dist: torch==2.1.2
+Requires-Dist: torch==2.2.0
 Requires-Dist: stanza==1.1.1
 Requires-Dist: soundfile==0.12.1
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: langchain>=0.1.12
 Requires-Dist: langchain-openai==0.0.8
 Requires-Dist: langchain-community==0.0.28
 Requires-Dist: unstructured==0.12.4
@@ -50,24 +50,25 @@
 Requires-Dist: openai==1.14.1
 Requires-Dist: chromadb==0.4.24
 Requires-Dist: opentelemetry-api==1.22.0
 Requires-Dist: opentelemetry-sdk==1.22.0
 Requires-Dist: opentelemetry-proto==1.22.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: pytz==2024.1
+Requires-Dist: schedule==1.2.1
 
 <img src="https://iili.io/JEatihb.png" width="64" height="64" align="right" />
 
 # AskAI
 >
 > Unleash the Power of AI in Your Terminal
 
 [![Terminal](https://badgen.net/badge/icon/terminal?icon=terminal&label)](https://github.com/yorevs/homesetup)
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v1.0.4/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v1.0.5/gray)](docs/CHANGELOG.md#unreleased)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 [![build-and-test](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml)
 
 <img src="https://iili.io/JGv7BTP.png)" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
```

### Comparing `hspylib-askai-1.0.4/README.md` & `hspylib-askai-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # AskAI
 >
 > Unleash the Power of AI in Your Terminal
 
 [![Terminal](https://badgen.net/badge/icon/terminal?icon=terminal&label)](https://github.com/yorevs/homesetup)
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v1.0.4/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v1.0.5/gray)](docs/CHANGELOG.md#unreleased)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 [![build-and-test](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml)
 
 <img src="https://iili.io/JGv7BTP.png)" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
```

### Comparing `hspylib-askai-1.0.4/askai/__classpath__.py` & `hspylib-askai-1.0.5/askai/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/__main__.py` & `hspylib-askai-1.0.5/askai/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,27 +9,35 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
 
-from askai.__classpath__ import classpath
-from askai.core.askai import AskAi
+import logging as log
+import sys
+from typing import Any, Optional
+
+from clitt.core.term.commons import is_a_tty
+
+if not is_a_tty():
+    log.getLogger().setLevel(log.ERROR)
+
+from textwrap import dedent
+
 from clitt.core.tui.tui_application import TUIApplication
 from hspylib.core.enums.charset import Charset
 from hspylib.core.tools.dict_tools import get_or_default
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.application.argparse.parser_action import ParserAction
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
-from textwrap import dedent
 
-import logging as log
-import sys
+from askai.__classpath__ import classpath
+from askai.core.askai import AskAi
 
 
 class Main(TUIApplication):
     """HomeSetup Ask-AI - Unleash the Power of AI in Your Terminal."""
 
     # The welcome message
     DESCRIPTION = classpath.get_source("welcome.txt").read_text(encoding=Charset.UTF_8.val)
@@ -45,45 +53,55 @@
         self._askai = None
 
     def _setup_arguments(self) -> None:
         """Initialize application parameters and options."""
         # fmt: off
         self._with_options() \
             .option(
-                "engine", "e", "engine",
-                "specifies which AI engine to use. If not provided, the default engine wil be used.",
-                choices=['openai', 'palm'],
-                nargs=1, default='openai')\
-            .option(
-                "model", "m", "model",
-                "specifies which AI model to use (depends on the engine).",
-                nargs=1, default='gpt-3.5-turbo')\
-            .option(
                 "interactive", "i", "interactive",
                 "whether you would like to run the program in an interactive mode.",
                 nargs="?", action=ParserAction.STORE_TRUE, default=False)\
             .option(
                 "quiet", "q", "quiet",
                 "whether you want touse speaking (audio in/out).",
-                nargs="?", action=ParserAction.STORE_FALSE, default=True)\
+                nargs="?", action=ParserAction.STORE_TRUE, default=False)\
+            .option(
+                "debug", "d", "debug",
+                "whether you want enter debug mode.",
+                nargs="?", action=ParserAction.STORE_TRUE, default=False)\
             .option(
                 "tempo", "t", "tempo",
                 "specifies the playback and streaming speed.",
                 choices=['1', '2', '3'],
-                nargs=1, default='1')
+                nargs=1, default='1')\
+            .option(
+                "prompt", "p", "prompt",
+                "specifies the query prompt file (not useful with interactive mode).",
+                nargs=1, default='qstring-prompt')\
+            .option(
+                "engine", "e", "engine",
+                "specifies which AI engine to use. If not provided, the default engine wil be used.",
+                choices=['openai', 'palm'],
+                nargs=1, default='openai')\
+            .option(
+                "model", "m", "model",
+                "specifies which AI model to use (depends on the engine).",
+                nargs=1, default='gpt-3.5-turbo')
         self._with_arguments() \
             .argument("query_string", "what to ask to the AI engine", nargs="*")
         # fmt: on
 
     def _main(self, *params, **kwargs) -> ExitStatus:
         """Run the application with the command line arguments."""
         self._askai = AskAi(
             self.get_arg("interactive"),
             self.get_arg("quiet"),
-            int(get_or_default(self.get_arg("tempo") or [], 0, "1")),
+            self.get_arg("debug"),
+            int(self._get_argument("tempo")),
+            str(self._get_argument("prompt")),
             self.get_arg("engine"),
             self.get_arg("model"),
             self.get_arg("query_string"),
         )
 
         log.info(
             dedent(
@@ -100,11 +118,23 @@
 
     def _exec_application(self) -> ExitStatus:
         """Execute the application main flow."""
         self._askai.run()
 
         return ExitStatus.SUCCESS
 
+    def _get_argument(self, arg_name: str) -> Optional[Any]:
+        """TODO"""
+        if arg := self.get_arg(arg_name):
+            if isinstance(arg, str):
+                return arg
+            elif isinstance(arg, list):
+                return get_or_default(arg, 0, '')
+            else:
+                raise TypeError("Argument '' has an invalid type: ''", arg, type(arg))
+        else:
+            return ''
+
 
 # Application entry point
 if __name__ == "__main__":
     Main("AskAI").INSTANCE.run(sys.argv[1:])
```

### Comparing `hspylib-askai-1.0.4/askai/core/askai.py` & `hspylib-askai-1.0.5/askai/core/askai.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,79 +8,96 @@
    @created: Fri, 5 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
+import logging as log
+import os
+import sys
+from functools import partial
+from threading import Thread
+from typing import List, Optional
+
+import nltk
+import pause
+from clitt.core.term.cursor import cursor
+from clitt.core.term.screen import screen
+from clitt.core.term.terminal import terminal
+from hspylib.core.enums.charset import Charset
+from hspylib.core.tools.commons import sysout, is_debugging
+from hspylib.modules.application.exit_status import ExitStatus
+from hspylib.modules.eventbus.event import Event
+from langchain_core.prompts import PromptTemplate
+
 from askai.__classpath__ import classpath
 from askai.core.askai_configs import configs
 from askai.core.askai_events import ASKAI_BUS_NAME, AskAiEvents, REPLY_ERROR_EVENT, REPLY_EVENT
 from askai.core.askai_messages import msg
+from askai.core.askai_prompt import prompt
 from askai.core.component.audio_player import player
 from askai.core.component.cache_service import cache, CACHE_DIR
 from askai.core.component.recorder import recorder
 from askai.core.engine.ai_engine import AIEngine
+from askai.core.engine.openai.temperature import Temperature
+from askai.core.features.router import router
 from askai.core.model.chat_context import ChatContext
-from askai.core.model.processor_response import ProcessorResponse
-from askai.core.processor.processor_factory import ProcessorFactory
-from askai.core.processor.processor_proxy import proxy
-from askai.core.support.object_mapper import object_mapper
+from askai.core.support.langchain_support import lc_llm
 from askai.core.support.shared_instances import shared
-from askai.core.support.utilities import display_text
-from clitt.core.term.cursor import cursor
-from clitt.core.term.screen import screen
-from clitt.core.term.terminal import terminal
-from functools import partial
-from hspylib.core.enums.charset import Charset
-from hspylib.core.tools.commons import sysout
-from hspylib.modules.application.exit_status import ExitStatus
-from hspylib.modules.eventbus.event import Event
-from threading import Thread
-from typing import List, Optional
-
-import logging as log
-import nltk
-import os
-import pause
-import sys
+from askai.core.support.utilities import display_text, read_stdin
+from askai.exception.exceptions import ImpossibleQuery, UnintelligibleQuery, TerminatingQuery, MaxInteractionsReached, \
+    InaccurateResponse
 
 
 class AskAi:
     """Responsible for the OpenAI functionalities."""
 
     SPLASH = classpath.get_resource("splash.txt").read_text(encoding=Charset.UTF_8.val)
 
     @staticmethod
     def _abort():
         """Abort the execution and exit."""
         sys.exit(ExitStatus.FAILED.val)
 
     def __init__(
-        self, interactive: bool, is_speak: bool, tempo: int, engine_name: str, model_name: str, query: str | List[str]
+        self, interactive: bool,
+        quiet: bool,
+        debug: bool,
+        tempo: int,
+        query_prompt: str,
+        engine_name: str,
+        model_name: str,
+        query: str | List[str]
     ):
         self._interactive: bool = interactive
         self._ready: bool = False
         self._processing: Optional[bool] = None
-        self._query_string: Optional[str] = str(" ".join(query) if isinstance(query, list) else query)
+        self._query_string: str | None = None
+        self._question: str | None = None
+        self._query_prompt: str | None = query_prompt
         self._engine: AIEngine = shared.create_engine(engine_name, model_name)
         self._context: ChatContext = shared.create_context(self._engine.ai_token_limit())
         # Setting configs from program args.
-        configs.is_speak = is_speak
+        self._get_query_string(interactive, query)
+        configs.is_speak = not quiet
+        configs.is_debug = is_debugging() or debug
         configs.tempo = tempo
+        configs.is_interactive = interactive
 
     def __str__(self) -> str:
         device_info = f"{recorder.input_device[1].title()}" if recorder.input_device else ""
         return (
             f"%GREEN%"
             f"{'-=' * 40} %EOL%"
             f"     Engine: {self.engine} %EOL%"
             f"   Language: {configs.language} %EOL%"
             f"{'-+' * 40} %EOL%"
             f" Microphone: {device_info or '%RED%Undetected'} %GREEN%%EOL%"
+            f"  Debugging: {'ON' if self.is_debugging else '%RED%OFF'} %GREEN%%EOL%"
             f"   Speaking: {'ON, tempo: ' + str(configs.tempo) if self.is_speak else '%RED%OFF'} %GREEN%%EOL%"
             f"    Caching: {'ON, TTL: ' + configs.ttl if cache.is_cache_enabled() else '%RED%OFF'} %GREEN%%EOL%"
             f"{'-=' * 40} %EOL%%NC%"
         )
 
     @property
     def engine(self) -> AIEngine:
@@ -95,14 +112,26 @@
         return configs.is_cache
 
     @property
     def query_string(self) -> str:
         return self._query_string
 
     @property
+    def question(self) -> str:
+        return self._question
+
+    @property
+    def is_interactive(self) -> bool:
+        return self._interactive
+
+    @property
+    def is_debugging(self) -> bool:
+        return configs.is_debug
+
+    @property
     def is_speak(self) -> bool:
         return configs.is_speak
 
     @property
     def is_processing(self) -> bool:
         return self._processing
 
@@ -112,20 +141,25 @@
             self.reply(msg.wait())
         elif not processing and self._processing is not None and processing != self._processing:
             terminal.cursor.erase_line()
         self._processing = processing
 
     def run(self) -> None:
         """Run the program."""
-        if self._interactive:
-            self._startup()
+        self._startup()
+        if self.is_interactive:
             self._prompt()
         elif self.query_string:
-            display_text(self.query_string, f"{shared.nickname}: ")
-            self._ask_and_reply(self.query_string)
+            llm = lc_llm.create_chat_model(Temperature.CREATIVE_WRITING.temp)
+            display_text(self.question, f"{shared.username}: ")
+            if output := llm.invoke(self.query_string):
+                self.reply(output.content)
+                cache.save_query_history()
+        else:
+            display_text(f"%RED%Error: {msg.no_query_string()}%NC%")
 
     def reply(self, message: str) -> None:
         """Reply to the user with the AI response.
         :param message: The message to reply to the user.
         """
         if self.is_speak:
             self.engine.text_to_speech(message, f"{shared.nickname}: ")
@@ -134,116 +168,111 @@
 
     def reply_error(self, message: str) -> None:
         """Reply API or system errors.
         :param message: The error message to be displayed.
         """
         log.error(message)
         if self.is_speak:
-            self.engine.text_to_speech(message, f"{shared.nickname}: ")
+            self.engine.text_to_speech(f"Error: {message}", f"{shared.nickname}: ")
         else:
-            display_text(message, f"{shared.nickname}: ")
+            display_text(f"Error: {message}", f"{shared.nickname}: ")
 
     def _cb_reply_event(self, ev: Event, error: bool = False) -> None:
-        """Callback to handle reply events."""
+        """Callback to handle reply events.
+        :param ev: The reply event.
+        :param error: Whether the event is an error not not.
+        """
         if error:
             self.reply_error(ev.args.message)
         else:
-            if ev.args.erase_last:
-                cursor.erase_line()
-            self.reply(ev.args.message)
+            verbose = ev.args.verbosity.lower()
+            if verbose == 'normal' or self.is_debugging:
+                if ev.args.erase_last:
+                    cursor.erase_line()
+                self.reply(ev.args.message)
 
     def _splash(self) -> None:
         """Display the AskAI splash screen."""
         splash_interval = 1000
         while not self._ready:
             if not self._processing:
                 screen.clear()
                 sysout(f"%GREEN%{self.SPLASH}%NC%")
             pause.milliseconds(splash_interval)
-        pause.milliseconds(splash_interval * 2)
+        pause.milliseconds(splash_interval)
         screen.clear()
 
     def _startup(self) -> None:
         """Initialize the application."""
-        splash_thread: Thread = Thread(daemon=True, target=self._splash)
-        splash_thread.start()
-        recorder.setup()
-        nltk.download("averaged_perceptron_tagger", quiet=True, download_dir=CACHE_DIR)
-        cache.set_cache_enable(self.cache_enabled)
-        cache.read_query_history()
         askai_bus = AskAiEvents.get_bus(ASKAI_BUS_NAME)
         askai_bus.subscribe(REPLY_EVENT, self._cb_reply_event)
         askai_bus.subscribe(REPLY_ERROR_EVENT, partial(self._cb_reply_event, error=True))
-        if configs.is_speak:
+        if self.is_interactive:
+            splash_thread: Thread = Thread(daemon=True, target=self._splash)
+            splash_thread.start()
+            recorder.setup()
+            nltk.download("averaged_perceptron_tagger", quiet=True, download_dir=CACHE_DIR)
+            cache.set_cache_enable(self.cache_enabled)
+            cache.read_query_history()
+            player.start_delay()
+            self._ready = True
+            splash_thread.join()
+            display_text(self, markdown=False)
+            self.reply(msg.welcome(os.getenv("USER", "you")))
+        else:
+            recorder.setup()
             player.start_delay()
-        self._ready = True
-        splash_thread.join()
-        display_text(self, markdown=False)
         log.info("AskAI is ready to use!")
-        self.reply(msg.welcome(os.getenv("USER", "you")))
 
     def _prompt(self) -> None:
         """Prompt for user interaction."""
         while query := shared.input_text(f"{shared.username}: "):
-
             if not self._ask_and_reply(query):
                 query = None
                 break
+            else:
+                cache.save_query_history()
         if not query:
             self.reply(msg.goodbye())
-        sysout("", end="")
+        sysout("")
 
     def _ask_and_reply(self, question: str) -> bool:
         """Ask the question and provide the reply.
         :param question: The question to ask to the AI engine.
         """
-        if not (reply := cache.read_reply(question)):
-            log.debug('Response not found for "%s" in cache. Querying from %s.', question, self.engine.nickname())
-            status, response = proxy.process(question)
-            if status and response:
-                return self._process_response(response)
-            self.reply_error(response)
-        else:
-            log.debug("Reply found for '%s' in cache.", question)
-            self.reply(reply)
-            status = True
-        return status
-
-    def _process_response(self, proxy_response: ProcessorResponse) -> bool:
-        """Process a query response using a processor that supports the query type.
-        :param proxy_response: The processor proxy response.
-        """
-        status, output, query_type, processor = False, None, None, None
-        # Intrinsic features
-        if not proxy_response.intelligible:
-            self.reply_error(msg.intelligible(proxy_response.question))
-            return True
-        elif proxy_response.terminating:
-            log.info("User wants to terminate the conversation.")
-            return False
-        elif proxy_response.require_summarization:
-            log.info("Summarization is required to fulfill the request.")
-            processor = ProcessorFactory.summary()
-            processor.bind(ProcessorFactory.generic())
-        # Query processors
-        if processor or (query_type := proxy_response.query_type or "AnalysisQuery"):
-            if not processor and not (processor := ProcessorFactory.find_processor(query_type)):
-                log.error(f"Unable to find a proper processor: {str(proxy_response)}")
-                self.reply_error(msg.no_processor(query_type))
-                return False
-            log.info("%s::Processing response for '%s'", processor.name(), proxy_response.question)
-            status, output = processor.process(proxy_response)
-            if status and output and processor.next_in_chain():
-                mapped_response = object_mapper.of_json(output, ProcessorResponse)
-                if isinstance(mapped_response, ProcessorResponse):
-                    self._process_response(mapped_response)
-                else:
-                    self.reply(str(mapped_response))
-            elif status:
-                if output:
+        status = True
+        try:
+            if not (reply := cache.read_reply(question)):
+                log.debug('Response not found for "%s" in cache. Querying from %s.', question, self.engine.nickname())
+                AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.wait())
+                if output := router.process(question):
                     self.reply(output)
             else:
-                self.reply_error(output)
-        else:
-            self.reply_error(msg.invalid_response(str(proxy_response)))
+                log.debug("Reply found for '%s' in cache.", question)
+                self.reply(reply)
+        except (NotImplementedError, ImpossibleQuery, UnintelligibleQuery) as err:
+            self.reply_error(str(err))
+        except (MaxInteractionsReached, InaccurateResponse) as err:
+            self.reply_error(msg.unprocessable(str(err)))
+        except TerminatingQuery:
+            status = False
 
         return status
+
+    def _get_query_string(self, interactive: bool, query_arg: str | list[str]) -> None:
+        """Retrieve the proper query string used in the non interactive mode.
+        :param interactive: The interactive mode.
+        :param query_arg: The query argument provided by the command line.
+        """
+        query: str = str(" ".join(query_arg) if isinstance(query_arg, list) else query_arg)
+        self._question = query
+        dir_name, file_name = os.path.split(self._query_prompt)
+        if not interactive:
+            stdin_args = read_stdin()
+            template = PromptTemplate(
+                input_variables=['context', 'question'],
+                template=prompt.read_prompt(file_name, dir_name.replace('~', os.getenv('HOME'))))
+            final_prompt = template.format(context=stdin_args, question=self._question)
+            self._query_string = final_prompt if query else stdin_args
+            self._question = self._question or self._query_string
+        else:
+            self._query_string = query
```

### Comparing `hspylib-askai-1.0.4/askai/core/askai_configs.py` & `hspylib-askai-1.0.5/askai/core/askai_configs.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,38 +8,41 @@
    @created: Fri, 5 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-from askai.__classpath__ import _Classpath
-from askai.language.language import Language
+import os
+from shutil import which
+
 from hspylib.core.config.app_config import AppConfigs
 from hspylib.core.enums.charset import Charset
 from hspylib.core.metaclass.singleton import Singleton
-from shutil import which
 
-import os
+from askai.__classpath__ import classpath
+from askai.language.language import Language
 
 
 class AskAiConfigs(metaclass=Singleton):
     """Provides access to AskAI configurations."""
 
     INSTANCE: "AskAiConfigs" = None
 
     # The resources folder
-    RESOURCE_DIR = str(_Classpath.resource_path())
+    RESOURCE_DIR = str(classpath.resource_path())
 
     def __init__(self):
         self._configs = AppConfigs.INSTANCE or AppConfigs(self.RESOURCE_DIR)
+        self._is_interactive = self._configs.get_bool("askai.interactive.enabled")
+        self._is_speak = self._configs.get_bool("askai.speak.enabled")
+        self._is_debug = self._configs.get_bool("askai.debug.enabled")
         self._is_cache = self._configs.get_bool("askai.cache.enabled")
         self._ttl = self._configs.get_int("askai.cache.ttl.minutes")
         self._tempo = self._configs.get_int("askai.speech.tempo")
-        self._is_speak = self._configs.get_bool("askai.speak.response")
         self._language = Language.of_locale(
             os.getenv("LC_ALL", os.getenv("LC_TYPE", os.getenv("LANG", os.getenv("LANGUAGE", "en_US.UTF-8"))))
         )
 
     @property
     def is_cache(self) -> bool:
         return self._is_cache
@@ -61,20 +64,36 @@
         return which("ffplay") and self._is_speak
 
     @is_speak.setter
     def is_speak(self, value: bool) -> None:
         self._is_speak = which("ffplay") and value
 
     @property
+    def is_debug(self) -> bool:
+        return self._is_debug
+
+    @is_debug.setter
+    def is_debug(self, value: bool) -> None:
+        self._is_debug = value
+
+    @property
+    def is_interactive(self) -> bool:
+        return self._is_interactive
+
+    @is_interactive.setter
+    def is_interactive(self, value: bool) -> None:
+        self._is_interactive = value
+
+    @property
     def language(self) -> Language:
         return self._language
 
     @property
     def encoding(self) -> Charset:
         return self.language.encoding
 
     @property
     def ttl(self) -> int:
-        return self.ttl
+        return self._ttl
 
 
 assert (configs := AskAiConfigs().INSTANCE) is not None
```

### Comparing `hspylib-askai-1.0.4/askai/core/askai_events.py` & `hspylib-askai-1.0.5/askai/core/askai_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         def __str__(self):
             return f"_EventBus-{self.bus.name}::({self.events})"
 
     # fmt: off
     ASKAI_BUS = _EventBus(
         ASKAI_BUS_NAME,
-        reply=_Event(REPLY_EVENT, erase_last=False),
+        reply=_Event(REPLY_EVENT, verbosity='normal', erase_last=False),
         reply_error=_Event(REPLY_ERROR_EVENT)
     )
 
     # fmt: on
 
     @staticmethod
     def get_bus(bus_name: str) -> Optional[EventBus]:
```

### Comparing `hspylib-askai-1.0.4/askai/core/askai_messages.py` & `hspylib-askai-1.0.5/askai/core/askai_messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from askai.core.askai_configs import configs
-from askai.language.argos_translator import ArgosTranslator
-from askai.language.language import Language
 from functools import lru_cache
+
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.modules.application.exit_status import ExitStatus
 
+from askai.core.askai_configs import configs
+from askai.language.argos_translator import ArgosTranslator
+from askai.language.language import Language
+
 
 class AskAiMessages(metaclass=Singleton):
     """Provide access to static 'translated' messages."""
 
     INSTANCE: "AskAiMessages" = None
 
     def __init__(self):
@@ -42,24 +44,24 @@
         return self.translate("I'm processing your voice…")
 
     @lru_cache
     def goodbye(self) -> str:
         return self.translate("Goodbye, have a nice day !")
 
     @lru_cache
-    def executing(self) -> str:
-        return self.translate(f"Executing command…")
+    def executing(self, command_line: str) -> str:
+        return self.translate(f"Executing `{command_line}`…")
 
     @lru_cache
-    def cmd_success(self, exit_code: ExitStatus) -> str:
-        return self.translate(f"OK, command executed with {str(exit_code).lower()}")
+    def cmd_success(self, command_line: str, exit_code: ExitStatus) -> str:
+        return self.translate(f"OK, command `{command_line}` executed with {str(exit_code).lower()}")
 
     @lru_cache
     def searching(self) -> str:
-        return self.translate(f"Searching…")
+        return self.translate(f"Searching on the internet…")
 
     @lru_cache
     def summarizing(self, path: str) -> str:
         return self.translate(f"Summarizing docs at:'{path}' …")
 
     @lru_cache
     def enter_qna(self) -> str:
@@ -73,69 +75,81 @@
     def qna_welcome(self) -> str:
         return self.translate("What specific information are you seeking about the content ?")
 
     @lru_cache
     def press_esc_enter(self) -> str:
         return self.translate("Press [Esc or Enter] to leave")
 
-    # Warnings and alerts
-
     @lru_cache
-    def cmd_no_output(self) -> str:
-        return self.translate("The command didn't return an output !")
+    def analysis(self) -> str:
+        return self.translate(f"Analysing the output…")
 
     @lru_cache
-    def search_empty(self) -> str:
-        return self.translate("The search didn't return an output !")
+    def assert_acc(self, ai_response: str, result: str) -> str:
+        return self.translate(f"Accuracy check: `{ai_response.strip()}` -> **{result.strip()}**")
 
     @lru_cache
-    def access_grant(self) -> str:
-        return self.translate("I require access to your files, folders and apps (grant/[deny])?")
+    def action_plan(self, plan_text: str) -> str:
+        return self.translate(f"Action plan: `{plan_text.strip()}`")
+
+    # Warnings and alerts
 
     @lru_cache
-    def not_a_command(self, shell: str, content: str) -> str:
-        return self.translate(f"Reply '{content}' is not a '{shell}' command !")
+    def search_empty(self) -> str:
+        return self.translate("The search didn't return an output !")
 
     @lru_cache
-    def invalid_cmd_format(self, output: str) -> str:
-        return self.translate(f"Reply '{output}' does not match the correct command format !")
+    def access_grant(self) -> str:
+        return self.translate("Do you approve executing this command on you terminal (yes/[no])?")
 
     # Failures
 
     @lru_cache
-    def no_processor(self, query_type: str) -> str:
-        return self.translate(f"Error: No suitable processor found for query type: '{query_type}' !")
+    def no_query_string(self) -> str:
+        return self.translate("No query string was provided in non-interactive mode !")
 
     @lru_cache
     def invalid_response(self, response_text: str) -> str:
-        return self.translate(f"Error: Received an invalid query response/type => '{response_text}' !")
+        return self.translate(f"Invalid query response/type => '{response_text}' !")
 
     @lru_cache
     def cmd_no_exist(self, command: str) -> str:
-        return self.translate(f"Error: Sorry! Command `{command}' does not exist !")
+        return self.translate(f"Command `{command}' does not exist !")
 
     @lru_cache
     def cmd_failed(self, cmd_line: str) -> str:
-        return self.translate(f"Error: Sorry! Command `{cmd_line}' failed to execute !")
+        return self.translate(f"Command `{cmd_line}' failed to execute !")
 
     @lru_cache
     def missing_package(self, err: ImportError) -> str:
-        return self.translate(f"Error: Unable to summarize => {str(err)}' !")
+        return self.translate(f"Unable to summarize => {str(err)}' !")
 
     @lru_cache
-    def summary_not_possible(self) -> str:
-        return self.translate("Sorry, summarization was not possible !")
+    def summary_not_possible(self, err: BaseException = None) -> str:
+        return self.translate(f"summarization was not possible {'=> ' + str(err) if err else ''}!")
 
     @lru_cache
-    def intelligible(self, question: str) -> str:
-        return self.translate(f"Error: Your question '{question}' is not clear, please reformulate !")
+    def intelligible(self, question: str, reason: str) -> str:
+        return self.translate(f"Your question '{question}' is unclear: '{reason}'")
+
+    @lru_cache
+    def impossible(self, reason: str) -> str:
+        return self.translate(f"Impossible to fulfill your request. Reason: {reason} !")
 
     @lru_cache
     def llm_error(self, error: str) -> str:
-        return self.translate(f"Error: 'LLM' failed to reply: {error} !")
+        return self.translate(f"'LLM' failed to reply: {error} !")
 
     @lru_cache
     def fail_to_search(self, error: str) -> str:
-        return self.translate(f"Error: 'InternetSearch' failed: {error} !")
+        return self.translate(f"'InternetSearch' failed: {error} !")
+
+    @lru_cache
+    def too_many_actions(self) -> str:
+        return self.translate("Failed to complete the request => 'Max chained actions reached' !")
+
+    @lru_cache
+    def unprocessable(self, reason: str) -> str:
+        return self.translate(f"Sorry, I was unable to process your request => {reason}")
 
 
 assert (msg := AskAiMessages().INSTANCE) is not None
```

### Comparing `hspylib-askai-1.0.4/askai/core/askai_prompt.py` & `hspylib-askai-1.0.5/askai/core/askai_prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,31 @@
    @created: Mon, 22 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-from askai.__classpath__ import _Classpath
+from functools import lru_cache
+
+from hspylib.core.metaclass.singleton import Singleton
+
+from askai.__classpath__ import classpath
 from askai.core.askai_configs import configs
 from askai.core.model.terminal_command import get_os, get_shell, get_user, SupportedPlatforms, SupportedShells
 from askai.core.support.utilities import read_resource
-from functools import lru_cache
-from hspylib.core.metaclass.singleton import Singleton
 
 
 class AskAiPrompt(metaclass=Singleton):
     """Provide the prompts used by the AskAi."""
 
     INSTANCE: "AskAiPrompt" = None
 
     # AI Prompts directory.
-    PROMPT_DIR = str(_Classpath.resource_path()) + "/assets/prompts"
+    PROMPT_DIR = str(classpath.resource_path()) + "/assets/prompts"
 
     def __init__(self):
         self._shell: SupportedShells = get_shell()
         self._os_type: SupportedPlatforms = get_os()
         self._user: str = get_user()
 
     @property
@@ -46,13 +48,13 @@
         return self._user
 
     @property
     def idiom(self) -> str:
         return f"{configs.language.name} ({configs.language.country})"
 
     @lru_cache
-    def read_prompt(self, template_file: str) -> str:
+    def read_prompt(self, template_file: str, prompt_dir: str = None) -> str:
         """Read a processor prompt template and set its persona."""
-        return read_resource(self.PROMPT_DIR, template_file)
+        return read_resource(prompt_dir or self.PROMPT_DIR, template_file)
 
 
 assert (prompt := AskAiPrompt().INSTANCE) is not None
```

### Comparing `hspylib-askai-1.0.4/askai/core/component/audio_player.py` & `hspylib-askai-1.0.5/askai/core/component/audio_player.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,37 @@
    @created: Wed, 22 Feb 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-from askai.__classpath__ import _Classpath
-from clitt.core.term.terminal import Terminal
+import logging as log
+import time
 from functools import lru_cache
+from shutil import which
+from typing import Literal
+
+from clitt.core.term.terminal import Terminal
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_argument
 from hspylib.core.tools.commons import file_is_not_empty
 from hspylib.core.tools.text_tools import ensure_endswith
 from hspylib.modules.application.exit_status import ExitStatus
-from shutil import which
-from typing import Literal
 
-import logging as log
-import time
+from askai.__classpath__ import classpath
 
 
 class AudioPlayer(metaclass=Singleton):
     """Provide an interface to play audio using the default speaker device."""
 
     INSTANCE: "AudioPlayer" = None
 
     # Sound effects directory.
-    SFX_DIR = str(_Classpath.resource_path()) + "/assets/sound-fx"
+    SFX_DIR = str(classpath.resource_path()) + "/assets/sound-fx"
 
     @staticmethod
     def play_audio_file(path_to_audio_file: str, tempo: int = 1) -> bool:
         """Play the specified mp3 file using ffplay (ffmpeg) application.
         :param path_to_audio_file: the path to the mp3 file to be played.
         :param tempo: the playing speed.
         """
```

### Comparing `hspylib-askai-1.0.4/askai/core/component/cache_service.py` & `hspylib-askai-1.0.5/askai/core/component/cache_service.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/component/geo_location.py` & `hspylib-askai-1.0.5/askai/core/component/geo_location.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/component/internet_service.py` & `hspylib-askai-1.0.5/askai/core/component/internet_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
 from askai.core.component.cache_service import PERSIST_DIR
 from askai.core.component.geo_location import geo_location
 from askai.core.component.summarizer import summarizer
+from askai.core.engine.openai.temperature import Temperature
 from askai.core.model.search_result import SearchResult
 from askai.core.support.langchain_support import lc_llm, load_document
 from askai.core.support.shared_instances import shared
 
 
 class InternetService(metaclass=Singleton):
     """Provide a internet search service to complete queries that require realtime data."""
@@ -104,29 +105,31 @@
         :param search: The AI search parameters.
         """
         AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.searching())
         search.sites = search.sites if len(search.sites) > 0 else ['google.com', 'bing.com']
         try:
             query = self._build_query(search).strip()
             log.info("Searching Google for '%s'", query)
-            content = str(self._tool.run(query))
+            ctx = str(self._tool.run(query))
             llm_prompt = ChatPromptTemplate.from_messages([("system", "{query}\n\n{context}")])
-            chain = create_stuff_documents_chain(lc_llm.create_chat_model(), llm_prompt)
-            output = chain.invoke({"query": search.question, "context": [Document(content)]})
+            context: List[Document] = [Document(ctx)]
+            chain = create_stuff_documents_chain(lc_llm.create_chat_model(
+                temperature=Temperature.DATA_ANALYSIS.temp), llm_prompt)
+            output = chain.invoke({"query": search.question, "context": context})
         except HttpError as err:
             output = msg.fail_to_search(str(err))
 
-        return self.refine_text(search.question, output) if output else None
+        return self.refine_text(search.question, output, search.sites) if output else None
 
-    def refine_text(self, question: str, text: str) -> str:
+    def refine_text(self, question: str, context: str, sites: list[str]) -> Optional[str]:
         """Refines the text retrieved by the search engine."""
         refine_prompt = PromptTemplate.from_template(self.refine_template()).format(
-            question=question, existing_answer=text, datetime=geo_location.datetime,
-            location=geo_location.location, idiom=shared.idiom
-        )
-        chain = create_stuff_documents_chain(
-            lc_llm.create_chat_model(), ChatPromptTemplate.from_messages([("system", "{query}\n\n{context}")])
-        )
-        return chain.invoke({"query": question, "context": [Document(refine_prompt)]})
+            idiom=shared.idiom, sources=sites, location=geo_location.location,
+            context=context, question=question)
+        log.info("STT::[QUESTION] '%s'", context)
+        llm = lc_llm.create_chat_model(temperature=Temperature.CREATIVE_WRITING.temp)
+        output = llm.predict(refine_prompt)
+
+        return output
 
 
 assert (internet := InternetService().INSTANCE) is not None
```

### Comparing `hspylib-askai-1.0.4/askai/core/component/recorder.py` & `hspylib-askai-1.0.5/askai/core/component/recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,34 +8,35 @@
    @created: Wed, 22 Feb 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-from askai.core.askai_events import AskAiEvents
-from askai.core.askai_messages import msg
-from askai.core.component.cache_service import REC_DIR
-from askai.core.support.settings import Settings
-from askai.core.support.utilities import display_text
-from askai.exception.exceptions import IntelligibleAudioError, InvalidInputDevice, InvalidRecognitionApiError
-from askai.language.language import Language
-from clitt.core.term.cursor import Cursor
+import logging as log
+import os
+from pathlib import Path
+from typing import Callable, List, Optional, Tuple
+
+import pause
+from clitt.core.term.cursor import cursor
 from clitt.core.tui.mselect.mselect import mselect
 from hspylib.core.enums.enumeration import Enumeration
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.commons import file_is_not_empty
 from hspylib.core.zoned_datetime import now_ms
-from pathlib import Path
 from speech_recognition import AudioData, Microphone, Recognizer, RequestError, UnknownValueError, WaitTimeoutError
-from typing import Callable, List, Optional, Tuple
 
-import logging as log
-import os
-import pause
+from askai.core.askai_events import AskAiEvents
+from askai.core.askai_messages import msg
+from askai.core.component.cache_service import REC_DIR
+from askai.core.support.settings import Settings
+from askai.core.support.utilities import display_text
+from askai.exception.exceptions import IntelligibleAudioError, InvalidInputDevice, InvalidRecognitionApiError
+from askai.language.language import Language
 
 
 class Recorder(metaclass=Singleton):
     """Provide an interface to record voice using the microphone device."""
 
     INSTANCE: "Recorder" = None
 
@@ -60,15 +61,15 @@
     def __init__(self):
         self._rec: Recognizer = Recognizer()
         self._settings: Settings = Settings(self.ASKAI_SETTINGS_FILE, load_dir=self.ASKAI_SETTINGS_DIR)
         self._devices = []
         self._device_index = None
         self._input_device = None
         self._rec_phrase_limit_s = 10
-        self._rec_wait_timeout_s = 0.5
+        self._rec_wait_timeout_s = 0.8
 
     def setup(self) -> None:
         """Setup the recorder."""
         self._devices = self.get_device_list()
         log.debug("Available audio devices:\n%s", "\n".join([f"{d[0]} - {d[1]}" for d in self._devices]))
         self._device_index = self._select_device()
         self._input_device = self._devices[self._device_index] if self._device_index is not None else None
@@ -90,25 +91,24 @@
         """
         audio_path = Path(f"{REC_DIR}/askai-stt-{now_ms()}.wav")
         with Microphone(device_index=self._device_index) as source:
             try:
                 self._detect_noise()
                 AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.listening())
                 audio: AudioData = self._rec.listen(
-                    source, phrase_time_limit=self._rec_phrase_limit_s, timeout=self._rec_wait_timeout_s
-                )
+                    source, phrase_time_limit=self._rec_phrase_limit_s, timeout=self._rec_wait_timeout_s)
                 AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.transcribing(), erase_last=True)
                 with open(audio_path, "wb") as f_rec:
                     f_rec.write(audio.get_wav_data())
                     log.debug("Voice recorded and saved as %s", audio_path)
                 if api := getattr(self._rec, recognition_api.value):
                     log.debug("Recognizing voice using %s", recognition_api)
                     assert isinstance(api, Callable)
                     stt_text = api(audio, language=language.language)
-                    Cursor.INSTANCE.erase_line()
+                    cursor.erase_line()
                 else:
                     raise InvalidRecognitionApiError(str(recognition_api or "<none>"))
             except WaitTimeoutError:
                 log.warning("Timed out while waiting for a speech!")
                 stt_text = ""
             except AttributeError as err:
                 raise InvalidInputDevice(str(err)) from err
```

### Comparing `hspylib-askai-1.0.4/askai/core/component/summarizer.py` & `hspylib-askai-1.0.5/askai/core/component/summarizer.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/engine/ai_engine.py` & `hspylib-askai-1.0.5/askai/core/engine/ai_engine.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/engine/engine_factory.py` & `hspylib-askai-1.0.5/askai/core/engine/engine_factory.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/engine/openai/openai_configs.py` & `hspylib-askai-1.0.5/askai/core/engine/openai/openai_configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,30 @@
    @created: Fri, 12 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-from askai.__classpath__ import _Classpath
-from askai.core.askai_configs import AskAiConfigs
+from typing import Literal
+
 from hspylib.core.config.app_config import AppConfigs
 from hspylib.core.metaclass.singleton import Singleton
-from typing import Literal
+
+from askai.__classpath__ import classpath
+from askai.core.askai_configs import AskAiConfigs
 
 
 class OpenAiConfigs(AskAiConfigs, metaclass=Singleton):
     """Provides access to OpenAI configurations."""
 
     INSTANCE: "OpenAiConfigs" = None
 
     # The resources folder
-    RESOURCE_DIR = str(_Classpath.resource_path())
+    RESOURCE_DIR = str(classpath.resource_path())
 
     def __init__(self):
         super().__init__()
         self._configs = AppConfigs.INSTANCE or AppConfigs(self.RESOURCE_DIR)
         self._stt_model = self._configs.get("openai.speech-to-text.model")
         self._tts_model = self._configs.get("openai.text-to-speech.model")
         self._tts_voice = self._configs.get("openai.text-to-speech.voice")
```

### Comparing `hspylib-askai-1.0.4/askai/core/engine/openai/openai_engine.py` & `hspylib-askai-1.0.5/askai/core/engine/openai/openai_engine.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/engine/openai/openai_model.py` & `hspylib-askai-1.0.5/askai/core/engine/openai/openai_model.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/engine/openai/temperatures.py` & `hspylib-askai-1.0.5/askai/core/engine/openai/temperature.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from hspylib.core.enums.enumeration import Enumeration
 
 
-class Temperatures(Enumeration):
+class Temperature(Enumeration):
     """Provide some recommended temperature x top_p combinations for ChatGPT prompts.
     Ref:. https://community.openai.com/t/cheat-sheet-mastering-temperature-and-top-p-in-chatgpt-api/172683
 
     - Lower temperature (e.g., 0.1 - 0.4): Produces more focused, conservative, and consistent responses.
     This is useful when the marketer needs factual information, precise answers, or messaging that adheres closely
     to a specific format or brand guideline.
 
@@ -16,15 +16,15 @@
     - Higher temperature (e.g., 0.8 - 1.0): Generates more creative, diverse, and unexpected outputs.
     Marketers may prefer this setting when brainstorming innovative campaign ideas, crafting engaging social media
     content, or seeking fresh perspectives on a topic.
     """
 
     # fmt: off
 
-    ZERO                        = 0.0, 0.0
+    COLDEST                     = 0.0, 0.0
 
     # Generates code that adheres to established patterns and conventions. Output is more deterministic and focused.
     # Useful for generating syntactically correct code.
     CODE_GENERATION             = 0.2, 0.1
 
     # Generates creative and diverse text for storytelling. Output is more exploratory and less constrained by patterns.
     CREATIVE_WRITING            = 0.7, 0.8
@@ -43,7 +43,16 @@
     # Generates code that explores alternative solutions and creative approaches. Output is less constrained by
     # established patterns.
     EXPLORATORY_CODE_WRITING    = 0.6, 0.7
 
     HOTTEST                     = 1.0, 1.0
 
     # fmt: on
+
+    @property
+    def temp(self) -> float:
+        return self.value[0]
+
+    @property
+    def top_p(self) -> float:
+        return self.value[1]
+
```

### Comparing `hspylib-askai-1.0.4/askai/core/model/ai_model.py` & `hspylib-askai-1.0.5/askai/core/model/ai_model.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/model/ai_reply.py` & `hspylib-askai-1.0.5/askai/core/model/ai_reply.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/model/chat_context.py` & `hspylib-askai-1.0.5/askai/core/model/chat_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,54 +6,56 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
 
-from askai.exception.exceptions import TokenLengthExceeded
+import os
 from collections import defaultdict, namedtuple
 from functools import reduce
+from typing import Any, List, Literal, Optional, TypeAlias
+
 from hspylib.core.zoned_datetime import now
-from typing import Any, Dict, List, Literal, Optional, TypeAlias
 
-import os
+from askai.exception.exceptions import TokenLengthExceeded
+
+ChatRoles: TypeAlias = Literal["system", "human", "assistant"]
+
+ContextRaw: TypeAlias = list[dict[str, str]]
 
-ChatRoles: TypeAlias = Literal["system", "user", "assistant"]
+LangChainContext: TypeAlias = list[tuple[str, str]]
 
-ContextRaw: TypeAlias = List[Dict[str, str]]
+ContextEntry = namedtuple("ContextEntry", ["created_at", "role", "content"], rename=False)
 
 
 class ChatContext:
     """Provide a chat context helper for AI engines."""
 
-    ContextEntry = namedtuple("ContextEntry", ["created_at", "role", "content"], rename=False)
-
     def __init__(self, token_limit: int):
-        self._context = defaultdict(list)
+        self._context: dict[Any, list] = defaultdict(list)
         self._token_limit: int = token_limit * 1024  # The limit is given in KB
 
     def __str__(self):
         return os.linesep.join(f"'{k}': '{v}'" for k, v in self._context.items())
 
     def __getitem__(self, key) -> List[ContextEntry]:
         return self._context[key]
 
-    def push(self, key: str, content: Any, role: ChatRoles = "user") -> ContextRaw:
+    def push(self, key: str, content: Any, role: ChatRoles = "human") -> ContextRaw:
         """Push a context message to the chat with the provided role."""
-        entry = ChatContext.ContextEntry(now(), role, str(content))
+        entry = ContextEntry(now(), role, str(content))
         ctx = self._context[key]
         token_length = reduce(lambda total, e: total + len(e.content), ctx, 0) if len(ctx) > 0 else 0
         if (token_length := token_length + len(content)) > self._token_limit:
             raise TokenLengthExceeded(f"Required token length={token_length}  limit={self._token_limit}")
-        if entry.content not in [c.content for c in ctx]:
-            ctx.append(entry)
+        ctx.append(entry)
         return self.get(key)
 
-    def set(self, key: str, content: Any, role: ChatRoles = "user") -> ContextRaw:
+    def set(self, key: str, content: Any, role: ChatRoles = "human") -> ContextRaw:
         """Set the context to the chat with the provided role."""
         self.clear(key)
         return self.push(key, content, role)
 
     def remove(self, key: str, index: int) -> Optional[str]:
         """Remove a context message from the chat at the provided index."""
         val = None
@@ -61,33 +63,47 @@
             if index < len(ctx):
                 val = ctx[index]
                 del ctx[index]
         return val
 
     def get(self, key: str) -> ContextRaw:
         """Retrieve a context from the specified by key."""
-        return [{"role": c.role, "content": c.content} for c in self._context[key]] or []
+        return [{"role": ctx.role, "content": ctx.content} for ctx in self._context[key]] or []
 
-    def join(self, *keys: str) -> ContextRaw:
+    def join(self, *keys: str) -> LangChainContext:
         """Join contexts specified by keys."""
-        context: ContextRaw = []
+        context: LangChainContext = []
         token_length = 0
         for key in keys:
-            ctx = self.get(key)
-            content = " ".join([t["content"] for t in ctx])
+            ctx: ContextRaw = self.get(key)
+            content: str = os.linesep.join([tk['content'] for tk in ctx])
             token_length += len(content or "")
             if token_length > self._token_limit:
                 raise TokenLengthExceeded(f"Required token length={token_length}k  limit={self._token_limit}k")
             if content and ctx not in context:
-                context.extend(ctx)
+                list(map(context.append, [(t['role'], t['content']) for t in ctx]))
         return context
 
     def flat(self, *keys: str) -> str:
         """Flatten contexts specified by keys."""
-        return os.linesep.join([ctx["content"] for ctx in self.join(*keys)])
+        return os.linesep.join([f"\n{ctx[0].upper()}\n{ctx[1]}" for ctx in self.join(*keys)])
 
     def clear(self, *keys: str) -> int:
         """Clear the all the chat context specified by key."""
         for key in keys:
             if self._context[key]:
                 del self._context[key]
         return len(self._context)
+
+    def forget(self) -> None:
+        """Forget all entries pushed to the chat context."""
+        del self._context
+        self._context = defaultdict(list)
+
+
+if __name__ == '__main__':
+    c = ChatContext(1000)
+    c.push("TESTE", 'What is the size of the moon?')
+    c.push("TESTE", 'What is the size of the moon?', 'assistant')
+    c.push("TESTE", 'Who are you?')
+    c.push("TESTE", "I'm Taius, you digital assistant", 'assistant')
+    print(c.join("TESTE"))
```

### Comparing `hspylib-askai-1.0.4/askai/core/model/processor_response.py` & `hspylib-askai-1.0.5/askai/core/model/search_result.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
 """
    @project: HsPyLib-AskAI
    @package: askai.core.model
-      @file: processor_response.py
-   @created: Fri, 23 Feb 2024
+      @file: search_result.py
+   @created: Sun, 12 Mar 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
-
-from askai.core.model.terminal_command import TerminalCommand
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from typing import List
 
 import json
 
 
 @dataclass
-class ProcessorResponse:
-    """Keep track of the processor responses."""
+class SearchResult:
+    """Keep track of the internet search responses."""
 
-    query_type: str = ""
-    question: str = ""
-    response: str = ""
-    terminating: bool = False
-    intelligible: bool = False
-    forwarded: bool = False
-    require_summarization: bool = False
-    commands: List[TerminalCommand] = field(default_factory=list)
+    question: str = None
+    datetime: str = None
+    category: str = None
+    keywords: List[str] = None
+    sites: List[str] = None
+    filters: List[str] = None
+    response: str = None
 
     def __str__(self):
-        return json.dumps(self.__dict__, default=lambda obj: obj.__dict__)
+        return f"Search Results: {json.dumps(self.__dict__, default=lambda obj: obj.__dict__)}"
```

### Comparing `hspylib-askai-1.0.4/askai/core/model/search_result.py` & `hspylib-askai-1.0.5/askai/core/model/summary_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.model
-      @file: search_result.py
-   @created: Sun, 12 Mar 2024
+      @file: summary_result.py
+   @created: Sun, 10 Mar 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
 from dataclasses import dataclass
-from typing import List
 
 import json
 
 
 @dataclass
-class SearchResult:
-    """Keep track of the internet search responses."""
+class SummaryResult:
+    """Keep track of the summarization responses."""
 
+    folder: str = None
+    glob: str = None
     question: str = None
-    datetime: str = None
-    category: str = None
-    keywords: List[str] = None
-    sites: List[str] = None
-    filters: List[str] = None
-    response: str = None
+    answer: str = None
 
     def __str__(self):
-        return f"Search Results: {json.dumps(self.__dict__, default=lambda obj: obj.__dict__)}"
+        return f"Summarization results: {json.dumps(self.__dict__, default=lambda obj: obj.__dict__)}"
```

### Comparing `hspylib-askai-1.0.4/askai/core/model/terminal_command.py` & `hspylib-askai-1.0.5/askai/core/model/terminal_command.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/processor/instances/summary_processor.py` & `hspylib-askai-1.0.5/askai/core/features/router.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,110 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
+import logging as log
+import os
+import re
+from functools import lru_cache
+from typing import TypeAlias, Optional
 
-"""
-   @project: HsPyLib-AskAI
-   @package: askai.core.processor
-      @file: generic_processor.py
-   @created: Fri, 23 Feb 2024
-    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
-   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+from hspylib.core.metaclass.singleton import Singleton
+from langchain.chains.combine_documents import create_stuff_documents_chain
+from langchain_core.documents import Document
+from langchain_core.prompts import PromptTemplate, ChatPromptTemplate
+from langchain_core.runnables import Runnable
+from langchain_core.runnables.utils import Input, Output
+from retry import retry
 
-   Copyright·(c)·2024,·HSPyLib
-"""
 from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
-from askai.core.component.summarizer import summarizer
-from askai.core.model.processor_response import ProcessorResponse
-from askai.core.model.query_type import QueryType
-from askai.core.model.summary_result import SummaryResult
-from askai.core.processor.processor_base import AIProcessor
+from askai.core.engine.openai.temperature import Temperature
+from askai.core.features.actions import features
+from askai.core.model.rag_response import RagResponse
 from askai.core.support.langchain_support import lc_llm
-from askai.core.support.object_mapper import object_mapper
 from askai.core.support.shared_instances import shared
-from askai.core.support.utilities import display_text
-from askai.exception.exceptions import DocumentsNotFound
-from functools import lru_cache
-from langchain.chains.combine_documents import create_stuff_documents_chain
-from langchain_core.documents import Document
-from langchain_core.prompts import ChatPromptTemplate, PromptTemplate
-from typing import List, Optional, Tuple
-
-import logging as log
-import os
+from askai.exception.exceptions import InaccurateResponse, MaxInteractionsReached
 
+RunnableTool: TypeAlias = Runnable[list[Input], list[Output]]
 
-class SummaryProcessor:
-    """Process generic prompts."""
 
-    @staticmethod
-    def _ask_and_reply(question: str) -> Optional[str]:
-        """Query the summarized for questions related to the summarized content.
-        :param question: the question to be asked to the AI.
-        """
-        output = None
-        if results := summarizer.query(question):
-            output = os.linesep.join([r.answer for r in results]).strip()
-        return output
+class Router(metaclass=Singleton):
+    """Class to provide a divide and conquer set of actions to fulfill an objective. This is responsible for the
+    orchestration and execution of the actions."""
 
-    @staticmethod
-    def q_type() -> str:
-        return QueryType.SUMMARY_QUERY.value
+    INSTANCE: 'Router' = None
 
     def __init__(self):
-        self._template_file: str = "summary-prompt"
-        self._next_in_chain: AIProcessor | None = None
-        self._supports: List[str] = [self.q_type()]
-
-    def name(self) -> str:
-        return type(self).__name__
-
-    def supports(self, query_type: str) -> bool:
-        return query_type in self._supports
-
-    def next_in_chain(self) -> Optional[str]:
-        return self._next_in_chain
-
-    def bind(self, next_in_chain: AIProcessor):
-        self._next_in_chain = next_in_chain
+        self._approved = False
 
     @lru_cache
     def template(self) -> str:
-        return prompt.read_prompt(self._template_file)
+        return prompt.read_prompt("router-prompt.txt")
 
-    def process(self, query_response: ProcessorResponse) -> Tuple[bool, Optional[str]]:
-        status = False
-        template = PromptTemplate(input_variables=["os_type", "idiom"], template=self.template())
-        final_prompt: str = template.format(os_type=prompt.os_type, idiom=shared.idiom)
-        shared.context.set("SETUP", final_prompt, "system")
-        shared.context.set("QUESTION", f"\n\nQuestion:\n{query_response.question}")
-        ctx: str = shared.context.flat("SETUP", "QUESTION")
-        log.info("Summary::[QUESTION] '%s'  context=%s", query_response.question, ctx)
-
-        chat_prompt = ChatPromptTemplate.from_messages([("system", "{query}\n\n{context}")])
-        chain = create_stuff_documents_chain(lc_llm.create_chat_model(), chat_prompt)
-        context = Document(ctx)
-
-        try:
-            if response := chain.invoke({"query": query_response.question, "context": [context]}):
-                log.debug("Summary::[RESPONSE] Received from AI: %s.", response)
-                summary: SummaryResult = object_mapper.of_json(response, SummaryResult)
-                if not isinstance(summary, SummaryResult):
-                    log.error(msg.invalid_response(SummaryResult))
-                    output = response
-                else:
-                    if not summarizer.exists(summary.folder, summary.glob):
-                        if not summarizer.generate(summary.folder, summary.glob):
-                            return True, msg.summary_not_possible()
-                    else:
-                        summarizer.folder = summary.folder
-                        summarizer.glob = summary.glob
-                        log.info("Reusing persisted summarized content: '%s'/'%s'", summary.folder, summary.glob)
-                    output = self._qna()
-                status = True
+    @staticmethod
+    def _assert_accuracy(question: str, ai_response: str) -> Optional[str]:
+        """Function responsible for asserting that the question was properly answered."""
+        if ai_response:
+            template = PromptTemplate(
+                input_variables=['context', 'question'],
+                template=prompt.read_prompt('ryg-prompt'))
+            final_prompt = template.format(context=ai_response, question=question)
+            log.info("Assert::[QUESTION] '%s'  context: '%s'", question, ai_response)
+            llm = lc_llm.create_chat_model(Temperature.DATA_ANALYSIS.temp)
+
+            if (output := llm.predict(final_prompt)) and (mat := RagResponse.matches(output)):
+                status, reason = mat.group(1), mat.group(2)
+                log.info("Accuracy check  status: '%s'  reason: '%s'", status, reason)
+                AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.assert_acc(ai_response, output), verbosity='debug')
+                if RagResponse.of_value(status.strip()).is_bad:
+                    raise InaccurateResponse(RagResponse.strip_code(output))
+                return ai_response
+
+        raise InaccurateResponse(f"The AI Assistant did not respond properly!")
+
+    def process(self, query: str) -> Optional[str]:
+        """Process the user query and retrieve the final response."""
+        @retry(exceptions=InaccurateResponse, tries=2, delay=0, backoff=0)
+        def _process_wrapper(question: str) -> Optional[str]:
+            """Wrapper to allow RAG retries."""
+            template = PromptTemplate(input_variables=[
+                'features', 'question', 'os_type'
+            ], template=self.template())
+            ctx: str = shared.context.flat("CONTEXT")
+            final_prompt = template.format(
+                features=features.enlist(), question=question, os_type=prompt.os_type)
+            log.info("Router::[QUESTION] '%s'  context: '%s'", question, ctx)
+
+            chat_prompt = ChatPromptTemplate.from_messages([("system", "{context}\n\n{query}")])
+            chain = create_stuff_documents_chain(
+                lc_llm.create_chat_model(Temperature.HOTTEST.temp), chat_prompt)
+            context = [Document(ctx)]
+
+            if response := chain.invoke({"query": final_prompt, "context": context}):
+                log.info("Router::[RESPONSE] Received from AI: \n%s.", str(response))
+                shared.context.push("CONTEXT", question)
+                actions: list[str] = re.sub(r'\d+[.:)-]\s+', '', response).split(os.linesep)
+                actions = list(filter(len, map(str.strip, actions)))
+                AskAiEvents.ASKAI_BUS.events.reply.emit(
+                    message=msg.action_plan('` -> `'.join(actions)), verbosity='debug')
+                output = self._route(question, actions)
             else:
-                output = msg.llm_error(response)
-        except (FileNotFoundError, ValueError, DocumentsNotFound) as err:
-            output = msg.llm_error(err)
-            status = True
-
-        return status, output
-
-    def _qna(self) -> str:
-        """Questions and Answers about the summarized content."""
-        display_text(
-            f"# {msg.enter_qna()} %EOL%"
-            f"> Content:  {summarizer.sum_path} %EOL%%EOL%"
-            f"`{msg.press_esc_enter()}` %EOL%"
-        )
-        AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.qna_welcome())
-        while question := shared.input_text(f"{shared.username}: %GREEN%"):
-            if not (output := self._ask_and_reply(question)):
+                output = response
+            return output
+
+        return _process_wrapper(query)
+
+    def _route(self, question: str, actions: list[str]) -> Optional[str]:
+        """Route the actions to the proper function invocations."""
+        max_actions: int = 20  # TODO Move to configs
+        result: str = ''
+        for idx, action in enumerate(actions):
+            AskAiEvents.ASKAI_BUS.events.reply.emit(message=f"> `{action}`", verbosity='debug')
+            if idx > max_actions:
+                AskAiEvents.ASKAI_BUS.events.reply_error.emit(message=msg.too_many_actions())
+                raise MaxInteractionsReached(f"Maximum number of action was reached")
+            if not (result := features.invoke(action, result)):
+                log.warning("Last result brought an empty response for '%s'", action)
                 break
-            AskAiEvents.ASKAI_BUS.events.reply.emit(message=f"%GREEN%{output}%NC%")
-        display_text(f"# {msg.leave_qna()} %EOL%")
 
-        return msg.welcome_back()
+        return self._assert_accuracy(question, result)
+
+
+assert (router := Router().INSTANCE) is not None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.4/askai/core/processor/processor_proxy.py` & `hspylib-askai-1.0.5/askai/core/features/tools/browser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,50 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-"""
-   @project: HsPyLib-AskAI
-   @package: askai.core.processor
-      @file: processor_proxy.py
-   @created: Fri, 23 Feb 2024
-    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
-   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+import logging as log
+from typing import Optional
 
-   Copyright·(c)·2024,·HSPyLib
-"""
+from langchain.chains.combine_documents import create_stuff_documents_chain
+from langchain_core.documents import Document
+from langchain_core.prompts import PromptTemplate, ChatPromptTemplate
 
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
-from askai.core.model.processor_response import ProcessorResponse
+from askai.core.component.cache_service import cache
+from askai.core.component.geo_location import geo_location
+from askai.core.component.internet_service import internet
+from askai.core.model.search_result import SearchResult
 from askai.core.support.langchain_support import lc_llm
 from askai.core.support.object_mapper import object_mapper
 from askai.core.support.shared_instances import shared
-from functools import lru_cache
-from hspylib.core.metaclass.singleton import Singleton
-from langchain.chains.combine_documents import create_stuff_documents_chain
-from langchain_core.documents import Document
-from langchain_core.prompts import ChatPromptTemplate, PromptTemplate
-from typing import Tuple
-
-import logging as log
 
 
-class ProcessorProxy(metaclass=Singleton):
-    """TODO"""
-
-    INSTANCE: "ProcessorProxy" = None
-
-    def __init__(self):
-        pass
-
-    @lru_cache
-    def template(self) -> str:
-        return prompt.read_prompt("proxy-prompt")
-
-    def process(self, question: str) -> Tuple[bool, ProcessorResponse]:
-        """Return the setup prompt.
-        :param question: The question to the AI engine.
-        """
-        status = False
-        template = PromptTemplate(input_variables=["idiom"], template=self.template())
-        final_prompt = template.format(idiom=shared.idiom)
-        shared.context.set("SETUP", final_prompt, "system")
-        shared.context.set("QUESTION", f"\n\nQuestion: {question}\n\nHelpful Answer:")
-        ctx: str = shared.context.flat("CONTEXT", "SETUP", "QUESTION")
-        log.info("Proxy::[QUESTION] '%s'  context=%s", question, ctx)
-
-        chat_prompt = ChatPromptTemplate.from_messages([("system", "{query}\n\n{context}")])
-        chain = create_stuff_documents_chain(lc_llm.create_chat_model(), chat_prompt)
-        context = Document(ctx)
-
-        if response := chain.invoke({"query": question, "context": [context]}):
-            log.info("Proxy::[RESPONSE] Received from AI: %s.", str(response))
-            output = object_mapper.of_json(response, ProcessorResponse)
-            if not isinstance(output, ProcessorResponse):
-                log.error(msg.invalid_response(output))
-                output = response
-            else:
-                status = True
+def browse(query: str) -> Optional[str]:
+    """Fetch the information from the Internet."""
+    template = PromptTemplate(input_variables=[
+        "idiom", "datetime", 'location', 'question'
+    ], template=prompt.read_prompt('internet-prompt'))
+    final_prompt: str = template.format(
+        idiom=shared.idiom, datetime=geo_location.datetime,
+        location=geo_location.location, question=query)
+    ctx: str = shared.context.flat("CONTEXT")
+    log.info("Browser::[QUESTION] '%s'  context=''", final_prompt)
+    chat_prompt = ChatPromptTemplate.from_messages([("system", "{query}\n\n{context}")])
+    chain = create_stuff_documents_chain(lc_llm.create_chat_model(), chat_prompt)
+    context = [Document(ctx)]
+
+    response = chain.invoke({"query": final_prompt, "context": context})
+    if response and shared.UNCERTAIN_ID not in response:
+        search: SearchResult = object_mapper.of_json(response, SearchResult)
+        if not isinstance(search, SearchResult):
+            log.error(msg.invalid_response(search))
+            output = response.strip()
         else:
-            output = ProcessorResponse(question=question, terminating=True, response=response)
-
-        return status, output
-
+            output = internet.search_google(search)
+            if output:
+                shared.context.push("CONTEXT", query)
+                shared.context.push("CONTEXT", output, "assistant")
+                cache.save_reply(query, output)
+            else:
+                output = msg.search_empty()
+    else:
+        output = msg.translate("Sorry, I don't know.")
 
-assert (proxy := ProcessorProxy().INSTANCE) is not None
+    return output
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.4/askai/core/support/langchain_support.py` & `hspylib-askai-1.0.5/askai/core/support/langchain_support.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/support/object_mapper.py` & `hspylib-askai-1.0.5/askai/core/support/object_mapper.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/support/presets.py` & `hspylib-askai-1.0.5/askai/core/support/presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 class Presets:
     """Provides text streaming presets according to the language used."""
 
     # fmt: off
 
     _ALL_RESETS = {
         "en": {
-            "words.per.breath": 10,
-             "words.interval.sec": Template("12.2 * ${base_speed}"),
-            "breath.interval.sec": Template("43 * ${base_speed}"),
-            "number.interval.sec": Template("25 * ${base_speed}"),
-             "comma.interval.sec": Template("25 * ${base_speed}"),
-             "punct.interval.sec": Template("32 * ${base_speed}"),
-              "enum.interval.sec": Template("10 * ${base_speed}"),
-            "period.interval.sec": Template("165 * ${base_speed}"),
+            "words.per.breath": 9,
+             "words.interval.sec": Template("12.6 * ${base_speed}"),
+            "breath.interval.sec": Template("90 * ${base_speed}"),
+            "number.interval.sec": Template("17 * ${base_speed}"),
+             "comma.interval.sec": Template("28 * ${base_speed}"),
+             "punct.interval.sec": Template("35 * ${base_speed}"),
+              "enum.interval.sec": Template("12 * ${base_speed}"),
+            "period.interval.sec": Template("190 * ${base_speed}"),
         },
         "pt": {
-            "words.per.breath": 10,
+            "words.per.breath": 9,
              "words.interval.sec": Template("8 * ${base_speed}"),
             "breath.interval.sec": Template("40 * ${base_speed}"),
             "number.interval.sec": Template("27 * ${base_speed}"),
              "comma.interval.sec": Template("25 * ${base_speed}"),
              "punct.interval.sec": Template("31 * ${base_speed}"),
               "enum.interval.sec": Template("10 * ${base_speed}"),
             "period.interval.sec": Template("160 * ${base_speed}"),
```

### Comparing `hspylib-askai-1.0.4/askai/core/support/settings.py` & `hspylib-askai-1.0.5/askai/core/support/settings.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/core/support/shared_instances.py` & `hspylib-askai-1.0.5/askai/core/support/shared_instances.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from typing import Optional
+
+from clitt.core.term.terminal import terminal
+from clitt.core.tui.line_input.line_input import line_input
+from hspylib.core.metaclass.singleton import Singleton
+from hspylib.core.preconditions import check_state
+from hspylib.modules.cli.keyboard import Keyboard
+
 from askai.core.askai_configs import configs
 from askai.core.askai_prompt import prompt
 from askai.core.engine.ai_engine import AIEngine
 from askai.core.engine.engine_factory import EngineFactory
 from askai.core.model.chat_context import ChatContext
 from askai.core.support.utilities import display_text
-from clitt.core.term.terminal import terminal
-from clitt.core.tui.line_input.line_input import line_input
-from hspylib.core.metaclass.singleton import Singleton
-from hspylib.core.preconditions import check_state
-from hspylib.modules.cli.keyboard import Keyboard
-from typing import Optional
 
 
 class SharedInstances(metaclass=Singleton):
     """TODO"""
 
     INSTANCE: "SharedInstances" = None
 
@@ -41,15 +43,15 @@
     @context.setter
     def context(self, value: ChatContext) -> None:
         check_state(self._context is None, "Once set, this instance is immutable.")
         self._context = value
 
     @property
     def nickname(self) -> str:
-        return f"%GREEN%  {self.engine.nickname()}%NC%"
+        return f"%GREEN%  Taius%NC%"
 
     @property
     def username(self) -> str:
         return f"%WHITE%  {prompt.user.title()}%NC%"
 
     @property
     def idiom(self) -> str:
@@ -74,12 +76,22 @@
         ret = None
         while ret is None:
             if (ret := line_input(input_prompt)) == Keyboard.VK_CTRL_L:  # Use STT as input method.
                 terminal.cursor.erase_line()
                 if spoken_text := self.engine.speech_to_text():
                     display_text(f"{self.username}: {spoken_text}")
                     ret = spoken_text
+            elif ret == Keyboard.VK_CTRL_K:
+                shared.context.forget()
+                display_text(f"{self.nickname}: Context reset", erase_last=True)
+                ret = None
+                continue
+            elif ret == Keyboard.VK_CTRL_G:
+                configs.is_speak = not configs.is_speak
+                display_text(f"{self.nickname}: Speaking is {'ON' if configs.is_speak else 'OFF'}", erase_last=True)
+                ret = None
+                continue
 
         return ret if not ret or isinstance(ret, str) else ret.val
 
 
 assert (shared := SharedInstances().INSTANCE) is not None
```

### Comparing `hspylib-askai-1.0.4/askai/core/support/text_formatter.py` & `hspylib-askai-1.0.5/askai/core/support/text_formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import os
+import re
+from textwrap import dedent
+from typing import Any
+
 from hspylib.core.metaclass.singleton import Singleton
-from hspylib.core.tools.dict_tools import get_or_default
+from hspylib.core.tools.text_tools import ensure_endswith, ensure_startswith
 from hspylib.modules.cli.vt100.vt_code import VtCode
 from hspylib.modules.cli.vt100.vt_color import VtColor
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.text import Text
-from textwrap import dedent
-from typing import Any
-
-import re
 
 
 class TextFormatter(metaclass=Singleton):
     """TODO"""
 
     INSTANCE: "TextFormatter" = None
 
@@ -20,16 +21,22 @@
         "": "\n%RED%  Error: ",
         "": "\n>   *TIP:* ",
         "": "\n>   *Analysis:* ",
         "": "\n>   *Summary:* ",
         "": "\n>   *Joke:* ",
         "": "\n>   *Fun-Fact:* ",
         "": "\n>   *Advice:* ",
+        "﬽": "\n> ﬽  *Conclusion:* ",
     }
 
+    @staticmethod
+    def ensure_ln(text: str) -> str:
+        """TODO"""
+        return ensure_endswith(ensure_startswith(text.strip(), os.linesep), os.linesep * 2)
+
     def __init__(self):
         self._console: Console = Console()
 
     @property
     def console(self) -> Console:
         return self._console
 
@@ -40,31 +47,33 @@
         # fmt: off
         re_url = (
             r"(https?:\/\/(?:www\.|(?!www))[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s')]{2,}|"
             r"www\.[a-zA-Z0-9][a-zA-Z0-9-]+[a-zA-Z0-9]\.[^\s')]{2,}|https?:\/\/(?:www\.|(?!www))"
             r"[a-zA-Z0-9]+\.[^\s')]{2,}|www\.[a-zA-Z0-9]+\.[^\s')]{2,})"
         )
         text = dedent(str(text))
-        text = re.sub(r"Errors?[-:\s]\s+", self.CHAT_ICONS[''], text)
-        text = re.sub(r"[Hh]ints?( (and|&) [Tt]ips)?[-:\s]\s+", self.CHAT_ICONS[''], text)
-        text = re.sub(r"[Aa]nalysis[-:\s]\s+", self.CHAT_ICONS[''], text)
-        text = re.sub(r"[Ss]ummary[-:\s]\s+", self.CHAT_ICONS[''], text)
-        text = re.sub(r"[Ff]un [Ff]acts?[-:\s]\s+", self.CHAT_ICONS[''], text)
-        text = re.sub(r"([Jj]oke( [Tt]ime)?)[-:\s]\s+", self.CHAT_ICONS[''], text)
-        text = re.sub(r"[Aa]dvice[-:\s]\s+", self.CHAT_ICONS[''], text)
-        fg = get_or_default(re.findall(r"%\w+%", text), 0, '%NC%')
+        text = re.sub(r"\**Errors?[-:\s][\s*]+", self.CHAT_ICONS[''], text)
+        text = re.sub(r"\**[Hh]ints?( (and|&) [Tt]ips)?[-:\s][\s*]+", self.CHAT_ICONS[''], text)
+        text = re.sub(r"\**[Aa]nalysis[-:\s][\s*]+", self.CHAT_ICONS[''], text)
+        text = re.sub(r"\**[Ss]ummary[-:\s][\s*]+", self.CHAT_ICONS[''], text)
+        text = re.sub(r"\**[Ff]un [Ff]acts?[-:\s][\s*]+", self.CHAT_ICONS[''], text)
+        text = re.sub(r"\**([Jj]oke( [Tt]ime)?)[-:\s][\s*]+", self.CHAT_ICONS[''], text)
+        text = re.sub(r"\**[Aa]dvice[-:\s][\s*]+", self.CHAT_ICONS[''], text)
+        text = re.sub(r"\**[Cc]onclusion[-:\s][\s*]+", self.CHAT_ICONS['﬽'], text)
         text = re.sub(re_url, r' [\1](\1)', text)
         text = re.sub(r'(`{3}.+`{3})', r'\n\1\n', text)
         # fmt: on
 
         return text.strip()
 
     def display_markdown(self, text: str) -> None:
+        """TODO"""
         colorized: str = VtColor.colorize(VtCode.decode(self.beautify(text)))
         self.console.print(Markdown(colorized))
 
     def display_text(self, text: str) -> None:
+        """TODO"""
         colorized: str = VtColor.colorize(VtCode.decode(self.beautify(text)))
         self.console.print(Text.from_ansi(colorized))
 
 
 assert (text_formatter := TextFormatter().INSTANCE) is not None
```

### Comparing `hspylib-askai-1.0.4/askai/core/support/utilities.py` & `hspylib-askai-1.0.5/askai/core/support/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,41 @@
    @created: Wed, 10 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright·(c)·2024,·HSPyLib
 """
+import hashlib
+import mimetypes
+import os
+import re
+import sys
+from os.path import basename, dirname
+from pathlib import Path
+from typing import Any, Optional, Tuple
 
-from askai.core.support.presets import Presets
-from askai.core.support.text_formatter import text_formatter
-from askai.language.language import Language
+import pause
 from clitt.core.term.cursor import Cursor
 from hspylib.core.enums.charset import Charset
 from hspylib.core.preconditions import check_argument
 from hspylib.core.tools.commons import file_is_not_empty, sysout
 from hspylib.core.tools.text_tools import ensure_endswith
 from hspylib.modules.cli.vt100.vt_color import VtColor
-from os.path import basename, dirname
-from pathlib import Path
-from typing import Any, Optional, Tuple
 
-import hashlib
-import os
-import pause
-import re
+from askai.core.support.presets import Presets
+from askai.core.support.text_formatter import text_formatter
+from askai.language.language import Language
+
+
+def read_stdin() -> Optional[str]:
+    """TODO"""
+    if not sys.stdin.isatty():
+        return sys.stdin.read()
+    return None
 
 
 def display_text(text: Any, prefix: Any = "", markdown: bool = True, erase_last=False) -> None:
     """Display the provided text ina proper way.
     :param text: The text to be displayed.
     :param prefix: the text prefix.
     :param markdown: Whether to enable markdown rendering.
@@ -157,7 +166,20 @@
     # Match a terminal command formatted in a markdown code block.
     re_command = r"^`{3}((\w+)\s*)?(.+)\s*?`{3}$"
     if markdown_text and (mat := re.search(re_command, markdown_text.replace("\n", " ").strip(), flags)):
         if mat and len(mat.groups()) == 3:
             shell, cmd = mat.group(1) or "", mat.group(3) or ""
             return shell.strip(), cmd.strip()
     return None
+
+
+def media_type_of(pathname: str) -> Optional[tuple[str, ...]] | None:
+    """Return the file media type, or none is guessing was not possible.
+    :param pathname: The file path to check.
+    """
+    mimetypes.init()
+    mtype, _ = mimetypes.guess_type(basename(pathname))
+
+    if mtype is not None:
+        return tuple(mtype.split('/'))
+
+    return None
```

### Comparing `hspylib-askai-1.0.4/askai/exception/exceptions.py` & `hspylib-askai-1.0.5/askai/exception/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -50,7 +50,28 @@
 
 class InvalidInputDevice(HSBaseException):
     """Raised when an invalid recording input device is used."""
 
 
 class DocumentsNotFound(HSBaseException):
     """Raised when no documents are found for summarization."""
+
+
+class InaccurateResponse(HSBaseException):
+    """Raised when detected an inaccurate response form the AI."""
+
+
+class MaxInteractionsReached(HSBaseException):
+    """Raised when the number of executed actions exceeded the limit."""
+
+
+class ImpossibleQuery(HSBaseException):
+    """Raised when tracing or executing an action plan is/was not possible."""
+
+
+class UnintelligibleQuery(HSBaseException):
+    """Raised when received an intelligible question."""
+
+
+class TerminatingQuery(HSBaseException):
+    """Raised when received a terminating question."""
+
```

### Comparing `hspylib-askai-1.0.4/askai/language/argos_translator.py` & `hspylib-askai-1.0.5/askai/language/argos_translator.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/askai/language/language.py` & `hspylib-askai-1.0.5/askai/language/language.py`

 * *Files identical despite different names*

### Comparing `hspylib-askai-1.0.4/hspylib_askai.egg-info/PKG-INFO` & `hspylib-askai-1.0.5/hspylib_askai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-askai
-Version: 1.0.4
+Version: 1.0.5
 Summary: HomeSetup - AskAI
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-askai/
@@ -20,21 +20,21 @@
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Terminals
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: hspylib>=1.12.35
-Requires-Dist: hspylib-clitt>=0.9.117
-Requires-Dist: retry==0.9.2
+Requires-Dist: hspylib-clitt>=0.9.119
+Requires-Dist: retry2==0.9.5
 Requires-Dist: pause==0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: argostranslate==1.9.1
 Requires-Dist: protobuf==4.22.1
-Requires-Dist: torch==2.1.2
+Requires-Dist: torch==2.2.0
 Requires-Dist: stanza==1.1.1
 Requires-Dist: soundfile==0.12.1
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: langchain>=0.1.12
 Requires-Dist: langchain-openai==0.0.8
 Requires-Dist: langchain-community==0.0.28
 Requires-Dist: unstructured==0.12.4
@@ -50,24 +50,25 @@
 Requires-Dist: openai==1.14.1
 Requires-Dist: chromadb==0.4.24
 Requires-Dist: opentelemetry-api==1.22.0
 Requires-Dist: opentelemetry-sdk==1.22.0
 Requires-Dist: opentelemetry-proto==1.22.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: pytz==2024.1
+Requires-Dist: schedule==1.2.1
 
 <img src="https://iili.io/JEatihb.png" width="64" height="64" align="right" />
 
 # AskAI
 >
 > Unleash the Power of AI in Your Terminal
 
 [![Terminal](https://badgen.net/badge/icon/terminal?icon=terminal&label)](https://github.com/yorevs/homesetup)
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v1.0.4/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v1.0.5/gray)](docs/CHANGELOG.md#unreleased)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 [![build-and-test](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml)
 
 <img src="https://iili.io/JGv7BTP.png)" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
```

### Comparing `hspylib-askai-1.0.4/hspylib_askai.egg-info/SOURCES.txt` & `hspylib-askai-1.0.5/hspylib_askai.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -22,35 +22,33 @@
 askai/core/engine/__init__.py
 askai/core/engine/ai_engine.py
 askai/core/engine/engine_factory.py
 askai/core/engine/openai/__init__.py
 askai/core/engine/openai/openai_configs.py
 askai/core/engine/openai/openai_engine.py
 askai/core/engine/openai/openai_model.py
-askai/core/engine/openai/temperatures.py
+askai/core/engine/openai/temperature.py
+askai/core/features/__init__.py
+askai/core/features/actions.py
+askai/core/features/router.py
+askai/core/features/tools/__init__.py
+askai/core/features/tools/analysis.py
+askai/core/features/tools/browser.py
+askai/core/features/tools/general.py
+askai/core/features/tools/summarization.py
+askai/core/features/tools/terminal.py
 askai/core/model/__init__.py
 askai/core/model/ai_model.py
 askai/core/model/ai_reply.py
 askai/core/model/chat_context.py
-askai/core/model/processor_response.py
 askai/core/model/query_type.py
+askai/core/model/rag_response.py
 askai/core/model/search_result.py
 askai/core/model/summary_result.py
 askai/core/model/terminal_command.py
-askai/core/processor/__init__.py
-askai/core/processor/processor_base.py
-askai/core/processor/processor_factory.py
-askai/core/processor/processor_proxy.py
-askai/core/processor/instances/__init__.py
-askai/core/processor/instances/analysis_processor.py
-askai/core/processor/instances/command_processor.py
-askai/core/processor/instances/generic_processor.py
-askai/core/processor/instances/internet_processor.py
-askai/core/processor/instances/output_processor.py
-askai/core/processor/instances/summary_processor.py
 askai/core/support/__init__.py
 askai/core/support/langchain_support.py
 askai/core/support/object_mapper.py
 askai/core/support/presets.py
 askai/core/support/settings.py
 askai/core/support/shared_instances.py
 askai/core/support/text_formatter.py
```

### Comparing `hspylib-askai-1.0.4/setup.py` & `hspylib-askai-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # The package requirements
 REQUIREMENTS = list(filter(None, (HERE / "requirements.txt").read_text().splitlines()))
 
 # This call to setup() does all the work
 setuptools.setup(
     name="hspylib-askai",
-    version="1.0.4",
+    version="1.0.5",
     description="HomeSetup - AskAI",
     author="Hugo Saporetti Junior",
     author_email="yorevs@hotmail.com",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/yorevs/hspylib",
     project_urls={"GitHub": "https://github.com/yorevs/hspylib", "PyPi": "https://pypi.org/project/hspylib-askai/"},
```

