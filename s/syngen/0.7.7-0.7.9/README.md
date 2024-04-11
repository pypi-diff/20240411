# Comparing `tmp/syngen-0.7.7.tar.gz` & `tmp/syngen-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.7.7.tar", last modified: Wed Feb  7 08:14:22 2024, max compression
+gzip compressed data, was "syngen-0.7.9.tar", last modified: Thu Feb  8 14:43:26 2024, max compression
```

## Comparing `syngen-0.7.7.tar` & `syngen-0.7.9.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.440914 syngen-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-07 08:12:57.000000 syngen-0.7.7/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-07 08:12:57.000000 syngen-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-07 08:12:57.000000 syngen-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-02-07 08:14:22.440914 syngen-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-02-07 08:12:57.000000 syngen-0.7.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-07 08:12:57.000000 syngen-0.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-07 08:14:22.440914 syngen-0.7.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.424915 syngen-0.7.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.428915 syngen-0.7.7/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/config/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/config/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/context/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   723528 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.432915 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/img/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/script.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46636 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/mlflow_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/mlflow_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/models/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    43114 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.436915 syngen-0.7.7/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.440914 syngen-0.7.7/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/ml/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.440914 syngen-0.7.7/src/syngen/streamlit_app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.440914 syngen-0.7.7/src/syngen/streamlit_app/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/streamlit_app/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.440914 syngen-0.7.7/src/syngen/streamlit_app/css/
--rw-r--r--   0 runner    (1001) docker     (127)   705614 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/streamlit_app/css/font_style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.440914 syngen-0.7.7/src/syngen/streamlit_app/img/
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/streamlit_app/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/streamlit_app/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-02-07 08:12:57.000000 syngen-0.7.7/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:14:22.440914 syngen-0.7.7/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-02-07 08:14:22.000000 syngen-0.7.7/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-02-07 08:14:22.000000 syngen-0.7.7/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 08:14:22.000000 syngen-0.7.7/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-07 08:14:22.000000 syngen-0.7.7/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-07 08:14:22.000000 syngen-0.7.7/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-07 08:14:22.000000 syngen-0.7.7/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-08 14:42:03.000000 syngen-0.7.9/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-08 14:42:03.000000 syngen-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-08 14:42:03.000000 syngen-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26239 2024-02-08 14:43:26.862353 syngen-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-02-08 14:42:03.000000 syngen-0.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-08 14:42:03.000000 syngen-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-08 14:43:26.866353 syngen-0.7.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.850353 syngen-0.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.854353 syngen-0.7.9/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.854353 syngen-0.7.9/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.854353 syngen-0.7.9/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/config/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/config/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.854353 syngen-0.7.9/src/syngen/ml/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.854353 syngen-0.7.9/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.854353 syngen-0.7.9/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.854353 syngen-0.7.9/src/syngen/ml/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.854353 syngen-0.7.9/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   723528 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/script.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46636 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/mlflow_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/mlflow_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.858353 syngen-0.7.9/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/models/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43114 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/ml/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen/streamlit_app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen/streamlit_app/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/streamlit_app/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen/streamlit_app/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   705614 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/streamlit_app/css/font_style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen/streamlit_app/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/streamlit_app/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10740 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/streamlit_app/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/streamlit_app/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-02-08 14:42:03.000000 syngen-0.7.9/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 14:43:26.862353 syngen-0.7.9/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26239 2024-02-08 14:43:26.000000 syngen-0.7.9/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-08 14:43:26.000000 syngen-0.7.9/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 14:43:26.000000 syngen-0.7.9/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-08 14:43:26.000000 syngen-0.7.9/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-08 14:43:26.000000 syngen-0.7.9/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-08 14:43:26.000000 syngen-0.7.9/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.7.7/LICENSE` & `syngen-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/PKG-INFO` & `syngen-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.7.7
+Version: 0.7.9
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -424,23 +424,18 @@
 
 ```bash
 pip install syngen[ui]
 ```
 then use the code below in your python file:
 
 ```python
-from syngen.streamlit_app.run import main
+from syngen import streamlit_app
 
 
-main()
-```
-and launch it with the following command:
-
-```bash
-streamlit run YOUR_PYTHON_FILE.py
+streamlit_app.start()
 ```
 
 You also can access the streamlit UI web interface by launching the container with the following command:
 
 ```bash
 docker pull tdspora/syngen
 docker run -p 8501:8501 tdspora/syngen --webui
```

### Comparing `syngen-0.7.7/README.md` & `syngen-0.7.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -365,23 +365,18 @@
 
 ```bash
 pip install syngen[ui]
 ```
 then use the code below in your python file:
 
 ```python
-from syngen.streamlit_app.run import main
+from syngen import streamlit_app
 
 
-main()
-```
-and launch it with the following command:
-
-```bash
-streamlit run YOUR_PYTHON_FILE.py
+streamlit_app.start()
 ```
 
 You also can access the streamlit UI web interface by launching the container with the following command:
 
 ```bash
 docker pull tdspora/syngen
 docker run -p 8501:8501 tdspora/syngen --webui
```

#### html2text {}

```diff
@@ -237,17 +237,16 @@
 v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \ --task=infer \ --
 metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
 arguments listed in the corresponding sections for infer and training processes
 in the CLI call, however, they will be overwritten by corresponding arguments
 in the metadata file. #### UI web interface You can access the streamlit UI web
 interface by running the following command after installing the library with
 the UI option: ```bash pip install syngen[ui] ``` then use the code below in
-your python file: ```python from syngen.streamlit_app.run import main main()
-``` and launch it with the following command: ```bash streamlit run
-YOUR_PYTHON_FILE.py ``` You also can access the streamlit UI web interface by
+your python file: ```python from syngen import streamlit_app
+streamlit_app.start() ``` You also can access the streamlit UI web interface by
 launching the container with the following command: ```bash docker pull
 tdspora/syngen docker run -p 8501:8501 tdspora/syngen --webui ``` The UI will
 be available at
 localhost:8501>. #### MLflow monitoring Set the `MLFLOW_TRACKING_URI`
 environment variable to the desired MLflow tracking server, for instance: http:
 //localhost:5000/. You can also set the `MLFLOW_ARTIFACTS_DESTINATION`
 environment variable to your preferred path (including the cloud path), where
```

### Comparing `syngen-0.7.7/setup.cfg` & `syngen-0.7.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/infer.py` & `syngen-0.7.9/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/config/configurations.py` & `syngen-0.7.9/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/config/validation.py` & `syngen-0.7.9/src/syngen/ml/config/validation.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/context/context.py` & `syngen-0.7.9/src/syngen/ml/context/context.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/convertor/convertor.py` & `syngen-0.7.9/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.7.9/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/handlers/handlers.py` & `syngen-0.7.9/src/syngen/ml/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg` & `syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/accuracy_test/src/main.css` & `syngen-0.7.9/src/syngen/ml/metrics/accuracy_test/src/main.css`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.7.9/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.7.9/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.7.9/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/metrics/utils.py` & `syngen-0.7.9/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/mlflow_tracker/mlflow_tracker.py` & `syngen-0.7.9/src/syngen/ml/mlflow_tracker/mlflow_tracker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/reporters/reporters.py` & `syngen-0.7.9/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/strategies/strategies.py` & `syngen-0.7.9/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/utils/__init__.py` & `syngen-0.7.9/src/syngen/ml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/utils/utils.py` & `syngen-0.7.9/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.7.9/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/vae/models/dataset.py` & `syngen-0.7.9/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/vae/models/features.py` & `syngen-0.7.9/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/vae/models/model.py` & `syngen-0.7.9/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.7.9/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.7.9/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/ml/worker/worker.py` & `syngen-0.7.9/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/streamlit_app/css/font_style.css` & `syngen-0.7.9/src/syngen/streamlit_app/css/font_style.css`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/streamlit_app/img/logo.svg` & `syngen-0.7.9/src/syngen/streamlit_app/img/logo.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen/streamlit_app/run.py` & `syngen-0.7.9/src/syngen/streamlit_app/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         st.session_state.running = True
         return True
     else:
         st.session_state.running = False
         return False
 
 
-def main():
+def run():
     path_to_logo = f"{os.path.join(os.path.dirname(__file__))}/img/logo.svg"
     st.set_page_config(
         page_title="SynGen UI",
         page_icon=path_to_logo
     )
     st.sidebar.image(path_to_logo, use_column_width=True)
     st.markdown(f"""
@@ -298,8 +298,8 @@
                         "Download report",
                         app.path_to_report,
                         f"accuracy_report_{app.sl_table_name}.html"
                     )
 
 
 if __name__ == "__main__":
-    main()
+    run()
```

### Comparing `syngen-0.7.7/src/syngen/train.py` & `syngen-0.7.9/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.7.7/src/syngen.egg-info/PKG-INFO` & `syngen-0.7.9/src/syngen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.7.7
+Version: 0.7.9
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -424,23 +424,18 @@
 
 ```bash
 pip install syngen[ui]
 ```
 then use the code below in your python file:
 
 ```python
-from syngen.streamlit_app.run import main
+from syngen import streamlit_app
 
 
-main()
-```
-and launch it with the following command:
-
-```bash
-streamlit run YOUR_PYTHON_FILE.py
+streamlit_app.start()
 ```
 
 You also can access the streamlit UI web interface by launching the container with the following command:
 
 ```bash
 docker pull tdspora/syngen
 docker run -p 8501:8501 tdspora/syngen --webui
```

### Comparing `syngen-0.7.7/src/syngen.egg-info/SOURCES.txt` & `syngen-0.7.9/src/syngen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,11 @@
 src/syngen/ml/vae/wrappers/wrappers.py
 src/syngen/ml/validation_schema/__init__.py
 src/syngen/ml/validation_schema/validation_schema.py
 src/syngen/ml/worker/__init__.py
 src/syngen/ml/worker/worker.py
 src/syngen/streamlit_app/__init__.py
 src/syngen/streamlit_app/run.py
+src/syngen/streamlit_app/start.py
 src/syngen/streamlit_app/.streamlit/config.toml
 src/syngen/streamlit_app/css/font_style.css
 src/syngen/streamlit_app/img/logo.svg
```

### Comparing `syngen-0.7.7/src/syngen.egg-info/requires.txt` & `syngen-0.7.9/src/syngen.egg-info/requires.txt`

 * *Files identical despite different names*

