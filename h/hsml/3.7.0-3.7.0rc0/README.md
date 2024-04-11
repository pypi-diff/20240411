# Comparing `tmp/hsml-3.7.0.tar.gz` & `tmp/hsml-3.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsml-3.7.0.tar", last modified: Thu Apr 11 18:09:32 2024, max compression
+gzip compressed data, was "hsml-3.7.0rc0.tar", last modified: Tue Feb  6 12:05:13 2024, max compression
```

## Comparing `hsml-3.7.0.tar` & `hsml-3.7.0rc0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/
--rw-r--r--   0     1006     1006       40 2024-04-11 18:09:27.000000 hsml-3.7.0/MANIFEST.in
--rw-r--r--   0     1006     1006     5163 2024-04-11 18:09:32.290808 hsml-3.7.0/PKG-INFO
--rw-r--r--   0     1006     1006     3398 2024-04-11 18:09:31.000000 hsml-3.7.0/README.md
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.286808 hsml-3.7.0/hsml/
--rw-r--r--   0     1006     1006     1016 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.286808 hsml-3.7.0/hsml/client/
--rw-r--r--   0     1006     1006     3896 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/__init__.py
--rw-r--r--   0     1006     1006     1876 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/auth.py
--rw-r--r--   0     1006     1006     3946 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/base.py
--rw-r--r--   0     1006     1006     2456 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/exceptions.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.286808 hsml-3.7.0/hsml/client/hopsworks/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/hopsworks/__init__.py
--rw-r--r--   0     1006     1006     3985 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/hopsworks/base.py
--rw-r--r--   0     1006     1006     2846 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/hopsworks/external.py
--rw-r--r--   0     1006     1006     7088 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/hopsworks/internal.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.286808 hsml-3.7.0/hsml/client/istio/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/istio/__init__.py
--rw-r--r--   0     1006     1006     3455 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/istio/base.py
--rw-r--r--   0     1006     1006     1663 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/istio/external.py
--rw-r--r--   0     1006     1006     6650 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/client/istio/internal.py
--rw-r--r--   0     1006     1006    10216 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/connection.py
--rw-r--r--   0     1006     1006     2701 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/constants.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.286808 hsml-3.7.0/hsml/core/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/core/__init__.py
--rw-r--r--   0     1006     1006    19702 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/core/dataset_api.py
--rw-r--r--   0     1006     1006     7327 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/core/model_api.py
--rw-r--r--   0     1006     1006     2745 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/core/model_registry_api.py
--rw-r--r--   0     1006     1006     5950 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/core/model_serving_api.py
--rw-r--r--   0     1006     1006     1775 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/core/native_hdfs_api.py
--rw-r--r--   0     1006     1006    11830 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/core/serving_api.py
--rw-r--r--   0     1006     1006     1656 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/decorators.py
--rw-r--r--   0     1006     1006     2917 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/deployable_component.py
--rw-r--r--   0     1006     1006     2946 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/deployable_component_logs.py
--rw-r--r--   0     1006     1006    14451 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/deployment.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/hsml/engine/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/engine/__init__.py
--rw-r--r--   0     1006     1006     2639 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/engine/hopsworks_engine.py
--rw-r--r--   0     1006     1006     2426 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/engine/local_engine.py
--rw-r--r--   0     1006     1006    21494 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/engine/model_engine.py
--rw-r--r--   0     1006     1006    23209 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/engine/serving_engine.py
--rw-r--r--   0     1006     1006     4405 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/inference_batcher.py
--rw-r--r--   0     1006     1006     4678 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/inference_endpoint.py
--rw-r--r--   0     1006     1006     4052 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/inference_logger.py
--rw-r--r--   0     1006     1006     4718 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/kafka_topic.py
--rw-r--r--   0     1006     1006    14977 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/model.py
--rw-r--r--   0     1006     1006     6592 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/model_registry.py
--rw-r--r--   0     1006     1006     1879 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/model_schema.py
--rw-r--r--   0     1006     1006    12755 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/model_serving.py
--rw-r--r--   0     1006     1006    15522 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/predictor.py
--rw-r--r--   0     1006     1006     5182 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/predictor_state.py
--rw-r--r--   0     1006     1006     2636 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/predictor_state_condition.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/hsml/python/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/python/__init__.py
--rw-r--r--   0     1006     1006     2330 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/python/model.py
--rw-r--r--   0     1006     1006     1150 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/python/predictor.py
--rw-r--r--   0     1006     1006     2515 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/python/signature.py
--rw-r--r--   0     1006     1006    11772 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/resources.py
--rw-r--r--   0     1006     1006     2558 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/schema.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/hsml/sklearn/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/sklearn/__init__.py
--rw-r--r--   0     1006     1006     2325 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/sklearn/model.py
--rw-r--r--   0     1006     1006      976 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/sklearn/predictor.py
--rw-r--r--   0     1006     1006     2510 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/sklearn/signature.py
--rw-r--r--   0     1006     1006     1955 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/tag.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/hsml/tensorflow/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/tensorflow/__init__.py
--rw-r--r--   0     1006     1006     2330 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/tensorflow/model.py
--rw-r--r--   0     1006     1006     1168 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/tensorflow/predictor.py
--rw-r--r--   0     1006     1006     2515 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/tensorflow/signature.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/hsml/torch/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/torch/__init__.py
--rw-r--r--   0     1006     1006     2320 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/torch/model.py
--rw-r--r--   0     1006     1006     1141 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/torch/predictor.py
--rw-r--r--   0     1006     1006     2505 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/torch/signature.py
--rw-r--r--   0     1006     1006     2986 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/transformer.py
--rw-r--r--   0     1006     1006     9842 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/util.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/hsml/utils/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/utils/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/hsml/utils/schema/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/utils/schema/__init__.py
--rw-r--r--   0     1006     1006      935 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/utils/schema/column.py
--rw-r--r--   0     1006     1006     3570 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/utils/schema/columnar_schema.py
--rw-r--r--   0     1006     1006      975 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/utils/schema/tensor.py
--rw-r--r--   0     1006     1006     2395 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/utils/schema/tensor_schema.py
--rw-r--r--   0     1006     1006      628 2024-04-11 18:09:27.000000 hsml-3.7.0/hsml/version.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.286808 hsml-3.7.0/hsml.egg-info/
--rw-r--r--   0     1006     1006     5163 2024-04-11 18:09:32.000000 hsml-3.7.0/hsml.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2009 2024-04-11 18:09:32.000000 hsml-3.7.0/hsml.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2024-04-11 18:09:32.000000 hsml-3.7.0/hsml.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      306 2024-04-11 18:09:32.000000 hsml-3.7.0/hsml.egg-info/requires.txt
--rw-r--r--   0     1006     1006       11 2024-04-11 18:09:32.000000 hsml-3.7.0/hsml.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2024-04-11 18:09:32.290808 hsml-3.7.0/setup.cfg
--rw-r--r--   0     1006     1006     2508 2024-04-11 18:09:27.000000 hsml-3.7.0/setup.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/tests/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/tests/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/tests/hsml/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/tests/hsml/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-04-11 18:09:32.290808 hsml-3.7.0/tests/hsml/core/
--rw-r--r--   0     1006     1006      605 2024-04-11 18:09:27.000000 hsml-3.7.0/tests/hsml/core/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.403120 hsml-3.7.0rc0/
+-rw-r--r--   0     1006     1006       40 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/MANIFEST.in
+-rw-r--r--   0     1006     1006     5169 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/PKG-INFO
+-rw-r--r--   0     1006     1006     3398 2024-02-06 12:05:12.000000 hsml-3.7.0rc0/README.md
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.391120 hsml-3.7.0rc0/hsml/
+-rw-r--r--   0     1006     1006     1016 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.391120 hsml-3.7.0rc0/hsml/client/
+-rw-r--r--   0     1006     1006     3896 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/__init__.py
+-rw-r--r--   0     1006     1006     1876 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/auth.py
+-rw-r--r--   0     1006     1006     3946 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/base.py
+-rw-r--r--   0     1006     1006     2456 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/exceptions.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.391120 hsml-3.7.0rc0/hsml/client/hopsworks/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/hopsworks/__init__.py
+-rw-r--r--   0     1006     1006     3985 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/hopsworks/base.py
+-rw-r--r--   0     1006     1006     2846 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/hopsworks/external.py
+-rw-r--r--   0     1006     1006     7088 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/hopsworks/internal.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.395120 hsml-3.7.0rc0/hsml/client/istio/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/istio/__init__.py
+-rw-r--r--   0     1006     1006     3455 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/istio/base.py
+-rw-r--r--   0     1006     1006     1663 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/istio/external.py
+-rw-r--r--   0     1006     1006     6650 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/client/istio/internal.py
+-rw-r--r--   0     1006     1006    10216 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/connection.py
+-rw-r--r--   0     1006     1006     2701 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/constants.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.395120 hsml-3.7.0rc0/hsml/core/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/core/__init__.py
+-rw-r--r--   0     1006     1006    19702 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/core/dataset_api.py
+-rw-r--r--   0     1006     1006     7327 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/core/model_api.py
+-rw-r--r--   0     1006     1006     2745 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/core/model_registry_api.py
+-rw-r--r--   0     1006     1006     5950 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/core/model_serving_api.py
+-rw-r--r--   0     1006     1006     1775 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/core/native_hdfs_api.py
+-rw-r--r--   0     1006     1006    11830 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/core/serving_api.py
+-rw-r--r--   0     1006     1006     1656 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/decorators.py
+-rw-r--r--   0     1006     1006     2917 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/deployable_component.py
+-rw-r--r--   0     1006     1006     2946 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/deployable_component_logs.py
+-rw-r--r--   0     1006     1006    14451 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/deployment.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.395120 hsml-3.7.0rc0/hsml/engine/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/engine/__init__.py
+-rw-r--r--   0     1006     1006     2639 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/engine/hopsworks_engine.py
+-rw-r--r--   0     1006     1006     2426 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/engine/local_engine.py
+-rw-r--r--   0     1006     1006    21494 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/engine/model_engine.py
+-rw-r--r--   0     1006     1006    23209 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/engine/serving_engine.py
+-rw-r--r--   0     1006     1006     4405 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/inference_batcher.py
+-rw-r--r--   0     1006     1006     4678 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/inference_endpoint.py
+-rw-r--r--   0     1006     1006     4052 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/inference_logger.py
+-rw-r--r--   0     1006     1006     4718 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/kafka_topic.py
+-rw-r--r--   0     1006     1006    14977 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/model.py
+-rw-r--r--   0     1006     1006     6592 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/model_registry.py
+-rw-r--r--   0     1006     1006     1879 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/model_schema.py
+-rw-r--r--   0     1006     1006    12755 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/model_serving.py
+-rw-r--r--   0     1006     1006    15522 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/predictor.py
+-rw-r--r--   0     1006     1006     5182 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/predictor_state.py
+-rw-r--r--   0     1006     1006     2636 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/predictor_state_condition.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/hsml/python/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/python/__init__.py
+-rw-r--r--   0     1006     1006     2330 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/python/model.py
+-rw-r--r--   0     1006     1006     1150 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/python/predictor.py
+-rw-r--r--   0     1006     1006     2515 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/python/signature.py
+-rw-r--r--   0     1006     1006    11772 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/resources.py
+-rw-r--r--   0     1006     1006     2558 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/schema.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/hsml/sklearn/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/sklearn/__init__.py
+-rw-r--r--   0     1006     1006     2325 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/sklearn/model.py
+-rw-r--r--   0     1006     1006      976 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/sklearn/predictor.py
+-rw-r--r--   0     1006     1006     2510 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/sklearn/signature.py
+-rw-r--r--   0     1006     1006     1955 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/tag.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/hsml/tensorflow/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/tensorflow/__init__.py
+-rw-r--r--   0     1006     1006     2330 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/tensorflow/model.py
+-rw-r--r--   0     1006     1006     1168 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/tensorflow/predictor.py
+-rw-r--r--   0     1006     1006     2515 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/tensorflow/signature.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/hsml/torch/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/torch/__init__.py
+-rw-r--r--   0     1006     1006     2320 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/torch/model.py
+-rw-r--r--   0     1006     1006     1141 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/torch/predictor.py
+-rw-r--r--   0     1006     1006     2505 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/torch/signature.py
+-rw-r--r--   0     1006     1006     2986 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/transformer.py
+-rw-r--r--   0     1006     1006     9842 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/util.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/hsml/utils/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/utils/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/hsml/utils/schema/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/utils/schema/__init__.py
+-rw-r--r--   0     1006     1006      935 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/utils/schema/column.py
+-rw-r--r--   0     1006     1006     3570 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/utils/schema/columnar_schema.py
+-rw-r--r--   0     1006     1006      975 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/utils/schema/tensor.py
+-rw-r--r--   0     1006     1006     2395 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/hsml/utils/schema/tensor_schema.py
+-rw-r--r--   0     1006     1006      631 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/hsml/version.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.391120 hsml-3.7.0rc0/hsml.egg-info/
+-rw-r--r--   0     1006     1006     5169 2024-02-06 12:05:13.000000 hsml-3.7.0rc0/hsml.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2009 2024-02-06 12:05:13.000000 hsml-3.7.0rc0/hsml.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2024-02-06 12:05:13.000000 hsml-3.7.0rc0/hsml.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      306 2024-02-06 12:05:13.000000 hsml-3.7.0rc0/hsml.egg-info/requires.txt
+-rw-r--r--   0     1006     1006       11 2024-02-06 12:05:13.000000 hsml-3.7.0rc0/hsml.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2024-02-06 12:05:13.403120 hsml-3.7.0rc0/setup.cfg
+-rw-r--r--   0     1006     1006     2508 2024-02-06 12:05:08.000000 hsml-3.7.0rc0/setup.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/tests/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/tests/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/tests/hsml/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/tests/hsml/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-02-06 12:05:13.399120 hsml-3.7.0rc0/tests/hsml/core/
+-rw-r--r--   0     1006     1006      605 2024-01-25 13:34:42.000000 hsml-3.7.0rc0/tests/hsml/core/__init__.py
```

### Comparing `hsml-3.7.0/PKG-INFO` & `hsml-3.7.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsml
-Version: 3.7.0
+Version: 3.7.0rc0
 Summary: HSML: An environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.7.0
+Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.7.0rc0
 Description: # Hopsworks Model Management
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: hsml Version: 3.7.0 Summary: HSML: An environment
-independent client to interact with the Hopsworks Model Registry Home-page:
-https://github.com/logicalclocks/machine-learning-api Author: Logical Clocks AB
-Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/machine-learning-api/releases/tag/3.7.0
-Description: # Hopsworks Model Management
+Metadata-Version: 2.1 Name: hsml Version: 3.7.0rc0 Summary: HSML: An
+environment independent client to interact with the Hopsworks Model Registry
+Home-page: https://github.com/logicalclocks/machine-learning-api Author:
+Logical Clocks AB Author-email: robin@logicalclocks.com License: Apache License
+2.0 Download-URL: https://github.com/logicalclocks/machine-learning-api/
+releases/tag/3.7.0rc0 Description: # Hopsworks Model Management
   _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _M_o_d_e_l_ _M_a_n_a_g_e_m_e_n_t_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]
              _[_S_c_a_l_a_/_J_a_v_a_ _A_r_t_i_f_a_c_t_s_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_S_t_y_l_e_][License]
 HSML is the library to interact with the Hopsworks Model Registry and Model
 Serving. The library makes it easy to export, manage and deploy models. The
 library automatically configures itself based on the environment it is run.
 However, to connect from an external Python environment additional connection
 information, such as host and port, is required. For more information about the
```

### Comparing `hsml-3.7.0/README.md` & `hsml-3.7.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/__init__.py` & `hsml-3.7.0rc0/hsml/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/__init__.py` & `hsml-3.7.0rc0/hsml/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/auth.py` & `hsml-3.7.0rc0/hsml/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/base.py` & `hsml-3.7.0rc0/hsml/client/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/exceptions.py` & `hsml-3.7.0rc0/hsml/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/hopsworks/__init__.py` & `hsml-3.7.0rc0/hsml/client/hopsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/hopsworks/base.py` & `hsml-3.7.0rc0/hsml/client/hopsworks/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/hopsworks/external.py` & `hsml-3.7.0rc0/hsml/client/hopsworks/external.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/hopsworks/internal.py` & `hsml-3.7.0rc0/hsml/client/hopsworks/internal.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/istio/__init__.py` & `hsml-3.7.0rc0/hsml/client/istio/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/istio/base.py` & `hsml-3.7.0rc0/hsml/client/istio/base.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/istio/external.py` & `hsml-3.7.0rc0/hsml/client/istio/external.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/client/istio/internal.py` & `hsml-3.7.0rc0/hsml/client/istio/internal.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/connection.py` & `hsml-3.7.0rc0/hsml/connection.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/constants.py` & `hsml-3.7.0rc0/hsml/constants.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/core/__init__.py` & `hsml-3.7.0rc0/hsml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/core/dataset_api.py` & `hsml-3.7.0rc0/hsml/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/core/model_api.py` & `hsml-3.7.0rc0/hsml/core/model_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/core/model_registry_api.py` & `hsml-3.7.0rc0/hsml/core/model_registry_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/core/model_serving_api.py` & `hsml-3.7.0rc0/hsml/core/model_serving_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/core/native_hdfs_api.py` & `hsml-3.7.0rc0/hsml/core/native_hdfs_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/core/serving_api.py` & `hsml-3.7.0rc0/hsml/core/serving_api.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/decorators.py` & `hsml-3.7.0rc0/hsml/decorators.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/deployable_component.py` & `hsml-3.7.0rc0/hsml/deployable_component.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/deployable_component_logs.py` & `hsml-3.7.0rc0/hsml/deployable_component_logs.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/deployment.py` & `hsml-3.7.0rc0/hsml/deployment.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/engine/__init__.py` & `hsml-3.7.0rc0/hsml/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/engine/hopsworks_engine.py` & `hsml-3.7.0rc0/hsml/engine/hopsworks_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/engine/local_engine.py` & `hsml-3.7.0rc0/hsml/engine/local_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/engine/model_engine.py` & `hsml-3.7.0rc0/hsml/engine/model_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/engine/serving_engine.py` & `hsml-3.7.0rc0/hsml/engine/serving_engine.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/inference_batcher.py` & `hsml-3.7.0rc0/hsml/inference_batcher.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/inference_endpoint.py` & `hsml-3.7.0rc0/hsml/inference_endpoint.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/inference_logger.py` & `hsml-3.7.0rc0/hsml/inference_logger.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/kafka_topic.py` & `hsml-3.7.0rc0/hsml/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/model.py` & `hsml-3.7.0rc0/hsml/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/model_registry.py` & `hsml-3.7.0rc0/hsml/model_registry.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/model_schema.py` & `hsml-3.7.0rc0/hsml/model_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/model_serving.py` & `hsml-3.7.0rc0/hsml/model_serving.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/predictor.py` & `hsml-3.7.0rc0/hsml/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/predictor_state.py` & `hsml-3.7.0rc0/hsml/predictor_state.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/predictor_state_condition.py` & `hsml-3.7.0rc0/hsml/predictor_state_condition.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/python/__init__.py` & `hsml-3.7.0rc0/hsml/python/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/python/model.py` & `hsml-3.7.0rc0/hsml/python/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/python/predictor.py` & `hsml-3.7.0rc0/hsml/python/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/python/signature.py` & `hsml-3.7.0rc0/hsml/python/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/resources.py` & `hsml-3.7.0rc0/hsml/resources.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/schema.py` & `hsml-3.7.0rc0/hsml/schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/sklearn/__init__.py` & `hsml-3.7.0rc0/hsml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/sklearn/model.py` & `hsml-3.7.0rc0/hsml/sklearn/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/sklearn/predictor.py` & `hsml-3.7.0rc0/hsml/sklearn/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/sklearn/signature.py` & `hsml-3.7.0rc0/hsml/sklearn/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/tag.py` & `hsml-3.7.0rc0/hsml/tag.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/tensorflow/__init__.py` & `hsml-3.7.0rc0/hsml/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/tensorflow/model.py` & `hsml-3.7.0rc0/hsml/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/tensorflow/predictor.py` & `hsml-3.7.0rc0/hsml/tensorflow/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/tensorflow/signature.py` & `hsml-3.7.0rc0/hsml/tensorflow/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/torch/__init__.py` & `hsml-3.7.0rc0/hsml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/torch/model.py` & `hsml-3.7.0rc0/hsml/torch/model.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/torch/predictor.py` & `hsml-3.7.0rc0/hsml/torch/predictor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/torch/signature.py` & `hsml-3.7.0rc0/hsml/torch/signature.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/transformer.py` & `hsml-3.7.0rc0/hsml/transformer.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/util.py` & `hsml-3.7.0rc0/hsml/util.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/utils/__init__.py` & `hsml-3.7.0rc0/hsml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/utils/schema/__init__.py` & `hsml-3.7.0rc0/hsml/utils/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/utils/schema/column.py` & `hsml-3.7.0rc0/hsml/utils/schema/column.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/utils/schema/columnar_schema.py` & `hsml-3.7.0rc0/hsml/utils/schema/columnar_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/utils/schema/tensor.py` & `hsml-3.7.0rc0/hsml/utils/schema/tensor.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/utils/schema/tensor_schema.py` & `hsml-3.7.0rc0/hsml/utils/schema/tensor_schema.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/hsml/version.py` & `hsml-3.7.0rc0/hsml/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.7.0"
+__version__ = "3.7.0rc0"
```

### Comparing `hsml-3.7.0/hsml.egg-info/PKG-INFO` & `hsml-3.7.0rc0/hsml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsml
-Version: 3.7.0
+Version: 3.7.0rc0
 Summary: HSML: An environment independent client to interact with the Hopsworks Model Registry
 Home-page: https://github.com/logicalclocks/machine-learning-api
 Author: Logical Clocks AB
 Author-email: robin@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.7.0
+Download-URL: https://github.com/logicalclocks/machine-learning-api/releases/tag/3.7.0rc0
 Description: # Hopsworks Model Management
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: hsml Version: 3.7.0 Summary: HSML: An environment
-independent client to interact with the Hopsworks Model Registry Home-page:
-https://github.com/logicalclocks/machine-learning-api Author: Logical Clocks AB
-Author-email: robin@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/machine-learning-api/releases/tag/3.7.0
-Description: # Hopsworks Model Management
+Metadata-Version: 2.1 Name: hsml Version: 3.7.0rc0 Summary: HSML: An
+environment independent client to interact with the Hopsworks Model Registry
+Home-page: https://github.com/logicalclocks/machine-learning-api Author:
+Logical Clocks AB Author-email: robin@logicalclocks.com License: Apache License
+2.0 Download-URL: https://github.com/logicalclocks/machine-learning-api/
+releases/tag/3.7.0rc0 Description: # Hopsworks Model Management
   _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _M_o_d_e_l_ _M_a_n_a_g_e_m_e_n_t_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]
              _[_S_c_a_l_a_/_J_a_v_a_ _A_r_t_i_f_a_c_t_s_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_S_t_y_l_e_][License]
 HSML is the library to interact with the Hopsworks Model Registry and Model
 Serving. The library makes it easy to export, manage and deploy models. The
 library automatically configures itself based on the environment it is run.
 However, to connect from an external Python environment additional connection
 information, such as host and port, is required. For more information about the
```

### Comparing `hsml-3.7.0/hsml.egg-info/SOURCES.txt` & `hsml-3.7.0rc0/hsml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/setup.py` & `hsml-3.7.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/tests/__init__.py` & `hsml-3.7.0rc0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/tests/hsml/__init__.py` & `hsml-3.7.0rc0/tests/hsml/__init__.py`

 * *Files identical despite different names*

### Comparing `hsml-3.7.0/tests/hsml/core/__init__.py` & `hsml-3.7.0rc0/tests/hsml/core/__init__.py`

 * *Files identical despite different names*

