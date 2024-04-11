# Comparing `tmp/cognitive-service-vision-model-customization-python-samples-0.0.5.tar.gz` & `tmp/cognitive-service-vision-model-customization-python-samples-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitive-service-vision-model-customization-python-samples-0.0.5.tar", last modified: Mon Jun 12 17:15:47 2023, max compression
+gzip compressed data, was "cognitive-service-vision-model-customization-python-samples-0.0.6.tar", last modified: Thu Apr 11 16:36:47 2024, max compression
```

## Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5.tar` & `cognitive-service-vision-model-customization-python-samples-0.0.6.tar`

### file list

```diff
@@ -1,50 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/training_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/training_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.123310 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 17:15:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:47.127310 cognitive-service-vision-model-customization-python-samples-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_coco_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-12 17:15:31.000000 cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.684669 cognitive-service-vision-model-customization-python-samples-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-11 16:36:47.684669 cognitive-service-vision-model-customization-python-samples-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.676669 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/adjust_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.676669 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.676669 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.676669 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/base/analyser_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/benchmarking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.680669 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/error_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/error_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/error_analysis/classification_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/error_analysis/error_analyser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.680669 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/helper_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/helper_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/helper_classes/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.680669 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/metrics/metric_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.680669 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/parsers/classification_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/common/analyser/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/aml-pipeline/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.680669 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.680669 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/training_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.684669 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.684669 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/training_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.684669 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.684669 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-11 16:36:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-11 16:36:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:36:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 16:36:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 16:36:47.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:36:47.684669 cognitive-service-vision-model-customization-python-samples-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:47.684669 cognitive-service-vision-model-customization-python-samples-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/test/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/test/test_coco_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-11 16:36:43.000000 cognitive-service-vision-model-customization-python-samples-0.0.6/test/test_e2e.py
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/LICENSE` & `cognitive-service-vision-model-customization-python-samples-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/LICENSE.md` & `cognitive-service-vision-model-customization-python-samples-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/PKG-INFO` & `cognitive-service-vision-model-customization-python-samples-0.0.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,17 @@
-Metadata-Version: 2.1
-Name: cognitive-service-vision-model-customization-python-samples
-Version: 0.0.5
-Summary: A sample code repo for model customization using Python for Cognitive Service for Vision.
-Home-page: 
-Author: Ping Jin
-License: MIT
-Keywords: vision datasets classification detection
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.md
-
 # Azure Cognitive Services Computer Vision - Python SDK Samples
 
 ## Model Customization
 
-Computer Vision's Model Customization is a custom model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding of machine learning or computer vision required.
+Computer Vision's Model Customization is a custom model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding of machine learning or computer vision required. The service is available in regions: West US 2, East US, West Europe.
 
 This is a sample repository demonstrating how to train and predict a custom model with Cognitive Service for Vision, using Python. To get started, check out [this tutorial in Python notebook](./docs/cognitive_service_vision_model_customization.ipynb).
 
+Moreover, you can use your familiar Azure Machine Learning (AML) environment and Data Science Tools (AML Data Assets or Jobs, CLIv2 or MLFlow) for training and evaluating your custom Florence model following [this documentation](./aml-pipeline/README.md).
+
 ### Product Recognition
 
 One of the scenarios we would like to introudce as a model customization scenario is Product Recognition. Computer Vision's product recognition service has been designed to be used in retail scenarios, where users would like to detect products, such as Consumer Packaged Goods (CPG), on a shelf. It comes with a set of APIs, a pre-built AI model, and a custom AI model that can be trained following the model customization guide above. You can try these out by following tutorials in Python notebooks: 
 * **[Image Composition](./docs/cognitive_service_vision_image_composition.ipynb)**: for stitching together the segmented shelf images using Image Stitching API, as well as adjusting any slanted or squished shelf images to a correct orientation using Image Rectification API
 * **[Product Recognition](./docs/cognitive_service_vision_product_recognition.ipynb)**: for detecting products and gaps on a shelf image using a pre-built model, and individually classifying the detected products using customized model, both using Product Understanding API
 * **[Planogram Compliance](./docs/cognitive_service_vision_planogram_compliance.ipynb)**: for assessing the matchings between a planogram schema and the detected products on a shelf using Planogram Compliance API
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/__init__.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/__init__.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/image_composition_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/planogram_compliance_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/product_recognition_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/clients/training_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/clients/training_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
     category_stats = {}
     for annotation in tqdm(annotations, 'Checking "annotations"...'):
         annotation_check(annotation, data_type, len(annotations), max_img_id, max_category_id)
         ann_cate_id = annotation['category_id']
         category_stats[ann_cate_id] = category_stats.get(ann_cate_id, 0) + 1
 
-    print(f'category stats {category_stats}.')
+    print(f'Number of images per category: {category_stats}.')
     for cat_id, stat in category_stats.items():
         _check(stat >= quota_limit.min_image_cnt_per_tag, f'Each category must have >= {quota_limit.min_image_cnt_per_tag} images present, only {stat} images found for category {cat_id}.')
 
 
 def check_coco_annotation_file(coco_dict: dict, data_type: str, purpose: Purpose):
     quota_limit = _get_quota_limit(data_type, purpose)
     _fields_present_and_has_value_check(coco_dict, None, 'images', 'annotations', 'categories')
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,38 @@
 from msrest.authentication import ApiKeyCredentials
 import argparse
 import time
 import json
 import pathlib
 import logging
 from azure.storage.blob import ContainerClient, BlobClient
+from azure.core.exceptions import ClientAuthenticationError
 import multiprocessing
 
 
 N_PROCESS = 8
 
 
 def get_file_name(sub_folder, image_id):
     return f'{sub_folder}/images/{image_id}'
 
 
 def blob_copy(params):
     container_client, sub_folder, image = params
     blob_client: BlobClient = container_client.get_blob_client(get_file_name(sub_folder, image.id))
-    blob_client.start_copy_from_url(image.original_image_uri)
-    return blob_client
+
+    try:
+        blob_client.start_copy_from_url(image.original_image_uri)
+        return blob_client
+    except ClientAuthenticationError as e:
+        logging.error(f'Error copying image {image.id} from {image.original_image_uri} to {blob_client.url}. Error: {e.reason}')
+    except Exception as e:
+        logging.error(f'Error copying image {image.id} from {image.original_image_uri} to {blob_client.url}. Error: {e}')
+
+    return None
 
 
 def wait_for_completion(blobs, time_out=5):
     pendings = blobs
     time_break = 0.5
     while pendings and time_out > 0:
         pendings = [b for b in pendings if b.get_blob_properties().copy.status == 'pending']
@@ -37,15 +46,20 @@
 
 
 def copy_images_with_retry(pool, container_client, sub_folder, images: List, batch_id, n_retries=5):
     retry_limit = n_retries
     urls = []
     while images and n_retries > 0:
         params = [(container_client, sub_folder, image) for image in images]
-        img_and_blobs = zip(images, pool.map(blob_copy, params))
+        blobs = pool.map(blob_copy, params)
+        if any(b is None for b in blobs):
+            raise RuntimeError(f'Copy failed for some images in batch {batch_id}. Check your provided Azure Storage information.')
+
+        img_and_blobs = zip(images, blobs)
+
         logging.info(f'Batch {batch_id}: Copied {len(images)} images.')
         urls = urls or [b.url for _, b in img_and_blobs]
 
         wait_for_completion([b for _, b in img_and_blobs])
         images = [image for image, b in img_and_blobs if b.get_blob_properties().copy.status in ['failed', 'aborted']]
         n_retries -= 1
         if images:
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/__init__.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,44 +7,46 @@
     OBJECT_DETECTION = 'imageObjectDetection'
 
     def __str__(self) -> str:
         return self.value
 
 
 class AuthenticationKind(Enum):
-    MI = 'managedIdentity',
+    MI = 'managedIdentity'
     SAS = 'sas'
 
     def __str__(self) -> str:
         return self.value
 
 
 class Authentication:
     def __init__(self, kind: AuthenticationKind = AuthenticationKind.MI, sas_token=None):
         kind = AuthenticationKind(kind) if isinstance(kind, str) else kind
         self.kind = kind
         self.sas_token = sas_token
 
     @property
     def params(self):
-        return {
-            'kind': self.kind.value,
-            'sasToken': self.sas_token
+        params = {
+            'kind': self.kind.value
         }
+        if self.kind == AuthenticationKind.SAS:
+            params['sasToken'] = self.sas_token
+        return params
 
     @staticmethod
     def from_response(json):
         if not json:
             return None
 
-        return Authentication(json['kind'], json.get('sas'))
+        return Authentication(json['kind'], json.get('sasToken'))
 
 
 class Dataset:
-    def __init__(self, name: str, annotation_kind: Union[AnnotationKind, str], annotation_file_uris: List[str], authentication: Authentication = None, custom_properties: dict = None) -> None:
+    def __init__(self, name: str, annotation_kind: Union[AnnotationKind, str], annotation_file_uris: List[str], authentication: Authentication = Authentication(), custom_properties: dict = None) -> None:
         annotation_kind = AnnotationKind(annotation_kind) if isinstance(annotation_kind, str) else annotation_kind
         assert name
         assert annotation_file_uris
 
         self.name = name
         self.annotation_kind = annotation_kind
         self.annotation_file_uris = annotation_file_uris
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/image_composition_model.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/planogram_matching_model.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/product_recognition_model.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/models/training_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/models/training_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/select_rectification_control_points.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/visualize_planogram_matching_result.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/cognitive_service_vision_model_customization_python_samples/tools/visualize_product_recognition_result.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO` & `cognitive-service-vision-model-customization-python-samples-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitive-service-vision-model-customization-python-samples
-Version: 0.0.5
+Version: 0.0.6
 Summary: A sample code repo for model customization using Python for Cognitive Service for Vision.
 Home-page: 
 Author: Ping Jin
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,23 +13,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
+Requires-Dist: requests
+Requires-Dist: tqdm
+Requires-Dist: azure-storage-blob
+Requires-Dist: azure-cognitiveservices-vision-customvision
+Requires-Dist: cffi
+Requires-Dist: opencv-python-headless
 
 # Azure Cognitive Services Computer Vision - Python SDK Samples
 
 ## Model Customization
 
-Computer Vision's Model Customization is a custom model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding of machine learning or computer vision required.
+Computer Vision's Model Customization is a custom model training service that allows users like developers to easily train an image classification model (Multiclass only for now) or object detection model, with low-code experience and very little understanding of machine learning or computer vision required. The service is available in regions: West US 2, East US, West Europe.
 
 This is a sample repository demonstrating how to train and predict a custom model with Cognitive Service for Vision, using Python. To get started, check out [this tutorial in Python notebook](./docs/cognitive_service_vision_model_customization.ipynb).
 
+Moreover, you can use your familiar Azure Machine Learning (AML) environment and Data Science Tools (AML Data Assets or Jobs, CLIv2 or MLFlow) for training and evaluating your custom Florence model following [this documentation](./aml-pipeline/README.md).
+
 ### Product Recognition
 
 One of the scenarios we would like to introudce as a model customization scenario is Product Recognition. Computer Vision's product recognition service has been designed to be used in retail scenarios, where users would like to detect products, such as Consumer Packaged Goods (CPG), on a shelf. It comes with a set of APIs, a pre-built AI model, and a custom AI model that can be trained following the model customization guide above. You can try these out by following tutorials in Python notebooks: 
 * **[Image Composition](./docs/cognitive_service_vision_image_composition.ipynb)**: for stitching together the segmented shelf images using Image Stitching API, as well as adjusting any slanted or squished shelf images to a correct orientation using Image Rectification API
 * **[Product Recognition](./docs/cognitive_service_vision_product_recognition.ipynb)**: for detecting products and gaps on a shelf image using a pre-built model, and individually classifying the detected products using customized model, both using Product Understanding API
 * **[Planogram Compliance](./docs/cognitive_service_vision_planogram_compliance.ipynb)**: for assessing the matchings between a planogram schema and the detected products on a shelf using Planogram Compliance API
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/setup.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 from os import path
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_clients.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_coco_check.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/test/test_coco_check.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.5/test/test_e2e.py` & `cognitive-service-vision-model-customization-python-samples-0.0.6/test/test_e2e.py`

 * *Files identical despite different names*

