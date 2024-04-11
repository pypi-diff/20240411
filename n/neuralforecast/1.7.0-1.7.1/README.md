# Comparing `tmp/neuralforecast-1.7.0.tar.gz` & `tmp/neuralforecast-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralforecast-1.7.0.tar", last modified: Wed Mar 27 18:35:23 2024, max compression
+gzip compressed data, was "neuralforecast-1.7.1.tar", last modified: Thu Apr 11 00:17:20 2024, max compression
```

## Comparing `neuralforecast-1.7.0.tar` & `neuralforecast-1.7.1.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:35:23.689391 neuralforecast-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-03-27 18:35:23.689391 neuralforecast-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:35:23.681391 neuralforecast-1.7.0/neuralforecast/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   165297 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    51860 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:35:23.681391 neuralforecast-1.7.0/neuralforecast/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/common/_base_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/common/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22189 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/common/_base_multivariate.py
--rw-r--r--   0 runner    (1001) docker     (127)    24532 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/common/_base_recurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    29653 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/common/_base_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/common/_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/common/_scalers.py
--rw-r--r--   0 runner    (1001) docker     (127)    43886 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:35:23.681391 neuralforecast-1.7.0/neuralforecast/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/losses/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    84578 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/losses/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:35:23.685391 neuralforecast-1.7.0/neuralforecast/models/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26697 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/autoformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/deepar.py
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/dilated_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/dlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/fedformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/hint.py
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/informer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/nbeats.py
--rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/nbeatsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/nhits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/nlinear.py
--rw-r--r--   0 runner    (1001) docker     (127)    36647 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/patchtst.py
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14948 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/stemgnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/tcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    23946 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/tft.py
--rw-r--r--   0 runner    (1001) docker     (127)    20157 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/timellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/timesnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/tsmixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17210 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/tsmixerx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/models/vanillatransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14152 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/tsdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/neuralforecast/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 18:35:23.685391 neuralforecast-1.7.0/neuralforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-03-27 18:35:23.000000 neuralforecast-1.7.0/neuralforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-27 18:35:23.000000 neuralforecast-1.7.0/neuralforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 18:35:23.000000 neuralforecast-1.7.0/neuralforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-27 18:35:23.000000 neuralforecast-1.7.0/neuralforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 18:35:23.000000 neuralforecast-1.7.0/neuralforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-27 18:35:23.000000 neuralforecast-1.7.0/neuralforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-27 18:35:23.000000 neuralforecast-1.7.0/neuralforecast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 18:35:23.689391 neuralforecast-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-27 18:35:19.000000 neuralforecast-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.658120 neuralforecast-1.7.1/neuralforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   176475 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59758 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.662120 neuralforecast-1.7.1/neuralforecast/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17381 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21416 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22755 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27930 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_base_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/common/_scalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53238 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.662120 neuralforecast-1.7.1/neuralforecast/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15633 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/losses/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84578 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/losses/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/neuralforecast/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26697 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/autoformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/bitcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22226 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/deepar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/dilated_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/dlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/fedformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/hint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/informer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/itransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/mlpmultivariate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/nbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/nbeatsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17853 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/nlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36647 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/patchtst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/stemgnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/tcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23669 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/tft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20157 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/timellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/timesnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/tsmixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/tsmixerx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/models/vanillatransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16128 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/tsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/neuralforecast/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/neuralforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 00:17:20.000000 neuralforecast-1.7.1/neuralforecast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:17:20.670120 neuralforecast-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-11 00:17:16.000000 neuralforecast-1.7.1/setup.py
```

### Comparing `neuralforecast-1.7.0/LICENSE` & `neuralforecast-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/PKG-INFO` & `neuralforecast-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.7.0
+Version: 1.7.1
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,19 @@
 Requires-Dist: numpy>=1.21.6
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: torch>=2.0.0
 Requires-Dist: pytorch-lightning>=2.0.0
 Requires-Dist: ray[tune]>=2.2.0
 Requires-Dist: optuna
 Requires-Dist: utilsforecast>=0.0.25
+Provides-Extra: aws
+Requires-Dist: fsspec[s3]; extra == "aws"
+Provides-Extra: spark
+Requires-Dist: fugue; extra == "spark"
+Requires-Dist: pyspark>=3.5; extra == "spark"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: hyperopt; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: nbdev; extra == "dev"
```

### Comparing `neuralforecast-1.7.0/README.md` & `neuralforecast-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/_modidx.py` & `neuralforecast-1.7.1/neuralforecast/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
                 'git_url': 'https://github.com/Nixtla/neuralforecast/',
                 'lib_path': 'neuralforecast'},
   'syms': { 'neuralforecast.auto': { 'neuralforecast.auto.AutoAutoformer': ('models.html#autoautoformer', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoAutoformer.__init__': ( 'models.html#autoautoformer.__init__',
                                                                                       'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoAutoformer.get_default_config': ( 'models.html#autoautoformer.get_default_config',
                                                                                                 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoBiTCN': ('models.html#autobitcn', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoBiTCN.__init__': ('models.html#autobitcn.__init__', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoBiTCN.get_default_config': ( 'models.html#autobitcn.get_default_config',
+                                                                                           'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDLinear': ('models.html#autodlinear', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDLinear.__init__': ( 'models.html#autodlinear.__init__',
                                                                                    'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDLinear.get_default_config': ( 'models.html#autodlinear.get_default_config',
                                                                                              'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDeepAR': ('models.html#autodeepar', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoDeepAR.__init__': ( 'models.html#autodeepar.__init__',
@@ -49,14 +53,20 @@
                                      'neuralforecast.auto.AutoLSTM.__init__': ('models.html#autolstm.__init__', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoLSTM.get_default_config': ( 'models.html#autolstm.get_default_config',
                                                                                           'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoMLP': ('models.html#automlp', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoMLP.__init__': ('models.html#automlp.__init__', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoMLP.get_default_config': ( 'models.html#automlp.get_default_config',
                                                                                          'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoMLPMultivariate': ( 'models.html#automlpmultivariate',
+                                                                                  'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoMLPMultivariate.__init__': ( 'models.html#automlpmultivariate.__init__',
+                                                                                           'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoMLPMultivariate.get_default_config': ( 'models.html#automlpmultivariate.get_default_config',
+                                                                                                     'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATS': ('models.html#autonbeats', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATS.__init__': ( 'models.html#autonbeats.__init__',
                                                                                   'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATS.get_default_config': ( 'models.html#autonbeats.get_default_config',
                                                                                             'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATSx': ('models.html#autonbeatsx', 'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoNBEATSx.__init__': ( 'models.html#autonbeatsx.__init__',
@@ -110,20 +120,28 @@
                                      'neuralforecast.auto.AutoTimesNet.get_default_config': ( 'models.html#autotimesnet.get_default_config',
                                                                                               'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoVanillaTransformer': ( 'models.html#autovanillatransformer',
                                                                                      'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoVanillaTransformer.__init__': ( 'models.html#autovanillatransformer.__init__',
                                                                                               'neuralforecast/auto.py'),
                                      'neuralforecast.auto.AutoVanillaTransformer.get_default_config': ( 'models.html#autovanillatransformer.get_default_config',
-                                                                                                        'neuralforecast/auto.py')},
+                                                                                                        'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoiTransformer': ('models.html#autoitransformer', 'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoiTransformer.__init__': ( 'models.html#autoitransformer.__init__',
+                                                                                        'neuralforecast/auto.py'),
+                                     'neuralforecast.auto.AutoiTransformer.get_default_config': ( 'models.html#autoitransformer.get_default_config',
+                                                                                                  'neuralforecast/auto.py')},
+            'neuralforecast.compat': {},
             'neuralforecast.core': { 'neuralforecast.core.NeuralForecast': ('core.html#neuralforecast', 'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast.__init__': ( 'core.html#neuralforecast.__init__',
                                                                                       'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast._check_nan': ( 'core.html#neuralforecast._check_nan',
                                                                                         'neuralforecast/core.py'),
+                                     'neuralforecast.core.NeuralForecast._get_model_names': ( 'core.html#neuralforecast._get_model_names',
+                                                                                              'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast._get_needed_futr_exog': ( 'core.html#neuralforecast._get_needed_futr_exog',
                                                                                                    'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast._no_refit_cross_validation': ( 'core.html#neuralforecast._no_refit_cross_validation',
                                                                                                         'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast._prepare_fit': ( 'core.html#neuralforecast._prepare_fit',
                                                                                           'neuralforecast/core.py'),
                                      'neuralforecast.core.NeuralForecast._reset_models': ( 'core.html#neuralforecast._reset_models',
@@ -448,14 +466,32 @@
                                                                                                           'neuralforecast/models/autoformer.py'),
                                                   'neuralforecast.models.autoformer.SeriesDecomp': ( 'models.autoformer.html#seriesdecomp',
                                                                                                      'neuralforecast/models/autoformer.py'),
                                                   'neuralforecast.models.autoformer.SeriesDecomp.__init__': ( 'models.autoformer.html#seriesdecomp.__init__',
                                                                                                               'neuralforecast/models/autoformer.py'),
                                                   'neuralforecast.models.autoformer.SeriesDecomp.forward': ( 'models.autoformer.html#seriesdecomp.forward',
                                                                                                              'neuralforecast/models/autoformer.py')},
+            'neuralforecast.models.bitcn': { 'neuralforecast.models.bitcn.BiTCN': ( 'models.bitcn.html#bitcn',
+                                                                                    'neuralforecast/models/bitcn.py'),
+                                             'neuralforecast.models.bitcn.BiTCN.__init__': ( 'models.bitcn.html#bitcn.__init__',
+                                                                                             'neuralforecast/models/bitcn.py'),
+                                             'neuralforecast.models.bitcn.BiTCN.forward': ( 'models.bitcn.html#bitcn.forward',
+                                                                                            'neuralforecast/models/bitcn.py'),
+                                             'neuralforecast.models.bitcn.CustomConv1d': ( 'models.bitcn.html#customconv1d',
+                                                                                           'neuralforecast/models/bitcn.py'),
+                                             'neuralforecast.models.bitcn.CustomConv1d.__init__': ( 'models.bitcn.html#customconv1d.__init__',
+                                                                                                    'neuralforecast/models/bitcn.py'),
+                                             'neuralforecast.models.bitcn.CustomConv1d.forward': ( 'models.bitcn.html#customconv1d.forward',
+                                                                                                   'neuralforecast/models/bitcn.py'),
+                                             'neuralforecast.models.bitcn.TCNCell': ( 'models.bitcn.html#tcncell',
+                                                                                      'neuralforecast/models/bitcn.py'),
+                                             'neuralforecast.models.bitcn.TCNCell.__init__': ( 'models.bitcn.html#tcncell.__init__',
+                                                                                               'neuralforecast/models/bitcn.py'),
+                                             'neuralforecast.models.bitcn.TCNCell.forward': ( 'models.bitcn.html#tcncell.forward',
+                                                                                              'neuralforecast/models/bitcn.py')},
             'neuralforecast.models.deepar': { 'neuralforecast.models.deepar.Decoder': ( 'models.deepar.html#decoder',
                                                                                         'neuralforecast/models/deepar.py'),
                                               'neuralforecast.models.deepar.Decoder.__init__': ( 'models.deepar.html#decoder.__init__',
                                                                                                  'neuralforecast/models/deepar.py'),
                                               'neuralforecast.models.deepar.Decoder.forward': ( 'models.deepar.html#decoder.forward',
                                                                                                 'neuralforecast/models/deepar.py'),
                                               'neuralforecast.models.deepar.DeepAR': ( 'models.deepar.html#deepar',
@@ -664,24 +700,56 @@
                                                                                                           'neuralforecast/models/informer.py'),
                                                 'neuralforecast.models.informer.ProbMask': ( 'models.informer.html#probmask',
                                                                                              'neuralforecast/models/informer.py'),
                                                 'neuralforecast.models.informer.ProbMask.__init__': ( 'models.informer.html#probmask.__init__',
                                                                                                       'neuralforecast/models/informer.py'),
                                                 'neuralforecast.models.informer.ProbMask.mask': ( 'models.informer.html#probmask.mask',
                                                                                                   'neuralforecast/models/informer.py')},
+            'neuralforecast.models.itransformer': { 'neuralforecast.models.itransformer.DataEmbedding_inverted': ( 'models.itransformer.html#dataembedding_inverted',
+                                                                                                                   'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.DataEmbedding_inverted.__init__': ( 'models.itransformer.html#dataembedding_inverted.__init__',
+                                                                                                                            'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.DataEmbedding_inverted.forward': ( 'models.itransformer.html#dataembedding_inverted.forward',
+                                                                                                                           'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.FullAttention': ( 'models.itransformer.html#fullattention',
+                                                                                                          'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.FullAttention.__init__': ( 'models.itransformer.html#fullattention.__init__',
+                                                                                                                   'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.FullAttention.forward': ( 'models.itransformer.html#fullattention.forward',
+                                                                                                                  'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.TriangularCausalMask': ( 'models.itransformer.html#triangularcausalmask',
+                                                                                                                 'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.TriangularCausalMask.__init__': ( 'models.itransformer.html#triangularcausalmask.__init__',
+                                                                                                                          'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.TriangularCausalMask.mask': ( 'models.itransformer.html#triangularcausalmask.mask',
+                                                                                                                      'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.iTransformer': ( 'models.itransformer.html#itransformer',
+                                                                                                         'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.iTransformer.__init__': ( 'models.itransformer.html#itransformer.__init__',
+                                                                                                                  'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.iTransformer.forecast': ( 'models.itransformer.html#itransformer.forecast',
+                                                                                                                  'neuralforecast/models/itransformer.py'),
+                                                    'neuralforecast.models.itransformer.iTransformer.forward': ( 'models.itransformer.html#itransformer.forward',
+                                                                                                                 'neuralforecast/models/itransformer.py')},
             'neuralforecast.models.lstm': { 'neuralforecast.models.lstm.LSTM': ('models.lstm.html#lstm', 'neuralforecast/models/lstm.py'),
                                             'neuralforecast.models.lstm.LSTM.__init__': ( 'models.lstm.html#lstm.__init__',
                                                                                           'neuralforecast/models/lstm.py'),
                                             'neuralforecast.models.lstm.LSTM.forward': ( 'models.lstm.html#lstm.forward',
                                                                                          'neuralforecast/models/lstm.py')},
             'neuralforecast.models.mlp': { 'neuralforecast.models.mlp.MLP': ('models.mlp.html#mlp', 'neuralforecast/models/mlp.py'),
                                            'neuralforecast.models.mlp.MLP.__init__': ( 'models.mlp.html#mlp.__init__',
                                                                                        'neuralforecast/models/mlp.py'),
                                            'neuralforecast.models.mlp.MLP.forward': ( 'models.mlp.html#mlp.forward',
                                                                                       'neuralforecast/models/mlp.py')},
+            'neuralforecast.models.mlpmultivariate': { 'neuralforecast.models.mlpmultivariate.MLPMultivariate': ( 'models.mlpmultivariate.html#mlpmultivariate',
+                                                                                                                  'neuralforecast/models/mlpmultivariate.py'),
+                                                       'neuralforecast.models.mlpmultivariate.MLPMultivariate.__init__': ( 'models.mlpmultivariate.html#mlpmultivariate.__init__',
+                                                                                                                           'neuralforecast/models/mlpmultivariate.py'),
+                                                       'neuralforecast.models.mlpmultivariate.MLPMultivariate.forward': ( 'models.mlpmultivariate.html#mlpmultivariate.forward',
+                                                                                                                          'neuralforecast/models/mlpmultivariate.py')},
             'neuralforecast.models.nbeats': { 'neuralforecast.models.nbeats.IdentityBasis': ( 'models.nbeats.html#identitybasis',
                                                                                               'neuralforecast/models/nbeats.py'),
                                               'neuralforecast.models.nbeats.IdentityBasis.__init__': ( 'models.nbeats.html#identitybasis.__init__',
                                                                                                        'neuralforecast/models/nbeats.py'),
                                               'neuralforecast.models.nbeats.IdentityBasis.forward': ( 'models.nbeats.html#identitybasis.forward',
                                                                                                       'neuralforecast/models/nbeats.py'),
                                               'neuralforecast.models.nbeats.NBEATS': ( 'models.nbeats.html#nbeats',
@@ -1152,15 +1220,25 @@
                                           'neuralforecast.tsdataset.TimeSeriesDataset.update_dataset': ( 'tsdataset.html#timeseriesdataset.update_dataset',
                                                                                                          'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesLoader': ( 'tsdataset.html#timeseriesloader',
                                                                                          'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesLoader.__init__': ( 'tsdataset.html#timeseriesloader.__init__',
                                                                                                   'neuralforecast/tsdataset.py'),
                                           'neuralforecast.tsdataset.TimeSeriesLoader._collate_fn': ( 'tsdataset.html#timeseriesloader._collate_fn',
-                                                                                                     'neuralforecast/tsdataset.py')},
+                                                                                                     'neuralforecast/tsdataset.py'),
+                                          'neuralforecast.tsdataset._DistributedTimeSeriesDataModule': ( 'tsdataset.html#_distributedtimeseriesdatamodule',
+                                                                                                         'neuralforecast/tsdataset.py'),
+                                          'neuralforecast.tsdataset._DistributedTimeSeriesDataModule.__init__': ( 'tsdataset.html#_distributedtimeseriesdatamodule.__init__',
+                                                                                                                  'neuralforecast/tsdataset.py'),
+                                          'neuralforecast.tsdataset._DistributedTimeSeriesDataModule.setup': ( 'tsdataset.html#_distributedtimeseriesdatamodule.setup',
+                                                                                                               'neuralforecast/tsdataset.py'),
+                                          'neuralforecast.tsdataset._FilesDataset': ( 'tsdataset.html#_filesdataset',
+                                                                                      'neuralforecast/tsdataset.py'),
+                                          'neuralforecast.tsdataset._FilesDataset.__init__': ( 'tsdataset.html#_filesdataset.__init__',
+                                                                                               'neuralforecast/tsdataset.py')},
             'neuralforecast.utils': { 'neuralforecast.utils.DayOfMonth': ('utils.html#dayofmonth', 'neuralforecast/utils.py'),
                                       'neuralforecast.utils.DayOfMonth.__call__': ( 'utils.html#dayofmonth.__call__',
                                                                                     'neuralforecast/utils.py'),
                                       'neuralforecast.utils.DayOfWeek': ('utils.html#dayofweek', 'neuralforecast/utils.py'),
                                       'neuralforecast.utils.DayOfWeek.__call__': ( 'utils.html#dayofweek.__call__',
                                                                                    'neuralforecast/utils.py'),
                                       'neuralforecast.utils.DayOfYear': ('utils.html#dayofyear', 'neuralforecast/utils.py'),
```

### Comparing `neuralforecast-1.7.0/neuralforecast/auto.py` & `neuralforecast-1.7.1/neuralforecast/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/models.ipynb.
 
 # %% auto 0
-__all__ = ['AutoRNN', 'AutoLSTM', 'AutoGRU', 'AutoTCN', 'AutoDeepAR', 'AutoDilatedRNN', 'AutoMLP', 'AutoNBEATS', 'AutoNBEATSx',
-           'AutoNHITS', 'AutoDLinear', 'AutoNLinear', 'AutoTFT', 'AutoVanillaTransformer', 'AutoInformer',
-           'AutoAutoformer', 'AutoFEDformer', 'AutoPatchTST', 'AutoTimesNet', 'AutoStemGNN', 'AutoHINT', 'AutoTSMixer',
-           'AutoTSMixerx']
+__all__ = ['AutoRNN', 'AutoLSTM', 'AutoGRU', 'AutoTCN', 'AutoDeepAR', 'AutoDilatedRNN', 'AutoBiTCN', 'AutoMLP', 'AutoNBEATS',
+           'AutoNBEATSx', 'AutoNHITS', 'AutoDLinear', 'AutoNLinear', 'AutoTFT', 'AutoVanillaTransformer',
+           'AutoInformer', 'AutoAutoformer', 'AutoFEDformer', 'AutoPatchTST', 'AutoiTransformer', 'AutoTimesNet',
+           'AutoStemGNN', 'AutoHINT', 'AutoTSMixer', 'AutoTSMixerx', 'AutoMLPMultivariate']
 
 # %% ../nbs/models.ipynb 2
 from os import cpu_count
 import torch
 
 from ray import tune
 from ray.tune.search.basic_variant import BasicVariantGenerator
@@ -18,14 +18,15 @@
 
 from .models.rnn import RNN
 from .models.gru import GRU
 from .models.tcn import TCN
 from .models.lstm import LSTM
 from .models.deepar import DeepAR
 from .models.dilated_rnn import DilatedRNN
+from .models.bitcn import BiTCN
 
 from .models.mlp import MLP
 from .models.nbeats import NBEATS
 from .models.nbeatsx import NBEATSx
 from .models.nhits import NHITS
 from .models.dlinear import DLinear
 from .models.nlinear import NLinear
@@ -33,19 +34,21 @@
 from .models.tft import TFT
 from .models.vanillatransformer import VanillaTransformer
 from .models.informer import Informer
 from .models.autoformer import Autoformer
 from .models.fedformer import FEDformer
 from .models.patchtst import PatchTST
 from .models.timesnet import TimesNet
+from .models.itransformer import iTransformer
 
 from .models.stemgnn import StemGNN
 from .models.hint import HINT
 from .models.tsmixer import TSMixer
 from .models.tsmixerx import TSMixerx
+from .models.mlpmultivariate import MLPMultivariate
 
 from .losses.pytorch import MAE, MQLoss, DistributionLoss
 
 # %% ../nbs/models.ipynb 13
 class AutoRNN(BaseAuto):
 
     default_config = {
@@ -471,15 +474,83 @@
         )
         del config["input_size_multiplier"], config["inference_input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 38
+# %% ../nbs/models.ipynb 37
+class AutoBiTCN(BaseAuto):
+
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "hidden_size": tune.choice([16, 32]),
+        "dropout": tune.uniform(0.0, 0.99),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.choice([500, 1000, 2000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "windows_batch_size": tune.choice([128, 256, 512, 1024]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+        backend="ray",
+        callbacks=None,
+    ):
+
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.get_default_config(h=h, backend=backend)
+
+        super(AutoBiTCN, self).__init__(
+            cls_model=BiTCN,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+            backend=backend,
+            callbacks=callbacks,
+        )
+
+    @classmethod
+    def get_default_config(cls, h, backend, n_series=None):
+        config = cls.default_config.copy()
+        config["input_size"] = tune.choice(
+            [h * x for x in config["input_size_multiplier"]]
+        )
+        config["step_size"] = tune.choice([1, h])
+        del config["input_size_multiplier"]
+        if backend == "optuna":
+            config = cls._ray_config_to_optuna(config)
+
+        return config
+
+# %% ../nbs/models.ipynb 42
 class AutoMLP(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([256, 512, 1024]),
         "num_layers": tune.randint(2, 6),
@@ -539,15 +610,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 42
+# %% ../nbs/models.ipynb 46
 class AutoNBEATS(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
@@ -605,15 +676,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 46
+# %% ../nbs/models.ipynb 50
 class AutoNBEATSx(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
@@ -671,15 +742,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 50
+# %% ../nbs/models.ipynb 54
 class AutoNHITS(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "n_pool_kernel_size": tune.choice(
             [[2, 2, 1], 3 * [1], 3 * [2], 3 * [4], [8, 4, 1], [16, 8, 1]]
@@ -750,15 +821,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 54
+# %% ../nbs/models.ipynb 58
 class AutoDLinear(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "moving_avg_window": tune.choice([11, 25, 51]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -817,15 +888,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 58
+# %% ../nbs/models.ipynb 62
 class AutoNLinear(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "learning_rate": tune.loguniform(1e-4, 1e-1),
         "scaler_type": tune.choice([None, "robust", "standard"]),
@@ -883,15 +954,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 63
+# %% ../nbs/models.ipynb 67
 class AutoTFT(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
@@ -951,15 +1022,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 67
+# %% ../nbs/models.ipynb 71
 class AutoVanillaTransformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
@@ -1019,15 +1090,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 71
+# %% ../nbs/models.ipynb 75
 class AutoInformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
@@ -1087,15 +1158,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 75
+# %% ../nbs/models.ipynb 79
 class AutoAutoformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "n_head": tune.choice([4, 8]),
@@ -1155,15 +1226,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 79
+# %% ../nbs/models.ipynb 83
 class AutoFEDformer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([64, 128, 256]),
         "learning_rate": tune.loguniform(1e-4, 1e-1),
@@ -1222,15 +1293,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 83
+# %% ../nbs/models.ipynb 87
 class AutoPatchTST(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3],
         "h": None,
         "hidden_size": tune.choice([16, 128, 256]),
         "n_heads": tune.choice([4, 16]),
@@ -1292,15 +1363,100 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 88
+# %% ../nbs/models.ipynb 91
+class AutoiTransformer(BaseAuto):
+
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "n_series": None,
+        "hidden_size": tune.choice([64, 128, 256]),
+        "n_heads": tune.choice([4, 8]),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.choice([500, 1000, 2000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        n_series,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+        backend="ray",
+        callbacks=None,
+    ):
+
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.get_default_config(h=h, backend=backend, n_series=n_series)
+
+        # Always use n_series from parameters, raise exception with Optuna because we can't enforce it
+        if backend == "ray":
+            config["n_series"] = n_series
+        elif backend == "optuna":
+            mock_trial = MockTrial()
+            if (
+                "n_series" in config(mock_trial)
+                and config(mock_trial)["n_series"] != n_series
+            ) or ("n_series" not in config(mock_trial)):
+                raise Exception(f"config needs 'n_series': {n_series}")
+
+        super(AutoiTransformer, self).__init__(
+            cls_model=iTransformer,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+            backend=backend,
+            callbacks=callbacks,
+        )
+
+    @classmethod
+    def get_default_config(cls, h, backend, n_series):
+        config = cls.default_config.copy()
+        config["input_size"] = tune.choice(
+            [h * x for x in config["input_size_multiplier"]]
+        )
+
+        # Rolling windows with step_size=1 or step_size=h
+        # See `BaseWindows` and `BaseRNN`'s create_windows
+        config["step_size"] = tune.choice([1, h])
+        del config["input_size_multiplier"]
+        if backend == "optuna":
+            # Always use n_series from parameters
+            config["n_series"] = n_series
+            config = cls._ray_config_to_optuna(config)
+
+        return config
+
+# %% ../nbs/models.ipynb 96
 class AutoTimesNet(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4, 5],
         "h": None,
         "hidden_size": tune.choice([32, 64, 128]),
         "conv_hidden_size": tune.choice([32, 64, 128]),
@@ -1360,15 +1516,15 @@
         config["step_size"] = tune.choice([1, h])
         del config["input_size_multiplier"]
         if backend == "optuna":
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 93
+# %% ../nbs/models.ipynb 101
 class AutoStemGNN(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4],
         "h": None,
         "n_series": None,
         "n_stacks": tune.choice([2]),
@@ -1445,15 +1601,15 @@
         if backend == "optuna":
             # Always use n_series from parameters
             config["n_series"] = n_series
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 97
+# %% ../nbs/models.ipynb 105
 class AutoHINT(BaseAuto):
 
     def __init__(
         self,
         cls_model,
         h,
         loss,
@@ -1495,30 +1651,37 @@
         if not ("reconciliation" in config.keys()):
             raise Exception(
                 "config needs reconciliation, \
                             try tune.choice(['BottomUp', 'MinTraceOLS', 'MinTraceWLS'])"
             )
         self.S = S
 
-    def _fit_model(self, cls_model, config, dataset, val_size, test_size):
+    def _fit_model(
+        self, cls_model, config, dataset, val_size, test_size, distributed_config=None
+    ):
         # Overwrite _fit_model for HINT two-stage instantiation
         reconciliation = config.pop("reconciliation")
         base_model = cls_model(**config)
         model = HINT(
             h=base_model.h, model=base_model, S=self.S, reconciliation=reconciliation
         )
         model.test_size = test_size
-        model.fit(dataset, val_size=val_size, test_size=test_size)
-        return model, None
+        model = model.fit(
+            dataset,
+            val_size=val_size,
+            test_size=test_size,
+            distributed_config=distributed_config,
+        )
+        return model
 
     @classmethod
     def get_default_config(cls, h, backend, n_series=None):
         raise Exception("AutoHINT has no default configuration.")
 
-# %% ../nbs/models.ipynb 102
+# %% ../nbs/models.ipynb 110
 class AutoTSMixer(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4],
         "h": None,
         "n_series": None,
         "n_block": tune.choice([1, 2, 4, 6, 8]),
@@ -1596,15 +1759,15 @@
         if backend == "optuna":
             # Always use n_series from parameters
             config["n_series"] = n_series
             config = cls._ray_config_to_optuna(config)
 
         return config
 
-# %% ../nbs/models.ipynb 106
+# %% ../nbs/models.ipynb 114
 class AutoTSMixerx(BaseAuto):
 
     default_config = {
         "input_size_multiplier": [1, 2, 3, 4],
         "h": None,
         "n_series": None,
         "n_block": tune.choice([1, 2, 4, 6, 8]),
@@ -1656,14 +1819,99 @@
             h=h,
             loss=loss,
             valid_loss=valid_loss,
             config=config,
             search_alg=search_alg,
             num_samples=num_samples,
             refit_with_val=refit_with_val,
+            cpus=cpus,
+            gpus=gpus,
+            verbose=verbose,
+            alias=alias,
+            backend=backend,
+            callbacks=callbacks,
+        )
+
+    @classmethod
+    def get_default_config(cls, h, backend, n_series):
+        config = cls.default_config.copy()
+        config["input_size"] = tune.choice(
+            [h * x for x in config["input_size_multiplier"]]
+        )
+
+        # Rolling windows with step_size=1 or step_size=h
+        # See `BaseWindows` and `BaseRNN`'s create_windows
+        config["step_size"] = tune.choice([1, h])
+        del config["input_size_multiplier"]
+        if backend == "optuna":
+            # Always use n_series from parameters
+            config["n_series"] = n_series
+            config = cls._ray_config_to_optuna(config)
+
+        return config
+
+# %% ../nbs/models.ipynb 118
+class AutoMLPMultivariate(BaseAuto):
+
+    default_config = {
+        "input_size_multiplier": [1, 2, 3, 4, 5],
+        "h": None,
+        "n_series": None,
+        "hidden_size": tune.choice([256, 512, 1024]),
+        "num_layers": tune.randint(2, 6),
+        "learning_rate": tune.loguniform(1e-4, 1e-1),
+        "scaler_type": tune.choice([None, "robust", "standard"]),
+        "max_steps": tune.choice([500, 1000]),
+        "batch_size": tune.choice([32, 64, 128, 256]),
+        "loss": None,
+        "random_seed": tune.randint(1, 20),
+    }
+
+    def __init__(
+        self,
+        h,
+        n_series,
+        loss=MAE(),
+        valid_loss=None,
+        config=None,
+        search_alg=BasicVariantGenerator(random_state=1),
+        num_samples=10,
+        refit_with_val=False,
+        cpus=cpu_count(),
+        gpus=torch.cuda.device_count(),
+        verbose=False,
+        alias=None,
+        backend="ray",
+        callbacks=None,
+    ):
+
+        # Define search space, input/output sizes
+        if config is None:
+            config = self.get_default_config(h=h, backend=backend, n_series=n_series)
+
+        # Always use n_series from parameters, raise exception with Optuna because we can't enforce it
+        if backend == "ray":
+            config["n_series"] = n_series
+        elif backend == "optuna":
+            mock_trial = MockTrial()
+            if (
+                "n_series" in config(mock_trial)
+                and config(mock_trial)["n_series"] != n_series
+            ) or ("n_series" not in config(mock_trial)):
+                raise Exception(f"config needs 'n_series': {n_series}")
+
+        super(AutoMLPMultivariate, self).__init__(
+            cls_model=MLPMultivariate,
+            h=h,
+            loss=loss,
+            valid_loss=valid_loss,
+            config=config,
+            search_alg=search_alg,
+            num_samples=num_samples,
+            refit_with_val=refit_with_val,
             cpus=cpus,
             gpus=gpus,
             verbose=verbose,
             alias=alias,
             backend=backend,
             callbacks=callbacks,
         )
```

### Comparing `neuralforecast-1.7.0/neuralforecast/common/_base_auto.py` & `neuralforecast-1.7.1/neuralforecast/common/_base_auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -306,29 +306,31 @@
         dataset,
         val_size,
         test_size,
         verbose,
         num_samples,
         search_alg,
         config,
+        distributed_config,
     ):
         import optuna
 
         def objective(trial):
             user_cfg = config(trial)
             cfg = deepcopy(user_cfg)
-            _, trainer = self._fit_model(
+            model = self._fit_model(
                 cls_model=cls_model,
                 config=cfg,
                 dataset=dataset,
                 val_size=val_size,
                 test_size=test_size,
+                distributed_config=distributed_config,
             )
             trial.set_user_attr("ALL_PARAMS", user_cfg)
-            metrics = trainer.callback_metrics
+            metrics = model.metrics
             trial.set_user_attr(
                 "METRICS",
                 {
                     "loss": metrics["ptl/val_loss"],
                     "train_loss": metrics["train_loss"],
                 },
             )
@@ -344,20 +346,34 @@
             objective,
             n_trials=num_samples,
             show_progress_bar=verbose,
             callbacks=self.callbacks,
         )
         return study
 
-    def _fit_model(self, cls_model, config, dataset, val_size, test_size):
+    def _fit_model(
+        self, cls_model, config, dataset, val_size, test_size, distributed_config=None
+    ):
         model = cls_model(**config)
-        trainer = model.fit(dataset, val_size=val_size, test_size=test_size)
-        return model, trainer
+        model = model.fit(
+            dataset,
+            val_size=val_size,
+            test_size=test_size,
+            distributed_config=distributed_config,
+        )
+        return model
 
-    def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
+    def fit(
+        self,
+        dataset,
+        val_size=0,
+        test_size=0,
+        random_seed=None,
+        distributed_config=None,
+    ):
         """BaseAuto.fit
 
         Perform the hyperparameter optimization as specified by the BaseAuto configuration
         dictionary `config`.
 
         The optimization is performed on the `TimeSeriesDataset` using temporal cross validation with
         the validation set that sequentially precedes the test set.
@@ -371,14 +387,18 @@
         `self`: fitted instance of `BaseAuto` with best hyperparameters and results<br>.
         """
         # we need val_size > 0 to perform
         # hyperparameter selection.
         search_alg = deepcopy(self.search_alg)
         val_size = val_size if val_size > 0 else self.h
         if self.backend == "ray":
+            if distributed_config is not None:
+                raise ValueError(
+                    "distributed training is not supported for the ray backend."
+                )
             results = self._tune_model(
                 cls_model=self.cls_model,
                 dataset=dataset,
                 val_size=val_size,
                 test_size=test_size,
                 cpus=self.cpus,
                 gpus=self.gpus,
@@ -394,29 +414,32 @@
                 dataset=dataset,
                 val_size=val_size,
                 test_size=test_size,
                 verbose=self.verbose,
                 num_samples=self.num_samples,
                 search_alg=search_alg,
                 config=self.config,
+                distributed_config=distributed_config,
             )
             best_config = results.best_trial.user_attrs["ALL_PARAMS"]
-        self.model, _ = self._fit_model(
+        self.model = self._fit_model(
             cls_model=self.cls_model,
             config=best_config,
             dataset=dataset,
             val_size=val_size * (1 - self.refit_with_val),
             test_size=test_size,
+            distributed_config=distributed_config,
         )
         self.results = results
 
         # Added attributes for compatibility with NeuralForecast core
         self.futr_exog_list = self.model.futr_exog_list
         self.hist_exog_list = self.model.hist_exog_list
         self.stat_exog_list = self.model.stat_exog_list
+        return self
 
     def predict(self, dataset, step_size=1, **data_kwargs):
         """BaseAuto.predict
 
         Predictions of the best performing model on validation.
 
         **Parameters:**<br>
@@ -439,8 +462,8 @@
         """BaseAuto.save
 
         Save the fitted model to disk.
 
         **Parameters:**<br>
         `path`: str, path to save the model.<br>
         """
-        self.model.trainer.save_checkpoint(path)
+        self.model.save(path)
```

### Comparing `neuralforecast-1.7.0/neuralforecast/common/_base_multivariate.py` & `neuralforecast-1.7.1/neuralforecast/common/_base_multivariate.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 __all__ = ['BaseMultivariate']
 
 # %% ../../nbs/common.base_multivariate.ipynb 5
 import numpy as np
 import torch
 import torch.nn as nn
 import pytorch_lightning as pl
-from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 
+import neuralforecast.losses.pytorch as losses
 from ._base_model import BaseModel
 from ._scalers import TemporalNorm
 from ..tsdataset import TimeSeriesDataModule
 from ..utils import get_indexer_raise_missing
 
 # %% ../../nbs/common.base_multivariate.ipynb 6
 class BaseMultivariate(BaseModel):
@@ -50,102 +50,79 @@
         drop_last_loader=False,
         random_seed=1,
         alias=None,
         optimizer=None,
         optimizer_kwargs=None,
         **trainer_kwargs,
     ):
-        super(BaseModel, self).__init__()
-
-        self.save_hyperparameters()  # Allows instantiation from a checkpoint from class
-        self.random_seed = random_seed
-        pl.seed_everything(self.random_seed, workers=True)
+        super().__init__(
+            random_seed=random_seed,
+            loss=loss,
+            valid_loss=valid_loss,
+            optimizer=optimizer,
+            optimizer_kwargs=optimizer_kwargs,
+            futr_exog_list=futr_exog_list,
+            hist_exog_list=hist_exog_list,
+            stat_exog_list=stat_exog_list,
+            max_steps=max_steps,
+            early_stop_patience_steps=early_stop_patience_steps,
+            **trainer_kwargs,
+        )
 
         # Padder to complete train windows,
         # example y=[1,2,3,4,5] h=3 -> last y_output = [5,0,0]
         self.h = h
         self.input_size = input_size
         self.n_series = n_series
         self.padder = nn.ConstantPad1d(padding=(0, self.h), value=0)
 
-        # Loss
-        self.loss = loss
-        if valid_loss is None:
-            self.valid_loss = loss
-        else:
-            self.valid_loss = valid_loss
-        self.train_trajectories = []
-        self.valid_trajectories = []
+        # Multivariate models do not support these loss functions yet.
+        unsupported_losses = (
+            losses.sCRPS,
+            losses.MQLoss,
+            losses.DistributionLoss,
+            losses.PMM,
+            losses.GMM,
+            losses.HuberMQLoss,
+            losses.MASE,
+            losses.relMSE,
+            losses.NBMM,
+        )
+        if isinstance(self.loss, unsupported_losses):
+            raise Exception(f"{self.loss} is not supported in a Multivariate model.")
+        if isinstance(self.valid_loss, unsupported_losses):
+            raise Exception(
+                f"{self.valid_loss} is not supported in a Multivariate model."
+            )
 
         self.batch_size = batch_size
 
         # Optimization
         self.learning_rate = learning_rate
         self.max_steps = max_steps
         self.num_lr_decays = num_lr_decays
         self.lr_decay_steps = (
             max(max_steps // self.num_lr_decays, 1) if self.num_lr_decays > 0 else 10e7
         )
         self.early_stop_patience_steps = early_stop_patience_steps
         self.val_check_steps = val_check_steps
         self.step_size = step_size
-        # custom optimizer defined by user
-        if optimizer is not None and not issubclass(optimizer, torch.optim.Optimizer):
-            raise TypeError(
-                "optimizer is not a valid subclass of torch.optim.Optimizer"
-            )
-        self.optimizer = optimizer
-        self.optimizer_kwargs = optimizer_kwargs if optimizer_kwargs else {}
 
         # Scaler
         self.scaler = TemporalNorm(
             scaler_type=scaler_type, dim=2
         )  # Time dimension is in the second axis
 
-        # Variables
-        self.futr_exog_list = list(futr_exog_list) if futr_exog_list is not None else []
-        self.hist_exog_list = list(hist_exog_list) if hist_exog_list is not None else []
-        self.stat_exog_list = list(stat_exog_list) if stat_exog_list is not None else []
-
         # Fit arguments
         self.val_size = 0
         self.test_size = 0
 
         # Model state
         self.decompose_forecast = False
 
-        ## Trainer arguments ##
-        # Max steps, validation steps and check_val_every_n_epoch
-        trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
-
-        if "max_epochs" in trainer_kwargs.keys():
-            raise Exception("max_epochs is deprecated, use max_steps instead.")
-
-        # Callbacks
-        if "callbacks" not in trainer_kwargs and self.early_stop_patience_steps > 0:
-            trainer_kwargs["callbacks"] = [
-                EarlyStopping(
-                    monitor="ptl/val_loss", patience=self.early_stop_patience_steps
-                )
-            ]
-
-        # Add GPU accelerator if available
-        if trainer_kwargs.get("accelerator", None) is None:
-            if torch.cuda.is_available():
-                trainer_kwargs["accelerator"] = "gpu"
-        if trainer_kwargs.get("devices", None) is None:
-            if torch.cuda.is_available():
-                trainer_kwargs["devices"] = -1
-
-        # Avoid saturating local memory, disabled fit model checkpoints
-        if trainer_kwargs.get("enable_checkpointing", None) is None:
-            trainer_kwargs["enable_checkpointing"] = False
-
-        self.trainer_kwargs = trainer_kwargs
-
         # DataModule arguments
         self.num_workers_loader = num_workers_loader
         self.drop_last_loader = drop_last_loader
         # used by on_validation_epoch_end hook
         self.validation_step_outputs = []
         self.alias = alias
 
@@ -509,15 +486,22 @@
                 y_hat = torch.concat((y_hat, distr_args), axis=2)
         else:
             y_hat, _, _ = self._inv_normalization(
                 y_hat=output, temporal_cols=batch["temporal_cols"], y_idx=y_idx
             )
         return y_hat
 
-    def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
+    def fit(
+        self,
+        dataset,
+        val_size=0,
+        test_size=0,
+        random_seed=None,
+        distributed_config=None,
+    ):
         """Fit.
 
         The `fit` method, optimizes the neural network's weights using the
         initialization parameters (`learning_rate`, `windows_batch_size`, ...)
         and the `loss` function as defined during the initialization.
         Within `fit` we use a PyTorch Lightning `Trainer` that
         inherits the initialization's `self.trainer_kwargs`, to customize
@@ -530,21 +514,27 @@
         disk memory, to get them change `enable_checkpointing=True` in `__init__`.
 
         **Parameters:**<br>
         `dataset`: NeuralForecast's `TimeSeriesDataset`, see [documentation](https://nixtla.github.io/neuralforecast/tsdataset.html).<br>
         `val_size`: int, validation size for temporal cross-validation.<br>
         `test_size`: int, test size for temporal cross-validation.<br>
         """
+        if distributed_config is not None:
+            raise ValueError(
+                "multivariate models cannot be trained using distributed data parallel."
+            )
         return self._fit(
             dataset=dataset,
             batch_size=self.n_series,
+            valid_batch_size=self.n_series,
             val_size=val_size,
             test_size=test_size,
             random_seed=random_seed,
             shuffle_train=False,
+            distributed_config=None,
         )
 
     def predict(
         self,
         dataset,
         test_size=None,
         step_size=1,
@@ -563,15 +553,18 @@
         """
         self._check_exog(dataset)
         self._restart_seed(random_seed)
 
         self.predict_step_size = step_size
         self.decompose_forecast = False
         datamodule = TimeSeriesDataModule(
-            dataset=dataset, batch_size=self.n_series, **data_module_kwargs
+            dataset=dataset,
+            valid_batch_size=self.n_series,
+            batch_size=self.n_series,
+            **data_module_kwargs,
         )
 
         # Protect when case of multiple gpu. PL does not support return preds with multiple gpu.
         pred_trainer_kwargs = self.trainer_kwargs.copy()
         if (pred_trainer_kwargs.get("accelerator", None) == "gpu") and (
             torch.cuda.device_count() > 1
         ):
```

### Comparing `neuralforecast-1.7.0/neuralforecast/common/_base_recurrent.py` & `neuralforecast-1.7.1/neuralforecast/common/_base_recurrent.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 __all__ = ['BaseRecurrent']
 
 # %% ../../nbs/common.base_recurrent.ipynb 6
 import numpy as np
 import torch
 import torch.nn as nn
 import pytorch_lightning as pl
-from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 
 from ._base_model import BaseModel
 from ._scalers import TemporalNorm
 from ..tsdataset import TimeSeriesDataModule
 from ..utils import get_indexer_raise_missing
 
 # %% ../../nbs/common.base_recurrent.ipynb 7
@@ -50,36 +49,35 @@
         drop_last_loader=False,
         random_seed=1,
         alias=None,
         optimizer=None,
         optimizer_kwargs=None,
         **trainer_kwargs,
     ):
-        super(BaseModel, self).__init__()
-
-        self.save_hyperparameters()  # Allows instantiation from a checkpoint from class
-        self.random_seed = random_seed
-        pl.seed_everything(self.random_seed, workers=True)
+        super().__init__(
+            random_seed=random_seed,
+            loss=loss,
+            valid_loss=valid_loss,
+            optimizer=optimizer,
+            optimizer_kwargs=optimizer_kwargs,
+            futr_exog_list=futr_exog_list,
+            hist_exog_list=hist_exog_list,
+            stat_exog_list=stat_exog_list,
+            max_steps=max_steps,
+            early_stop_patience_steps=early_stop_patience_steps,
+            **trainer_kwargs,
+        )
 
         # Padder to complete train windows,
         # example y=[1,2,3,4,5] h=3 -> last y_output = [5,0,0]
         self.h = h
         self.input_size = input_size
         self.inference_input_size = inference_input_size
         self.padder = nn.ConstantPad1d(padding=(0, self.h), value=0)
 
-        # Loss
-        self.loss = loss
-        if valid_loss is None:
-            self.valid_loss = loss
-        else:
-            self.valid_loss = valid_loss
-        self.train_trajectories = []
-        self.valid_trajectories = []
-
         if (
             str(type(self.loss))
             == "<class 'neuralforecast.losses.pytorch.DistributionLoss'>"
             and self.loss.distribution == "Bernoulli"
         ):
             raise Exception(
                 "Temporal Classification not yet available for Recurrent-based models"
@@ -97,67 +95,26 @@
         self.max_steps = max_steps
         self.num_lr_decays = num_lr_decays
         self.lr_decay_steps = (
             max(max_steps // self.num_lr_decays, 1) if self.num_lr_decays > 0 else 10e7
         )
         self.early_stop_patience_steps = early_stop_patience_steps
         self.val_check_steps = val_check_steps
-        # custom optimizer defined by user
-        if optimizer is not None and not issubclass(optimizer, torch.optim.Optimizer):
-            raise TypeError(
-                "optimizer is not a valid subclass of torch.optim.Optimizer"
-            )
-        self.optimizer = optimizer
-        self.optimizer_kwargs = optimizer_kwargs if optimizer_kwargs else {}
-
-        # Variables
-        self.futr_exog_list = list(futr_exog_list) if futr_exog_list is not None else []
-        self.hist_exog_list = list(hist_exog_list) if hist_exog_list is not None else []
-        self.stat_exog_list = list(stat_exog_list) if stat_exog_list is not None else []
 
         # Scaler
         self.scaler = TemporalNorm(
             scaler_type=scaler_type,
             dim=-1,  # Time dimension is -1.
             num_features=1 + len(self.hist_exog_list) + len(self.futr_exog_list),
         )
 
         # Fit arguments
         self.val_size = 0
         self.test_size = 0
 
-        ## Trainer arguments ##
-        # Max steps, validation steps and check_val_every_n_epoch
-        trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
-
-        if "max_epochs" in trainer_kwargs.keys():
-            raise Exception("max_epochs is deprecated, use max_steps instead.")
-
-        # Callbacks
-        if "callbacks" not in trainer_kwargs and self.early_stop_patience_steps > 0:
-            trainer_kwargs["callbacks"] = [
-                EarlyStopping(
-                    monitor="ptl/val_loss", patience=self.early_stop_patience_steps
-                )
-            ]
-
-        # Add GPU accelerator if available
-        if trainer_kwargs.get("accelerator", None) is None:
-            if torch.cuda.is_available():
-                trainer_kwargs["accelerator"] = "gpu"
-        if trainer_kwargs.get("devices", None) is None:
-            if torch.cuda.is_available():
-                trainer_kwargs["devices"] = -1
-
-        # Avoid saturating local memory, disabled fit model checkpoints
-        if trainer_kwargs.get("enable_checkpointing", None) is None:
-            trainer_kwargs["enable_checkpointing"] = False
-
-        self.trainer_kwargs = trainer_kwargs
-
         # DataModule arguments
         self.num_workers_loader = num_workers_loader
         self.drop_last_loader = drop_last_loader
         # used by on_validation_epoch_end hook
         self.validation_step_outputs = []
         self.alias = alias
 
@@ -533,15 +490,22 @@
                 y_hat = torch.concat((y_hat, distr_args), axis=3)
         else:
             y_hat, _, _ = self._inv_normalization(
                 y_hat=output, temporal_cols=batch["temporal_cols"], y_idx=y_idx
             )
         return y_hat
 
-    def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
+    def fit(
+        self,
+        dataset,
+        val_size=0,
+        test_size=0,
+        random_seed=None,
+        distributed_config=None,
+    ):
         """Fit.
 
         The `fit` method, optimizes the neural network's weights using the
         initialization parameters (`learning_rate`, `batch_size`, ...)
         and the `loss` function as defined during the initialization.
         Within `fit` we use a PyTorch Lightning `Trainer` that
         inherits the initialization's `self.trainer_kwargs`, to customize
@@ -562,14 +526,15 @@
         return self._fit(
             dataset=dataset,
             batch_size=self.batch_size,
             valid_batch_size=self.valid_batch_size,
             val_size=val_size,
             test_size=test_size,
             random_seed=random_seed,
+            distributed_config=distributed_config,
         )
 
     def predict(self, dataset, step_size=1, random_seed=None, **data_module_kwargs):
         """Predict.
 
         Neural network prediction with PL's `Trainer` execution of `predict_step`.
```

### Comparing `neuralforecast-1.7.0/neuralforecast/common/_base_windows.py` & `neuralforecast-1.7.1/neuralforecast/common/_base_windows.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 __all__ = ['BaseWindows']
 
 # %% ../../nbs/common.base_windows.ipynb 5
 import numpy as np
 import torch
 import torch.nn as nn
 import pytorch_lightning as pl
-from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 
 from ._base_model import BaseModel
 from ._scalers import TemporalNorm
 from ..tsdataset import TimeSeriesDataModule
 from ..utils import get_indexer_raise_missing
 
 # %% ../../nbs/common.base_windows.ipynb 6
@@ -54,41 +53,41 @@
         drop_last_loader=False,
         random_seed=1,
         alias=None,
         optimizer=None,
         optimizer_kwargs=None,
         **trainer_kwargs,
     ):
-        super(BaseModel, self).__init__()
-
-        self.save_hyperparameters()  # Allows instantiation from a checkpoint from class
-        self.random_seed = random_seed
-        pl.seed_everything(self.random_seed, workers=True)
+        super().__init__(
+            random_seed=random_seed,
+            loss=loss,
+            valid_loss=valid_loss,
+            optimizer=optimizer,
+            optimizer_kwargs=optimizer_kwargs,
+            futr_exog_list=futr_exog_list,
+            hist_exog_list=hist_exog_list,
+            stat_exog_list=stat_exog_list,
+            max_steps=max_steps,
+            early_stop_patience_steps=early_stop_patience_steps,
+            **trainer_kwargs,
+        )
 
         # Padder to complete train windows,
         # example y=[1,2,3,4,5] h=3 -> last y_output = [5,0,0]
         self.h = h
         self.input_size = input_size
+        self.windows_batch_size = windows_batch_size
         self.start_padding_enabled = start_padding_enabled
         if start_padding_enabled:
             self.padder_train = nn.ConstantPad1d(
                 padding=(self.input_size - 1, self.h), value=0
             )
         else:
             self.padder_train = nn.ConstantPad1d(padding=(0, self.h), value=0)
 
-        # Loss
-        self.loss = loss
-        if valid_loss is None:
-            self.valid_loss = loss
-        else:
-            self.valid_loss = valid_loss
-        self.train_trajectories = []
-        self.valid_trajectories = []
-
         # Batch sizes
         self.batch_size = batch_size
         if valid_batch_size is None:
             self.valid_batch_size = batch_size
         else:
             self.valid_batch_size = valid_batch_size
         if inference_windows_batch_size is None:
@@ -103,26 +102,15 @@
         self.lr_decay_steps = (
             max(max_steps // self.num_lr_decays, 1) if self.num_lr_decays > 0 else 10e7
         )
         self.early_stop_patience_steps = early_stop_patience_steps
         self.val_check_steps = val_check_steps
         self.windows_batch_size = windows_batch_size
         self.step_size = step_size
-        # custom optimizer defined by user
-        if optimizer is not None and not issubclass(optimizer, torch.optim.Optimizer):
-            raise TypeError(
-                "optimizer is not a valid subclass of torch.optim.Optimizer"
-            )
-        self.optimizer = optimizer
-        self.optimizer_kwargs = optimizer_kwargs if optimizer_kwargs else {}
-
-        # Variables
-        self.futr_exog_list = list(futr_exog_list) if futr_exog_list is not None else []
-        self.hist_exog_list = list(hist_exog_list) if hist_exog_list is not None else []
-        self.stat_exog_list = list(stat_exog_list) if stat_exog_list is not None else []
+
         self.exclude_insample_y = exclude_insample_y
 
         # Scaler
         self.scaler = TemporalNorm(
             scaler_type=scaler_type,
             dim=1,  # Time dimension is 1.
             num_features=1 + len(self.hist_exog_list) + len(self.futr_exog_list),
@@ -131,43 +119,14 @@
         # Fit arguments
         self.val_size = 0
         self.test_size = 0
 
         # Model state
         self.decompose_forecast = False
 
-        ## Trainer arguments ##
-        # Max steps, validation steps and check_val_every_n_epoch
-        trainer_kwargs = {**trainer_kwargs, **{"max_steps": max_steps}}
-
-        if "max_epochs" in trainer_kwargs.keys():
-            raise Exception("max_epochs is deprecated, use max_steps instead.")
-
-        # Callbacks
-        if "callbacks" not in trainer_kwargs and self.early_stop_patience_steps > 0:
-            trainer_kwargs["callbacks"] = [
-                EarlyStopping(
-                    monitor="ptl/val_loss", patience=self.early_stop_patience_steps
-                )
-            ]
-
-        # Add GPU accelerator if available
-        if trainer_kwargs.get("accelerator", None) is None:
-            if torch.cuda.is_available():
-                trainer_kwargs["accelerator"] = "gpu"
-        if trainer_kwargs.get("devices", None) is None:
-            if torch.cuda.is_available():
-                trainer_kwargs["devices"] = -1
-
-        # Avoid saturating local memory, disabled fit model checkpoints
-        if trainer_kwargs.get("enable_checkpointing", None) is None:
-            trainer_kwargs["enable_checkpointing"] = False
-
-        self.trainer_kwargs = trainer_kwargs
-
         # DataModule arguments
         self.num_workers_loader = num_workers_loader
         self.drop_last_loader = drop_last_loader
         # used by on_validation_epoch_end hook
         self.validation_step_outputs = []
         self.alias = alias
 
@@ -643,15 +602,22 @@
                     temporal_cols=batch["temporal_cols"],
                     y_idx=y_idx,
                 )
             y_hats.append(y_hat)
         y_hat = torch.cat(y_hats, dim=0)
         return y_hat
 
-    def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
+    def fit(
+        self,
+        dataset,
+        val_size=0,
+        test_size=0,
+        random_seed=None,
+        distributed_config=None,
+    ):
         """Fit.
 
         The `fit` method, optimizes the neural network's weights using the
         initialization parameters (`learning_rate`, `windows_batch_size`, ...)
         and the `loss` function as defined during the initialization.
         Within `fit` we use a PyTorch Lightning `Trainer` that
         inherits the initialization's `self.trainer_kwargs`, to customize
@@ -672,14 +638,15 @@
         return self._fit(
             dataset=dataset,
             batch_size=self.batch_size,
             valid_batch_size=self.valid_batch_size,
             val_size=val_size,
             test_size=test_size,
             random_seed=random_seed,
+            distributed_config=distributed_config,
         )
 
     def predict(
         self,
         dataset,
         test_size=None,
         step_size=1,
```

### Comparing `neuralforecast-1.7.0/neuralforecast/common/_modules.py` & `neuralforecast-1.7.1/neuralforecast/common/_modules.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/common/_scalers.py` & `neuralforecast-1.7.1/neuralforecast/common/_scalers.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/core.py` & `neuralforecast-1.7.1/neuralforecast/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     LocalMinMaxScaler,
     LocalRobustScaler,
     LocalStandardScaler,
 )
 from utilsforecast.compat import DataFrame, Series, pl_DataFrame, pl_Series
 from utilsforecast.validation import validate_freq
 
-from .tsdataset import TimeSeriesDataset
+from .common._base_model import DistributedConfig
+from .compat import SparkDataFrame
+from .tsdataset import _FilesDataset, TimeSeriesDataset
 from neuralforecast.models import (
     GRU,
     LSTM,
     RNN,
     TCN,
     DeepAR,
     DilatedRNN,
@@ -47,14 +49,17 @@
     FEDformer,
     StemGNN,
     PatchTST,
     TimesNet,
     TimeLLM,
     TSMixer,
     TSMixerx,
+    MLPMultivariate,
+    iTransformer,
+    BiTCN,
 )
 
 # %% ../nbs/core.ipynb 5
 def _insample_times(
     times: np.ndarray,
     uids: Series,
     indptr: np.ndarray,
@@ -149,14 +154,20 @@
     "vanillatransformer": VanillaTransformer,
     "autovanillatransformer": VanillaTransformer,
     "timellm": TimeLLM,
     "tsmixer": TSMixer,
     "autotsmixer": TSMixer,
     "tsmixerx": TSMixerx,
     "autotsmixerx": TSMixerx,
+    "mlpmultivariate": MLPMultivariate,
+    "automlpmultivariate": MLPMultivariate,
+    "itransformer": iTransformer,
+    "autoitransformer": iTransformer,
+    "bitcn": BiTCN,
+    "autobitcn": BiTCN,
 }
 
 # %% ../nbs/core.ipynb 8
 _type2scaler = {
     "standard": LocalStandardScaler,
     "robust": lambda: LocalRobustScaler(scale="mad"),
     "robust-iqr": lambda: LocalRobustScaler(scale="iqr"),
@@ -300,35 +311,36 @@
                     cols_with_nans.append(col)
 
         if cols_with_nans:
             raise ValueError(f"Found missing values in {cols_with_nans}.")
 
     def fit(
         self,
-        df: Optional[DataFrame] = None,
-        static_df: Optional[DataFrame] = None,
+        df: Optional[Union[DataFrame, SparkDataFrame]] = None,
+        static_df: Optional[Union[DataFrame, SparkDataFrame]] = None,
         val_size: Optional[int] = 0,
         sort_df: bool = True,
         use_init_models: bool = False,
         verbose: bool = False,
         id_col: str = "unique_id",
         time_col: str = "ds",
         target_col: str = "y",
+        distributed_config: Optional[DistributedConfig] = None,
     ) -> None:
         """Fit the core.NeuralForecast.
 
         Fit `models` to a large set of time series from DataFrame `df`.
         and store fitted models for later inspection.
 
         Parameters
         ----------
-        df : pandas or polars DataFrame, optional (default=None)
+        df : pandas, polars or spark DataFrame, optional (default=None)
             DataFrame with columns [`unique_id`, `ds`, `y`] and exogenous variables.
             If None, a previously stored dataset is required.
-        static_df : pandas or polars DataFrame, optional (default=None)
+        static_df : pandas, polars or spark DataFrame, optional (default=None)
             DataFrame with columns [`unique_id`] and static exogenous.
         val_size : int, optional (default=0)
             Size of validation set.
         sort_df : bool, optional (default=False)
             Sort `df` before fitting.
         use_init_models : bool, optional (default=False)
             Use initial model passed when NeuralForecast object was instantiated.
@@ -336,14 +348,16 @@
             Print processing steps.
         id_col : str (default='unique_id')
             Column that identifies each serie.
         time_col : str (default='ds')
             Column that identifies each timestep, its values can be timestamps or integers.
         target_col : str (default='y')
             Column that contains the target.
+        distributed_config : neuralforecast.DistributedConfig
+            Configuration to use for DDP training. Currently only spark is supported.
 
         Returns
         -------
         self : NeuralForecast
             Returns `NeuralForecast` class with fitted `models`.
         """
         if (df is None) and not (hasattr(self, "dataset")):
@@ -352,42 +366,94 @@
         # Model and datasets interactions protections
         if (any(model.early_stop_patience_steps > 0 for model in self.models)) and (
             val_size == 0
         ):
             raise Exception("Set val_size>0 if early stopping is enabled.")
 
         # Process and save new dataset (in self)
-        if df is not None:
+        if isinstance(df, (pd.DataFrame, pl_DataFrame)):
             validate_freq(df[time_col], self.freq)
             self.dataset, self.uids, self.last_dates, self.ds = self._prepare_fit(
                 df=df,
                 static_df=static_df,
                 sort_df=sort_df,
                 predict_only=False,
                 id_col=id_col,
                 time_col=time_col,
                 target_col=target_col,
             )
             self.sort_df = sort_df
-        else:
+        elif isinstance(df, SparkDataFrame):
+            if distributed_config is None:
+                raise ValueError(
+                    "Must set `distributed_config` when using a spark dataframe"
+                )
+            if self.local_scaler_type is not None:
+                raise ValueError(
+                    "Historic scaling isn't supported in distributed. "
+                    "Please open an issue if this would be valuable to you."
+                )
+            temporal_cols = [c for c in df.columns if c not in (id_col, time_col)]
+            if static_df is not None:
+                if not isinstance(static_df, SparkDataFrame):
+                    raise ValueError(
+                        "`static_df` must be a spark dataframe when `df` is a spark dataframe."
+                    )
+                static_cols = [c for c in static_df.columns if c != id_col]
+                df = df.join(static_df, on=[id_col], how="left")
+            else:
+                static_cols = None
+            self.id_col = id_col
+            self.time_col = time_col
+            self.target_col = target_col
+            self.scalers_ = {}
+            self.sort_df = sort_df
+            num_partitions = distributed_config.num_nodes * distributed_config.devices
+            df = df.repartitionByRange(num_partitions, id_col)
+            df.write.parquet(path=distributed_config.partitions_path, mode="overwrite")
+            fs, _, _ = fsspec.get_fs_token_paths(distributed_config.partitions_path)
+            protocol = fs.protocol
+            if isinstance(protocol, tuple):
+                protocol = protocol[0]
+            files = [
+                f"{protocol}://{file}"
+                for file in fs.ls(distributed_config.partitions_path)
+                if file.endswith("parquet")
+            ]
+            self.dataset = _FilesDataset(
+                files=files,
+                temporal_cols=temporal_cols,
+                static_cols=static_cols,
+                id_col=id_col,
+                time_col=time_col,
+                target_col=target_col,
+                min_size=df.groupBy(id_col).count().agg({"count": "min"}).first()[0],
+            )
+        elif df is None:
             if verbose:
                 print("Using stored dataset.")
+        else:
+            raise ValueError(
+                f"`df` must be a pandas, polars or spark DataFrame or `None`, got: {type(df)}"
+            )
 
         if val_size is not None:
             if self.dataset.min_size < val_size:
                 warnings.warn(
                     "Validation set size is larger than the shorter time-series."
                 )
 
         # Recover initial model if use_init_models
         if use_init_models:
             self._reset_models()
 
-        for model in self.models:
-            model.fit(self.dataset, val_size=val_size)
+        for i, model in enumerate(self.models):
+            self.models[i] = model.fit(
+                self.dataset, val_size=val_size, distributed_config=distributed_config
+            )
 
         self._fitted = True
 
     def make_future_dataframe(self, df: Optional[DataFrame] = None) -> DataFrame:
         """Create a dataframe with all ids and future times in the forecasting horizon.
 
         Parameters
@@ -438,40 +504,54 @@
         return ufp.anti_join(expected, futr_df[ids], on=ids)
 
     def _get_needed_futr_exog(self):
         return set(
             chain.from_iterable(getattr(m, "futr_exog_list", []) for m in self.models)
         )
 
+    def _get_model_names(self) -> List[str]:
+        names: List[str] = []
+        count_names = {"model": 0}
+        for model in self.models:
+            model_name = repr(model)
+            count_names[model_name] = count_names.get(model_name, -1) + 1
+            if count_names[model_name] > 0:
+                model_name += str(count_names[model_name])
+            names.extend(model_name + n for n in model.loss.output_names)
+        return names
+
     def predict(
         self,
-        df: Optional[DataFrame] = None,
-        static_df: Optional[DataFrame] = None,
-        futr_df: Optional[DataFrame] = None,
+        df: Optional[Union[DataFrame, SparkDataFrame]] = None,
+        static_df: Optional[Union[DataFrame, SparkDataFrame]] = None,
+        futr_df: Optional[Union[DataFrame, SparkDataFrame]] = None,
         sort_df: bool = True,
         verbose: bool = False,
+        engine=None,
         **data_kwargs,
     ):
         """Predict with core.NeuralForecast.
 
         Use stored fitted `models` to predict large set of time series from DataFrame `df`.
 
         Parameters
         ----------
-        df : pandas or polars DataFrame, optional (default=None)
+        df : pandas, polars or spark DataFrame, optional (default=None)
             DataFrame with columns [`unique_id`, `ds`, `y`] and exogenous variables.
             If a DataFrame is passed, it is used to generate forecasts.
-        static_df : pandas or polars DataFrame, optional (default=None)
+        static_df : pandas, polars or spark DataFrame, optional (default=None)
             DataFrame with columns [`unique_id`] and static exogenous.
-        futr_df : pandas or polars DataFrame, optional (default=None)
+        futr_df : pandas, polars or spark DataFrame, optional (default=None)
             DataFrame with [`unique_id`, `ds`] columns and `df`'s future exogenous.
         sort_df : bool (default=True)
             Sort `df` before fitting.
         verbose : bool (default=False)
             Print processing steps.
+        engine : spark session
+            Distributed engine for inference. Only used if df is a spark dataframe or if fit was called on a spark dataframe.
         data_kwargs : kwargs
             Extra arguments to be passed to the dataset within each model.
 
         Returns
         -------
         fcsts_df : pandas or polars DataFrame
             DataFrame with insample `models` columns for point predictions and probabilistic
@@ -493,14 +573,129 @@
             else:
                 missing = needed_futr_exog - set(futr_df.columns)
                 if missing:
                     raise ValueError(
                         f"The following features are missing from `futr_df`: {missing}"
                     )
 
+        # distributed df or NeuralForecast instance was trained with a distributed input and no df is provided
+        # we assume the user wants to perform distributed inference as well
+        if isinstance(df, SparkDataFrame) or (
+            df is None and isinstance(getattr(self, "dataset", None), _FilesDataset)
+        ):
+            import fugue.api as fa
+
+            def _predict(
+                df: pd.DataFrame,
+                static_cols,
+                futr_exog_cols,
+                models,
+                freq,
+                id_col,
+                time_col,
+                target_col,
+            ) -> pd.DataFrame:
+                from neuralforecast import NeuralForecast
+
+                nf = NeuralForecast(models=models, freq=freq)
+                nf.id_col = id_col
+                nf.time_col = time_col
+                nf.target_col = target_col
+                nf.scalers_ = {}
+                nf._fitted = True
+                if futr_exog_cols:
+                    # if we have futr_exog we'll have extra rows with the future values
+                    futr_rows = df[target_col].isnull()
+                    futr_df = df.loc[
+                        futr_rows, [self.id_col, self.time_col] + futr_exog_cols
+                    ].copy()
+                    df = df[~futr_rows].copy()
+                else:
+                    futr_df = None
+                if static_cols:
+                    static_df = (
+                        df[[self.id_col] + static_cols]
+                        .groupby(self.id_col, observed=True)
+                        .head(1)
+                    )
+                    df = df.drop(columns=static_cols)
+                else:
+                    static_df = None
+                preds = nf.predict(df=df, static_df=static_df, futr_df=futr_df)
+                if preds.index.name == id_col:
+                    preds = preds.reset_index()
+                return preds
+
+            # df
+            if isinstance(df, SparkDataFrame):
+                repartition = True
+            else:
+                if engine is None:
+                    raise ValueError("engine is required for distributed inference")
+                df = engine.read.parquet(*self.dataset.files)
+                # we save the datataset with partitioning
+                repartition = False
+
+            # static
+            static_cols = set(
+                chain.from_iterable(
+                    getattr(m, "stat_exog_list", []) for m in self.models
+                )
+            )
+            if static_df is not None:
+                if not isinstance(static_df, SparkDataFrame):
+                    raise ValueError(
+                        "`static_df` must be a spark dataframe when `df` is a spark dataframe "
+                        "or the models were trained in a distributed setting.\n"
+                        "You can also provide local dataframes (pandas or polars) as `df` and `static_df`."
+                    )
+                missing_static = static_cols - set(static_df.columns)
+                if missing_static:
+                    raise ValueError(
+                        f"The following static columns are missing from the static_df: {missing_static}"
+                    )
+                # join is supposed to preserve the partitioning
+                df = df.join(static_df, on=[self.id_col], how="left")
+
+            # exog
+            if futr_df is not None:
+                if not isinstance(futr_df, SparkDataFrame):
+                    raise ValueError(
+                        "`futr_df` must be a spark dataframe when `df` is a spark dataframe "
+                        "or the models were trained in a distributed setting.\n"
+                        "You can also provide local dataframes (pandas or polars) as `df` and `futr_df`."
+                    )
+                if self.target_col in futr_df.columns:
+                    raise ValueError("`futr_df` must not contain the target column.")
+                # df has the statics, historic exog and target at this point, futr_df doesnt
+                df = df.unionByName(futr_df, allowMissingColumns=True)
+                # union doesn't guarantee preserving the partitioning
+                repartition = True
+
+            if repartition:
+                df = df.repartitionByRange(df.rdd.getNumPartitions(), self.id_col)
+
+            # predict
+            base_schema = fa.get_schema(df).extract([self.id_col, self.time_col])
+            models_schema = {model: "float" for model in self._get_model_names()}
+            return fa.transform(
+                df=df,
+                using=_predict,
+                schema=base_schema.append(models_schema),
+                params=dict(
+                    static_cols=list(static_cols),
+                    futr_exog_cols=list(needed_futr_exog),
+                    models=self.models,
+                    freq=self.freq,
+                    id_col=self.id_col,
+                    time_col=self.time_col,
+                    target_col=self.target_col,
+                ),
+            )
+
         # Process new dataset but does not store it.
         if df is not None:
             validate_freq(df[self.time_col], self.freq)
             dataset, uids, last_dates, _ = self._prepare_fit(
                 df=df,
                 static_df=static_df,
                 sort_df=sort_df,
@@ -512,22 +707,15 @@
         else:
             dataset = self.dataset
             uids = self.uids
             last_dates = self.last_dates
             if verbose:
                 print("Using stored dataset.")
 
-        cols = []
-        count_names = {"model": 0}
-        for model in self.models:
-            model_name = repr(model)
-            count_names[model_name] = count_names.get(model_name, -1) + 1
-            if count_names[model_name] > 0:
-                model_name += str(count_names[model_name])
-            cols += [model_name + n for n in model.loss.output_names]
+        cols = self._get_model_names()
 
         # Placeholder dataframe for predictions with unique_id and ds
         fcsts_df = ufp.make_future_dataframe(
             uids=uids,
             last_times=last_dates,
             freq=self.freq,
             h=self.h,
@@ -779,14 +967,20 @@
                 raise Exception("`test_size - h` should be module `step_size`")
             n_windows = int((test_size - h) / step_size) + 1
         else:
             raise Exception("you must define `n_windows` or `test_size` but not both")
         # Recover initial model if use_init_models.
         if use_init_models:
             self._reset_models()
+        if isinstance(df, pd.DataFrame) and df.index.name == id_col:
+            warnings.warn(
+                "Passing the id as index is deprecated, please provide it as a column instead.",
+                FutureWarning,
+            )
+            df = df.reset_index(id_col)
         if not refit:
             return self._no_refit_cross_validation(
                 df=df,
                 static_df=static_df,
                 n_windows=n_windows,
                 step_size=step_size,
                 val_size=val_size,
@@ -1011,70 +1205,83 @@
         if path[-1] == "/":
             path = path[:-1]
 
         # Model index list
         if model_index is None:
             model_index = list(range(len(self.models)))
 
-        fs, _, paths = fsspec.get_fs_token_paths(path)
+        fs, _, _ = fsspec.get_fs_token_paths(path)
         if not fs.exists(path):
             fs.makedirs(path)
         else:
             # Check if directory is empty to protect overwriting files
-            dir = fs.ls(path)
+            files = fs.ls(path)
 
             # Checking if the list is empty or not
-            if dir and not overwrite:
-                raise Exception(
-                    "Directory is not empty. Set `overwrite=True` to overwrite files."
-                )
+            if files:
+                if not overwrite:
+                    raise Exception(
+                        "Directory is not empty. Set `overwrite=True` to overwrite files."
+                    )
+                else:
+                    fs.rm(path, recursive=True)
+                    fs.mkdir(path)
 
         # Save models
         count_names = {"model": 0}
         alias_to_model = {}
         for i, model in enumerate(self.models):
             # Skip model if not in list
             if i not in model_index:
                 continue
 
-            model_name = repr(model).lower().replace("_", "")
+            model_name = repr(model)
             model_class_name = model.__class__.__name__.lower()
-            if model_name != model_class_name:
-                alias_to_model[model_name] = model_class_name
+            alias_to_model[model_name] = model_class_name
             count_names[model_name] = count_names.get(model_name, -1) + 1
             model.save(f"{path}/{model_name}_{count_names[model_name]}.ckpt")
-        if alias_to_model:
-            with fsspec.open(f"{path}/alias_to_model.pkl", "wb") as f:
-                pickle.dump(alias_to_model, f)
+        with fsspec.open(f"{path}/alias_to_model.pkl", "wb") as f:
+            pickle.dump(alias_to_model, f)
 
         # Save dataset
-        if (save_dataset) and (hasattr(self, "dataset")):
+        if save_dataset and hasattr(self, "dataset"):
+            if isinstance(self.dataset, _FilesDataset):
+                raise ValueError(
+                    "Cannot save distributed dataset.\n"
+                    "You can set `save_dataset=False` and use the `df` argument in the predict method after loading "
+                    "this model to use it for inference."
+                )
             with fsspec.open(f"{path}/dataset.pkl", "wb") as f:
                 pickle.dump(self.dataset, f)
         elif save_dataset:
             raise Exception(
                 "You need to have a stored dataset to save it, \
                              set `save_dataset=False` to skip saving dataset."
             )
 
         # Save configuration and parameters
         config_dict = {
             "h": self.h,
             "freq": self.freq,
-            "uids": self.uids,
-            "last_dates": self.last_dates,
-            "ds": self.ds,
             "sort_df": self.sort_df,
             "_fitted": self._fitted,
             "local_scaler_type": self.local_scaler_type,
             "scalers_": self.scalers_,
             "id_col": self.id_col,
             "time_col": self.time_col,
             "target_col": self.target_col,
         }
+        if save_dataset:
+            config_dict.update(
+                {
+                    "uids": self.uids,
+                    "last_dates": self.last_dates,
+                    "ds": self.ds,
+                }
+            )
 
         with fsspec.open(f"{path}/configuration.pkl", "wb") as f:
             pickle.dump(config_dict, f)
 
     @staticmethod
     def load(path, verbose=False, **kwargs):
         """Load NeuralForecast
@@ -1094,15 +1301,15 @@
         result : NeuralForecast
             Instantiated `NeuralForecast` class.
         """
         # Standarize path without '/'
         if path[-1] == "/":
             path = path[:-1]
 
-        fs, _, paths = fsspec.get_fs_token_paths(path)
+        fs, _, _ = fsspec.get_fs_token_paths(path)
         files = [f.split("/")[-1] for f in fs.ls(path) if fs.isfile(f)]
 
         # Load models
         models_ckpt = [f for f in files if f.endswith(".ckpt")]
         if len(models_ckpt) == 0:
             raise Exception("No model found in directory.")
 
@@ -1111,21 +1318,21 @@
         models = []
         try:
             with fsspec.open(f"{path}/alias_to_model.pkl", "rb") as f:
                 alias_to_model = pickle.load(f)
         except FileNotFoundError:
             alias_to_model = {}
         for model in models_ckpt:
-            model_name = model.split("_")[0]
+            model_name = "_".join(model.split("_")[:-1])
             model_class_name = alias_to_model.get(model_name, model_name)
-            models.append(
-                MODEL_FILENAME_DICT[model_class_name].load_from_checkpoint(
-                    f"{path}/{model}", **kwargs
-                )
+            loaded_model = MODEL_FILENAME_DICT[model_class_name].load(
+                f"{path}/{model}", **kwargs
             )
+            loaded_model.alias = model_name
+            models.append(loaded_model)
             if verbose:
                 print(f"Model {model_name} loaded.")
 
         if verbose:
             print(10 * "-" + " Loading dataset " + 10 * "-")
         # Load dataset
         try:
```

### Comparing `neuralforecast-1.7.0/neuralforecast/losses/numpy.py` & `neuralforecast-1.7.1/neuralforecast/losses/numpy.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/losses/pytorch.py` & `neuralforecast-1.7.1/neuralforecast/losses/pytorch.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/__init__.py` & `neuralforecast-1.7.1/neuralforecast/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 __all__ = ['RNN', 'GRU', 'LSTM', 'TCN', 'DeepAR', 'DilatedRNN',
            'MLP', 'NHITS', 'NBEATS', 'NBEATSx', 'DLinear', 'NLinear',
            'TFT', 'VanillaTransformer', 'Informer', 'Autoformer', 'PatchTST', 'FEDformer',
-           'StemGNN', 'HINT', 'TimesNet', 'TimeLLM', 'TSMixer', 'TSMixerx']
+           'StemGNN', 'HINT', 'TimesNet', 'TimeLLM', 'TSMixer', 'TSMixerx', 'MLPMultivariate',
+           'iTransformer', 'BiTCN',
+           ]
 
 from .rnn import RNN
 from .gru import GRU
 from .lstm import LSTM
 from .tcn import TCN
 from .deepar import DeepAR
 from .dilated_rnn import DilatedRNN
@@ -22,8 +24,12 @@
 from .autoformer import Autoformer
 from .fedformer import FEDformer
 from .patchtst import PatchTST
 from .hint import HINT
 from .timesnet import TimesNet
 from .timellm import TimeLLM
 from .tsmixer import TSMixer
-from .tsmixerx import TSMixerx
+from .tsmixerx import TSMixerx
+from .mlpmultivariate import MLPMultivariate
+from .itransformer import iTransformer
+from .bitcn import BiTCN
+
```

### Comparing `neuralforecast-1.7.0/neuralforecast/models/autoformer.py` & `neuralforecast-1.7.1/neuralforecast/models/autoformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/deepar.py` & `neuralforecast-1.7.1/neuralforecast/models/deepar.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 
 # %% ../../nbs/models.deepar.ipynb 4
 import numpy as np
 
 import torch
 import torch.nn as nn
 
-import logging
-import warnings
-
-logging.getLogger("pytorch_lightning").setLevel(logging.ERROR)
-warnings.filterwarnings("ignore")
-
 from typing import Optional
 
 from ..common._base_windows import BaseWindows
 from ..losses.pytorch import DistributionLoss, MQLoss
 
 # %% ../../nbs/models.deepar.ipynb 7
 class Decoder(nn.Module):
```

### Comparing `neuralforecast-1.7.0/neuralforecast/models/dilated_rnn.py` & `neuralforecast-1.7.1/neuralforecast/models/dilated_rnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/dlinear.py` & `neuralforecast-1.7.1/neuralforecast/models/dlinear.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/fedformer.py` & `neuralforecast-1.7.1/neuralforecast/models/fedformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/gru.py` & `neuralforecast-1.7.1/neuralforecast/models/gru.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/hint.py` & `neuralforecast-1.7.1/neuralforecast/models/hint.py`

 * *Files 8% similar despite different names*

```diff
@@ -180,15 +180,22 @@
         qs = torch.Tensor((np.arange(self.loss.num_samples) / self.loss.num_samples))
         self.sample_quantiles = torch.nn.Parameter(qs, requires_grad=False)
         self.alias = alias
 
     def __repr__(self):
         return type(self).__name__ if self.alias is None else self.alias
 
-    def fit(self, dataset, val_size=0, test_size=0, random_seed=None):
+    def fit(
+        self,
+        dataset,
+        val_size=0,
+        test_size=0,
+        random_seed=None,
+        distributed_config=None,
+    ):
         """HINT.fit
 
         HINT trains on the entire hierarchical dataset, by minimizing a composite log likelihood objective.
         HINT framework integrates `TemporalNorm` into the neural forecast architecture for a scale-decoupled
         optimization that robustifies cross-learning the hierachy's series scales.
 
         **Parameters:**<br>
@@ -196,25 +203,27 @@
         `val_size`: int, size of the validation set, (default 0).<br>
         `test_size`: int, size of the test set, (default 0).<br>
         `random_seed`: int, random seed for the prediction.<br>
 
         **Returns:**<br>
         `self`: A fitted base `NeuralForecast` model.<br>
         """
-        self.model.fit(
+        model = self.model.fit(
             dataset=dataset,
             val_size=val_size,
             test_size=test_size,
             random_seed=random_seed,
+            distributed_config=distributed_config,
         )
 
         # Added attributes for compatibility with NeuralForecast core
         self.futr_exog_list = self.model.futr_exog_list
         self.hist_exog_list = self.model.hist_exog_list
         self.stat_exog_list = self.model.stat_exog_list
+        return model
 
     def predict(self, dataset, step_size=1, random_seed=None, **data_module_kwargs):
         """HINT.predict
 
         After fitting a base model on the entire hierarchical dataset.
         HINT restores the hierarchical aggregation constraints using
         bootstrapped sample reconciliation.
@@ -261,20 +270,23 @@
         aux_col_idx = np.arange(len(samples))[:, None] * num_samples
         idxs = idxs + aux_col_idx
         samples = samples.flatten()[idxs]
         samples = samples.reshape(dataset.n_groups, -1, self.h, num_samples)
 
         # Bootstrap Sample Reconciliation
         # Default output [mean, quantiles]
-        samples = np.einsum("ij,jwhp->iwhp", self.SP, samples)
+        samples = np.einsum("ij, jwhp -> iwhp", self.SP, samples)
+
+        sample_mean = np.mean(samples, axis=-1, keepdims=True)
+        sample_mean = sample_mean.reshape(-1, 1)
+
         forecasts = np.quantile(samples, self.model.loss.quantiles, axis=-1)
         forecasts = forecasts.transpose(1, 2, 3, 0)  # [...,samples]
         forecasts = forecasts.reshape(-1, len(self.model.loss.quantiles))
 
-        sample_mean = np.mean(forecasts, axis=-1, keepdims=True)
         forecasts = np.concatenate([sample_mean, forecasts], axis=-1)
         return forecasts
 
     def set_test_size(self, test_size):
         self.model.test_size = test_size
 
     def get_test_size(self):
@@ -284,8 +296,8 @@
         """HINT.save
 
         Save the HINT fitted model to disk.
 
         **Parameters:**<br>
         `path`: str, path to save the model.<br>
         """
-        self.model.trainer.save_checkpoint(path)
+        self.model.save(path)
```

### Comparing `neuralforecast-1.7.0/neuralforecast/models/informer.py` & `neuralforecast-1.7.1/neuralforecast/models/informer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/lstm.py` & `neuralforecast-1.7.1/neuralforecast/models/lstm.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/mlp.py` & `neuralforecast-1.7.1/neuralforecast/models/mlp.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/nbeats.py` & `neuralforecast-1.7.1/neuralforecast/models/nbeats.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/nbeatsx.py` & `neuralforecast-1.7.1/neuralforecast/models/nbeatsx.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/nhits.py` & `neuralforecast-1.7.1/neuralforecast/models/nhits.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/nlinear.py` & `neuralforecast-1.7.1/neuralforecast/models/nlinear.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/patchtst.py` & `neuralforecast-1.7.1/neuralforecast/models/patchtst.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/rnn.py` & `neuralforecast-1.7.1/neuralforecast/models/rnn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/stemgnn.py` & `neuralforecast-1.7.1/neuralforecast/models/stemgnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/models.stemgnn.ipynb.
 
 # %% auto 0
 __all__ = ['GLU', 'StockBlockLayer', 'StemGNN']
 
-# %% ../../nbs/models.stemgnn.ipynb 5
+# %% ../../nbs/models.stemgnn.ipynb 6
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from ..losses.pytorch import MAE
 from ..common._base_multivariate import BaseMultivariate
 
-# %% ../../nbs/models.stemgnn.ipynb 6
+# %% ../../nbs/models.stemgnn.ipynb 7
 class GLU(nn.Module):
     def __init__(self, input_channel, output_channel):
         super(GLU, self).__init__()
         self.linear_left = nn.Linear(input_channel, output_channel)
         self.linear_right = nn.Linear(input_channel, output_channel)
 
     def forward(self, x):
         return torch.mul(self.linear_left(x), torch.sigmoid(self.linear_right(x)))
 
-# %% ../../nbs/models.stemgnn.ipynb 7
+# %% ../../nbs/models.stemgnn.ipynb 8
 class StockBlockLayer(nn.Module):
     def __init__(self, time_step, unit, multi_layer, stack_cnt=0):
         super(StockBlockLayer, self).__init__()
         self.time_step = time_step
         self.unit = unit
         self.stack_cnt = stack_cnt
         self.multi = multi_layer
@@ -123,15 +123,15 @@
         if self.stack_cnt == 0:
             backcast_short = self.backcast_short_cut(x).squeeze(1)
             backcast_source = torch.sigmoid(self.backcast(igfted) - backcast_short)
         else:
             backcast_source = None
         return forecast, backcast_source
 
-# %% ../../nbs/models.stemgnn.ipynb 8
+# %% ../../nbs/models.stemgnn.ipynb 9
 class StemGNN(BaseMultivariate):
     """StemGNN
 
     The Spectral Temporal Graph Neural Network (`StemGNN`) is a Graph-based multivariate
     time-series forecasting model. `StemGNN` jointly learns temporal dependencies and
     inter-series correlations in the spectral domain, by combining Graph Fourier Transform (GFT)
     and Discrete Fourier Transform (DFT).
@@ -354,11 +354,12 @@
         forecast = forecast.permute(0, 2, 1).contiguous()
         forecast = forecast.reshape(
             batch_size, self.h, self.loss.outputsize_multiplier * self.n_series
         )
         forecast = self.loss.domain_map(forecast)
 
         # domain_map might have squeezed the last dimension in case n_series == 1
+        # Note that this fails in case of a tuple loss, but Multivariate does not support tuple losses yet.
         if forecast.ndim == 2:
             return forecast.unsqueeze(-1)
         else:
             return forecast
```

### Comparing `neuralforecast-1.7.0/neuralforecast/models/tcn.py` & `neuralforecast-1.7.1/neuralforecast/models/tcn.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/tft.py` & `neuralforecast-1.7.1/neuralforecast/models/tft.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/models.tft.ipynb.
 
 # %% auto 0
 __all__ = ['TFT']
 
 # %% ../../nbs/models.tft.ipynb 4
+from typing import Tuple, Optional
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import LayerNorm
 
-import logging
-import warnings
-
-logging.getLogger("pytorch_lightning").setLevel(logging.ERROR)
-warnings.filterwarnings("ignore")
-
-from typing import Tuple, Optional
-
 from ..losses.pytorch import MAE
 from ..common._base_windows import BaseWindows
 
 # %% ../../nbs/models.tft.ipynb 10
 class MaybeLayerNorm(nn.Module):
     def __init__(self, output_size, hidden_size, eps):
         super().__init__()
@@ -465,14 +459,17 @@
         **trainer_kwargs
     ):
 
         # Inherit BaseWindows class
         super(TFT, self).__init__(
             h=h,
             input_size=input_size,
+            stat_exog_list=stat_exog_list,
+            hist_exog_list=hist_exog_list,
+            futr_exog_list=futr_exog_list,
             loss=loss,
             valid_loss=valid_loss,
             max_steps=max_steps,
             learning_rate=learning_rate,
             num_lr_decays=num_lr_decays,
             early_stop_patience_steps=early_stop_patience_steps,
             val_check_steps=val_check_steps,
@@ -488,19 +485,14 @@
             random_seed=random_seed,
             optimizer=optimizer,
             optimizer_kwargs=optimizer_kwargs,
             **trainer_kwargs
         )
         self.example_length = input_size + h
 
-        # Parse lists hyperparameters
-        self.stat_exog_list = [] if stat_exog_list is None else stat_exog_list
-        self.hist_exog_list = [] if hist_exog_list is None else hist_exog_list
-        self.futr_exog_list = [] if futr_exog_list is None else futr_exog_list
-
         stat_input_size = len(self.stat_exog_list)
         futr_input_size = max(len(self.futr_exog_list), 1)
         hist_input_size = len(self.hist_exog_list)
         num_historic_vars = futr_input_size + hist_input_size + tgt_size
 
         # ------------------------------- Encoders -----------------------------#
         self.embedding = TFTEmbedding(
```

### Comparing `neuralforecast-1.7.0/neuralforecast/models/timellm.py` & `neuralforecast-1.7.1/neuralforecast/models/timellm.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/timesnet.py` & `neuralforecast-1.7.1/neuralforecast/models/timesnet.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/models/tsmixer.py` & `neuralforecast-1.7.1/neuralforecast/models/tsmixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         optimizer=None,
         optimizer_kwargs=None,
         **trainer_kwargs
     ):
 
-        # Inherit BaseWindows class
+        # Inherit BaseMultivariate class
         super(TSMixer, self).__init__(
             h=h,
             input_size=input_size,
             n_series=n_series,
             futr_exog_list=futr_exog_list,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
@@ -261,11 +261,12 @@
 
         x = x.reshape(
             batch_size, self.h, self.loss.outputsize_multiplier * self.n_series
         )
         forecast = self.loss.domain_map(x)
 
         # domain_map might have squeezed the last dimension in case n_series == 1
+        # Note that this fails in case of a tuple loss, but Multivariate does not support tuple losses yet.
         if forecast.ndim == 2:
             return forecast.unsqueeze(-1)
         else:
             return forecast
```

### Comparing `neuralforecast-1.7.0/neuralforecast/models/tsmixerx.py` & `neuralforecast-1.7.1/neuralforecast/models/tsmixerx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/models.tsmixerx.ipynb.
 
 # %% auto 0
 __all__ = ['TSMixerx']
 
 # %% ../../nbs/models.tsmixerx.ipynb 5
-from typing import Optional
-
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from ..losses.pytorch import MAE
 from ..common._base_multivariate import BaseMultivariate
 
@@ -212,15 +210,15 @@
         num_workers_loader: int = 0,
         drop_last_loader: bool = False,
         optimizer=None,
         optimizer_kwargs=None,
         **trainer_kwargs
     ):
 
-        # Inherit BaseWindows class
+        # Inherit BaseMultvariate class
         super(TSMixerx, self).__init__(
             h=h,
             input_size=input_size,
             n_series=n_series,
             futr_exog_list=futr_exog_list,
             hist_exog_list=hist_exog_list,
             stat_exog_list=stat_exog_list,
@@ -421,11 +419,12 @@
                 batch_size, self.h, -1
             )  #   [B, h, n_outputs, N] -> [B, h, n_outputs * N]
 
         # Map to loss domain
         forecast = self.loss.domain_map(x)
 
         # domain_map might have squeezed the last dimension in case n_series == 1
+        # Note that this fails in case of a tuple loss, but Multivariate does not support tuple losses yet.
         if forecast.ndim == 2:
             return forecast.unsqueeze(-1)
         else:
             return forecast
```

### Comparing `neuralforecast-1.7.0/neuralforecast/models/vanillatransformer.py` & `neuralforecast-1.7.1/neuralforecast/models/vanillatransformer.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast/tsdataset.py` & `neuralforecast-1.7.1/neuralforecast/tsdataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # %% auto 0
 __all__ = ['TimeSeriesLoader', 'TimeSeriesDataset', 'TimeSeriesDataModule']
 
 # %% ../nbs/tsdataset.ipynb 4
 import warnings
 from collections.abc import Mapping
+from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 import pytorch_lightning as pl
 import torch
 import utilsforecast.processing as ufp
 from torch.utils.data import Dataset, DataLoader
@@ -338,14 +339,34 @@
         )
         ds = df[time_col].to_numpy()
         if sort_idxs is not None:
             ds = ds[sort_idxs]
         return dataset, indices, dates, ds
 
 # %% ../nbs/tsdataset.ipynb 10
+class _FilesDataset:
+    def __init__(
+        self,
+        files: List[str],
+        temporal_cols: List[str],
+        static_cols: Optional[List[str]],
+        id_col: str,
+        time_col: str,
+        target_col: str,
+        min_size: int,
+    ):
+        self.files = files
+        self.temporal_cols = pd.Index(temporal_cols)
+        self.static_cols = pd.Index(static_cols) if static_cols is not None else None
+        self.id_col = id_col
+        self.time_col = time_col
+        self.target_col = target_col
+        self.min_size = min_size
+
+# %% ../nbs/tsdataset.ipynb 11
 class TimeSeriesDataModule(pl.LightningDataModule):
 
     def __init__(
         self,
         dataset: TimeSeriesDataset,
         batch_size=32,
         valid_batch_size=1024,
@@ -385,7 +406,48 @@
         loader = TimeSeriesLoader(
             self.dataset,
             batch_size=self.valid_batch_size,
             num_workers=self.num_workers,
             shuffle=False,
         )
         return loader
+
+# %% ../nbs/tsdataset.ipynb 25
+class _DistributedTimeSeriesDataModule(TimeSeriesDataModule):
+    def __init__(
+        self,
+        dataset: _FilesDataset,
+        batch_size=32,
+        valid_batch_size=1024,
+        num_workers=0,
+        drop_last=False,
+        shuffle_train=True,
+    ):
+        super(TimeSeriesDataModule, self).__init__()
+        self.files_ds = dataset
+        self.batch_size = batch_size
+        self.valid_batch_size = valid_batch_size
+        self.num_workers = num_workers
+        self.drop_last = drop_last
+        self.shuffle_train = shuffle_train
+
+    def setup(self, stage):
+        import torch.distributed as dist
+
+        df = pd.read_parquet(self.files_ds.files[dist.get_rank()])
+        if self.files_ds.static_cols is not None:
+            static_df = (
+                df[[self.files_ds.id_col] + self.files_ds.static_cols.tolist()]
+                .groupby(self.files_ds.id_col, observed=True)
+                .head(1)
+            )
+            df = df.drop(columns=self.files_ds.static_cols)
+        else:
+            static_df = None
+        self.dataset, *_ = TimeSeriesDataset.from_df(
+            df=df,
+            static_df=static_df,
+            sort_df=True,
+            id_col=self.files_ds.id_col,
+            time_col=self.files_ds.time_col,
+            target_col=self.files_ds.target_col,
+        )
```

### Comparing `neuralforecast-1.7.0/neuralforecast/utils.py` & `neuralforecast-1.7.1/neuralforecast/utils.py`

 * *Files identical despite different names*

### Comparing `neuralforecast-1.7.0/neuralforecast.egg-info/PKG-INFO` & `neuralforecast-1.7.1/neuralforecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralforecast
-Version: 1.7.0
+Version: 1.7.1
 Summary: Time series forecasting suite using deep learning models
 Home-page: https://github.com/Nixtla/neuralforecast/
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series forecasting deep-learning
 Classifier: Development Status :: 3 - Alpha
@@ -22,14 +22,19 @@
 Requires-Dist: numpy>=1.21.6
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: torch>=2.0.0
 Requires-Dist: pytorch-lightning>=2.0.0
 Requires-Dist: ray[tune]>=2.2.0
 Requires-Dist: optuna
 Requires-Dist: utilsforecast>=0.0.25
+Provides-Extra: aws
+Requires-Dist: fsspec[s3]; extra == "aws"
+Provides-Extra: spark
+Requires-Dist: fugue; extra == "spark"
+Requires-Dist: pyspark>=3.5; extra == "spark"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: gitpython; extra == "dev"
 Requires-Dist: hyperopt; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: nbdev; extra == "dev"
```

### Comparing `neuralforecast-1.7.0/neuralforecast.egg-info/SOURCES.txt` & `neuralforecast-1.7.1/neuralforecast.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 settings.ini
 setup.py
 neuralforecast/__init__.py
 neuralforecast/_modidx.py
 neuralforecast/auto.py
+neuralforecast/compat.py
 neuralforecast/core.py
 neuralforecast/tsdataset.py
 neuralforecast/utils.py
 neuralforecast.egg-info/PKG-INFO
 neuralforecast.egg-info/SOURCES.txt
 neuralforecast.egg-info/dependency_links.txt
 neuralforecast.egg-info/entry_points.txt
@@ -26,23 +27,26 @@
 neuralforecast/common/_modules.py
 neuralforecast/common/_scalers.py
 neuralforecast/losses/__init__.py
 neuralforecast/losses/numpy.py
 neuralforecast/losses/pytorch.py
 neuralforecast/models/__init__.py
 neuralforecast/models/autoformer.py
+neuralforecast/models/bitcn.py
 neuralforecast/models/deepar.py
 neuralforecast/models/dilated_rnn.py
 neuralforecast/models/dlinear.py
 neuralforecast/models/fedformer.py
 neuralforecast/models/gru.py
 neuralforecast/models/hint.py
 neuralforecast/models/informer.py
+neuralforecast/models/itransformer.py
 neuralforecast/models/lstm.py
 neuralforecast/models/mlp.py
+neuralforecast/models/mlpmultivariate.py
 neuralforecast/models/nbeats.py
 neuralforecast/models/nbeatsx.py
 neuralforecast/models/nhits.py
 neuralforecast/models/nlinear.py
 neuralforecast/models/patchtst.py
 neuralforecast/models/rnn.py
 neuralforecast/models/stemgnn.py
```

### Comparing `neuralforecast-1.7.0/settings.ini` & `neuralforecast-1.7.1/settings.ini`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 user = Nixtla
 description = Time series forecasting suite using deep learning models
 keywords = time-series forecasting deep-learning 
 author = Nixtla
 author_email = business@nixtla.io
 copyright = Nixtla Inc.
 branch = main
-version = 1.7.0
+version = 1.7.1
 min_python = 3.8
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
 requirements = coreforecast>=0.0.6 fsspec numpy>=1.21.6 pandas>=1.3.5 torch>=2.0.0 pytorch-lightning>=2.0.0 ray[tune]>=2.2.0 optuna utilsforecast>=0.0.25
+spark_requirements = fugue pyspark>=3.5
+aws_requirements = fsspec[s3]
 dev_requirements = black gitpython hyperopt matplotlib mypy nbdev polars pre-commit pyarrow ruff s3fs transformers
 nbs_path = nbs
 doc_path = _docs
 recursive = True
 doc_host =  https://%(user)s.github.io
 doc_baseurl = /neuralforecast/
 git_url = https://github.com/%(user)s/neuralforecast/
```

### Comparing `neuralforecast-1.7.0/setup.py` & `neuralforecast-1.7.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
 py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
 
 requirements = cfg.get('requirements','').split()
+aws_requirements = cfg['aws_requirements'].split()
+spark_requirements = cfg['spark_requirements'].split()
 if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 dev_requirements = (cfg.get('dev_requirements') or '').split()
 
 setuptools.setup(
     name = 'neuralforecast',
@@ -38,15 +40,19 @@
         'Intended Audience :: ' + cfg['audience'].title(),
         'Natural Language :: ' + cfg['language'].title(),
     ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
-    extras_require={'dev': dev_requirements},
+    extras_require={
+        'aws': aws_requirements,
+        'spark': spark_requirements,
+        'dev': dev_requirements,
+    },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
     long_description = open('README.md', encoding='utf8').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     entry_points = {
         'console_scripts': cfg.get('console_scripts','').split(),
```

