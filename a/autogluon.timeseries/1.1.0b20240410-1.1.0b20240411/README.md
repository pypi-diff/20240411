# Comparing `tmp/autogluon.timeseries-1.1.0b20240410.tar.gz` & `tmp/autogluon.timeseries-1.1.0b20240411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.1.0b20240410.tar", last modified: Wed Apr 10 09:06:44 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.1.0b20240411.tar", last modified: Thu Apr 11 09:05:01 2024, max compression
```

## Comparing `autogluon.timeseries-1.1.0b20240410.tar` & `autogluon.timeseries-1.1.0b20240411.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.055498 autogluon.timeseries-1.1.0b20240410/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.055498 autogluon.timeseries-1.1.0b20240410/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.059497 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.059497 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.059497 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45567 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32111 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.063498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    81222 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.067498 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-10 09:05:21.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 09:06:43.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:44.059497 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:44.000000 autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.210771 autogluon.timeseries-1.1.0b20240411/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.210771 autogluon.timeseries-1.1.0b20240411/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.214771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.214771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.214771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45593 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31299 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34031 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19930 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.218771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81222 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.222771 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19261 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-11 09:03:38.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:05:01.214771 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:05:01.000000 autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.1.0b20240410/PKG-INFO` & `autogluon.timeseries-1.1.0b20240411/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240410
+Version: 1.1.0b20240411
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.0b20240410/setup.py` & `autogluon.timeseries-1.1.0b20240411/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -755,27 +755,27 @@
                 2019-01-07     2.0
         1       2019-02-04     3.0
                 2019-02-05     3.0
                 2019-02-06     3.0
                 2019-02-07     4.0
 
         """
-        if self.freq is None:
-            raise ValueError(
-                "Please make sure that all time series have a regular index before calling `fill_missing_values`"
-                "(for example, using the `convert_frequency` method)."
-            )
-
         # Convert to pd.DataFrame for faster processing
         df = pd.DataFrame(self)
 
         # Skip filling if there are no NaNs
         if not df.isna().any(axis=None):
             return self
 
+        if not self.index.is_monotonic_increasing:
+            logger.warning(
+                "Trying to fill missing values in an unsorted dataframe. "
+                "It is highly recommended to call `ts_df.sort_index()` before calling `ts_df.fill_missing_values()`"
+            )
+
         grouped_df = df.groupby(level=ITEMID, sort=False, group_keys=False)
         if method == "auto":
             filled_df = grouped_df.ffill()
             # If necessary, fill missing values at the start of each time series with bfill
             if filled_df.isna().any(axis=None):
                 filled_df = filled_df.groupby(level=ITEMID, sort=False, group_keys=False).bfill()
         elif method in ["ffill", "pad"]:
```

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
         self.trainer_type = trainer_type
         self.target = target
         self.known_covariates_names = [] if known_covariates_names is None else known_covariates_names
         self.prediction_length = prediction_length
         self.quantile_levels = kwargs.get("quantile_levels", [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9])
         self.cache_predictions = cache_predictions
+        self.freq: Optional[str] = None
 
         self.feature_generator = TimeSeriesFeatureGenerator(
             target=self.target, known_covariates_names=self.known_covariates_names
         )
 
     def load_trainer(self) -> AbstractTimeSeriesTrainer:
         """Return the trainer object corresponding to the learner."""
@@ -83,14 +84,16 @@
         self._time_limit = time_limit
         time_start = time.time()
 
         train_data = self.feature_generator.fit_transform(train_data, data_frame_name="train_data")
         if val_data is not None:
             val_data = self.feature_generator.transform(val_data, data_frame_name="tuning_data")
 
+        self.freq = train_data.freq
+
         trainer_init_kwargs = kwargs.copy()
         trainer_init_kwargs.update(
             dict(
                 path=self.model_context,
                 prediction_length=self.prediction_length,
                 eval_metric=self.eval_metric,
                 eval_metric_seasonal_period=self.eval_metric_seasonal_period,
@@ -151,15 +154,17 @@
 
         missing_item_ids = data.item_ids.difference(known_covariates.item_ids)
         if len(missing_item_ids) > 0:
             raise ValueError(
                 f"known_covariates are missing information for the following item_ids: {reprlib.repr(missing_item_ids.to_list())}."
             )
 
-        forecast_index = get_forecast_horizon_index_ts_dataframe(data, prediction_length=self.prediction_length)
+        forecast_index = get_forecast_horizon_index_ts_dataframe(
+            data, prediction_length=self.prediction_length, freq=self.freq
+        )
         try:
             known_covariates = known_covariates.loc[forecast_index]
         except KeyError:
             raise ValueError(
                 f"known_covariates should include the values for prediction_length={self.prediction_length} "
                 "many time steps into the future."
             )
```

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,29 +170,14 @@
         """Apply a mask that mimics the situation at prediction time when target/covariates are unknown during the
         forecast horizon.
 
         This method is overridden by DirectTabularModel.
         """
         return df
 
-    def _add_scale_as_static_feature(self, data: TimeSeriesDataFrame) -> TimeSeriesDataFrame:
-        """Add mean/std of the target column for each series as a static feature."""
-        data = data.copy(deep=False)
-        scale_features = (
-            data[self.target]
-            .groupby(ITEMID, sort=False)
-            .agg(["mean", "std"])
-            .rename(columns={"mean": "__target_mean", "std": "__target_scale"})
-        )
-        if data.static_features is None:
-            data.static_features = scale_features
-        else:
-            data.static_features = pd.concat([data.static_features, scale_features], axis=1)
-        return data
-
     @staticmethod
     def _shorten_all_series(mlforecast_df: pd.DataFrame, max_length: int):
         logger.debug(f"Shortening all series to at most {max_length}")
         return mlforecast_df.groupby(MLF_ITEMID, as_index=False, sort=False).tail(max_length)
 
     def _generate_train_val_dfs(
         self, data: TimeSeriesDataFrame, max_num_items: Optional[int] = None, max_num_samples: Optional[int] = None
@@ -281,16 +266,14 @@
         val_data: Optional[TimeSeriesDataFrame] = None,
         time_limit: Optional[int] = None,
         verbosity: int = 2,
         **kwargs,
     ) -> None:
         from mlforecast import MLForecast
 
-        train_data = self._add_scale_as_static_feature(train_data)
-
         self._check_fit_params()
         fit_start_time = time.time()
         self._train_target_median = train_data[self.target].median()
         # TabularEstimator is passed to MLForecast later to include tuning_data
         model_params = self._get_model_params()
 
         mlforecast_init_args = self._get_mlforecast_init_args(train_data, model_params)
@@ -481,32 +464,31 @@
 
     def _predict(
         self,
         data: TimeSeriesDataFrame,
         known_covariates: Optional[TimeSeriesDataFrame] = None,
         **kwargs,
     ) -> TimeSeriesDataFrame:
-        data = self._add_scale_as_static_feature(data)
         original_item_id_order = data.item_ids
         data, known_covariates, forecast_for_short_series = self._remove_short_ts_and_generate_fallback_forecast(
             data=data, known_covariates=known_covariates
         )
         if len(data) == 0:
             # All time series are too short for chosen differences
             return forecast_for_short_series
 
         if known_covariates is not None:
             data_future = known_covariates.copy()
         else:
-            future_index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length)
+            future_index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length, freq=self.freq)
             data_future = pd.DataFrame(columns=[self.target], index=future_index, dtype="float32")
         # MLForecast raises exception of target contains NaN. We use inf as placeholder, replace them by NaN afterwards
         data_future[self.target] = float("inf")
         data_extended = pd.concat([data, data_future])
-        mlforecast_df = self._to_mlforecast_df(data_extended, data_extended.static_features)
+        mlforecast_df = self._to_mlforecast_df(data_extended, data.static_features)
         if self._max_ts_length is not None:
             # We appended `prediction_length` time steps to each series, so increase length
             mlforecast_df = self._shorten_all_series(mlforecast_df, self._max_ts_length + self.prediction_length)
         df = self._mlf.preprocess(mlforecast_df, dropna=False, static_features=[])
         df = df.groupby(MLF_ITEMID, sort=False).tail(self.prediction_length)
         df = df.replace(float("inf"), float("nan"))
 
@@ -613,28 +595,27 @@
 
     def _predict(
         self,
         data: TimeSeriesDataFrame,
         known_covariates: Optional[TimeSeriesDataFrame] = None,
         **kwargs,
     ) -> TimeSeriesDataFrame:
-        data = self._add_scale_as_static_feature(data)
         original_item_id_order = data.item_ids
         data, known_covariates, forecast_for_short_series = self._remove_short_ts_and_generate_fallback_forecast(
             data=data, known_covariates=known_covariates
         )
         if len(data) == 0:
             # All time series are too short for chosen differences
             return forecast_for_short_series
 
         new_df = self._to_mlforecast_df(data, data.static_features)
         if self._max_ts_length is not None:
             new_df = self._shorten_all_series(new_df, self._max_ts_length)
         if known_covariates is None:
-            future_index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length)
+            future_index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length, freq=self.freq)
             known_covariates = pd.DataFrame(columns=[self.target], index=future_index, dtype="float32")
         X_df = self._to_mlforecast_df(known_covariates, data.static_features, include_target=False)
         # If both covariates & static features are missing, set X_df = None to avoid exception from MLForecast
         if len(X_df.columns.difference([MLF_ITEMID, MLF_TIMESTAMP])) == 0:
             X_df = None
         with warning_filter():
             raw_predictions = self._mlf.predict(
```

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 
         mean = samples.mean(axis=-1, keepdims=True)
         quantiles = np.quantile(samples, self.quantile_levels, axis=-1).T
 
         df = pd.DataFrame(
             np.concatenate([mean, quantiles], axis=1),
             columns=["mean"] + [str(q) for q in self.quantile_levels],
-            index=get_forecast_horizon_index_ts_dataframe(data, self.prediction_length),
+            index=get_forecast_horizon_index_ts_dataframe(data, self.prediction_length, freq=self.freq),
         )
 
         return TimeSeriesDataFrame(df)
 
     def _more_tags(self) -> Dict:
         return {"allow_nan": True}
```

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/chronos/utils.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/chronos/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,35 +42,35 @@
 
 class SimpleGluonTSDataset(GluonTSDataset):
     """Wrapper for TimeSeriesDataFrame that is compatible with the GluonTS Dataset API."""
 
     def __init__(
         self,
         target_df: TimeSeriesDataFrame,
+        freq: str,
         target_column: str = "target",
         feat_static_cat: Optional[np.ndarray] = None,
         feat_static_real: Optional[np.ndarray] = None,
         feat_dynamic_cat: Optional[np.ndarray] = None,
         feat_dynamic_real: Optional[np.ndarray] = None,
         past_feat_dynamic_cat: Optional[np.ndarray] = None,
         past_feat_dynamic_real: Optional[np.ndarray] = None,
         includes_future: bool = False,
         prediction_length: int = None,
     ):
         assert target_df is not None
-        assert target_df.freq, "Initializing GluonTS data sets without freq is not allowed"
         # Convert TimeSeriesDataFrame to pd.Series for faster processing
         self.target_array = target_df[target_column].to_numpy(np.float32)
         self.feat_static_cat = self._astype(feat_static_cat, dtype=np.int64)
         self.feat_static_real = self._astype(feat_static_real, dtype=np.float32)
         self.feat_dynamic_cat = self._astype(feat_dynamic_cat, dtype=np.int64)
         self.feat_dynamic_real = self._astype(feat_dynamic_real, dtype=np.float32)
         self.past_feat_dynamic_cat = self._astype(past_feat_dynamic_cat, dtype=np.int64)
         self.past_feat_dynamic_real = self._astype(past_feat_dynamic_real, dtype=np.float32)
-        self.freq = self._to_gluonts_freq(target_df.freq)
+        self.freq = self._to_gluonts_freq(freq)
 
         # Necessary to compute indptr for known_covariates at prediction time
         self.includes_future = includes_future
         self.prediction_length = prediction_length
 
         # Replace inefficient groupby ITEMID with indptr that stores start:end of each time series
         item_id_index = target_df.index.get_level_values(ITEMID)
@@ -230,21 +230,14 @@
         return model
 
     def _get_hpo_backend(self):
         return RAY_BACKEND
 
     def _deferred_init_params_aux(self, dataset: TimeSeriesDataFrame) -> None:
         """Update GluonTS specific parameters with information available only at training time."""
-        self.freq = dataset.freq or self.freq
-        if not self.freq:
-            raise ValueError(
-                "Dataset frequency not provided in the dataset, fit arguments or "
-                "during initialization. Please provide a `freq` string to `fit`."
-            )
-
         model_params = self._get_model_params()
         disable_static_features = model_params.get("disable_static_features", False)
         if not disable_static_features:
             self.num_feat_static_cat = len(self.metadata.static_features_cat)
             self.num_feat_static_real = len(self.metadata.static_features_real)
             if self.num_feat_static_cat > 0:
                 feat_static_cat = dataset.static_features[self.metadata.static_features_cat]
@@ -498,14 +491,15 @@
                         [past_feat_dynamic_real, past_feat_dynamic_cat_ohe], axis=1
                     )
             else:
                 past_feat_dynamic_real = None
 
             return SimpleGluonTSDataset(
                 target_df=time_series_df[[self.target]],
+                freq=self.freq,
                 target_column=self.target,
                 feat_static_cat=feat_static_cat,
                 feat_static_real=feat_static_real,
                 feat_dynamic_cat=feat_dynamic_cat,
                 feat_dynamic_real=feat_dynamic_real,
                 past_feat_dynamic_cat=past_feat_dynamic_cat,
                 past_feat_dynamic_real=past_feat_dynamic_real,
@@ -588,15 +582,15 @@
         if self.gts_predictor is None:
             raise ValueError("Please fit the model before predicting.")
 
         with warning_filter(), gluonts.core.settings.let(gluonts.env.env, use_tqdm=False):
             predicted_targets = self._predict_gluonts_forecasts(data, known_covariates=known_covariates, **kwargs)
             df = self._gluonts_forecasts_to_data_frame(
                 predicted_targets,
-                forecast_index=get_forecast_horizon_index_ts_dataframe(data, self.prediction_length),
+                forecast_index=get_forecast_horizon_index_ts_dataframe(data, self.prediction_length, freq=self.freq),
             )
         return df
 
     def _predict_gluonts_forecasts(
         self, data: TimeSeriesDataFrame, known_covariates: Optional[TimeSeriesDataFrame] = None, **kwargs
     ) -> List[Forecast]:
         gts_data = self._to_gluonts_dataset(data, known_covariates=known_covariates)
```

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         if number_failed_models > 0:
             fraction_failed_models = number_failed_models / len(predictions_with_flags)
             logger.warning(
                 f"\tWarning: {self.name} failed for {number_failed_models} time series "
                 f"({fraction_failed_models:.1%}). Fallback model SeasonalNaive was used for these time series."
             )
         predictions_df = pd.concat([pred for pred, _ in predictions_with_flags])
-        predictions_df.index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length)
+        predictions_df.index = get_forecast_horizon_index_ts_dataframe(data, self.prediction_length, freq=self.freq)
         return TimeSeriesDataFrame(predictions_df)
 
     def score_and_cache_oof(
         self,
         val_data: TimeSeriesDataFrame,
         store_val_score: bool = False,
         store_predict_time: bool = False,
```

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/forecast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
 
 
@@ -11,25 +12,29 @@
 ) -> pd.DatetimeIndex:
     """Get timestamps for the next prediction_length many time steps of the time series with given frequency."""
     start_ts = past_timestamps.max() + 1 * pd.tseries.frequencies.to_offset(freq)
     return pd.date_range(start=start_ts, periods=prediction_length, freq=freq, name=TIMESTAMP)
 
 
 def get_forecast_horizon_index_ts_dataframe(
-    ts_dataframe: TimeSeriesDataFrame, prediction_length: int
+    ts_dataframe: TimeSeriesDataFrame,
+    prediction_length: int,
+    freq: Optional[str] = None,
 ) -> pd.MultiIndex:
     """For each item in the dataframe, get timestamps for the next prediction_length many time steps into the future.
 
     Returns a pandas.MultiIndex, where
     - level 0 ("item_id") contains the same item_ids as the input ts_dataframe.
     - level 1 ("timestamp") contains the next prediction_length time steps starting from the end of each time series.
     """
     last = ts_dataframe.reset_index()[[ITEMID, TIMESTAMP]].groupby(by=ITEMID, sort=False, as_index=False).last()
     item_ids = np.repeat(last[ITEMID], prediction_length)
 
-    offset = pd.tseries.frequencies.to_offset(ts_dataframe.freq)
+    if freq is None:
+        freq = ts_dataframe.freq
+    offset = pd.tseries.frequencies.to_offset(freq)
     last_ts = pd.DatetimeIndex(last[TIMESTAMP])
     # Non-vectorized offsets like BusinessDay may produce a PerformanceWarning - we filter them
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=pd.errors.PerformanceWarning)
         timestamps = np.dstack([last_ts + step * offset for step in range(1, prediction_length + 1)]).ravel()
     return pd.MultiIndex.from_arrays([item_ids, timestamps], names=[ITEMID, TIMESTAMP])
```

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.1.0b20240411/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240410
+Version: 1.1.0b20240411
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240410/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.1.0b20240411/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.1.0b20240410
-autogluon.common==1.1.0b20240410
-autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240410
+autogluon.core[raytune]==1.1.0b20240411
+autogluon.common==1.1.0b20240411
+autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240411
 
 [all]
 optimum[onnxruntime]<1.19,>=1.17
 
 [chronos-onnx]
 optimum[onnxruntime]<1.19,>=1.17
```

