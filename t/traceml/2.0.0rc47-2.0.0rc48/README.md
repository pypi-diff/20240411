# Comparing `tmp/traceml-2.0.0rc47.tar.gz` & `tmp/traceml-2.0.0rc48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceml-2.0.0rc47.tar", last modified: Mon Sep 25 12:30:55 2023, max compression
+gzip compressed data, was "traceml-2.0.0rc48.tar", last modified: Mon Sep 25 21:18:16 2023, max compression
```

## Comparing `traceml-2.0.0rc47.tar` & `traceml-2.0.0rc48.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2023-09-25 12:30:55.659431 traceml-2.0.0rc47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.647431 traceml-2.0.0rc47/traceml/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.647431 traceml-2.0.0rc47/traceml/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/artifacts/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/artifacts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.651431 traceml-2.0.0rc47/traceml/events/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/events/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    15262 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.651431 traceml-2.0.0rc47/traceml/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/fastai.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/fastai_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/ignite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/pytorch_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/scikit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/integrations/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.651431 traceml-2.0.0rc47/traceml/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/logging/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/logging/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/logging/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/logging/streamer.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.651431 traceml-2.0.0rc47/traceml/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/df_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.651431 traceml-2.0.0rc47/traceml/processors/events_processors/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/events_artifacts_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/events_audio_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/events_charts_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/events_image_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/events_metrics_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/events_models_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/events_tables_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/events_processors/events_video_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/gpu_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/importance_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/logs_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/processors/psutil_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/traceml/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/serialization/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/serialization/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/traceml/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/summary/df.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/traceml/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)    28289 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62553 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/tracking/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/traceml/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/traceml/vendor/matplotlylib/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/_py3k_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.655431 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12040 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20688 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/mpltools.py
--rw-r--r--   0 runner    (1001) docker     (127)    35762 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/matplotlylib/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)   166500 2023-09-25 12:30:45.000000 traceml-2.0.0rc47/traceml/vendor/pynvml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 12:30:55.647431 traceml-2.0.0rc47/traceml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-09-25 12:30:55.000000 traceml-2.0.0rc47/traceml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2023-09-25 12:30:55.000000 traceml-2.0.0rc47/traceml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 12:30:55.000000 traceml-2.0.0rc47/traceml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-09-25 12:30:55.000000 traceml-2.0.0rc47/traceml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-25 12:30:55.000000 traceml-2.0.0rc47/traceml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.036739 traceml-2.0.0rc48/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-09-25 21:18:16.036739 traceml-2.0.0rc48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2023-09-25 21:18:16.040739 traceml-2.0.0rc48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.028739 traceml-2.0.0rc48/traceml/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.028739 traceml-2.0.0rc48/traceml/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/artifacts/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/artifacts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.028739 traceml-2.0.0rc48/traceml/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/events/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.032739 traceml-2.0.0rc48/traceml/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/fastai_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/ignite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/pytorch_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/scikit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/integrations/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.032739 traceml-2.0.0rc48/traceml/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/logging/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/logging/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/logging/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/logging/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.032739 traceml-2.0.0rc48/traceml/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/df_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.032739 traceml-2.0.0rc48/traceml/processors/events_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/events_artifacts_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/events_audio_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/events_charts_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/events_image_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/events_metrics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/events_models_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/events_tables_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/events_processors/events_video_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/gpu_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/importance_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/logs_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/processors/psutil_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.032739 traceml-2.0.0rc48/traceml/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/serialization/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/serialization/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.032739 traceml-2.0.0rc48/traceml/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/summary/df.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.032739 traceml-2.0.0rc48/traceml/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)    28289 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62553 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/tracking/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.036739 traceml-2.0.0rc48/traceml/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.036739 traceml-2.0.0rc48/traceml/vendor/matplotlylib/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.036739 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/_py3k_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.036739 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20688 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/mpltools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35762 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/matplotlylib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166500 2023-09-25 21:18:04.000000 traceml-2.0.0rc48/traceml/vendor/pynvml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 21:18:16.028739 traceml-2.0.0rc48/traceml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-09-25 21:18:15.000000 traceml-2.0.0rc48/traceml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2023-09-25 21:18:15.000000 traceml-2.0.0rc48/traceml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 21:18:15.000000 traceml-2.0.0rc48/traceml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-09-25 21:18:15.000000 traceml-2.0.0rc48/traceml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-25 21:18:15.000000 traceml-2.0.0rc48/traceml.egg-info/top_level.txt
```

### Comparing `traceml-2.0.0rc47/PKG-INFO` & `traceml-2.0.0rc48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceml
-Version: 2.0.0rc47
+Version: 2.0.0rc48
 Summary: Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon.
 Home-page: https://github.com/polyaxon/traceml
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

### Comparing `traceml-2.0.0rc47/setup.cfg` & `traceml-2.0.0rc48/setup.cfg`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/setup.py` & `traceml-2.0.0rc48/setup.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/artifacts/enums.py` & `traceml-2.0.0rc48/traceml/artifacts/enums.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/artifacts/schemas.py` & `traceml-2.0.0rc48/traceml/artifacts/schemas.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/events/paths.py` & `traceml-2.0.0rc48/traceml/events/paths.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/events/schemas.py` & `traceml-2.0.0rc48/traceml/events/schemas.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/fastai.py` & `traceml-2.0.0rc48/traceml/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/fastai_v1.py` & `traceml-2.0.0rc48/traceml/integrations/fastai_v1.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/hugging_face.py` & `traceml-2.0.0rc48/traceml/integrations/hugging_face.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/keras.py` & `traceml-2.0.0rc48/traceml/integrations/keras.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/pytorch_lightning.py` & `traceml-2.0.0rc48/traceml/integrations/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/scikit.py` & `traceml-2.0.0rc48/traceml/integrations/scikit.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/tensorboard.py` & `traceml-2.0.0rc48/traceml/integrations/tensorboard.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/tensorflow.py` & `traceml-2.0.0rc48/traceml/integrations/tensorflow.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/integrations/xgboost.py` & `traceml-2.0.0rc48/traceml/integrations/xgboost.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/logging/handler.py` & `traceml-2.0.0rc48/traceml/logging/handler.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/logging/parser.py` & `traceml-2.0.0rc48/traceml/logging/parser.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/logging/schemas.py` & `traceml-2.0.0rc48/traceml/logging/schemas.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/logging/streamer.py` & `traceml-2.0.0rc48/traceml/logging/streamer.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/df_processors.py` & `traceml-2.0.0rc48/traceml/processors/df_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/errors.py` & `traceml-2.0.0rc48/traceml/processors/errors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/events_processors/__init__.py` & `traceml-2.0.0rc48/traceml/processors/events_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/events_processors/events_audio_processors.py` & `traceml-2.0.0rc48/traceml/processors/events_processors/events_audio_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/events_processors/events_charts_processors.py` & `traceml-2.0.0rc48/traceml/processors/events_processors/events_charts_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/events_processors/events_image_processors.py` & `traceml-2.0.0rc48/traceml/processors/events_processors/events_image_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/events_processors/events_metrics_processors.py` & `traceml-2.0.0rc48/traceml/processors/events_processors/events_metrics_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/events_processors/events_models_processors.py` & `traceml-2.0.0rc48/traceml/processors/events_processors/events_models_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/events_processors/events_video_processors.py` & `traceml-2.0.0rc48/traceml/processors/events_processors/events_video_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/gpu_processor.py` & `traceml-2.0.0rc48/traceml/processors/gpu_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/importance_processors.py` & `traceml-2.0.0rc48/traceml/processors/importance_processors.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/logs_processor.py` & `traceml-2.0.0rc48/traceml/processors/logs_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/processors/psutil_processor.py` & `traceml-2.0.0rc48/traceml/processors/psutil_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/serialization/base.py` & `traceml-2.0.0rc48/traceml/serialization/base.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/serialization/writer.py` & `traceml-2.0.0rc48/traceml/serialization/writer.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/summary/df.py` & `traceml-2.0.0rc48/traceml/summary/df.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/tracking/__init__.py` & `traceml-2.0.0rc48/traceml/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/tracking/run.py` & `traceml-2.0.0rc48/traceml/tracking/run.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/exporter.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/exporter.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/base.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/base.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/tools.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/tools.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/mplexporter/utils.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/mplexporter/utils.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/mpltools.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/mpltools.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/renderer.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/matplotlylib/tools.py` & `traceml-2.0.0rc48/traceml/vendor/matplotlylib/tools.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml/vendor/pynvml.py` & `traceml-2.0.0rc48/traceml/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `traceml-2.0.0rc47/traceml.egg-info/PKG-INFO` & `traceml-2.0.0rc48/traceml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceml
-Version: 2.0.0rc47
+Version: 2.0.0rc48
 Summary: Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon.
 Home-page: https://github.com/polyaxon/traceml
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

### Comparing `traceml-2.0.0rc47/traceml.egg-info/SOURCES.txt` & `traceml-2.0.0rc48/traceml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

