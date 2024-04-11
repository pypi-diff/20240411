# Comparing `tmp/happy_vllm-0.9.0.tar.gz` & `tmp/happy_vllm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happy_vllm-0.9.0.tar", last modified: Mon Mar 18 14:25:32 2024, max compression
+gzip compressed data, was "happy_vllm-1.0.0.tar", last modified: Thu Apr 11 09:11:18 2024, max compression
```

## Comparing `happy_vllm-0.9.0.tar` & `happy_vllm-1.0.0.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.496164 happy_vllm-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-03-18 14:25:32.496164 happy_vllm-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 14:25:32.496164 happy_vllm-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.488164 happy_vllm-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.492164 happy_vllm-0.9.0/src/happy_vllm/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.492164 happy_vllm-0.9.0/src/happy_vllm/core/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/core/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.492164 happy_vllm-0.9.0/src/happy_vllm/logits_processors/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/logits_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/logits_processors/json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/logits_processors/min_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/logits_processors/response_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.492164 happy_vllm-0.9.0/src/happy_vllm/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/middlewares/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.492164 happy_vllm-0.9.0/src/happy_vllm/model/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/model/model_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.492164 happy_vllm-0.9.0/src/happy_vllm/routers/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/routers/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.496164 happy_vllm-0.9.0/src/happy_vllm/routers/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/routers/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/routers/schemas/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/routers/schemas/technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/routers/schemas/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/routers/technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/src/happy_vllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.496164 happy_vllm-0.9.0/src/happy_vllm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-03-18 14:25:32.000000 happy_vllm-0.9.0/src/happy_vllm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-18 14:25:32.000000 happy_vllm-0.9.0/src/happy_vllm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 14:25:32.000000 happy_vllm-0.9.0/src/happy_vllm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-18 14:25:32.000000 happy_vllm-0.9.0/src/happy_vllm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-18 14:25:32.000000 happy_vllm-0.9.0/src/happy_vllm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-18 14:25:32.000000 happy_vllm-0.9.0/src/happy_vllm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 14:25:32.496164 happy_vllm-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_min_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_response_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    24342 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_routers_functionnal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_routers_technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_schemas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-18 14:25:11.000000 happy_vllm-0.9.0/tests/test_utils_parse_logits_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-18 14:25:27.000000 happy_vllm-0.9.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.140568 happy_vllm-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.140568 happy_vllm-1.0.0/src/happy_vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/core/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/logits_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/logits_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/logits_processors/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/logits_processors/response_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/middlewares/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/model/model_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.144568 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/examples/request.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/examples/response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/schemas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/routers/technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/src/happy_vllm/utils_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/src/happy_vllm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 09:11:18.000000 happy_vllm-1.0.0/src/happy_vllm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:11:18.148568 happy_vllm-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_response_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_routers_functionnal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_routers_technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_schemas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_utils_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-11 09:11:14.000000 happy_vllm-1.0.0/tests/test_utils_parse_logits_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 09:11:16.000000 happy_vllm-1.0.0/version.txt
```

### Comparing `happy_vllm-0.9.0/LICENSE` & `happy_vllm-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/pyproject.toml` & `happy_vllm-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 [project]
 name = "happy_vllm"
 description = "happy_vllm is a REST API for vLLM, production ready"
 readme = "README.md"
 requires-python = ">=3.10,<4.0"
 dependencies = [
-    "vllm>=0.3.2, <1.0",
-    "fastapi>=0.100.0,<1.0",
-    "pydantic_settings>=2.0.1,<3.0",
-    "uvicorn[standard]>=0.20,<1.0",
-    "starlette-prometheus>=0.9,<1.0",
-    "numpy>=1.19",
-    "lm-format-enforcer>=0.9.0,<0.10.0",
-    "torch>=2.0.0,<3.0.0"
+    "vllm>=0.4.0,<1.0",
+    "fastapi>=0.110.1,<1.0",
+    "pydantic_settings>=2.2.1,<3.0",
+    "uvicorn[standard]>=0.29.0,<1.0",
+    "prometheus_client>=0.20.0,<1.0",
+    "numpy>=1.26.4",
+    "lm-format-enforcer>=0.9.0,<0.10.0"
 ]
 
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {file = "version.txt"}
 
@@ -38,8 +37,11 @@
 addopts = "-v --cov=happy_vllm"
 filterwarnings = [
     "ignore:The hookimpl CovPlugin.pytest_",
     "ignore:IPython could not be loaded!"
 ]
 
 [tool.isort]
-profile = "black"
+profile = "black"
+
+[tool.setuptools.package-data]
+"happy_vllm.routers.schemas.examples" = ["*.json"]
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/__init__.py` & `happy_vllm-1.0.0/src/happy_vllm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 import os
 import logging
 
-from .core.config import settings
+from .core.config import log_settings
 from .core.logtools import get_pattern_log
 
-level = settings.log_level
+level = log_settings.log_level
 
 logger = logging.getLogger(__name__)
 logger.setLevel(level)
 
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/application.py` & `happy_vllm-1.0.0/src/happy_vllm/application.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,49 +14,49 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from fastapi import FastAPI
 from argparse import Namespace
 from fastapi.middleware.cors import CORSMiddleware
-from starlette_prometheus import metrics, PrometheusMiddleware
 
-from .core.config import settings
 from .routers import main_routeur
 from .core.resources import get_lifespan
 from happy_vllm.middlewares.exception import ExceptionHandlerMiddleware
+from prometheus_client import make_asgi_app
 
-
-def declare_application(cli_args: Namespace) -> FastAPI:
+def declare_application(args: Namespace) -> FastAPI:
     """Create the FastAPI application
 
     See https://fastapi.tiangolo.com/tutorial/first-steps/ to learn how to
     customize your FastAPI application
     """
     app = FastAPI(
-        title=f"REST API form {settings.app_name}",
-        description=f"Use {settings.app_name} thanks to FastAPI",
-        lifespan=get_lifespan(cli_args=cli_args)
+        title=f"REST API for vLLM",
+        description=f"A REST API for vLLM, production ready",
+        lifespan=get_lifespan(args=args)
     )
 
-    # Add PrometheusMiddleware
-    app.add_middleware(PrometheusMiddleware)
-    app.add_route("/metrics", metrics)
+    # Add prometheus asgi middleware to route /metrics requests
+    metrics_app = make_asgi_app()
+    app.mount("/metrics", metrics_app)
 
     # CORS middleware that allows all origins to avoid CORS problems
     # see https://fastapi.tiangolo.com/tutorial/cors/#use-corsmiddleware
     app.add_middleware(
         CORSMiddleware,
-        allow_origins=["*"],
-        allow_credentials=True,
-        allow_methods=["*"],
-        allow_headers=["*"],
+        allow_origins=args.allowed_origins,
+        allow_credentials=args.allow_credentials,
+        allow_methods=args.allowed_methods,
+        allow_headers=args.allowed_headers,
     )
 
     # Add exception middleware
-    if cli_args.explicit_errors:
+    if args.explicit_errors:
         app.add_middleware(ExceptionHandlerMiddleware)
 
     #
-    app.include_router(main_routeur, prefix=settings.api_entrypoint)
+    app.include_router(main_routeur, prefix=args.api_endpoint_prefix)
+
+    app.root_path = args.root_path
 
     return app
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/core/__init__.py` & `happy_vllm-1.0.0/src/happy_vllm/core/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/src/happy_vllm/core/config.py` & `happy_vllm-1.0.0/src/happy_vllm/core/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,21 +17,17 @@
 
 """Config global settings
 
 This module handle global app configuration
 """
 
 
-from happy_vllm import utils
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
-class Settings(BaseSettings):
-    app_name: str = "happy_vllm"
-    app_version: str = utils.get_package_version()
-    api_entrypoint: str = "/happy_vllm/rs/v1"
+class LogSettings(BaseSettings):
     log_level: str = "INFO"
 
     model_config = SettingsConfigDict(env_file=".env", extra='ignore', protected_namespaces=('settings', ))
 
 
-settings = Settings()
+log_settings = LogSettings()
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/core/logtools.py` & `happy_vllm-1.0.0/src/happy_vllm/core/logtools.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 
 """Logs utilities
 
 This module is used to define log pattern, add log filters, etc.
 """
 
 
-from .config import settings
+from happy_vllm import utils
 
 
 def get_pattern_log():
+    app_version = utils.get_package_version()
     return (
         "{"
         '"date": "%(asctime)s", '
         '"level": "%(levelname)s", '
         '"message": "%(message)s", '
-        f'"version": "{settings.app_version}", '
+        f'"version": "{app_version}", '
         '"function": "File %(pathname)s, line %(lineno)d, in %(funcName)s", '
         '"logger": "%(name)s"'
         "}"
     )
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/core/resources.py` & `happy_vllm-1.0.0/src/happy_vllm/core/resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 from ..model.model_base import Model
 
 logger = logging.getLogger(__name__)
 
 RESOURCES = {}
 RESOURCE_MODEL = "model"
 
-def get_lifespan(cli_args: Namespace) -> Callable:
+def get_lifespan(args: Namespace) -> Callable:
     @asynccontextmanager
     async def lifespan(app: FastAPI):
         # Load the ML model
-        model = Model()
-        model.loading(cli_args=cli_args)
+        model = Model(app_name=args.app_name)
+        model.loading(args=args)
         logger.info("Model loaded")
 
         RESOURCES[RESOURCE_MODEL] = model
         yield
 
         # Clean up the ML models and release the resources
         RESOURCES.clear()
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/logits_processors/__init__.py` & `happy_vllm-1.0.0/src/happy_vllm/logits_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/src/happy_vllm/logits_processors/json_format.py` & `happy_vllm-1.0.0/src/happy_vllm/logits_processors/json_format.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/src/happy_vllm/logits_processors/min_tokens.py` & `happy_vllm-1.0.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-import math
-import torch
-from typing import List
-
-class VLLMLogitsProcessorMinTokens:
-
-    def __init__(self, tokenizer, min_tokens: int) -> None:
-        '''Initializes the logits processor with min_tokens
-
-        Args:
-            tokenizer : The tokenizer used by the model
-            min_tokens (int) : The minimal number of tokens we want to generate 
-
-        '''
-        self.min_tokens = min_tokens
-        self.eos_token_id = tokenizer.eos_token_id
-
-
-    def __call__(self, input_ids: List[int], scores: torch.Tensor) -> torch.Tensor:
-        """Prevents the generation of the eos token before min_tokens is reached
-
-        Args:
-            inputs_ids (list) : The list of tokens ids generated by the LLM
-            scores (torch.tensor) : The tensor containing the logits for the next token
-        
-        Returns:
-            toch.tensor : The updated scores ie the initial scores masked to only allow possible tokens
-        """
-        if len(input_ids) < self.min_tokens:
-            mask = torch.full_like(scores, 0)
-            mask[self.eos_token_id] = -math.inf
-            scores = scores + mask
-        return scores
+from happy_vllm.logits_processors.json_format import VLLMLogitsProcessorJSON
+from happy_vllm.logits_processors.response_pool import VLLMLogitsProcessorResponsePool
+
+# In the following parser, we have entries of the form:
+# api_keyword_main : {'class': a_logits_processor_class
+#                'arguments': {api_keyword: argument_of_the_class,
+#                              api_keyword: argument_of_the_class}, ...},
+#                  'tokenizer': False, 'model': False, 'prompt': False
+# The purpose of this parser is that, if the api_keyword_main is present in the json sent via API, then
+# we know we must use the corresponding logits processor. Then we look for all keyword in the 'arguments' 
+# dictionary which we each corresponds to an argument of the init of the class except for the tokenizer, the model or the prompt 
+# which are passed by the tokenizer, model or prompt boolean values if needed
+
+logits_processors_parser = {'response_pool': {'class': VLLMLogitsProcessorResponsePool,
+                                                'arguments': {'response_pool': 'possible_responses'},
+                                                'tokenizer': True},
+                            'json_format':{'class': VLLMLogitsProcessorJSON,
+                                            'arguments': {'json_format': 'json_format',
+                                                          'json_format_is_json_schema': 'json_format_is_json_schema'},
+                                            'tokenizer_lmformatenforcer': True}}
+
+logits_processors_incompatibilities = [('response_pool', 'json_format')]
+
+def detect_logits_processors_incompatibilities(request_dict: dict) -> None:
+    """Detects if some keywords present in request_dict could allow incompatible logits_processors
+    to be present
+
+    Args:
+        request_dict (dict) : The body of the request with the different keywords
+    """
+    for first_keyword, second_keyword in logits_processors_incompatibilities:
+        if first_keyword in request_dict and second_keyword in request_dict:
+            raise ValueError(f"Two keywords are incompatible : {first_keyword} and {second_keyword}")
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/logits_processors/response_pool.py` & `happy_vllm-1.0.0/src/happy_vllm/logits_processors/response_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.possible_tokens_responses = {response: list(utils.proper_tokenization(tokenizer, response)) for response in possible_responses}
         self.eos_token_id = tokenizer.eos_token_id
 
     def __call__(self, input_ids: List[int], scores: torch.Tensor) -> torch.Tensor:
         """Puts a mask to allow only tokens which could provide a response in the pool
 
         Args:
-            inputs_ids (list) : The list of tokens ids generated by the LLM
+            input_ids (list) : The list of tokens ids generated by the LLM
             scores (torch.tensor) : The tensor containing the logits for the next token
         
         Returns:
             toch.tensor : The updated scores ie the initial scores masked to only allow possible tokens
 
         """
         if self.possible_tokens_responses == {}:
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/middlewares/exception.py` & `happy_vllm-1.0.0/src/happy_vllm/middlewares/exception.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/src/happy_vllm/model/__init__.py` & `happy_vllm-1.0.0/src/happy_vllm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/src/happy_vllm/model/model_base.py` & `happy_vllm-1.0.0/src/happy_vllm/model/model_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,105 +15,80 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """This module contains the base Model class
 """
 
 
+import os
 import logging
 from pathlib import Path
 from argparse import Namespace
 from transformers import AutoTokenizer
 from typing import Any, Tuple, Union, List
 from vllm.engine.arg_utils import AsyncEngineArgs
 from vllm.engine.async_llm_engine import AsyncLLMEngine
-from vllm.transformers_utils.tokenizer import TokenizerGroup
-from pydantic_settings import BaseSettings, SettingsConfigDict
+from vllm.transformers_utils.tokenizer_group.tokenizer_group import TokenizerGroup
 from lmformatenforcer.integrations.transformers import build_token_enforcer_tokenizer_data
 
 from happy_vllm import utils
 
 logger = logging.getLogger(__name__)
 
 
-class ModelSettings(BaseSettings):
-    """Download settings
-
-    This class is used for settings management purpose, have a look at the pydantic
-    documentation for more details : https://pydantic-docs.helpmanual.io/usage/settings/
-
-    By default, it looks for environment variables (case insensitive) to set the settings
-    if a variable is not found, it looks for a file name .env in your working directory
-    where you can declare the values of the variables and finally it sets the values
-    to the default ones one can define above
-    """
-    model : str = 'None'
-    model_name : str = '?'
-    tokenizer_name : str = 'None'
-    TEST_MODELS_DIR : str = 'None'
-
-    model_config = SettingsConfigDict(env_file=".env", extra='ignore', protected_namespaces=('settings', ))
-
-
 class Model:
     """Parent model class.
     """
 
     def __init__(self, **kwargs):
         '''Init. model class'''
         self._model = None
         self._tokenizer = None
         self._model_conf = None
         self._model_explainer = None
         self._loaded = False
+        self.app_name = kwargs.get('app_name', "happy_vllm")
 
     def is_model_loaded(self):
         """return the state of the model"""
         return self._loaded
 
-    def loading(self, cli_args: Namespace, **kwargs):
+    def loading(self, args: Namespace, **kwargs):
         """load the model"""
-        self._load_model(cli_args, **kwargs)
+        self._load_model(args, **kwargs)
         self._loaded = True
 
-    def _load_model(self, cli_args: Namespace, **kwargs) -> None:
+    def _load_model(self, args: Namespace, **kwargs) -> None:
         """Load a model from a file
 
         Returns:
             Tuple[Any, dict]: A tuple containing the model and a dict of metadata about it.
         """
-        settings = ModelSettings(**kwargs)
-        if settings.model != 'None':
-            cli_args.model = settings.model
-        if settings.model_name != '?':
-            model_name = settings.model_name
-        else:
-            model_name = cli_args.model_name
 
-        self._model_conf = {'model_name': model_name}
+        self._model_conf = {'model_name': args.model_name}
 
-        logger.info(f"Loading the model from {cli_args.model}")
-        if model_name != "TEST MODEL":
-            engine_args = AsyncEngineArgs.from_cli_args(cli_args) 
+        logger.info(f"Loading the model from {args.model}")
+        if args.model_name != "TEST MODEL":
+            engine_args = AsyncEngineArgs.from_cli_args(args) 
             self._model = AsyncLLMEngine.from_engine_args(engine_args) # type: ignore
             if isinstance(self._model.engine.tokenizer, TokenizerGroup): # type: ignore
                 self._tokenizer = self._model.engine.tokenizer.tokenizer # type: ignore
             else:
                 self._tokenizer = self._model.engine.tokenizer # type: ignore
             self._tokenizer_lmformatenforcer = build_token_enforcer_tokenizer_data(self._tokenizer)
             self.max_model_len = self._model.engine.model_config.max_model_len # type: ignore
             self.original_truncation_side = self._tokenizer.truncation_side
         # For test purpose
         else:
             self.max_model_len = 2048
             self.original_truncation_side = 'right'
-            self._tokenizer = AutoTokenizer.from_pretrained(settings.tokenizer_name,
-                                                     cache_dir=settings.TEST_MODELS_DIR, truncation_side=self.original_truncation_side)
+            self._tokenizer = AutoTokenizer.from_pretrained(utils.TEST_TOKENIZER_NAME,
+                                                     cache_dir=os.environ["TEST_MODELS_DIR"], truncation_side=self.original_truncation_side)
             self._tokenizer_lmformatenforcer = build_token_enforcer_tokenizer_data(self._tokenizer)
-            self._model = MockModel(self._tokenizer)
+            self._model = MockModel(self._tokenizer, self.app_name)
         logger.info(f"Model loaded")
 
     def tokenize(self, text: str) -> List[int]:
         """Tokenizes a text
         
         Args:
             text (str) : The text to tokenize
@@ -166,18 +141,20 @@
     def extract_text_outside_truncation(self, text: str, truncation_side: Union[str, None] = None, max_length: Union[int, None] = None) -> str:
         """Extracts the part of the prompt not kept after truncation, which will not be infered by the model.
         First, we tokenize the prompt while applying truncation.
         We obtain a list of sequences of token ids padded, which are outside the truncation.
         Then we decode this list of tensors of token IDs containing special tokens to a string.
 
         Args:
-            prompt (str)
+            text (str) : The text we want to parse
+            truncation_side (str) : The side of the truncation
+            max_length (int) : The length above which the text will be truncated
 
         Returns:
-            prompt outside the truncation (str)
+            The part of the text which will be dropped by the truncation (str)
         """
         if max_length is None:
             max_length = self.max_model_len
         if truncation_side is None:
             truncation_side = self.original_truncation_side
         self._tokenizer.truncation_side = truncation_side
         list_tokens = self._tokenizer(text, truncation=True, add_special_tokens=False, max_length=max_length, return_overflowing_tokens=True)['input_ids']
@@ -253,23 +230,23 @@
         if big_list[index - len_sub_list + 1: index + 1] == sub_list:
             indices.append(index)
     return indices
 
 
 class MockModel():
 
-    def __init__(self, tokenizer):
+    def __init__(self, tokenizer, app_name: str = "happy_vllm"):
         self.tokenizer = tokenizer
+        self.app_name = app_name
 
     async def generate(self, prompt, sampling_params, request_id):
         stream_txts = [f"n={i} "*i + prompt + " This is the generated text. I find it really good don't you ?" for i in range(sampling_params.n)]
         stream_ids = [self.tokenizer(stream_txt, add_special_tokens=False, truncation=True, max_length=sampling_params.max_tokens)['input_ids'] for stream_txt in stream_txts]
         max_length = max([len(element) for element in stream_ids]) + 1
         stream_tmp = [[self.tokenizer.decode(text[:i]) for text in stream_ids] for i in range(max_length)]
-        print(stream_tmp)
         stream = [MockGenerateResponse(prompt, texts) for texts in stream_tmp]
         # Mock the length finish_reason
         for i in range(sampling_params.n):
             if stream[-1].outputs[i].finish_reason is None:
                 stream[-1].outputs[i].finish_reason = "length"
         stream = self.async_iter(stream)
         async for outputs in stream:
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/routers/__init__.py` & `happy_vllm-1.0.0/src/happy_vllm/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/src/happy_vllm/routers/functional.py` & `happy_vllm-1.0.0/src/happy_vllm/routers/functional.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,32 +10,41 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-
+import os
 import json
-from fastapi import APIRouter
 from vllm.utils import random_uuid
+from fastapi import APIRouter, Body
+from pydantic import BaseModel, Field
 from starlette.requests import Request
-from typing import AsyncGenerator, Tuple
 from vllm.sampling_params import SamplingParams
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from lmformatenforcer import TokenEnforcerTokenizerData
+from typing import Annotated, AsyncGenerator, Tuple, List
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 from starlette.responses import JSONResponse, Response, StreamingResponse
 
 from happy_vllm import utils
-from happy_vllm.logits_processors.min_tokens import VLLMLogitsProcessorMinTokens
+from happy_vllm.logits_processors.response_pool import VLLMLogitsProcessorResponsePool
 from happy_vllm.logits_processors.utils_parse_logits_processors import logits_processors_parser, detect_logits_processors_incompatibilities
 
 from ..model.model_base import Model
 from ..core.resources import RESOURCE_MODEL, RESOURCES
+from .schemas.functional import ResponseGenerate, RequestGenerate, ResponseTokenizer, RequestTokenizer, ResponseDecode, RequestDecode, ResponseSplitText, RequestSplitText, ResponseMetadata, RequestMetadata
+
+
+# Load the response examples
+directory = os.path.dirname(os.path.abspath(__file__))
+request_examples_path = os.path.join(directory, "schemas", "examples", "request.json")
+with open(request_examples_path, 'r') as file:
+    request_openapi_examples = json.load(file)
 
 # Functional router
 router = APIRouter()
 
 
 def parse_logits_processors(request_dict: dict, prompt: str, model: AsyncLLMEngine, tokenizer: PreTrainedTokenizerBase,
                             tokenizer_lmformatenforcer: TokenEnforcerTokenizerData) -> list:
@@ -97,28 +106,35 @@
     else:
         prompt_in_response = False
     detect_logits_processors_incompatibilities(request_dict)
     logits_processors = parse_logits_processors(request_dict, prompt, model, tokenizer, tokenizer_lmformatenforcer)
     sampling_params = SamplingParams(**request_dict)
     sampling_params.logits_processors = logits_processors
     for logits_processor in logits_processors:
-        if isinstance(logits_processor, VLLMLogitsProcessorMinTokens):
-            min_tokens = logits_processor.min_tokens
-            if min_tokens > sampling_params.max_tokens:
-                raise ValueError(f"min_tokens : {min_tokens} can't be superior to max_tokens : {sampling_params.max_tokens}")
+        if isinstance(logits_processor, VLLMLogitsProcessorResponsePool):
+            min_tokens = sampling_params.min_tokens
+            reponse_pool = logits_processor.possible_tokens_responses
+            if min_tokens > 0 and len(reponse_pool):
+                raise ValueError(f"min_tokens : {min_tokens} is incompatible with the `response_pool` keyword")
     return prompt, prompt_in_response, sampling_params
 
 
-@router.post("/generate")
-async def generate(request: Request) -> Response:
+@router.post("/generate", response_model=ResponseGenerate)
+async def generate(
+    request: Request,
+    request_type: Annotated[
+        RequestGenerate,
+        Body(openapi_examples=request_openapi_examples["generate"])] = None
+    ) -> Response:
     """Generate completion for the request.
 
     The request should be a JSON object with the following fields:
     - prompt: The prompt to use for the generation.
-    - other fields: The sampling parameters (See `SamplingParams` for details).
+    - other fields: The sampling parameters (See `SamplingParams` from vLLM for more details : 
+                                             https://github.com/vllm-project/vllm/blob/main/vllm/sampling_params.py).
     """
     
     model: Model = RESOURCES.get(RESOURCE_MODEL)
     request_dict = await request.json()
     prompt, prompt_in_response, sampling_params = parse_generate_parameters(request_dict, model._model, model._tokenizer, model._tokenizer_lmformatenforcer)
     request_id = random_uuid()
     model._tokenizer.truncation_side = model.original_truncation_side
@@ -141,16 +157,20 @@
     finish_reasons = ["None" if finish_reason is None else finish_reason for finish_reason in finish_reasons]
     ret = {"responses": text_outputs, "finish_reasons": finish_reasons}
     if prompt_in_response:
         ret['prompt'] = prompt
     return JSONResponse(ret)
 
 
-@router.post("/generate_stream")
-async def generate_stream(request: Request) -> StreamingResponse:
+@router.post("/generate_stream", response_model=ResponseGenerate)
+async def generate_stream(request: Request,
+    request_type: Annotated[
+        RequestGenerate,
+        Body(openapi_examples=request_openapi_examples["generate_stream"])] = None
+    ) -> StreamingResponse:
     """Generate completion for the request.
 
     The request should be a JSON object with the following fields:
     - prompt: The prompt to use for the generation.
     - other fields: The sampling parameters (See `SamplingParams` for details).
     """
     model: Model = RESOURCES.get(RESOURCE_MODEL)
@@ -172,16 +192,20 @@
             if prompt_in_response:
                 ret['prompt'] = prompt
             yield (json.dumps(ret) + "\n")#.encode("utf-8")
 
     return StreamingResponse(stream_results())
 
 
-@router.post("/tokenizer")
-async def tokenizer(request: Request) -> Response:
+@router.post("/tokenizer", response_model=ResponseTokenizer)
+async def tokenizer(request: Request,
+    request_type: Annotated[
+        RequestTokenizer,
+        Body(openapi_examples=request_openapi_examples["tokenizer"])] = None
+    ) -> Response:
     """Tokenizes a text
 
     The request should be a JSON object with the following fields:
     - text: The text to tokenize
     - with_tokens_str (optional): Whether we want the tokens strings in the output
     - vanilla (optional) : Whether we want the vanilla version of the tokenizers
     """
@@ -203,16 +227,20 @@
 
     ret = {"tokens_ids": tokens_ids, "tokens_nb": len(tokens_ids)}
     if with_tokens_str:
         ret['tokens_str'] = tokens_str
     return JSONResponse(ret)
 
 
-@router.post("/decode")
-async def decode(request: Request) -> Response:
+@router.post("/decode", response_model=ResponseDecode)
+async def decode(request: Request,
+    request_type: Annotated[
+        RequestDecode,
+        Body(openapi_examples=request_openapi_examples["decode"])] = None
+    ) -> Response:
     """Decodes token ids
 
     The request should be a JSON object with the following fields:
     - token_ids: The ids of the tokens
     - with_tokens_str : If the result should also include a list of str
     - vanilla (optional) : Whether we want the vanilla version of the tokenizers
     """
@@ -234,34 +262,41 @@
 
     ret = {"decoded_string": decoded_string}
     if with_tokens_str:
         ret[ "tokens_str"] = tokens_str
     return JSONResponse(ret)
 
 
-@router.post("/split_text")
-async def split_text(request: Request):
-    """Splits a text
+@router.post("/split_text", response_model=ResponseSplitText)
+async def split_text(request: Request,
+    request_type: Annotated[
+        RequestSplitText,
+        Body(openapi_examples=request_openapi_examples["split_text"])] = None
+    ):
+    """Splits a text with a minimal number of token in each chunk. Each chunk is delimited by a separator
 
     The request should be a JSON object with the following fields:
     - text: The text to split
-    - num_tokens_in_chunk (optional): The minimal number of tokens we want in each split
+    - num_tokens_in_chunk (optional): The minimal number of tokens we want in each chunk
     - separators (optional) : The allowed separators between the chunks
     """
     model: Model = RESOURCES.get(RESOURCE_MODEL)
 
     request_dict = await request.json()
     split_text = model.split_text(**request_dict)
     response = {"split_text": split_text}
 
     return JSONResponse(response)
 
 
-@router.post("/metadata_text")
-async def metadata_text(request: Request):
+@router.post("/metadata_text", response_model=ResponseMetadata)
+async def metadata_text(request: Request,
+    request_type: Annotated[
+        RequestMetadata,
+        Body(openapi_examples=request_openapi_examples["metadata_text"])] = None):
     """Gives meta data on a text
 
     The request should be a JSON object with the following fields:
     - text: The text to parse
     - truncation_side (optional): The truncation side of the tokenizer
     - max_length (optional) : The max length before truncation
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/routers/schemas/__init__.py` & `happy_vllm-1.0.0/src/happy_vllm/routers/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/src/happy_vllm/routers/schemas/utils.py` & `happy_vllm-1.0.0/src/happy_vllm/routers/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/src/happy_vllm/routers/technical.py` & `happy_vllm-1.0.0/src/happy_vllm/routers/technical.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
+from typing import Annotated
 from fastapi import APIRouter
+from pydantic import BaseModel, Field
 from starlette.responses import JSONResponse
 
-from ..core.config import settings
 from ..core.resources import RESOURCES, RESOURCE_MODEL
 from ..model.model_base import Model
-from .schemas.technical import ResponseInformation, ResponseLiveness, ResponseReadiness
+from .schemas.technical import ResponseInformation, ResponseLiveness, ResponseReadiness, ResponseLiveMetrics
+
+from happy_vllm import utils
 
 # Technical router
 router = APIRouter()
 
 
 @router.get(
     "/liveness",
@@ -62,24 +65,27 @@
     tags=["technical"],
 )
 async def info() -> ResponseInformation:
     """Rest resource for info"""
     model: Model = RESOURCES.get(RESOURCE_MODEL)
 
     return ResponseInformation(
-        application=settings.app_name,
-        version=settings.app_version,
+        application=model.app_name,
+        version=utils.get_package_version(),
         model_name=model._model_conf.get("model_name", "?"),
+        vllm_version=utils.get_vllm_version(),
         truncation_side=model.original_truncation_side,
         max_length=model.max_model_len
     )
 
 
-@router.get("/live_metrics")
+@router.get("/live_metrics", response_model=ResponseLiveMetrics)
 async def get_live_metrics() -> JSONResponse:
+    """Deprecated. You should use now the /metrics endpoint
+    """
     model: Model = RESOURCES.get(RESOURCE_MODEL)
 
     gpu_cache_usage = model.get_gpu_kv_cache_usage()
     cpu_cache_usage = model.get_cpu_kv_cache_usage()
     metrics = model.get_status_requests()
     metrics["gpu_cache_usage"] = gpu_cache_usage
     metrics["cpu_cache_usage"] = cpu_cache_usage
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm/utils.py` & `happy_vllm-1.0.0/src/happy_vllm/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,32 +18,43 @@
 from pathlib import Path
 import importlib.metadata
 from typing import List, Union
 
 
 logger = logging.getLogger(__name__)
 
+TEST_TOKENIZER_NAME = "mistralai/Mixtral-8x7B-Instruct-v0.1"
 
 def get_package_version() -> str:
     '''Returns the current version of the package
 
     Returns:
         str: version of the package
     '''
     version = importlib.metadata.version("happy_vllm")
     return version
 
 
+def get_vllm_version() -> str:
+    '''Returns the installed version of vLLM 
+
+    Returns:
+        str: version of vLLM
+    '''
+    version = importlib.metadata.version("vllm")
+    return version
+
+
 def proper_tokenization(tokenizer, str_to_tokenize: str) -> tuple:
     """Gets the token ids for a str. We must use this technique in order to get the right token ids
     with their whitespace in the case of some tokenizers (e.g. Llama) adding whitespace in front of the tokenized sentence
 
     Args:
         tokenizer : A tokenizer
-        str_to_tokenizer (str) : The string one wants to tokenize
+        str_to_tokenize (str) : The string one wants to tokenize
 
     Returns:
         tuple : The tuple containing the token ids for the input string
     """
     big_word = 'thisisareallybigwordisntit'
     token_ids_big_word = tokenizer(big_word, add_special_tokens=False)['input_ids']
     # We concatenate the big word with the str in order for the str not to be at the beginning of the sentence
```

### Comparing `happy_vllm-0.9.0/src/happy_vllm.egg-info/SOURCES.txt` & `happy_vllm-1.0.0/src/happy_vllm.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 pyproject.toml
 setup.py
 version.txt
 src/happy_vllm/__init__.py
 src/happy_vllm/application.py
 src/happy_vllm/launch.py
 src/happy_vllm/utils.py
+src/happy_vllm/utils_args.py
 src/happy_vllm.egg-info/PKG-INFO
 src/happy_vllm.egg-info/SOURCES.txt
 src/happy_vllm.egg-info/dependency_links.txt
 src/happy_vllm.egg-info/entry_points.txt
 src/happy_vllm.egg-info/requires.txt
 src/happy_vllm.egg-info/top_level.txt
 src/happy_vllm/core/__init__.py
 src/happy_vllm/core/config.py
 src/happy_vllm/core/logtools.py
 src/happy_vllm/core/resources.py
 src/happy_vllm/logits_processors/__init__.py
 src/happy_vllm/logits_processors/json_format.py
-src/happy_vllm/logits_processors/min_tokens.py
 src/happy_vllm/logits_processors/response_pool.py
 src/happy_vllm/logits_processors/utils_parse_logits_processors.py
+src/happy_vllm/middlewares/__init__.py
 src/happy_vllm/middlewares/exception.py
 src/happy_vllm/model/__init__.py
 src/happy_vllm/model/model_base.py
 src/happy_vllm/routers/__init__.py
 src/happy_vllm/routers/functional.py
 src/happy_vllm/routers/technical.py
 src/happy_vllm/routers/schemas/__init__.py
 src/happy_vllm/routers/schemas/functional.py
 src/happy_vllm/routers/schemas/technical.py
 src/happy_vllm/routers/schemas/utils.py
-tests/test_config.py
+src/happy_vllm/routers/schemas/examples/request.json
+src/happy_vllm/routers/schemas/examples/response.json
 tests/test_json_format.py
-tests/test_min_tokens.py
 tests/test_model_base.py
 tests/test_response_pool.py
 tests/test_routers_functionnal.py
 tests/test_routers_technical.py
 tests/test_schemas_utils.py
 tests/test_utils.py
+tests/test_utils_args.py
 tests/test_utils_parse_logits_processors.py
```

### Comparing `happy_vllm-0.9.0/tests/test_json_format.py` & `happy_vllm-1.0.0/tests/test_json_format.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/tests/test_model_base.py` & `happy_vllm-1.0.0/tests/test_model_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,26 +29,26 @@
 def teardown_module():
     if os.path.exists(TEST_MODELS_DIR):
         if os.path.isdir(TEST_MODELS_DIR):
             shutil.rmtree(TEST_MODELS_DIR)
 
 
 def init_model(truncation_side="left"):
-    model = Model()
+    model = Model(app_name=os.environ['app_name'])
     model._tokenizer = AutoTokenizer.from_pretrained(os.environ["tokenizer_name"],
                                                      cache_dir=TEST_MODELS_DIR, truncation_side=truncation_side)
     model.original_truncation_side = truncation_side
     model.max_model_len = 2048
     return model
 
 
 def test_is_model_loaded():
     model = init_model()
     assert not(model.is_model_loaded())
-    model.loading(Namespace())
+    model.loading(Namespace(model_name=os.environ["MODEL_NAME"], model=os.environ['MODEL']))
     assert model.is_model_loaded()
 
 
 def test_tokenize():
     model = init_model()
     prompts = ["Hey it's me. How are you ?", "Fine. You ?", " I'm feeling really great "]
     for prompt in prompts:
```

### Comparing `happy_vllm-0.9.0/tests/test_response_pool.py` & `happy_vllm-1.0.0/tests/test_response_pool.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/tests/test_routers_functionnal.py` & `happy_vllm-1.0.0/tests/test_routers_functionnal.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,26 +25,25 @@
 
 
 from happy_vllm import utils
 from .conftest import TEST_MODELS_DIR
 from happy_vllm.routers import functional
 from happy_vllm.model.model_base import Model
 from happy_vllm.logits_processors.json_format import VLLMLogitsProcessorJSON
-from happy_vllm.logits_processors.min_tokens import VLLMLogitsProcessorMinTokens
 from happy_vllm.logits_processors.response_pool import VLLMLogitsProcessorResponsePool
 
 
 def teardown_module():
     if os.path.exists(TEST_MODELS_DIR):
         if os.path.isdir(TEST_MODELS_DIR):
             shutil.rmtree(TEST_MODELS_DIR)
 
 
 def init_model(truncation_side="left"):
-    model = Model()
+    model = Model(app_name=os.environ['app_name'])
     model._tokenizer = AutoTokenizer.from_pretrained(os.environ["tokenizer_name"],
                                                      cache_dir=TEST_MODELS_DIR, truncation_side=truncation_side)
     model._tokenizer_lmformatenforcer = build_token_enforcer_tokenizer_data(model._tokenizer)
     model.original_truncation_side = truncation_side
     model.max_model_len = 2048
     return model
 
@@ -62,25 +61,14 @@
         logits_processors = functional.parse_logits_processors(request_dict, prompt, model, tokenizer, tokenizer_lmformatenforcer)
         assert request_dict == {"temperature": 0, "keyword": "value"}
         assert len(logits_processors) == 1
         assert isinstance(logits_processors[0], VLLMLogitsProcessorResponsePool)
         assert len(logits_processors[0].possible_tokens_responses) == len(response_pool)
         assert logits_processors[0].eos_token_id == tokenizer.eos_token_id
 
-    # With min_tokens
-    prompt = "This is the prompt"
-    for min_tokens in [10, 500]:
-        request_dict = {'temperature': 0, "keyword": "value", "min_tokens": min_tokens}
-        logits_processors = functional.parse_logits_processors(request_dict, prompt, model, tokenizer, tokenizer_lmformatenforcer)
-        assert request_dict == {"temperature": 0, "keyword": "value"}
-        assert len(logits_processors) == 1
-        assert isinstance(logits_processors[0], VLLMLogitsProcessorMinTokens)
-        assert logits_processors[0].min_tokens == min_tokens
-        assert logits_processors[0].eos_token_id == tokenizer.eos_token_id
-
     # With json_format
     prompt = "This is the prompt"
     json_format = {"name": "string",
                     "surname": "string",
                     "favorite_food": "string",
                     "current_number_of_children": "integer",
                     "team_name": "string",
@@ -97,38 +85,15 @@
     json_format = {}
     request_dict = {"temperature": 0, "keyword": "value", "json_format": json_format}
     logits_processors = functional.parse_logits_processors(request_dict, prompt, model, tokenizer, tokenizer_lmformatenforcer)
     assert request_dict == {"temperature": 0, "keyword": "value"}
     assert len(logits_processors) == 1
     assert isinstance(logits_processors[0], VLLMLogitsProcessorJSON)
     assert not(logits_processors[0].logits_processor_activated)
-
-    # With min_tokens and response_pool
-    prompt = "This is the prompt"
-    for min_tokens in [10, 500]:
-        for response_pool in [["Yes", "No"], ["Certainly", "I think so", "Of course"], ["Without a doubt"]]:
-            request_dict = {'temperature': 0, "keyword": "value", "min_tokens": min_tokens, "response_pool": response_pool}
-            logits_processors = functional.parse_logits_processors(request_dict, prompt, model, tokenizer, tokenizer_lmformatenforcer)
-            assert request_dict == {"temperature": 0, "keyword": "value"}
-            assert len(logits_processors) == 2
-            if isinstance(logits_processors[0], VLLMLogitsProcessorMinTokens):
-                assert isinstance(logits_processors[1], VLLMLogitsProcessorResponsePool)
-                assert logits_processors[0].min_tokens == min_tokens
-                assert logits_processors[0].eos_token_id == tokenizer.eos_token_id
-                assert len(logits_processors[1].possible_tokens_responses) == len(response_pool)
-                assert logits_processors[1].eos_token_id == tokenizer.eos_token_id
-            else:
-                assert isinstance(logits_processors[0], VLLMLogitsProcessorResponsePool)
-                assert isinstance(logits_processors[1], VLLMLogitsProcessorMinTokens)
-                assert logits_processors[1].min_tokens == min_tokens
-                assert logits_processors[1].eos_token_id == tokenizer.eos_token_id
-                assert len(logits_processors[0].possible_tokens_responses) == len(response_pool)
-                assert logits_processors[0].eos_token_id == tokenizer.eos_token_id
             
-
     # Without logits_processors
     request_dict = {"temperature": 0, "keyword": "value"}
     logits_processors = functional.parse_logits_processors(request_dict, prompt, model, tokenizer, tokenizer_lmformatenforcer)
     assert request_dict == {"temperature": 0, "keyword": "value"}
     assert logits_processors == []
 
 
@@ -146,26 +111,14 @@
     assert prompt == prompt_ini
     assert not(prompt_in_response)
     assert isinstance(sampling_params, SamplingParams)
     assert sampling_params.temperature == temperature
     assert len(sampling_params.logits_processors) == 1
     assert isinstance(sampling_params.logits_processors[0], VLLMLogitsProcessorResponsePool)
 
-    # with min_tokens
-    prompt_ini = "This is the prompt"
-    temperature = 0
-    request_dict = {"temperature": temperature, "min_tokens": 10, "prompt": prompt_ini, "max_tokens": 100}
-    prompt, prompt_in_response, sampling_params = functional.parse_generate_parameters(request_dict, model, tokenizer, tokenizer_lmformatenforcer)
-    assert prompt == prompt_ini
-    assert not(prompt_in_response)
-    assert isinstance(sampling_params, SamplingParams)
-    assert sampling_params.temperature == temperature
-    assert len(sampling_params.logits_processors) == 1
-    assert isinstance(sampling_params.logits_processors[0], VLLMLogitsProcessorMinTokens)
-
     # with json_format
     prompt_ini = "This is the prompt"
     temperature = 0
     json_format = {"name": "string",
                     "surname": "string",
                     "favorite_food": "string",
                     "current_number_of_children": "integer",
@@ -202,23 +155,14 @@
     assert prompt == prompt_ini
     assert not(prompt_in_response)
     assert isinstance(sampling_params, SamplingParams)
     assert sampling_params.temperature == temperature
     assert sampling_params.max_tokens == max_tokens
     assert sampling_params.logits_processors == []
 
-    # Raise ValueError if min_tokens superior to max_tokens
-    prompt_ini = "Here"
-    temperature = 0.1
-    max_tokens = 10
-    min_tokens = 20
-    request_dict = {'temperature': temperature, "prompt": prompt_ini, "max_tokens": max_tokens, "min_tokens": min_tokens}
-    with pytest.raises(ValueError):
-        prompt, prompt_in_response, sampling_params = functional.parse_generate_parameters(request_dict, model, tokenizer, tokenizer_lmformatenforcer)
-
     # Raise ValueError if response_pool and min_tokens are present
     prompt_ini = "This is the prompt"
     temperature = 0
     request_dict = {"temperature": temperature, "response_pool": ["Yes", "No"], "prompt": prompt_ini, "min_tokens": 10, "max_tokens": 100}
     with pytest.raises(ValueError):
         prompt, prompt_in_response, sampling_params = functional.parse_generate_parameters(request_dict, model, tokenizer, tokenizer_lmformatenforcer)
```

### Comparing `happy_vllm-0.9.0/tests/test_routers_technical.py` & `happy_vllm-1.0.0/tests/test_routers_technical.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/tests/test_schemas_utils.py` & `happy_vllm-1.0.0/tests/test_schemas_utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-0.9.0/tests/test_utils.py` & `happy_vllm-1.0.0/tests/test_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 
 def test_get_package_version():
     # Nominal case
     version = utils.get_package_version()
     assert version == importlib.metadata.version("happy_vllm")
 
 
+def test_get_vllm_version():
+    # Nominal case
+    version = utils.get_vllm_version()
+    assert version == importlib.metadata.version("vllm")
+
+
 def test_proper_tokenization():
     tokenizer = AutoTokenizer.from_pretrained(os.environ["tokenizer_name"],
                                                      cache_dir=TEST_MODELS_DIR)
     for string in ['.', '!', '?', 'Hey', 'hey']:
         assert utils.proper_tokenization(tokenizer, f' {string}') != utils.proper_tokenization(tokenizer, f'{string}')
     for string in ['.', '!', '?']:
         assert utils.proper_tokenization(tokenizer, f'reallybigword{string}')[-1] == utils.proper_tokenization(tokenizer, f'{string}')[-1]
```

### Comparing `happy_vllm-0.9.0/tests/test_utils_parse_logits_processors.py` & `happy_vllm-1.0.0/tests/test_utils_parse_logits_processors.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,16 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import pytest
 from happy_vllm.logits_processors.utils_parse_logits_processors import detect_logits_processors_incompatibilities
 
 
 def test_detect_logits_processors_incompatibilities():
-    request_dict = {"prompt": "my_prompt", "min_tokens": 10}
-    assert detect_logits_processors_incompatibilities(request_dict) is None
-
     request_dict = {"prompt": "my_prompt", "response_pool": ["Yes", "No"]}
     assert detect_logits_processors_incompatibilities(request_dict) is None
 
     request_dict = {"prompt": "my_prompt", "json_format": {"name": "Smith"}}
     assert detect_logits_processors_incompatibilities(request_dict) is None
 
-    request_dict = {"prompt": "my_prompt", "response_pool": ["Yes", "No"], "min_tokens": 10}
-    with pytest.raises(ValueError):
-        detect_logits_processors_incompatibilities(request_dict)
-
     request_dict = {"prompt": "my_prompt", "response_pool": ["Yes", "No"], "json_format": {"name": "Smith"}}
     with pytest.raises(ValueError):
         detect_logits_processors_incompatibilities(request_dict)
```

