# Comparing `tmp/autogluon.timeseries-1.1.0b20240409.tar.gz` & `tmp/autogluon.timeseries-1.1.0b20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.1.0b20240409.tar", last modified: Tue Apr  9 09:06:08 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.1.0b20240410.tar", last modified: Wed Apr 10 09:06:44 2024, max compression
```

## Comparing `autogluon.timeseries-1.1.0b20240409.tar` & `autogluon.timeseries-1.1.0b20240410.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.545612 autogluon.timeseries-1.1.0b20240409/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.545612 autogluon.timeseries-1.1.0b20240409/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30977 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.553612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    81222 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.557612 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-09 09:04:42.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:06:08.549612 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11850 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:06:08.000000 autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.055498 autogluon.timeseries-1.1.0b20240410/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.055498 autogluon.timeseries-1.1.0b20240410/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.059497 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.059497 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.059497 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32111 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81222 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 09:06:43.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.059497 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.1.0b20240409/PKG-INFO` & `autogluon.timeseries-1.1.0b20240410/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240409
-Summary: AutoML for Image, Text, and Tabular Data
+Version: 1.1.0b20240410
+Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
 Project-URL: Contribute!, https://github.com/autogluon/autogluon/blob/master/CONTRIBUTING.md
 Description: 
         
         <div align="center">
         <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
         
-        ## AutoML for Image, Text, Time Series, and Tabular Data
+        ## Fast and Accurate ML in 3 Lines of Code
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Conda Forge](https://img.shields.io/conda/vn/conda-forge/autogluon.svg)](https://anaconda.org/conda-forge/autogluon)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/autogluon/)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Discord](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
```

### Comparing `autogluon.timeseries-1.1.0b20240409/setup.py` & `autogluon.timeseries-1.1.0b20240410/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,14 +170,29 @@
         """Apply a mask that mimics the situation at prediction time when target/covariates are unknown during the
         forecast horizon.
 
         This method is overridden by DirectTabularModel.
         """
         return df
 
+    def _add_scale_as_static_feature(self, data: TimeSeriesDataFrame) -> TimeSeriesDataFrame:
+        """Add mean/std of the target column for each series as a static feature."""
+        data = data.copy(deep=False)
+        scale_features = (
+            data[self.target]
+            .groupby(ITEMID, sort=False)
+            .agg(["mean", "std"])
+            .rename(columns={"mean": "__target_mean", "std": "__target_scale"})
+        )
+        if data.static_features is None:
+            data.static_features = scale_features
+        else:
+            data.static_features = pd.concat([data.static_features, scale_features], axis=1)
+        return data
+
     @staticmethod
     def _shorten_all_series(mlforecast_df: pd.DataFrame, max_length: int):
         logger.debug(f"Shortening all series to at most {max_length}")
         return mlforecast_df.groupby(MLF_ITEMID, as_index=False, sort=False).tail(max_length)
 
     def _generate_train_val_dfs(
         self, data: TimeSeriesDataFrame, max_num_items: Optional[int] = None, max_num_samples: Optional[int] = None
@@ -248,27 +263,34 @@
             selected_columns += [self.target]
             column_name_mapping[self.target] = MLF_TARGET
 
         df = pd.DataFrame(data)[selected_columns].reset_index()
         if static_features is not None:
             df = pd.merge(df, static_features, how="left", on=ITEMID, suffixes=(None, "_static_feat"))
 
+        for col in self.metadata.known_covariates_real:
+            # Normalize non-boolean features using mean_abs scaling
+            if not df[col].isin([0, 1]).all():
+                df[f"__scaled_{col}"] = df[col] / df[col].abs().groupby(df[ITEMID]).mean().reindex(df[ITEMID]).values
+
         # We assume that df is sorted by 'unique_id' inside `TimeSeriesPredictor._check_and_prepare_data_frame`
         return df.rename(columns=column_name_mapping)
 
     def _fit(
         self,
         train_data: TimeSeriesDataFrame,
         val_data: Optional[TimeSeriesDataFrame] = None,
         time_limit: Optional[int] = None,
         verbosity: int = 2,
         **kwargs,
     ) -> None:
         from mlforecast import MLForecast
 
+        train_data = self._add_scale_as_static_feature(train_data)
+
         self._check_fit_params()
         fit_start_time = time.time()
         self._train_target_median = train_data[self.target].median()
         # TabularEstimator is passed to MLForecast later to include tuning_data
         model_params = self._get_model_params()
 
         mlforecast_init_args = self._get_mlforecast_init_args(train_data, model_params)
@@ -459,14 +481,15 @@
 
     def _predict(
         self,
         data: TimeSeriesDataFrame,
         known_covariates: Optional[TimeSeriesDataFrame] = None,
         **kwargs,
     ) -> TimeSeriesDataFrame:
+        data = self._add_scale_as_static_feature(data)
         original_item_id_order = data.item_ids
         data, known_covariates, forecast_for_short_series = self._remove_short_ts_and_generate_fallback_forecast(
             data=data, known_covariates=known_covariates
         )
         if len(data) == 0:
             # All time series are too short for chosen differences
             return forecast_for_short_series
@@ -475,15 +498,15 @@
             data_future = known_covariates.copy()
         else:
             future_index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length)
             data_future = pd.DataFrame(columns=[self.target], index=future_index, dtype="float32")
         # MLForecast raises exception of target contains NaN. We use inf as placeholder, replace them by NaN afterwards
         data_future[self.target] = float("inf")
         data_extended = pd.concat([data, data_future])
-        mlforecast_df = self._to_mlforecast_df(data_extended, data.static_features)
+        mlforecast_df = self._to_mlforecast_df(data_extended, data_extended.static_features)
         if self._max_ts_length is not None:
             # We appended `prediction_length` time steps to each series, so increase length
             mlforecast_df = self._shorten_all_series(mlforecast_df, self._max_ts_length + self.prediction_length)
         df = self._mlf.preprocess(mlforecast_df, dropna=False, static_features=[])
         df = df.groupby(MLF_ITEMID, sort=False).tail(self.prediction_length)
         df = df.replace(float("inf"), float("nan"))
 
@@ -590,14 +613,15 @@
 
     def _predict(
         self,
         data: TimeSeriesDataFrame,
         known_covariates: Optional[TimeSeriesDataFrame] = None,
         **kwargs,
     ) -> TimeSeriesDataFrame:
+        data = self._add_scale_as_static_feature(data)
         original_item_id_order = data.item_ids
         data, known_covariates, forecast_for_short_series = self._remove_short_ts_and_generate_fallback_forecast(
             data=data, known_covariates=known_covariates
         )
         if len(data) == 0:
             # All time series are too short for chosen differences
             return forecast_for_short_series
```

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/chronos/utils.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,26 +181,25 @@
             val_data, store_val_score, store_predict_time, time_limit=self.time_limit, **predict_kwargs
         )
 
     def _predict_wrapper(self, time_series: pd.Series, end_time: Optional[float] = None) -> Tuple[pd.DataFrame, bool]:
         if end_time is not None and time.time() >= end_time:
             raise TimeLimitExceeded
 
+        model_failed = False
         if time_series.isna().all():
             result = self._dummy_forecast.copy()
-            model_failed = True
         else:
             try:
                 result = self._predict_with_local_model(
                     time_series=time_series,
                     local_model_args=self._local_model_args.copy(),
                 )
                 if not np.isfinite(result.values).all():
                     raise RuntimeError("Forecast contains NaN or Inf values.")
-                model_failed = False
             except Exception:
                 if self.use_fallback_model:
                     result = seasonal_naive_forecast(
                         target=time_series.values.ravel(),
                         prediction_length=self.prediction_length,
                         quantile_levels=self.quantile_levels,
                         seasonal_period=self._seasonal_period,
```

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240409
-Summary: AutoML for Image, Text, and Tabular Data
+Version: 1.1.0b20240410
+Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
 Project-URL: Contribute!, https://github.com/autogluon/autogluon/blob/master/CONTRIBUTING.md
 Description: 
         
         <div align="center">
         <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
         
-        ## AutoML for Image, Text, Time Series, and Tabular Data
+        ## Fast and Accurate ML in 3 Lines of Code
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Conda Forge](https://img.shields.io/conda/vn/conda-forge/autogluon.svg)](https://anaconda.org/conda-forge/autogluon)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/autogluon/)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Discord](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
```

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240409/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.1.0b20240409
-autogluon.common==1.1.0b20240409
-autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240409
+autogluon.core[raytune]==1.1.0b20240410
+autogluon.common==1.1.0b20240410
+autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240410
 
 [all]
 optimum[onnxruntime]<1.19,>=1.17
 
 [chronos-onnx]
 optimum[onnxruntime]<1.19,>=1.17
```

