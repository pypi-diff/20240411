# Comparing `tmp/mct-quantizers-1.4.0.tar.gz` & `tmp/mct-quantizers-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-1.4.0.tar", last modified: Mon Dec 18 11:55:41 2023, max compression
+gzip compressed data, was "mct-quantizers-1.5.0.tar", last modified: Thu Apr 11 07:10:37 2024, max compression
```

## Comparing `mct-quantizers-1.4.0.tar` & `mct-quantizers-1.5.0.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.327621 mct-quantizers-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2023-12-18 11:55:41.327621 mct-quantizers-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.319621 mct-quantizers-1.4.0/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.323621 mct-quantizers-1.4.0/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.323621 mct-quantizers-1.4.0/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.323621 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.323621 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.323621 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.327621 mct-quantizers-1.4.0/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/onnxruntime_session_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/onnxruntime_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.327621 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.327621 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.327621 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15290 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 11:55:41.319621 mct-quantizers-1.4.0/mct_quantizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2023-12-18 11:55:40.000000 mct-quantizers-1.4.0/mct_quantizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-12-18 11:55:41.000000 mct-quantizers-1.4.0/mct_quantizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 11:55:40.000000 mct-quantizers-1.4.0/mct_quantizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-18 11:55:40.000000 mct-quantizers-1.4.0/mct_quantizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-18 11:55:40.000000 mct-quantizers-1.4.0/mct_quantizers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-18 11:55:41.331621 mct-quantizers-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2023-12-18 11:55:28.000000 mct-quantizers-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.901091 mct-quantizers-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-11 07:10:37.901091 mct-quantizers-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.889091 mct-quantizers-1.5.0/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.893091 mct-quantizers-1.5.0/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/common/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.893091 mct-quantizers-1.5.0/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.893091 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.893091 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.897091 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.897091 mct-quantizers-1.5.0/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/onnxruntime_session_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/onnxruntime_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.897091 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.897091 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.901091 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:10:37.893091 mct-quantizers-1.5.0/mct_quantizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-11 07:10:37.000000 mct-quantizers-1.5.0/mct_quantizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-11 07:10:37.000000 mct-quantizers-1.5.0/mct_quantizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:10:37.000000 mct-quantizers-1.5.0/mct_quantizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 07:10:37.000000 mct-quantizers-1.5.0/mct_quantizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 07:10:37.000000 mct-quantizers-1.5.0/mct_quantizers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 07:10:37.901091 mct-quantizers-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-11 07:10:24.000000 mct-quantizers-1.5.0/setup.py
```

### Comparing `mct-quantizers-1.4.0/LICENSE.md` & `mct-quantizers-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/PKG-INFO` & `mct-quantizers-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers
-Version: 1.4.0
+Version: 1.5.0
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-1.4.0/README.md` & `mct-quantizers-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
 
 
 from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, BaseInferableQuantizer, mark_quantizer
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.keras.activation_quantization_holder import KerasActivationQuantizationHolder
 from mct_quantizers.pytorch.activation_quantization_holder import PytorchActivationQuantizationHolder
 from mct_quantizers.keras.load_model import keras_load_quantized_model
```

### Comparing `mct-quantizers-1.4.0/mct_quantizers/common/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/common/constants.py` & `mct-quantizers-1.5.0/mct_quantizers/common/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 FOUND_ONNXRUNTIME_EXTENSIONS = importlib.util.find_spec(ONNXRUNTIME_EXTENSIONS) is not None
 
 
 ## Quantization properties
 IS_WEIGHTS = "is_weights"
 IS_ACTIVATIONS = "is_activations"
 WEIGHTS_QUANTIZERS = "weights_quantizer"
+WEIGHTS_VALUES = "weights_value"
+OP_CALL_ARGS = 'op_call_args'
+OP_CALL_KWARGS = 'op_call_kwargs'
+IS_INPUT_AS_LIST = 'is_inputs_as_list'
 WEIGHTS_QUANTIZATION_METHOD = 'weights_quantization_method'
 WEIGHTS_N_BITS = 'weights_n_bits'
 WEIGHTS_QUANTIZATION_PARAMS = 'weights_quantization_params'
 ENABLE_WEIGHTS_QUANTIZATION = 'enable_weights_quantization'
 WEIGHTS_CHANNELS_AXIS = 'weights_channels_axis'
 WEIGHTS_PER_CHANNEL_THRESHOLD = 'weights_per_channel_threshold'
 MIN_THRESHOLD = 'min_threshold'
@@ -74,11 +78,20 @@
 ## Constant values
 
 LAYER = "layer"
 STEPS = "optimizer_step"
 TRAINING = "training"
 EPS = 1e-8
 LUT_VALUES_BITWIDTH = 8
-MCTQ_VERSION = "mctq_version"
+
+POSITIONAL_WEIGHT = 'positional_weight'
+QUANTIZED_POSITIONAL_WEIGHT = f'quantized_{POSITIONAL_WEIGHT}'
 
 # ONNX ops domain
 ONNX_CUSTOM_OP_DOMAIN = f"mct_quantizers"
+
+
+## Metadata common fields
+FRAMEWORK_VERSION = 'framework_version'
+PYTHON_VERSION = 'python_version'
+MCTQ_VERSION = "mctq_version"
+ONNX_VERSION = 'onnx_version'
```

### Comparing `mct-quantizers-1.4.0/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-1.5.0/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-1.5.0/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/common/quant_info.py` & `mct-quantizers-1.5.0/mct_quantizers/common/quant_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,24 +18,21 @@
 
 class QuantizationMethod(Enum):
     """
     Method for quantization function selection:
 
     POWER_OF_TWO - Symmetric, uniform, threshold is power of two quantization.
 
-    KMEANS - k-means quantization.
-
     LUT_POT_QUANTIZER - quantization using a lookup table and power of 2 threshold.
 
     SYMMETRIC - Symmetric, uniform, quantization.
 
     UNIFORM - uniform quantization,
 
     LUT_SYM_QUANTIZER - quantization using a lookup table and symmetric threshold.
 
     """
     POWER_OF_TWO = 0
-    KMEANS = 1
-    LUT_POT_QUANTIZER = 2
-    SYMMETRIC = 3
-    UNIFORM = 4
-    LUT_SYM_QUANTIZER = 5
+    LUT_POT_QUANTIZER = 1
+    SYMMETRIC = 2
+    UNIFORM = 3
+    LUT_SYM_QUANTIZER = 4
```

### Comparing `mct-quantizers-1.4.0/mct_quantizers/common/quant_utils.py` & `mct-quantizers-1.5.0/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/load_model.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/load_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from mct_quantizers.logger import Logger
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.python.saved_model.load_options import LoadOptions
     from mct_quantizers.keras.activation_quantization_holder import KerasActivationQuantizationHolder
     from mct_quantizers.keras.quantize_wrapper import KerasQuantizationWrapper
+    from mct_quantizers.keras.metadata import MetadataLayer
     from mct_quantizers.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
     keras = tf.keras
 
     def keras_load_quantized_model(filepath: str, custom_objects: Any = None, compile: bool = True,
                                    options: LoadOptions = None):
         """
         This function wraps the keras load model and MCT quantization custom class to it.
@@ -55,15 +56,26 @@
 
         if custom_objects is not None:
             qi_custom_objects.update(custom_objects)
         # in keras format (v3) passing option is an error
         kwargs = {}
         if options is not None:
             kwargs['options'] = options
-        return tf.keras.models.load_model(filepath, custom_objects=qi_custom_objects, compile=compile, **kwargs)
+
+        # Load model
+        loaded_model = tf.keras.models.load_model(filepath, custom_objects=qi_custom_objects, compile=compile, **kwargs)
+
+        # Extract metadata if exists
+        metadata_layers = [l for l in loaded_model.layers if isinstance(l, MetadataLayer)]
+        if len(metadata_layers) > 0:
+            if len(metadata_layers) > 1:
+                Logger.warning('Found more than 1 MetadataLayer layers in model. Loading the metadata from the first layer only.')
+            loaded_model.metadata_layer = metadata_layers[0]
+            loaded_model.metadata = metadata_layers[0].metadata
+        return loaded_model
 else:
     def keras_load_quantized_model(filepath, custom_objects=None, compile=True, options=None):
         """
         This function wraps the keras load model and MCT quantization custom class to it.
 
         Args:
             filepath: the model file path.
```

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,276 +8,287 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Dict, List, Any, Tuple
+from typing import List, Union, Any, Dict, Tuple, Callable
+
+import inspect
 
 from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer
-from mct_quantizers.common.constants import FOUND_TF, WEIGHTS_QUANTIZERS, STEPS, LAYER, TRAINING, MCTQ_VERSION
+from mct_quantizers.common.constants import FOUND_TORCH, LAYER, TRAINING, POSITIONAL_WEIGHT, \
+    QUANTIZED_POSITIONAL_WEIGHT
 from mct_quantizers.logger import Logger
-from mct_quantizers.common.get_all_subclasses import get_all_subclasses
-from mct_quantizers import __version__ as mctq_version
-
-if FOUND_TF:
-    import tensorflow as tf
-    from tensorflow.python.util import tf_inspect
-    from tensorflow.python.keras.utils.control_flow_util import smart_cond
-
-    from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
-
-    keras = tf.keras
 
-    def _make_quantizer_fn(quantizer, x, training):
-        """Use currying to return True/False specialized fns to the cond."""
+if FOUND_TORCH:
+    import torch
+    import torch.nn as nn
 
-        def quantizer_fn():
-            return quantizer(x, training)
-
-        return quantizer_fn
 
+    class PytorchQuantizationWrapper(nn.Module):
+        def __init__(self,
+                     module: Union[nn.Module, Callable],
+                     weights_quantizers: Dict[Union[int, str], BaseInferableQuantizer],
+                     weight_values: Dict[int, torch.Tensor] = None,
+                     op_call_args: List = None,
+                     op_call_kwargs: Dict[str, Any] = None,
+                     is_inputs_as_list: bool = False):
+            """
+            The PytorchQuantizationWrapper takes a Pytorch layer and quantization information and creates
+            a quantized layer. The quantization information includes a quantizer per layer attribute for
+            a Torch layer that contains weight attributes (e.g. Conv2d, BatchNorm2d, etc.). For
+            layers that get constants (e.g. torch.add(Tensor, constant), the quantization information
+            also includes a weight values per attribute, the function call args & kwargs and a boolean for
+            whether the layer\function accepts the inputs as a list (e.g. torch.cat). Note that for a layer
+            with constants, the constants are referred to as "positional weights" whose attributes are integers
+            representing the input index in the function\layer's inputs.
 
-    def _weight_name(name: str) -> str:
-        """Extracts the weight name from the full TensorFlow variable name.
+            Args:
+                module: A pytorch module or as function.
+                weights_quantizers: A dictionary between a weight's name or position to its quantizer.
+                weight_values: A dictionary between a weight's position to its value.
+                op_call_args: A list containing the layer's call arguments.
+                op_call_kwargs: A dictionary containing the layer's call keyword arguments.
+                is_inputs_as_list: A boolean indicating the layer accepts the input tensors as a list.
 
-        For example, returns 'kernel' for 'dense_2/kernel:0'.
+            Examples:
 
-        Args:
-          name: TensorFlow variable name.
+                Creating a quantized Conv2d (weight only):
 
-        Returns:
-          Extracted weight name.
-        """
-        return name.split(':')[0].split('/')[-1]
+                >>> import mct_quantizers as mctq
+                >>> import torch
 
+                >>> attr_quant_dict = {'weight': mctq.pytorch.quantizers.WeightsPOTInferableQuantizer(4, [2.0], False)}
+                >>> QuantizedConv2D = mctq.PytorchQuantizationWrapper(torch.nn.Conv2d(3, 3, 3), attr_quant_dict)
 
-    class KerasQuantizationWrapper(tf.keras.layers.Wrapper):
-        def __init__(self,
-                     layer,
-                     weights_quantizers: Dict[str, BaseInferableQuantizer] = None,
-                     **kwargs):
-            """
-            Keras Quantization Wrapper takes a keras layer and quantizers and infer a quantized layer.
+                creating a quantized function with a constant: torch.sub(constant, Tensor)
 
-            Args:
-                layer: A keras layer.
-                weights_quantizers: A dictionary between a weight's name to its quantizer.
-            """
-            super(KerasQuantizationWrapper, self).__init__(layer, **kwargs)
-            self._track_trackable(layer, name='layer')
-            self.weights_quantizers = weights_quantizers if weights_quantizers is not None else dict()
+                >>> attr_quant_dict = {0: mctq.pytorch.quantizers.WeightsPOTInferableQuantizer(4, [2.0], False)}
+                >>> attr_values = {0: torch.Tensor([1, 2, 3], dtype=torch.float32)}
+                >>> QuantizedSub = mctq.PytorchQuantizationWrapper(torch.sub), attr_quant_dict, attr_values)
 
-            self._mctq_version = mctq_version
+                creating a quantized function with constants and arguments: tf.cat([constant#1, Tensor, constant#2], dim=1)
+                >>> attr_quant_dict = {0: mctq.pytorch.quantizers.WeightsPOTInferableQuantizer(4, [2.0], False),
+                >>>                    2: mctq.pytorch.quantizers.WeightsPOTInferableQuantizer(4, [1.0], False)}
+                >>> attr_values = {0: torch.Tensor([[1,2,3], [4, 5, 6]], dtype=torch.float32),
+                >>>                2: torch.Tensor([[4,5,6], [4, 5, 6]], dtype=torch.float32)}
+                >>> QuantizedConcat = mctq.PytorchQuantizationWrapper(torch.cat, attr_quant_dict, attr_values,
+                >>>                                                   op_call_kwargs={'dim', 1})
 
-        def add_weights_quantizer(self, param_name: str, quantizer: BaseInferableQuantizer):
             """
-            This function adds a weights quantizer to existing wrapper
-
-            Args:
-                param_name: The name of the parameter to quantize
-                quantizer: A quantizer.
+            super().__init__()
+            if isinstance(module, nn.Module):
+                self.add_module(LAYER, module)
+            else:
+                # Functional layers
+                setattr(self, LAYER, module)
 
-            Returns: None
+            self.weights_quantizers = weights_quantizers
+            # Initialize positional weights:
+            self.weight_values = weight_values if weight_values is not None else dict()
+            for pos, weight_val in self.weight_values.items():
+                if not isinstance(weight_val, torch.Tensor):
+                    Logger.error(f'Positional weight at position {pos} should be a torch.Tensor, '
+                                 f'but type is {type(weight_val)}.')
+
+            # Initialize functional module arguments. For examples, see the class description.
+            self.op_call_args = [] if op_call_args is None else op_call_args
+            self.op_call_kwargs = {} if op_call_kwargs is None else op_call_kwargs
+            self.is_inputs_as_list = is_inputs_as_list
+
+            # Sanity checks:
+            # 1. If there are no weight_values: verify all weight_quantizers are strings
+            # 2. If there are weight_values: verify all weight_quantizers and weight_values keys
+            #    are integers, and that they match.
+            # 3. A module with both weights as attributes and positional weights is not supported.
+            if len(self.weight_values) == 0:
+                # expecting weights_quantizers keys to be all strings.
+                if not all([isinstance(w, str) for w in self.weights_quantizers]):
+                    Logger.error('"weights_quantizers" keys should be all strings')
+                self.is_str_attr = True
+            else:
+                # expecting both weights_quantizers and weight_values keys to be all integers.
+                if not all([isinstance(w, int) for w in self.weight_values]):
+                    Logger.error('All "weight_values" keys should be integers')
+                if not all([a == b for a, b in zip(weights_quantizers, weight_values)]):
+                    Logger.error('Mismatch between "weights_quantizers" and "weight_values" keys')
+                self.is_str_attr = False
 
-            """
-            self.weights_quantizers.update({param_name: quantizer})
+            self._set_weights_vars(True)
 
         @property
         def is_weights_quantization(self) -> bool:
             """
             This function check weights quantizer exists in wrapper.
 
-            Returns: a boolean if weights quantizer exists
+            Returns: a boolean if weights quantizer exists.
 
             """
             return self.num_weights_quantizers > 0
 
         @property
         def num_weights_quantizers(self) -> int:
             """
-            Returns: number of weights quantizers
+            Returns: number of weights quantizers.
             """
             return len(self.weights_quantizers)
 
-        def get_config(self):
+        def convert_to_inferable_quantizers(self):
             """
-            Returns: Configuration of KerasQuantizationWrapper.
+            Convert the wrapper quantizers with inferable quantizers.
 
             """
-            base_config = super(KerasQuantizationWrapper, self).get_config()
-            config = {WEIGHTS_QUANTIZERS: {k: keras.utils.serialize_keras_object(v) for k, v in self.weights_quantizers.items()}}
-
-            return_config = dict(list(base_config.items()) + list(config.items()))
-            return_config[MCTQ_VERSION] = self._mctq_version
-
-            return return_config
-
-        @property
-        def mctq_version(self):
-            return self._mctq_version
+            # Weight quantizers
+            if self.is_weights_quantization:
+                inferable_weight_quantizers = {}
+                for name, quantizer in self.weights_quantizers.items():
+                    if hasattr(quantizer, 'convert2inferable') and callable(quantizer.convert2inferable):
+                        inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
+                self.weights_quantizers = inferable_weight_quantizers
+                self._set_weights_vars(False)
 
         def _set_weights_vars(self, is_training: bool = True):
             """
-            This function sets weights quantizers vars to the layer
+            Initialize learnable weights as parameters in the wrapper, and their quantizers.
 
             Args:
-                is_training: Flag to indicate whether training or not
+                is_training: Whether working with InferableQuantizers or not. If so, do not register weight as parameter.
 
-            Returns: None
             """
             self._weights_vars = []
-            for name, quantizer in self.weights_quantizers.items():
-                weight = getattr(self.layer, name)
-                quantizer.initialize_quantization(weight.shape, _weight_name(weight.name) if is_training else None,
-                                                  self)
-                # Add weight to wrapper weight lists (rather than the layer weight lists), because it will be deleted
-                # from the layer's lists after the first call
-                self._weights_vars.append((name, weight, quantizer))
-                if is_training and not any([weight is w for w in self._trainable_weights]):
-                    self._trainable_weights.append(weight)
-                elif not is_training and any([weight is w for w in self._non_trainable_weights]):
-                    self._non_trainable_weights.append(weight)
 
-        @classmethod
-        def from_config(cls, config):
-            """
-
-            Args:
-                config(dict): dictionary  of  KerasQuantizationWrapper Configuration
+            # Init weights quantizers
+            for name, quantizer in self.weights_quantizers.items():
+                if self.is_str_attr:
+                    if is_training:
+                        weight = getattr(self.layer, name).detach()
+                        delattr(self.layer, name)
+                        setattr(self.layer, name, weight)
+                        self.register_parameter(name, torch.nn.Parameter(weight, requires_grad=True))
+                    else:
+                        weight = getattr(self, name).detach()
+                        delattr(self.layer, name)
+                        setattr(self.layer, name, weight)
+                    weight_var = getattr(self, name)
+                else:
+                    weight = self.weight_values[name]
+                    self.register_parameter(f'{POSITIONAL_WEIGHT}_{name}',
+                                            torch.nn.Parameter(weight, requires_grad=False))
+                    setattr(self, f'{QUANTIZED_POSITIONAL_WEIGHT}_{name}', weight)
+                    weight_var = getattr(self, f'{POSITIONAL_WEIGHT}_{name}')
 
-            Returns: A KerasQuantizationWrapper
+                quantizer.initialize_quantization(weight.shape, name, self)
+                self._weights_vars.append((name, weight_var, quantizer))
 
+        def set_quantize_weights(self, quantized_weights: dict):
             """
-            config = config.copy()
-            qi_inferable_custom_objects = {subclass.__name__: subclass for subclass in
-                                           get_all_subclasses(BaseKerasInferableQuantizer)}
-            weights_quantizers = {k: keras.utils.deserialize_keras_object(v,
-                                                                          module_objects=globals(),
-                                                                          custom_objects=qi_inferable_custom_objects) for k, v in config.pop(WEIGHTS_QUANTIZERS).items()}
-            layer = tf.keras.layers.deserialize(config.pop(LAYER))
-
-            v = config.pop(MCTQ_VERSION, None)
-
-            obj = cls(layer=layer, weights_quantizers=weights_quantizers, **config)
-            obj._mctq_version = mctq_version if v is None else v
+            This function updates layer weights after quantization.
 
-            return obj
-
-        def build(self, input_shape):
-            """
-            KerasQuantization Wrapper build function.
             Args:
-                input_shape: the layer input shape
+                quantized_weights: a dict of weight to update.
 
             Returns: None
 
             """
-            super(KerasQuantizationWrapper, self).build(input_shape)
-
-            self.optimizer_step = self.add_weight(
-                STEPS,
-                initializer=tf.keras.initializers.Constant(-1),
-                dtype=tf.dtypes.int32,
-                trainable=False)
-
-            self._set_weights_vars()
+            for weight_attr in self.weights_quantizers:
+                weight = quantized_weights.get(weight_attr)
+                if self.is_str_attr:
+                    setattr(self.layer, weight_attr, weight)
+                else:
+                    setattr(self, f'{QUANTIZED_POSITIONAL_WEIGHT}_{weight_attr}', weight)
 
-        def set_quantize_weights(self, quantized_weights: dict):
+        def get_weights_vars(self) -> List[Tuple[str, Any, BaseInferableQuantizer]]:
             """
-            This function update layer weights after quantization.
-
-            Args:
-                quantized_weights: a dict of weight to update
+            A getter of the layer's weights variables.
 
-            Returns: None
+            Returns:
+                List pf tuples of the wrapped layer's weights variables with weight name, values and assigned quantizer.
 
             """
-            for weight_attr in self.weights_quantizers.keys():
-                weight = quantized_weights.get(weight_attr)
-                current_weight = getattr(self.layer, weight_attr)
-                if current_weight.shape != weight.shape:
-                    Logger.error(
-                        f"Existing layer weight shape {current_weight.shape} is incompatible with provided weight "
-                        f"shape {weight.shape}")  # pragma: no cover
 
-                setattr(self.layer, weight_attr, weight)
+            return self._weights_vars
 
-        def call(self, inputs, training=None, **kwargs):
+        def forward(self,
+                    *args: List[Any],
+                    **kwargs: Dict[str, Any]) -> Union[torch.Tensor, List[torch.Tensor]]:
             """
-            KerasQuantizationWrapper call functions
+            PytorchQuantizationWrapper forward functions.
             Args:
-                inputs: Input tensors to specified layer
-                training: a boolean stating if layer is in training mode.
-                **kwargs:
+                args: arguments to pass to internal layer.
+                kwargs: key-word dictionary to pass to the internal layer.
 
-            Returns: tensors that simulate a quantized layer.
+            Returns: a tensor that simulates a quantized layer.
 
             """
-            if training is None:
-                training = tf.keras.backend.learning_phase()
 
+            # ----------------------------------
             # Quantize all weights, and replace them in the underlying layer.
-            quantized_weights = {}
-            for name, unquantized_weight, quantizer in self._weights_vars:
+            # ----------------------------------
+            if self.is_weights_quantization:
+
+                quantized_weights = {}
+                for name, unquantized_weight, quantizer in self._weights_vars:
+                    s = inspect.signature(quantizer.__call__)
+                    if TRAINING in s.parameters.keys():
+                        quantized_weight = quantizer(unquantized_weight, self.training)
+                    else:
+                        quantized_weight = quantizer(unquantized_weight)
 
-                weights_quantizer_args_spec = tf_inspect.getfullargspec(quantizer.__call__).args
-                if TRAINING in weights_quantizer_args_spec:
-                    quantized_weight = smart_cond(
-                        training,
-                        _make_quantizer_fn(quantizer, unquantized_weight, True),
-                        _make_quantizer_fn(quantizer, unquantized_weight, False))
-                    quantized_weights.update({name: quantized_weight})
-                else:
-                    # Keras weights inferable quantizer
-                    quantized_weight = quantizer(unquantized_weight)
                     quantized_weights.update({name: quantized_weight})
 
-            self.set_quantize_weights(quantized_weights)
+                self.set_quantize_weights(quantized_weights)
 
-            args_spec = tf_inspect.getfullargspec(self.layer.call).args
-            if TRAINING in args_spec:
-                outputs = self.layer.call(inputs, training=training, **kwargs)
+            if not self.is_str_attr:
+                # Positional weights need to be inserted in the wrapper input list according to their (key) position.
+                args = list(args)
+                weight_positions = [w[0] for w in self._weights_vars]
+                for pos in sorted(weight_positions):
+                    args.insert(pos, getattr(self, f'{QUANTIZED_POSITIONAL_WEIGHT}_{pos}'))
+
+            _kwargs = {**self.op_call_kwargs, **kwargs}
+            # ----------------------------------
+            # Layer operation
+            # ----------------------------------
+            if self.is_inputs_as_list:
+                outputs = self.layer(args, *self.op_call_args, **_kwargs)
             else:
-                outputs = self.layer.call(inputs, **kwargs)
+                outputs = self.layer(*args, *self.op_call_args, **_kwargs)
 
             return outputs
 
-        def get_weights_vars(self) -> List[Tuple[str, Any, BaseInferableQuantizer]]:
-            """
-            A getter of the layer's weights variables.
-
-            Returns:
-                List pf tuples of the wrapped layer's weights variables with weight name, values and assigned quantizer.
-
-            """
-
-            return self._weights_vars
-
-        def get_quantized_weights(self) -> Dict[str, tf.Tensor]:
+        def get_quantized_weights(self) -> Dict[str, torch.Tensor]:
             """
 
             Returns: A dictionary of weights attributes to quantized weights.
 
             """
             quantized_weights = {}
             weights_var = self.get_weights_vars()
             for name, w, quantizer in weights_var:
                 quantized_weights[name] = quantizer(w)
             return quantized_weights
 
 else:
-    class KerasQuantizationWrapper(object):
+    class PytorchQuantizationWrapper:
         def __init__(self,
                      layer,
-                     weights_quantizers: Dict[str, BaseInferableQuantizer] = None):
+                     weight_quantizers: Dict[str, BaseInferableQuantizer],
+                     weight_values: Dict = None,
+                     op_call_args: List = None,
+                     op_call_kwargs: Dict[str, Any] = None,
+                     is_inputs_as_list: bool = False):
             """
-            Keras Quantization Wrapper takes a keras layer and quantizers and infer a quantized layer.
+            Pytorch Quantization Wrapper takes a pytorch module and quantizers and infer a quantized layer.
 
             Args:
-                layer: A keras layer.
-                weights_quantizers: A dictionary between a weight's name to its quantizer.
-            """
-            Logger.critical('Installing tensorflow is mandatory '
-                            'when using KerasQuantizationWrapper. '
-                            'Could not find Tensorflow package.')  # pragma: no cover
+                layer: A pytorch module.
+                weight_quantizers: A dictionary between a weight's name to its quantizer.
+                weight_values: A dictionary between a weight's position to its value.
+                op_call_args: A list containing the layer's call arguments.
+                op_call_kwargs: A dictionary containing the layer's call keyword arguments.
+                is_inputs_as_list: A boolean indicating the layer accepts the input tensors as a list.
+            """
+            Logger.critical('Installing Pytorch is mandatory '
+                            'when using PytorchQuantizationWrapper. '
+                            'Could not find torch package.')  # pragma: no cover
```

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-1.5.0/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/logger.py` & `mct-quantizers-1.5.0/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/onnxruntime_session_options.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/onnxruntime_session_options.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/onnxruntime_validations.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/onnxruntime_validations.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-1.5.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.4.0/mct_quantizers.egg-info/PKG-INFO` & `mct-quantizers-1.5.0/mct_quantizers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers
-Version: 1.4.0
+Version: 1.5.0
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-1.4.0/mct_quantizers.egg-info/SOURCES.txt` & `mct-quantizers-1.5.0/mct_quantizers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 mct_quantizers.egg-info/requires.txt
 mct_quantizers.egg-info/top_level.txt
 mct_quantizers/common/__init__.py
 mct_quantizers/common/base_inferable_quantizer.py
 mct_quantizers/common/constants.py
 mct_quantizers/common/get_all_subclasses.py
 mct_quantizers/common/get_quantizers.py
+mct_quantizers/common/metadata.py
 mct_quantizers/common/quant_info.py
 mct_quantizers/common/quant_utils.py
 mct_quantizers/keras/__init__.py
 mct_quantizers/keras/activation_quantization_holder.py
 mct_quantizers/keras/load_model.py
+mct_quantizers/keras/metadata.py
 mct_quantizers/keras/quantize_wrapper.py
 mct_quantizers/keras/quantizer_utils.py
 mct_quantizers/keras/validation_functions.py
 mct_quantizers/keras/quantizers/__init__.py
 mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
 mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
 mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
@@ -34,14 +36,15 @@
 mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
 mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
 mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
 mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
 mct_quantizers/pytorch/__init__.py
 mct_quantizers/pytorch/activation_quantization_holder.py
 mct_quantizers/pytorch/load_model.py
+mct_quantizers/pytorch/metadata.py
 mct_quantizers/pytorch/onnxruntime_session_options.py
 mct_quantizers/pytorch/onnxruntime_validations.py
 mct_quantizers/pytorch/quantize_wrapper.py
 mct_quantizers/pytorch/quantizer_utils.py
 mct_quantizers/pytorch/quantizers/__init__.py
 mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
 mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
```

### Comparing `mct-quantizers-1.4.0/setup.py` & `mct-quantizers-1.5.0/setup.py`

 * *Files identical despite different names*

