# Comparing `tmp/codeflash-0.4.1.tar.gz` & `tmp/codeflash-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflash-0.4.1.tar", max compression
+gzip compressed data, was "codeflash-0.5.0.tar", max compression
```

## Comparing `codeflash-0.4.1.tar` & `codeflash-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.4.1/README.md
--rw-r--r--   0        0        0     4405 2024-03-28 19:41:32.236055 codeflash-0.4.1/codeflash/LICENSE
--rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.4.1/codeflash/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.4.1/codeflash/api/__init__.py
--rw-r--r--   0        0        0     8032 2024-03-24 21:57:44.195257 codeflash-0.4.1/codeflash/api/aiservice.py
--rw-r--r--   0        0        0     4703 2024-03-06 13:45:57.132901 codeflash-0.4.1/codeflash/api/cfapi.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.4.1/codeflash/cli_cmds/__init__.py
--rw-r--r--   0        0        0     5663 2024-03-28 19:34:42.184309 codeflash-0.4.1/codeflash/cli_cmds/cli.py
--rw-r--r--   0        0        0    22938 2024-03-28 19:23:17.899995 codeflash-0.4.1/codeflash/cli_cmds/cmd_init.py
--rw-r--r--   0        0        0      156 2024-02-01 23:15:04.021654 codeflash-0.4.1/codeflash/cli_cmds/logging_config.py
--rw-r--r--   0        0        0     1827 2024-03-24 21:57:44.196107 codeflash-0.4.1/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.4.1/codeflash/code_utils/__init__.py
--rw-r--r--   0        0        0     6075 2024-03-27 00:52:14.608080 codeflash-0.4.1/codeflash/code_utils/code_extractor.py
--rw-r--r--   0        0        0     8886 2024-03-13 16:48:07.259135 codeflash-0.4.1/codeflash/code_utils/code_replacer.py
--rw-r--r--   0        0        0     2618 2024-03-27 23:33:18.926667 codeflash-0.4.1/codeflash/code_utils/code_utils.py
--rw-r--r--   0        0        0      273 2024-03-09 12:14:07.997779 codeflash-0.4.1/codeflash/code_utils/compat.py
--rw-r--r--   0        0        0      224 2024-02-10 04:17:44.568348 codeflash-0.4.1/codeflash/code_utils/config_consts.py
--rw-r--r--   0        0        0     3787 2024-03-28 02:17:40.188233 codeflash-0.4.1/codeflash/code_utils/config_parser.py
--rw-r--r--   0        0        0     2908 2024-03-27 00:52:14.608425 codeflash-0.4.1/codeflash/code_utils/env_utils.py
--rw-r--r--   0        0        0     1126 2024-03-04 14:49:38.000000 codeflash-0.4.1/codeflash/code_utils/formatter.py
--rw-r--r--   0        0        0     3314 2024-03-06 13:45:57.133899 codeflash-0.4.1/codeflash/code_utils/git_utils.py
--rw-r--r--   0        0        0    22288 2024-03-27 23:33:18.927147 codeflash-0.4.1/codeflash/code_utils/instrument_existing_tests.py
--rw-r--r--   0        0        0     3501 2024-03-28 19:16:33.995378 codeflash-0.4.1/codeflash/code_utils/shell_utils.py
--rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.4.1/codeflash/code_utils/sqlalchemy_utils.py
--rw-r--r--   0        0        0     1860 2024-01-24 20:13:21.332617 codeflash-0.4.1/codeflash/code_utils/time_utils.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.4.1/codeflash/discovery/__init__.py
--rw-r--r--   0        0        0    16183 2024-03-13 16:48:07.259994 codeflash-0.4.1/codeflash/discovery/discover_unit_tests.py
--rw-r--r--   0        0        0    12154 2024-03-27 23:33:18.927697 codeflash-0.4.1/codeflash/discovery/functions_to_optimize.py
--rw-r--r--   0        0        0     1229 2024-02-13 02:11:11.092168 codeflash-0.4.1/codeflash/github/PrComment.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.4.1/codeflash/github/__init__.py
--rw-r--r--   0        0        0    42941 2024-03-28 19:40:56.867619 codeflash-0.4.1/codeflash/main.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.4.1/codeflash/optimization/__init__.py
--rw-r--r--   0        0        0    10994 2024-03-27 23:33:18.928748 codeflash-0.4.1/codeflash/optimization/function_context.py
--rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.4.1/codeflash/result/__init__.py
--rw-r--r--   0        0        0     3959 2024-03-02 17:26:31.551442 codeflash-0.4.1/codeflash/result/create_pr.py
--rw-r--r--   0        0        0     1982 2024-02-01 23:15:04.024170 codeflash-0.4.1/codeflash/result/explanation.py
--rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.4.1/codeflash/telemetry/__init__.py
--rw-r--r--   0        0        0     1257 2024-03-19 02:04:16.181201 codeflash-0.4.1/codeflash/telemetry/posthog.py
--rw-r--r--   0        0        0      579 2024-03-19 02:04:16.181306 codeflash-0.4.1/codeflash/telemetry/sentry.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278612 codeflash-0.4.1/codeflash/tracing/__init__.py
--rw-r--r--   0        0        0     4812 2024-01-27 05:49:30.994620 codeflash-0.4.1/codeflash/tracing/replay_test.py
--rw-r--r--   0        0        0     5112 2024-03-24 21:57:44.197418 codeflash-0.4.1/codeflash/tracing/tracer.py
--rw-r--r--   0        0        0     1910 2024-03-24 21:57:44.197591 codeflash-0.4.1/codeflash/update_license_version.py
--rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.4.1/codeflash/verification/__init__.py
--rw-r--r--   0        0        0     4140 2024-03-27 00:52:14.608873 codeflash-0.4.1/codeflash/verification/comparator.py
--rw-r--r--   0        0        0      772 2024-01-05 04:36:50.279407 codeflash-0.4.1/codeflash/verification/equivalence.py
--rw-r--r--   0        0        0    14367 2024-03-28 19:16:33.996574 codeflash-0.4.1/codeflash/verification/parse_test_output.py
--rw-r--r--   0        0        0     6310 2024-01-27 18:00:34.971647 codeflash-0.4.1/codeflash/verification/test_results.py
--rw-r--r--   0        0        0     1580 2024-03-24 21:57:44.197705 codeflash-0.4.1/codeflash/verification/test_runner.py
--rw-r--r--   0        0        0     2366 2024-01-27 18:57:54.493049 codeflash-0.4.1/codeflash/verification/verification_utils.py
--rw-r--r--   0        0        0     4242 2024-03-24 21:57:44.198063 codeflash-0.4.1/codeflash/verification/verifier.py
--rw-r--r--   0        0        0      150 2024-03-28 19:41:58.962067 codeflash-0.4.1/codeflash/version.py
--rw-r--r--   0        0        0     2754 2024-03-28 19:41:58.961404 codeflash-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 codeflash-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.5.0/README.md
+-rw-r--r--   0        0        0     4405 2024-04-11 20:54:38.441461 codeflash-0.5.0/codeflash/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.5.0/codeflash/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.5.0/codeflash/api/__init__.py
+-rw-r--r--   0        0        0     8122 2024-04-10 21:49:12.465747 codeflash-0.5.0/codeflash/api/aiservice.py
+-rw-r--r--   0        0        0     4703 2024-03-06 13:45:57.132901 codeflash-0.5.0/codeflash/api/cfapi.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.5.0/codeflash/cli_cmds/__init__.py
+-rw-r--r--   0        0        0     5655 2024-04-10 20:56:46.198285 codeflash-0.5.0/codeflash/cli_cmds/cli.py
+-rw-r--r--   0        0        0    22938 2024-03-30 21:18:28.910786 codeflash-0.5.0/codeflash/cli_cmds/cmd_init.py
+-rw-r--r--   0        0        0      156 2024-02-01 23:15:04.021654 codeflash-0.5.0/codeflash/cli_cmds/logging_config.py
+-rw-r--r--   0        0        0     1827 2024-03-24 21:57:44.196107 codeflash-0.5.0/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.5.0/codeflash/code_utils/__init__.py
+-rw-r--r--   0        0        0     7170 2024-04-10 21:49:12.465898 codeflash-0.5.0/codeflash/code_utils/code_extractor.py
+-rw-r--r--   0        0        0     9450 2024-04-10 21:49:12.466063 codeflash-0.5.0/codeflash/code_utils/code_replacer.py
+-rw-r--r--   0        0        0     2618 2024-03-27 23:33:18.926667 codeflash-0.5.0/codeflash/code_utils/code_utils.py
+-rw-r--r--   0        0        0      273 2024-03-09 12:14:07.997779 codeflash-0.5.0/codeflash/code_utils/compat.py
+-rw-r--r--   0        0        0      224 2024-02-10 04:17:44.568348 codeflash-0.5.0/codeflash/code_utils/config_consts.py
+-rw-r--r--   0        0        0     3906 2024-04-02 23:26:25.038599 codeflash-0.5.0/codeflash/code_utils/config_parser.py
+-rw-r--r--   0        0        0     2908 2024-03-30 02:05:25.997181 codeflash-0.5.0/codeflash/code_utils/env_utils.py
+-rw-r--r--   0        0        0     1988 2024-03-29 22:03:45.051414 codeflash-0.5.0/codeflash/code_utils/formatter.py
+-rw-r--r--   0        0        0     3308 2024-04-08 00:04:34.442696 codeflash-0.5.0/codeflash/code_utils/git_utils.py
+-rw-r--r--   0        0        0    22288 2024-03-27 23:33:18.927147 codeflash-0.5.0/codeflash/code_utils/instrument_existing_tests.py
+-rw-r--r--   0        0        0     3501 2024-03-28 19:16:33.995378 codeflash-0.5.0/codeflash/code_utils/shell_utils.py
+-rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.5.0/codeflash/code_utils/sqlalchemy_utils.py
+-rw-r--r--   0        0        0     1860 2024-01-24 20:13:21.332617 codeflash-0.5.0/codeflash/code_utils/time_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.5.0/codeflash/discovery/__init__.py
+-rw-r--r--   0        0        0    16183 2024-03-13 16:48:07.259994 codeflash-0.5.0/codeflash/discovery/discover_unit_tests.py
+-rw-r--r--   0        0        0    12182 2024-04-10 20:56:46.198974 codeflash-0.5.0/codeflash/discovery/functions_to_optimize.py
+-rw-r--r--   0        0        0     1229 2024-02-13 02:11:11.092168 codeflash-0.5.0/codeflash/github/PrComment.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.5.0/codeflash/github/__init__.py
+-rw-r--r--   0        0        0    44529 2024-04-10 21:49:12.466361 codeflash-0.5.0/codeflash/main.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.5.0/codeflash/optimization/__init__.py
+-rw-r--r--   0        0        0    11557 2024-04-10 21:49:12.466508 codeflash-0.5.0/codeflash/optimization/function_context.py
+-rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.5.0/codeflash/result/__init__.py
+-rw-r--r--   0        0        0     3959 2024-03-02 17:26:31.551442 codeflash-0.5.0/codeflash/result/create_pr.py
+-rw-r--r--   0        0        0     1982 2024-02-01 23:15:04.024170 codeflash-0.5.0/codeflash/result/explanation.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.5.0/codeflash/telemetry/__init__.py
+-rw-r--r--   0        0        0     1257 2024-03-19 02:04:16.181201 codeflash-0.5.0/codeflash/telemetry/posthog.py
+-rw-r--r--   0        0        0      579 2024-03-19 02:04:16.181306 codeflash-0.5.0/codeflash/telemetry/sentry.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:56:46.199644 codeflash-0.5.0/codeflash/tracing/__init__.py
+-rw-r--r--   0        0        0     4908 2024-04-10 20:56:46.200028 codeflash-0.5.0/codeflash/tracing/replay_test.py
+-rw-r--r--   0        0        0     5174 2024-04-10 20:56:46.200480 codeflash-0.5.0/codeflash/tracing/tracer.py
+-rw-r--r--   0        0        0     1910 2024-03-24 21:57:44.197591 codeflash-0.5.0/codeflash/update_license_version.py
+-rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.5.0/codeflash/verification/__init__.py
+-rw-r--r--   0        0        0     4733 2024-04-04 03:26:48.352761 codeflash-0.5.0/codeflash/verification/comparator.py
+-rw-r--r--   0        0        0     1139 2024-03-30 00:35:38.112124 codeflash-0.5.0/codeflash/verification/equivalence.py
+-rw-r--r--   0        0        0    14539 2024-04-08 00:04:34.443972 codeflash-0.5.0/codeflash/verification/parse_test_output.py
+-rw-r--r--   0        0        0     6681 2024-04-08 00:04:34.444171 codeflash-0.5.0/codeflash/verification/test_results.py
+-rw-r--r--   0        0        0     1580 2024-03-24 21:57:44.197705 codeflash-0.5.0/codeflash/verification/test_runner.py
+-rw-r--r--   0        0        0     2366 2024-04-10 20:56:46.200732 codeflash-0.5.0/codeflash/verification/verification_utils.py
+-rw-r--r--   0        0        0     4242 2024-03-24 21:57:44.198063 codeflash-0.5.0/codeflash/verification/verifier.py
+-rw-r--r--   0        0        0      150 2024-04-11 20:55:45.133024 codeflash-0.5.0/codeflash/version.py
+-rw-r--r--   0        0        0     2915 2024-04-11 20:55:45.132371 codeflash-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 codeflash-0.5.0/PKG-INFO
```

### Comparing `codeflash-0.4.1/codeflash/LICENSE` & `codeflash-0.5.0/codeflash/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/api/aiservice.py` & `codeflash-0.5.0/codeflash/api/aiservice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 import os
 import platform
-from typing import Any, Dict, List, Tuple, Optional
+from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 from pydantic.dataclasses import dataclass
 from pydantic.json import pydantic_encoder
 
 from codeflash.code_utils.env_utils import get_codeflash_api_key
 from codeflash.discovery.functions_to_optimize import FunctionToOptimize
@@ -21,29 +21,31 @@
 
 def make_ai_service_request(
     endpoint: str,
     method: str = "POST",
     payload: Optional[Dict[str, Any]] = None,
     timeout: float = None,
 ) -> requests.Response:
-    """
-    Make an API request to the given endpoint on the AI service.
+    """Make an API request to the given endpoint on the AI service.
     :param endpoint: The endpoint to call, e.g., "/optimize".
     :param method: The HTTP method to use ('GET' or 'POST').
     :param payload: Optional JSON payload to include in the POST request body.
     :param timeout: The timeout for the request.
     :return: The response object from the API.
     """
     url = f"{AI_SERVICE_BASE_URL}/ai{endpoint}"
     ai_service_headers = {"Authorization": f"Bearer {get_codeflash_api_key()}"}
     if method.upper() == "POST":
         json_payload = json.dumps(payload, indent=None, default=pydantic_encoder)
         ai_service_headers["Content-Type"] = "application/json"
         response = requests.post(
-            url, data=json_payload, headers=ai_service_headers, timeout=timeout
+            url,
+            data=json_payload,
+            headers=ai_service_headers,
+            timeout=timeout,
         )
     else:
         response = requests.get(url, headers=ai_service_headers, timeout=timeout)
     # response.raise_for_status()  # Will raise an HTTPError if the HTTP request returned an unsuccessful status code
     return response
 
 
@@ -56,55 +58,57 @@
 
 @dataclass(frozen=True)
 class Optimizations:
     optimizations: List[Optimization]
 
 
 def optimize_python_code(source_code: str, trace_id: str, num_variants: int = 10) -> Optimizations:
-    """
-    Optimize the given python code for performance by making a request to the Django endpoint.
+    """Optimize the given python code for performance by making a request to the Django endpoint.
 
-    Parameters:
+    Parameters
+    ----------
     - source_code (str): The python code to optimize.
     - num_variants (int): Number of optimization variants to generate. Default is 10.
 
-    Returns:
+    Returns
+    -------
     - List[Tuple[str, str]]: A list of tuples where the first element is the optimized code and the second is the explanation.
+
     """
     payload = {
         "source_code": source_code,
         "num_variants": num_variants,
         "trace_id": trace_id,
         "python_version": platform.python_version(),
     }
-    logging.info(f"Generating optimized candidates ...")
+    logging.info("Generating optimized candidates ...")
     try:
         response = make_ai_service_request("/optimize", payload=payload, timeout=600)
     except requests.exceptions.RequestException as e:
-        logging.error(f"Error generating optimized candidates: {e}")
+        logging.exception(f"Error generating optimized candidates: {e}")
         ph("cli-optimize-error-caught", {"error": str(e)})
         return Optimizations(optimizations=[])
 
     if response.status_code == 200:
         optimizations = response.json()["optimizations"]
         logging.info(f"Generated {len(optimizations)} candidates.")
         return Optimizations(
             [
                 Optimization(
                     source_code=opt["source_code"],
                     explanation=opt["explanation"],
                     optimization_id=opt["optimization_id"],
                 )
                 for opt in optimizations
-            ]
+            ],
         )
     else:
         try:
             error = response.json()["error"]
-        except Exception as e:
+        except Exception:
             error = response.text
         logging.error(f"Error generating optimized candidates: {response.status_code} - {error}")
         ph(
             "cli-optimize-error-response",
             {"response_status_code": response.status_code, "error": error},
         )
         return Optimizations(optimizations=[])
@@ -113,61 +117,64 @@
 def log_results(
     function_trace_id: str,
     speedup_ratio: Optional[Dict[str, float]],
     original_runtime: Optional[float],
     optimized_runtime: Optional[Dict[str, float]],
     is_correct: Optional[Dict[str, bool]],
 ) -> None:
-    """
-    Log features to the database.
+    """Log features to the database.
 
-    Parameters:
+    Parameters
+    ----------
     - function_trace_id (str): The UUID.
     - speedup_ratio (Optional[Dict[str, float]]): The speedup.
     - original_runtime (Optional[Dict[str, float]]): The original runtime.
     - optimized_runtime (Optional[Dict[str, float]]): The optimized runtime.
     - is_correct (Optional[Dict[str, bool]]): Whether the optimized code is correct.
+
     """
     payload = {
         "trace_id": function_trace_id,
         "speedup_ratio": speedup_ratio,
         "original_runtime": original_runtime,
         "optimized_runtime": optimized_runtime,
         "is_correct": is_correct,
     }
     try:
         make_ai_service_request("/log_features", payload=payload, timeout=5)
     except requests.exceptions.RequestException as e:
-        logging.error(f"Error logging features: {e}")
+        logging.exception(f"Error logging features: {e}")
 
 
 def generate_regression_tests(
     source_code_being_tested: str,
     function_to_optimize: FunctionToOptimize,
     dependent_function_names: list[str],
     module_path: str,
     test_module_path: str,
     test_framework: str,
     test_timeout: int,
     trace_id: str,
 ) -> Optional[Tuple[str, str]]:
-    """
-    Generate regression tests for the given function by making a request to the Django endpoint.
+    """Generate regression tests for the given function by making a request to the Django endpoint.
 
-    Parameters:
+    Parameters
+    ----------
     - source_code_being_tested (str): The source code of the function being tested.
     - function_to_optimize (FunctionToOptimize): The function to optimize.
     - dependent_function_names (list[Source]): List of dependent function names.
     - module_path (str): The module path where the function is located.
     - test_module_path (str): The module path for the test code.
     - test_framework (str): The test framework to use, e.g., "pytest".
     - test_timeout (int): The timeout for each test in seconds.
 
-    Returns:
+    Returns
+    -------
     - Dict[str, str] | None: The generated regression tests and instrumented tests, or None if an error occurred.
+
     """
     assert test_framework in [
         "pytest",
         "unittest",
     ], f"Invalid test framework, got {test_framework} but expected 'pytest' or 'unittest'"
     payload = {
         "source_code_being_tested": source_code_being_tested,
@@ -179,15 +186,15 @@
         "test_timeout": test_timeout,
         "trace_id": trace_id,
         "python_version": platform.python_version(),
     }
     try:
         response = make_ai_service_request("/testgen", payload=payload, timeout=600)
     except requests.exceptions.RequestException as e:
-        logging.error(f"Error generating tests: {e}")
+        logging.exception(f"Error generating tests: {e}")
         ph("cli-testgen-error-caught", {"error": str(e)})
         return None
 
     # the timeout should be the same as the timeout for the AI service backend
 
     if response.status_code == 200:
         response_json = response.json()
@@ -198,14 +205,14 @@
             error = response.json()["error"]
             logging.error(f"Error generating tests: {response.status_code} - {error}")
             ph(
                 "cli-testgen-error-response",
                 {"response_status_code": response.status_code, "error": error},
             )
             return None
-        except Exception as e:
-            logging.error(f"Error generating tests: {response.status_code} - {response.text}")
+        except Exception:
+            logging.exception(f"Error generating tests: {response.status_code} - {response.text}")
             ph(
                 "cli-testgen-error-response",
                 {"response_status_code": response.status_code, "error": response.text},
             )
             return None
```

### Comparing `codeflash-0.4.1/codeflash/api/cfapi.py` & `codeflash-0.5.0/codeflash/api/cfapi.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/cli_cmds/cli.py` & `codeflash-0.5.0/codeflash/cli_cmds/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         "tests_root",
         "test_framework",
         "ignore_paths",
         "minimum_performance_gain",
         "pytest_cmd",
         "formatter_cmd",
         "disable_telemetry",
+        "imports_sort_cmd",
     ]
     for key in supported_keys:
         if key in pyproject_config:
             if (
                 hasattr(args, key.replace("-", "_"))
                 and getattr(args, key.replace("-", "_")) is None
             ) or not hasattr(args, key.replace("-", "_")):
@@ -103,17 +104,15 @@
                 "I couldn't find a git repository in the current directory. "
                 "I need a git repository to run --all and open PRs for optimizations. Exiting..."
             )
             apologize_and_exit()
         owner, repo = get_repo_owner_and_name(git_repo)
         try:
             response = check_github_app_installed_on_repo(owner, repo)
-            if response.ok and response.text == "true":
-                pass
-            else:
+            if not response.ok or response.text != "true":
                 logging.error(f"Error: {response.text}")
                 raise Exception
         except Exception as e:
             logging.error(
                 f"Could not find the Codeflash GitHub App installed on the repository {owner}/{repo} or the GitHub"
                 f" account linked to your CODEFLASH_API_KEY does not have access to the repository {owner}/{repo}.{LF}"
                 "Please install the Codeflash GitHub App on your repository to use --all. You can install it by going to "
```

### Comparing `codeflash-0.4.1/codeflash/cli_cmds/cmd_init.py` & `codeflash-0.5.0/codeflash/cli_cmds/cmd_init.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/cli_cmds/workflows/codeflash-optimize.yaml` & `codeflash-0.5.0/codeflash/cli_cmds/workflows/codeflash-optimize.yaml`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/code_utils/code_extractor.py` & `codeflash-0.5.0/codeflash/code_utils/code_extractor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,38 @@
+from __future__ import annotations
+
 import ast
 import logging
 from collections import deque
-from typing import Optional, Union
 
 from codeflash.discovery.functions_to_optimize import FunctionToOptimize
 
 
-def get_code(function_to_optimize: FunctionToOptimize) -> Optional[str]:
-    """Returns the code for a class or function in a file."""
-    file_path: str = function_to_optimize.file_path
-    class_skeleton: list[tuple[int, int]] = []
+def get_code(
+    functions_to_optimize: list[FunctionToOptimize],
+) -> tuple[str | None, set[tuple[str, str]]]:
+    """Return the code for a class or functions in a file."""
+    file_path: str = functions_to_optimize[0].file_path
+    class_skeleton: set[tuple[int, int | None]] = set()
+    contextual_dunder_methods: set[tuple[str, str]] = set()
+    target_code: str = ""
 
     def find_target(
-        node_list: list[ast.stmt], name_parts: Union[tuple[str, str], tuple[str]]
-    ) -> Optional[ast.AST]:
-        target: Optional[
-            Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Assign, ast.AnnAssign]
-        ] = None
-        node: Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Assign, ast.AnnAssign]
-
+        node_list: list[ast.stmt],
+        name_parts: tuple[str, str] | tuple[str],
+    ) -> ast.AST | None:
+        target: (
+            ast.FunctionDef
+            | ast.AsyncFunctionDef
+            | ast.ClassDef
+            | ast.Assign
+            | ast.AnnAssign
+            | None
+        ) = None
+        node: ast.stmt
         for node in node_list:
             if (
                 # The many mypy issues will be fixed once this code moves to the backend,
                 # using Type Guards as we move to 3.10+.
                 # We will cover the Type Alias case on the backend since it's a 3.12 feature.
                 (
                     isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef))
@@ -44,94 +54,98 @@
                 target = node
                 break
 
         if target is None or len(name_parts) == 1:
             return target
 
         if isinstance(target, ast.ClassDef):
-            class_skeleton.append((target.lineno, target.lineno))
+            class_skeleton.add((target.lineno, target.lineno))
             cbody = target.body
             if isinstance(cbody[0], ast.expr):  # Is a docstring
-                class_skeleton.append((cbody[0].lineno, cbody[0].end_lineno))
+                class_skeleton.add((cbody[0].lineno, cbody[0].end_lineno))
                 cbody = cbody[1:]
-                cnode: Union[ast.FunctionDef, ast.AsyncFunctionDef]
+                cnode: ast.stmt
             for cnode in cbody:
                 # Collect all dunder methods.
                 cnode_name: str
                 if (
                     isinstance(cnode, (ast.FunctionDef, ast.AsyncFunctionDef))
                     and len(cnode_name := cnode.name) > 4
+                    and cnode_name != name_parts[1]
                     and cnode_name.isascii()
                     and cnode_name.startswith("__")
                     and cnode_name.endswith("__")
                 ):
-                    class_skeleton.append((cnode.lineno, cnode.end_lineno))
+                    contextual_dunder_methods.add((target.name, cnode_name))
+                    class_skeleton.add((cnode.lineno, cnode.end_lineno))
 
             return find_target(target.body, name_parts[1:])
 
         return None
 
-    with open(file_path, "r", encoding="utf8") as file:
+    with open(file_path, encoding="utf8") as file:
         source_code = file.read()
     try:
         module_node = ast.parse(source_code)
     except SyntaxError as e:
-        logging.error(f"get_code - Syntax error in code: {e}")
-        return None
-    if len(function_to_optimize.parents) == 1:
-        if function_to_optimize.parents[0].type == "ClassDef":
-            qualified_name_parts: Union[tuple[str, str], tuple[str]] = (
-                function_to_optimize.parents[0].name,
-                function_to_optimize.function_name,
-            )
+        logging.exception(f"get_code - Syntax error in code: {e}")
+        return None, set()
+    # Get the source code lines for the target node
+    lines = source_code.splitlines(keepends=True)
+    if len(functions_to_optimize[0].parents) == 1:
+        if (
+            functions_to_optimize[0].parents[0].type == "ClassDef"
+        ):  # All functions_to_optimize functions are methods of the same class.
+            qualified_name_parts_list: list[tuple[str, str] | tuple[str]] = [
+                (fto.parents[0].name, fto.function_name) for fto in functions_to_optimize
+            ]
+
         else:
             logging.error(
-                f"Error: get_code does not support nesting function in functions: {function_to_optimize.parents}"
+                f"Error: get_code does not support nesting function in functions: {functions_to_optimize[0].parents}",
             )
-            return None
-    elif len(function_to_optimize.parents) == 0:
-        qualified_name_parts = (function_to_optimize.function_name,)
+            return None, set()
+    elif len(functions_to_optimize[0].parents) == 0:
+        qualified_name_parts_list = [(functions_to_optimize[0].function_name,)]
     else:
         logging.error(
             "Error: get_code does not support more than one level of nesting for now. "
-            f"Parents: {function_to_optimize.parents}"
+            f"Parents: {functions_to_optimize[0].parents}",
         )
-        return None
-    target_node = find_target(module_node.body, qualified_name_parts)
-    if target_node is None:
-        return None
+        return None, set()
+    for qualified_name_parts in qualified_name_parts_list:
+        target_node: ast.AST | None = find_target(module_node.body, qualified_name_parts)
+        if target_node is None:
+            continue
 
-    # Get the source code lines for the target node
-    lines = source_code.splitlines(keepends=True)
+        if (
+            isinstance(target_node, (ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef))
+            and target_node.decorator_list
+        ):
+            target_code += "".join(
+                lines[target_node.decorator_list[0].lineno - 1 : target_node.end_lineno],
+            )
+        else:
+            target_code += "".join(lines[target_node.lineno - 1 : target_node.end_lineno])
+    class_list: list[tuple[int, int | None]] = sorted(class_skeleton)
     class_code = "".join(
-        ["".join(lines[s_lineno - 1 : e_lineno]) for (s_lineno, e_lineno) in class_skeleton]
+        ["".join(lines[s_lineno - 1 : e_lineno]) for (s_lineno, e_lineno) in class_list],
     )
-    if (
-        isinstance(target_node, (ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef))
-        and target_node.decorator_list
-    ):
-        target_code = "".join(
-            lines[target_node.decorator_list[0].lineno - 1 : target_node.end_lineno]
-        )
-    else:
-        target_code = "".join(lines[target_node.lineno - 1 : target_node.end_lineno])
+    return class_code + target_code, contextual_dunder_methods
 
-    return class_code + target_code
 
-
-def get_code_no_skeleton(file_path: str, target_name: str) -> Optional[str]:
-    """Returns the code for a function in a file. Irrespective of class skeleton."""
-
-    with open(file_path, "r", encoding="utf8") as file:
+def get_code_no_skeleton(file_path: str, target_name: str) -> str | None:
+    """Return the code for a function in a file, irrespective of class skeleton."""
+    with open(file_path, encoding="utf8") as file:
         source_code = file.read()
 
     try:
         module_node = ast.parse(source_code)
     except SyntaxError as e:
-        logging.error(f"get_code_no_skeleton - Syntax error in code: {e}")
+        logging.exception(f"get_code_no_skeleton - Syntax error in code: {e}")
         return None
 
     name_parts = target_name.split(".")
     target_node = None
     stack: deque[ast.AST] = deque([module_node])
 
     while stack:
@@ -147,13 +161,29 @@
     if target_node is None:
         return None
 
     # Get the source code lines for the target node
     lines = source_code.splitlines(keepends=True)
     if hasattr(target_node, "decorator_list") and target_node.decorator_list:
         target_code = "".join(
-            lines[target_node.decorator_list[0].lineno - 1 : target_node.end_lineno]
+            lines[target_node.decorator_list[0].lineno - 1 : target_node.end_lineno],
         )
     else:
         target_code = "".join(lines[target_node.lineno - 1 : target_node.end_lineno])
 
     return target_code
+
+
+def extract_code(
+    functions_to_optimize: list[FunctionToOptimize],
+) -> tuple[str | None, set[tuple[str, str]]]:
+    edited_code, contextual_dunder_methods = get_code(functions_to_optimize)
+    if edited_code is None:
+        return None, set()
+    try:
+        compile(edited_code, "edited_code", "exec")
+    except SyntaxError as e:
+        logging.exception(
+            f"extract_code - Syntax error in extracted optimization candidate code: {e}",
+        )
+        return None, set()
+    return edited_code, contextual_dunder_methods
```

### Comparing `codeflash-0.4.1/codeflash/code_utils/code_replacer.py` & `codeflash-0.5.0/codeflash/code_utils/code_replacer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,40 @@
-from typing import List, Union, Optional, IO
+from __future__ import annotations
+
+from typing import IO
 
 import libcst as cst
-from libcst import SimpleStatementLine, FunctionDef
+from libcst import FunctionDef
 
 
 class OptimFunctionCollector(cst.CSTVisitor):
     METADATA_DEPENDENCIES = (cst.metadata.ParentNodeProvider,)
 
-    def __init__(self, function_name: str, preexisting_functions: Optional[List[str]] = None):
+    def __init__(
+        self,
+        function_name: str,
+        class_name: str | None,
+        contextual_functions: set[tuple[str, str]],
+        preexisting_functions: list[str] | None = None,
+    ) -> None:
         super().__init__()
         if preexisting_functions is None:
             preexisting_functions = []
         self.function_name = function_name
-        self.optim_body: Union[FunctionDef, None] = None
+        self.class_name = class_name
+        self.optim_body: FunctionDef | None = None
         self.optim_new_class_functions: list[cst.FunctionDef] = []
         self.optim_new_functions: list[cst.FunctionDef] = []
-        self.optim_imports: List[Union[cst.Import, cst.ImportFrom]] = []
+        self.optim_imports: list[cst.SimpleStatementLine] = []
         self.preexisting_functions = preexisting_functions
+        self.contextual_functions = contextual_functions.union(
+            {(self.class_name, self.function_name)},
+        )
 
-    def visit_FunctionDef(self, node: cst.FunctionDef):
+    def visit_FunctionDef(self, node: cst.FunctionDef) -> None:
         parent = self.get_metadata(cst.metadata.ParentNodeProvider, node)
         parent2 = None
         try:
             if parent is not None and isinstance(parent, cst.Module):
                 parent2 = self.get_metadata(cst.metadata.ParentNodeProvider, parent)
         except:
             pass
@@ -35,53 +47,57 @@
                 isinstance(parent, cst.Module)
                 or (parent2 is not None and not isinstance(parent2, cst.ClassDef))
             )
         ):
             self.optim_new_functions.append(node)
 
     def visit_ClassDef_body(self, node: cst.ClassDef) -> None:
-        for class_node in node.body.body:
-            if isinstance(class_node, cst.FunctionDef) and class_node.name.value not in [
-                "__init__",
-                self.function_name,
-            ]:
-                self.optim_new_class_functions.append(class_node)
+        for child_node in node.body.body:
+            if (
+                isinstance(child_node, cst.FunctionDef)
+                and (
+                    node.name.value,
+                    child_node.name.value,
+                )
+                not in self.contextual_functions
+            ):
+                self.optim_new_class_functions.append(child_node)
 
-    def leave_SimpleStatementLine(self, original_node: "SimpleStatementLine") -> None:
-        if isinstance(original_node.body[0], cst.Import):
-            self.optim_imports.append(original_node)
-        elif isinstance(original_node.body[0], cst.ImportFrom):
+    def leave_SimpleStatementLine(self, original_node: cst.SimpleStatementLine) -> None:
+        if isinstance(original_node.body[0], (cst.Import, cst.ImportFrom)):
             self.optim_imports.append(original_node)
 
 
 class OptimFunctionReplacer(cst.CSTTransformer):
     def __init__(
         self,
         function_name: str,
         optim_body: cst.FunctionDef,
-        optim_new_class_functions: List[cst.FunctionDef],
-        optim_imports: List[Union[cst.Import, cst.ImportFrom]],
-        optim_new_functions,
-        class_name=None,
-    ):
+        optim_new_class_functions: list[cst.FunctionDef],
+        optim_imports: list[cst.SimpleStatementLine],
+        optim_new_functions: list[cst.FunctionDef],
+        class_name: str | None = None,
+    ) -> None:
         super().__init__()
         self.function_name = function_name
         self.optim_body = optim_body
         self.optim_new_class_functions = optim_new_class_functions
         self.optim_new_imports = optim_imports
         self.optim_new_functions = optim_new_functions
         self.class_name = class_name
         self.depth: int = 0
         self.in_class: bool = False
 
     def visit_FunctionDef(self, node: cst.FunctionDef) -> bool:
         return False
 
     def leave_FunctionDef(
-        self, original_node: cst.FunctionDef, updated_node: cst.FunctionDef
+        self,
+        original_node: cst.FunctionDef,
+        updated_node: cst.FunctionDef,
     ) -> cst.FunctionDef:
         if original_node.name.value == self.function_name and (
             self.depth == 0 or (self.depth == 1 and self.in_class)
         ):
             return self.optim_body
         return updated_node
 
@@ -89,23 +105,25 @@
         self.depth += 1
         if self.in_class:
             return False
         self.in_class = (self.depth == 1) and (node.name.value == self.class_name)
         return self.in_class
 
     def leave_ClassDef(
-        self, original_node: cst.ClassDef, updated_node: cst.ClassDef
+        self,
+        original_node: cst.ClassDef,
+        updated_node: cst.ClassDef,
     ) -> cst.ClassDef:
         self.depth -= 1
         if self.in_class and (self.depth == 0) and (original_node.name.value == self.class_name):
             self.in_class = False
             return updated_node.with_changes(
                 body=updated_node.body.with_changes(
                     body=(list(updated_node.body.body) + self.optim_new_class_functions),
-                )
+                ),
             )
         return updated_node
 
     def leave_Module(self, original_node: cst.Module, updated_node: cst.Module) -> cst.Module:
         if len(self.optim_new_imports) == 0:
             node = updated_node
         else:
@@ -119,23 +137,23 @@
                 class_index = index
         if max_function_index is not None:
             node = node.with_changes(
                 body=(
                     *node.body[: max_function_index + 1],
                     *self.optim_new_functions,
                     *node.body[max_function_index + 1 :],
-                )
+                ),
             )
         elif class_index is not None:
             node = node.with_changes(
                 body=(
                     *node.body[: class_index + 1],
                     *self.optim_new_functions,
                     *node.body[class_index + 1 :],
-                )
+                ),
             )
         else:
             node = node.with_changes(body=(*self.optim_new_functions, *node.body))
         return node
 
     # TODO: Implement the logic to not duplicate imports. This is supported by libcst, figure out how to use it.
     # def leave_Module(self, original_node: "Module", updated_node: "Module") -> "Module":
@@ -161,36 +179,42 @@
 
 
 def replace_functions_in_file(
     source_code: str,
     original_function_names: list[str],
     optimized_code: str,
     preexisting_functions: list[str],
+    contextual_functions: set[tuple[str, str]],
 ) -> str:
     parsed_function_names = []
     for original_function_name in original_function_names:
         if original_function_name.count(".") == 0:
             class_name, function_name = None, original_function_name
         elif original_function_name.count(".") == 1:
             class_name, function_name = original_function_name.split(".")
         else:
             raise ValueError(f"Don't know how to find {original_function_name} yet!")
         parsed_function_names.append((function_name, class_name))
 
     module = cst.metadata.MetadataWrapper(cst.parse_module(optimized_code))
 
     for i, (function_name, class_name) in enumerate(parsed_function_names):
-        visitor = OptimFunctionCollector(function_name, preexisting_functions)
-        visited = module.visit(visitor)
+        visitor = OptimFunctionCollector(
+            function_name,
+            class_name,
+            contextual_functions,
+            preexisting_functions,
+        )
+        module.visit(visitor)
 
         if visitor.optim_body is None and not preexisting_functions:
             continue
-        elif visitor.optim_body is None:
+        if visitor.optim_body is None:
             raise ValueError(f"Did not find the function {function_name} in the optimized code")
-        optim_imports = [] if i > 0 else visitor.optim_imports
+        optim_imports: list[cst.SimpleStatementLine] = [] if i > 0 else visitor.optim_imports
 
         transformer = OptimFunctionReplacer(
             visitor.function_name,
             visitor.optim_body,
             visitor.optim_new_class_functions,
             optim_imports,
             visitor.optim_new_functions,
@@ -204,19 +228,21 @@
 
 
 def replace_function_definitions_in_module(
     function_names: list[str],
     optimized_code: str,
     module_abspath: str,
     preexisting_functions: list[str],
+    contextual_functions: set[tuple[str, str]],
 ) -> None:
     file: IO[str]
-    with open(module_abspath, "r", encoding="utf8") as file:
+    with open(module_abspath, encoding="utf8") as file:
         source_code: str = file.read()
     new_code: str = replace_functions_in_file(
         source_code,
         function_names,
         optimized_code,
         preexisting_functions,
+        contextual_functions,
     )
     with open(module_abspath, "w", encoding="utf8") as file:
         file.write(new_code)
```

### Comparing `codeflash-0.4.1/codeflash/code_utils/code_utils.py` & `codeflash-0.5.0/codeflash/code_utils/code_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/code_utils/config_parser.py` & `codeflash-0.5.0/codeflash/code_utils/config_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     # TODO: minimum-peformance-gain should become a more dynamic auto-detection in the future
     float_keys = {
         "minimum-performance-gain": MIN_IMPROVEMENT_THRESHOLD,
     }  # the value is the default value
     str_keys = {
         "pytest-cmd": "pytest",
         "formatter-cmd": "black",
+        "imports-sort-cmd": "isort",
     }
     bool_keys = {
         "disable-telemetry": False,
     }
 
     for key in float_keys:
         if key in config:
@@ -82,20 +83,23 @@
     for key in bool_keys:
         if key in config:
             config[key] = bool(config[key])
         else:
             config[key] = bool_keys[key]
     for key in path_keys:
         if key in config:
-            config[key] = os.path.join(os.path.dirname(config_file_path), config[key])
+            config[key] = os.path.realpath(
+                os.path.join(os.path.dirname(config_file_path), config[key])
+            )
 
     for key in path_list_keys:
         if key in config:
             config[key] = [
-                os.path.join(os.path.dirname(config_file_path), path) for path in config[key]
+                os.path.realpath(os.path.join(os.path.dirname(config_file_path), path))
+                for path in config[key]
             ]
         else:  # Default to empty list
             config[key] = []
 
     assert config["test-framework"] in [
         "pytest",
         "unittest",
```

### Comparing `codeflash-0.4.1/codeflash/code_utils/env_utils.py` & `codeflash-0.5.0/codeflash/code_utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/code_utils/git_utils.py` & `codeflash-0.5.0/codeflash/code_utils/git_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,19 +67,16 @@
 
 def get_remote_url(repo: Optional[Repo] = None) -> str:
     repository: Repo = repo if repo else git.Repo(search_parent_directories=True)
     return repository.remote().url
 
 
 def get_repo_owner_and_name(repo: Optional[Repo] = None) -> tuple[str, str]:
-    remote_url = (
-        get_remote_url(repo).rstrip(".git")
-        if get_remote_url(repo).endswith(".git")
-        else get_remote_url(repo)
-    )
+    remote_url = get_remote_url(repo)  # call only once
+    remote_url = remote_url.rstrip(".git") if remote_url.endswith(".git") else remote_url
     split_url = remote_url.split("/")
     repo_owner_with_github, repo_name = split_url[-2], split_url[-1]
     repo_owner = (
         repo_owner_with_github.split(":")[1]
         if ":" in repo_owner_with_github
         else repo_owner_with_github
     )
```

### Comparing `codeflash-0.4.1/codeflash/code_utils/instrument_existing_tests.py` & `codeflash-0.5.0/codeflash/code_utils/instrument_existing_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/code_utils/shell_utils.py` & `codeflash-0.5.0/codeflash/code_utils/shell_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/code_utils/sqlalchemy_utils.py` & `codeflash-0.5.0/codeflash/code_utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/code_utils/time_utils.py` & `codeflash-0.5.0/codeflash/code_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/discovery/discover_unit_tests.py` & `codeflash-0.5.0/codeflash/discovery/discover_unit_tests.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/discovery/functions_to_optimize.py` & `codeflash-0.5.0/codeflash/discovery/functions_to_optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,16 @@
         return True
     except git.InvalidGitRepositoryError:
         return False
 
 
 def ignored_submodule_paths(git_repo: git.Repo) -> List[str]:
     return [
-        os.path.realpath(submodule.module().working_tree_dir) for submodule in git_repo.submodules
+        os.path.realpath(os.path.join(git_repo.working_tree_dir, submodule.path))
+        for submodule in git_repo.submodules
     ]
 
 
 def filter_functions(
     modified_functions: Dict[str, List[FunctionToOptimize]],
     tests_root: str,
     ignore_paths: List[str],
```

### Comparing `codeflash-0.4.1/codeflash/github/PrComment.py` & `codeflash-0.5.0/codeflash/github/PrComment.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/main.py` & `codeflash-0.5.0/codeflash/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 """Thanks for being curious about how codeflash works! If you might want to work with us on finally making performance a
 solved problem, please reach out to us at careers@codeflash.ai. We're hiring!
 """
 
+from __future__ import annotations
+
 import concurrent.futures
 import logging
 import os
 import pathlib
 import uuid
-from argparse import ArgumentParser, SUPPRESS, Namespace
+from argparse import SUPPRESS, ArgumentParser, Namespace
 from collections import defaultdict
-from typing import IO, Tuple, Union
+from typing import IO, Dict, Tuple, Union
 
 import libcst as cst
 
-from codeflash.api.aiservice import log_results
-from codeflash.api.aiservice import optimize_python_code
+from codeflash.api.aiservice import log_results, optimize_python_code
 from codeflash.cli_cmds.cli import process_cmd_args
 from codeflash.cli_cmds.cmd_init import CODEFLASH_LOGO
 from codeflash.code_utils import env_utils
-from codeflash.code_utils.code_extractor import get_code
+from codeflash.code_utils.code_extractor import extract_code
 from codeflash.code_utils.code_replacer import replace_function_definitions_in_module
 from codeflash.code_utils.code_utils import (
-    module_name_from_file_path,
     get_all_function_names,
     get_run_tmp_file,
+    module_name_from_file_path,
 )
 from codeflash.code_utils.config_consts import (
-    MAX_TEST_RUN_ITERATIONS,
-    MAX_FUNCTION_TEST_SECONDS,
     INDIVIDUAL_TEST_TIMEOUT,
-    N_CANDIDATES,
-    MAX_TEST_FUNCTION_RUNS,
     MAX_CUMULATIVE_TEST_RUNTIME_NANOSECONDS,
+    MAX_FUNCTION_TEST_SECONDS,
+    MAX_TEST_FUNCTION_RUNS,
+    MAX_TEST_RUN_ITERATIONS,
+    N_CANDIDATES,
 )
-from codeflash.code_utils.formatter import format_code
+from codeflash.code_utils.formatter import format_code, sort_imports
 from codeflash.code_utils.instrument_existing_tests import (
     inject_profiling_into_existing_test,
 )
 from codeflash.code_utils.time_utils import humanize_runtime
-from codeflash.discovery.discover_unit_tests import discover_unit_tests, TestsInFile
+from codeflash.discovery.discover_unit_tests import TestsInFile, discover_unit_tests
 from codeflash.discovery.functions_to_optimize import (
-    get_functions_to_optimize_by_file,
+    FunctionParent,
     FunctionToOptimize,
+    get_functions_to_optimize_by_file,
 )
 from codeflash.optimization.function_context import (
-    get_constrained_function_context_and_dependent_functions,
     Source,
+    get_constrained_function_context_and_dependent_functions,
 )
 from codeflash.result.create_pr import check_create_pr
 from codeflash.result.explanation import Explanation
 from codeflash.telemetry import posthog
 from codeflash.telemetry.posthog import ph
 from codeflash.telemetry.sentry import init_sentry
 from codeflash.verification.equivalence import compare_results
-from codeflash.verification.parse_test_output import (
+from codeflash.verification.parse_test_output import parse_test_results
+from codeflash.verification.test_results import (
+    TestResults,
     TestType,
-    parse_test_results,
 )
-from codeflash.verification.test_results import TestResults
 from codeflash.verification.test_runner import run_tests
 from codeflash.verification.verification_utils import (
-    get_test_file_path,
     TestConfig,
+    get_test_file_path,
 )
 from codeflash.verification.verifier import generate_tests
 
 
 def parse_args() -> Namespace:
     parser = ArgumentParser()
     parser.add_argument("command", nargs="?", help="The command to run (e.g., 'init')")
@@ -163,332 +165,383 @@
             if num_optimizable_functions == 0:
                 logging.info("No functions found to optimize. Exiting...")
                 return
             logging.info(f"Discovering existing unit tests in {self.test_cfg.tests_root} ...")
             function_to_tests: dict[str, list[TestsInFile]] = discover_unit_tests(self.test_cfg)
             num_discovered_tests: int = sum([len(value) for value in function_to_tests.values()])
             logging.info(
-                f"Discovered {num_discovered_tests} existing unit tests in {self.test_cfg.tests_root}"
+                f"Discovered {num_discovered_tests} existing unit tests in {self.test_cfg.tests_root}",
             )
             ph("cli-optimize-discovered-tests", {"num_tests": num_discovered_tests})
             path: str
             for path in file_to_funcs_to_optimize:
                 logging.info(f"Examining file {path} ...")
                 # TODO: Sequence the functions one goes through intelligently. If we are optimizing f(g(x)),
                 #  then we might want to first optimize f rather than g because optimizing f would already
                 #  optimize g as it is a dependency
                 f: IO[str]
-                with open(path, "r", encoding="utf8") as f:
+                with open(path, encoding="utf8") as f:
                     original_code: str = f.read()
+                should_sort_imports = True
+                if (
+                    sort_imports(self.args.imports_sort_cmd, should_sort_imports, path)
+                    != original_code
+                ):
+                    should_sort_imports = False
+
                 function_to_optimize: FunctionToOptimize
                 for function_to_optimize in file_to_funcs_to_optimize[path]:
                     function_trace_id: str = str(uuid.uuid4())
                     ph("cli-optimize-function-start", {"function_trace_id": function_trace_id})
                     function_name: str = (
                         function_to_optimize.function_name
                         if function_to_optimize.parents == []
                         else ".".join(
                             [
                                 function_to_optimize.parents[0].name,
                                 function_to_optimize.function_name,
-                            ]
+                            ],
                         )
                     )
                     function_iterator_count += 1
                     logging.info(
-                        f"Optimizing function {function_iterator_count} of {num_optimizable_functions} - {function_name}"
+                        f"Optimizing function {function_iterator_count} of {num_optimizable_functions} - {function_name}",
                     )
                     winning_test_results = None
                     # remove leftovers from previous run
                     pathlib.Path(get_run_tmp_file("test_return_values_0.bin")).unlink(
-                        missing_ok=True
+                        missing_ok=True,
                     )
                     pathlib.Path(get_run_tmp_file("test_return_values_0.sqlite")).unlink(
-                        missing_ok=True
+                        missing_ok=True,
+                    )
+                    code_to_optimize, contextual_dunder_methods = extract_code(
+                        [function_to_optimize],
                     )
-                    code_to_optimize = get_code(function_to_optimize)
                     if code_to_optimize is None:
                         logging.error("Could not find function to optimize.")
                         continue
 
                     success, preexisting_functions = get_all_function_names(code_to_optimize)
                     if not success:
                         logging.error("Error in parsing the code, skipping optimization.")
                         continue
 
-                    (
-                        code_to_optimize_with_dependents,
-                        dependent_functions,
-                    ) = get_constrained_function_context_and_dependent_functions(
-                        function_to_optimize, self.args.project_root, code_to_optimize
-                    )
-                    preexisting_functions.extend(
-                        [fn[0].full_name.split(".")[-1] for fn in dependent_functions]
-                    )
-                    dependent_functions_by_module_abspath = defaultdict(set)
-                    for _, module_abspath, qualified_name in dependent_functions:
-                        dependent_functions_by_module_abspath[module_abspath].add(qualified_name)
-                    original_dependent_code = {}
-                    for module_abspath in dependent_functions_by_module_abspath.keys():
-                        with open(module_abspath, "r", encoding="utf8") as f:
-                            dependent_code = f.read()
-                            original_dependent_code[module_abspath] = dependent_code
-                    logging.info(f"Code to be optimized:\n{code_to_optimize_with_dependents}")
-                    module_path = module_name_from_file_path(path, self.args.project_root)
-
-                    instrumented_unittests_created_for_function = self.prepare_existing_tests(
-                        function_name=function_name,
-                        module_path=module_path,
-                        function_to_tests=function_to_tests,
-                    )
-                    instrumented_unittests_created.update(
-                        instrumented_unittests_created_for_function
-                    )
-
-                    (
-                        success,
-                        generated_original_test_source,
-                        instrumented_test_source,
-                        optimizations,
-                    ) = self.generate_tests_and_optimizations(
-                        code_to_optimize_with_dependents,
-                        function_to_optimize,
-                        dependent_functions,
-                        module_path,
-                        function_trace_id,
-                    )
-                    if not success:
-                        continue
-
-                    generated_tests_path = get_test_file_path(
-                        self.args.tests_root, function_to_optimize.function_name, 0
-                    )
-                    with open(generated_tests_path, "w", encoding="utf8") as file:
-                        file.write(instrumented_test_source)
-
-                    test_files_created.add(generated_tests_path)
-                    (
-                        success,
-                        original_gen_results,
-                        overall_original_test_results,
-                        original_runtime,
-                    ) = self.establish_original_code_baseline(
-                        function_name,
-                        instrumented_unittests_created_for_function,
-                        generated_tests_path,
-                    )
-                    if not success:
-                        continue
-                    best_runtime = original_runtime  # The fastest code runtime until now
-                    logging.info("Optimizing code ...")
-                    # TODO: Postprocess the optimized function to include the original docstring and such
-
-                    best_optimization = []
-                    speedup_ratios = dict()
-                    optimized_runtimes = dict()
-                    is_correct = dict()
-
-                    for i, optimization in enumerate(optimizations.optimizations):
-                        j = i + 1
-                        if optimization.source_code is None:
-                            continue
-                        # remove left overs from previous run
-                        pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.bin")).unlink(
-                            missing_ok=True
-                        )
-                        pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.sqlite")).unlink(
-                            missing_ok=True
+                    dependent_code, dependent_functions = (
+                        get_constrained_function_context_and_dependent_functions(
+                            function_to_optimize,
+                            self.args.project_root,
+                            code_to_optimize,
                         )
-                        logging.info("Optimized candidate:")
-                        logging.info(optimization.source_code)
-                        try:
-                            replace_function_definitions_in_module(
-                                [function_name],
-                                optimization.source_code,
-                                path,
-                                preexisting_functions,
+                    )
+                    if function_to_optimize.parents:
+                        function_class = function_to_optimize.parents[0].name
+                        dependent_methods = [
+                            df
+                            for df in dependent_functions
+                            if df[2].count(".") > 0 and df[2].split(".")[0] == function_class
+                        ]
+                        optimizable_methods = [function_to_optimize] + [
+                            FunctionToOptimize(
+                                df[2].split(".")[0],
+                                "",
+                                [FunctionParent(df[2].split(".")[0], "ClassDef")],
+                                None,
+                                None,
                             )
-                            for (
-                                module_abspath,
-                                qualified_names,
-                            ) in dependent_functions_by_module_abspath.items():
-                                replace_function_definitions_in_module(
-                                    list(qualified_names),
-                                    optimization.source_code,
-                                    module_abspath,
-                                    [],
-                                )
-                        except (
-                            ValueError,
-                            SyntaxError,
-                            cst.ParserSyntaxError,
-                            AttributeError,
-                        ) as e:
-                            logging.error(e)
-                            with open(path, "w", encoding="utf8") as f:
-                                f.write(original_code)
-                            for module_abspath in dependent_functions_by_module_abspath.keys():
-                                with open(module_abspath, "w", encoding="utf8") as f:
-                                    f.write(original_dependent_code[module_abspath])
-                            continue
-
-                        (
-                            success,
-                            times_run,
-                            best_test_runtime,
-                            best_test_results,
-                        ) = self.run_optimized_candidate(
-                            optimization_index=j,
-                            instrumented_unittests_created_for_function=instrumented_unittests_created_for_function,
-                            overall_original_test_results=overall_original_test_results,
-                            original_gen_results=original_gen_results,
-                            generated_tests_path=generated_tests_path,
-                            best_runtime_until_now=best_runtime,
-                        )
-                        optimized_runtimes[optimization.optimization_id] = best_test_runtime
-                        speedup_ratios[optimization.optimization_id] = None
-                        is_correct[optimization.optimization_id] = success
-
-                        if success:
-                            speedup_ratios[optimization.optimization_id] = (
-                                original_runtime - best_test_runtime
-                            ) / best_test_runtime
-
-                            logging.info(
-                                f"Candidate runtime measured over {times_run} run{'s' if times_run > 1 else ''}: "
-                                f"{humanize_runtime(best_test_runtime)}, speedup ratio = "
-                                f"{((original_runtime - best_test_runtime) / best_test_runtime):.3f}"
+                            for df in dependent_methods
+                        ]
+                        if len(optimizable_methods) > 1:
+                            code_to_optimize, contextual_dunder_methods = extract_code(
+                                optimizable_methods,
                             )
-                            if (
-                                ((original_runtime - best_test_runtime) / best_test_runtime)
-                                > self.args.minimum_performance_gain
-                            ) and best_test_runtime < best_runtime:
-                                logging.info(
-                                    "This candidate is better than the previous best candidate."
-                                )
-
-                                logging.info(
-                                    f"Original runtime: {humanize_runtime(original_runtime)} Best test runtime: "
-                                    f"{humanize_runtime(best_test_runtime)}, ratio = "
-                                    f"{((original_runtime - best_test_runtime) / best_test_runtime)}"
-                                )
-                                best_optimization = [
-                                    optimization.source_code,
-                                    optimization.explanation,
-                                    dependent_functions,
-                                ]
-                                best_runtime = best_test_runtime
-                                winning_test_results = best_test_results
-                        with open(path, "w", encoding="utf8") as f:
-                            f.write(original_code)
-                        for module_abspath in dependent_functions_by_module_abspath.keys():
-                            with open(module_abspath, "w", encoding="utf8") as f:
-                                f.write(original_dependent_code[module_abspath])
-                        logging.info("----------------")
-                    logging.info(f"Best optimization: {best_optimization[0:2]}")
+                            if code_to_optimize is None:
+                                logging.error("Could not find function to optimize.")
+                                continue
+                    code_to_optimize_with_dependents = dependent_code + "\n" + code_to_optimize
+                preexisting_functions.extend(
+                    [fn[0].full_name.split(".")[-1] for fn in dependent_functions],
+                )
+                dependent_functions_by_module_abspath = defaultdict(set)
+                for _, module_abspath, qualified_name in dependent_functions:
+                    dependent_functions_by_module_abspath[module_abspath].add(qualified_name)
+                original_dependent_code = {}
+                for module_abspath in dependent_functions_by_module_abspath.keys():
+                    with open(module_abspath, encoding="utf8") as f:
+                        dependent_code = f.read()
+                        original_dependent_code[module_abspath] = dependent_code
+                logging.info(f"Code to be optimized:\n{code_to_optimize_with_dependents}")
+                module_path = module_name_from_file_path(path, self.args.project_root)
+
+                instrumented_unittests_created_for_function = self.prepare_existing_tests(
+                    function_name=function_name,
+                    module_path=module_path,
+                    function_to_tests=function_to_tests,
+                )
+                instrumented_unittests_created.update(
+                    instrumented_unittests_created_for_function,
+                )
 
-                    log_results(
-                        function_trace_id=function_trace_id,
-                        speedup_ratio=speedup_ratios,
-                        original_runtime=original_runtime,
-                        optimized_runtime=optimized_runtimes,
-                        is_correct=is_correct,
-                    )
-                    ph("cli-optimize-function-finished", {"function_trace_id": function_trace_id})
-
-                    if best_optimization:
-                        optimizations_found += 1
-                        logging.info(f"Best candidate:\n{best_optimization[0]}")
+                (
+                    success,
+                    generated_original_test_source,
+                    instrumented_test_source,
+                    optimizations,
+                ) = self.generate_tests_and_optimizations(
+                    code_to_optimize_with_dependents,
+                    function_to_optimize,
+                    dependent_functions,
+                    module_path,
+                    function_trace_id,
+                )
+                if not success:
+                    continue
 
-                        optimized_code = best_optimization[0]
+                generated_tests_path = get_test_file_path(
+                    self.args.tests_root,
+                    function_to_optimize.function_name,
+                    0,
+                )
+                with open(generated_tests_path, "w", encoding="utf8") as file:
+                    file.write(instrumented_test_source)
+
+                test_files_created.add(generated_tests_path)
+                (
+                    success,
+                    original_gen_results,
+                    overall_original_test_results,
+                    original_runtime,
+                ) = self.establish_original_code_baseline(
+                    function_name,
+                    instrumented_unittests_created_for_function,
+                    generated_tests_path,
+                )
+                if not success:
+                    continue
+                best_runtime = original_runtime  # The fastest code runtime until now
+                logging.info("Optimizing code ...")
+                # TODO: Postprocess the optimized function to include the original docstring and such
+
+                best_optimization = []
+                speedup_ratios: Dict[str, float | None] = dict()
+                optimized_runtimes = dict()
+                is_correct = dict()
+
+                for i, optimization in enumerate(optimizations.optimizations):
+                    j = i + 1
+                    if optimization.source_code is None:
+                        continue
+                    # remove left overs from previous run
+                    pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.bin")).unlink(
+                        missing_ok=True,
+                    )
+                    pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.sqlite")).unlink(
+                        missing_ok=True,
+                    )
+                    logging.info("Optimized candidate:")
+                    logging.info(optimization.source_code)
+                    try:
                         replace_function_definitions_in_module(
                             [function_name],
-                            optimized_code,
+                            optimization.source_code,
                             path,
                             preexisting_functions,
+                            contextual_dunder_methods,
                         )
                         for (
                             module_abspath,
                             qualified_names,
                         ) in dependent_functions_by_module_abspath.items():
                             replace_function_definitions_in_module(
                                 list(qualified_names),
-                                optimized_code,
+                                optimization.source_code,
                                 module_abspath,
                                 [],
+                                contextual_dunder_methods,
                             )
-                        explanation_final = Explanation(
-                            raw_explanation_message=best_optimization[1],
-                            winning_test_results=winning_test_results,
-                            original_runtime_ns=original_runtime,
-                            best_runtime_ns=best_runtime,
-                            function_name=function_name,
-                            path=path,
-                        )
-                        logging.info(f"Explanation: \n{explanation_final.to_console_string()}")
+                    except (
+                        ValueError,
+                        SyntaxError,
+                        cst.ParserSyntaxError,
+                        AttributeError,
+                    ) as e:
+                        logging.exception(e)
+                        with open(path, "w", encoding="utf8") as f:
+                            f.write(original_code)
+                        for module_abspath in dependent_functions_by_module_abspath.keys():
+                            with open(module_abspath, "w", encoding="utf8") as f:
+                                f.write(original_dependent_code[module_abspath])
+                        continue
+
+                    (
+                        success,
+                        times_run,
+                        best_test_runtime,
+                        best_test_results,
+                    ) = self.run_optimized_candidate(
+                        optimization_index=j,
+                        instrumented_unittests_created_for_function=instrumented_unittests_created_for_function,
+                        overall_original_test_results=overall_original_test_results,
+                        original_gen_results=original_gen_results,
+                        generated_tests_path=generated_tests_path,
+                        best_runtime_until_now=best_runtime,
+                    )
+                    optimized_runtimes[optimization.optimization_id] = best_test_runtime
+                    speedup_ratios[optimization.optimization_id] = None
+                    is_correct[optimization.optimization_id] = success
+
+                    if success:
+                        speedup_ratios[optimization.optimization_id] = (
+                            original_runtime - best_test_runtime
+                        ) / best_test_runtime
 
-                        new_code = format_code(self.args.formatter_cmd, path)
-                        new_dependent_code: dict[str, str] = {
-                            module_abspath: format_code(self.args.formatter_cmd, module_abspath)
-                            for module_abspath in dependent_functions_by_module_abspath.keys()
-                        }
                         logging.info(
-                            f"Optimization was validated for correctness by running the following tests - "
-                            f"\n{generated_original_test_source}"
+                            f"Candidate runtime measured over {times_run} run{'s' if times_run > 1 else ''}: "
+                            f"{humanize_runtime(best_test_runtime)}, speedup ratio = "
+                            f"{((original_runtime - best_test_runtime) / best_test_runtime):.3f}",
                         )
+                        if (
+                            ((original_runtime - best_test_runtime) / best_test_runtime)
+                            > self.args.minimum_performance_gain
+                        ) and best_test_runtime < best_runtime:
+                            logging.info(
+                                "This candidate is better than the previous best candidate.",
+                            )
 
-                        logging.info(f"⚡️ Optimization successful! 📄 {function_name} in {path}")
-                        logging.info(f"📈 {explanation_final.perf_improvement_line}")
+                            logging.info(
+                                f"Original runtime: {humanize_runtime(original_runtime)} Best test runtime: "
+                                f"{humanize_runtime(best_test_runtime)}, ratio = "
+                                f"{((original_runtime - best_test_runtime) / best_test_runtime)}",
+                            )
+                            best_optimization = [
+                                optimization.source_code,
+                                optimization.explanation,
+                                dependent_functions,
+                            ]
+                            best_runtime = best_test_runtime
+                            winning_test_results = best_test_results
+                    with open(path, "w", encoding="utf8") as f:
+                        f.write(original_code)
+                    for module_abspath in dependent_functions_by_module_abspath.keys():
+                        with open(module_abspath, "w", encoding="utf8") as f:
+                            f.write(original_dependent_code[module_abspath])
+                    logging.info("----------------")
+                logging.info(f"Best optimization: {best_optimization[0:2]}")
+
+                log_results(
+                    function_trace_id=function_trace_id,
+                    speedup_ratio=speedup_ratios,
+                    original_runtime=original_runtime,
+                    optimized_runtime=optimized_runtimes,
+                    is_correct=is_correct,
+                )
+                ph("cli-optimize-function-finished", {"function_trace_id": function_trace_id})
 
-                        ph(
-                            "cli-optimize-success",
-                            {
-                                "function_trace_id": function_trace_id,
-                                "speedup_x": explanation_final.speedup_x,
-                                "speedup_pct": explanation_final.speedup_pct,
-                                "best_runtime": explanation_final.best_runtime_ns,
-                                "original_runtime": explanation_final.original_runtime_ns,
-                                "winning_test_results": {
-                                    tt.to_name(): v
-                                    for tt, v in explanation_final.winning_test_results.get_test_pass_fail_report_by_type().items()
-                                },
-                            },
+                if best_optimization:
+                    optimizations_found += 1
+                    logging.info(f"Best candidate:\n{best_optimization[0]}")
+
+                    optimized_code = best_optimization[0]
+                    replace_function_definitions_in_module(
+                        [function_name],
+                        optimized_code,
+                        path,
+                        preexisting_functions,
+                        contextual_dunder_methods,
+                    )
+                    for (
+                        module_abspath,
+                        qualified_names,
+                    ) in dependent_functions_by_module_abspath.items():
+                        replace_function_definitions_in_module(
+                            list(qualified_names),
+                            optimized_code,
+                            module_abspath,
+                            [],
+                            contextual_dunder_methods,
                         )
-                        test_files = function_to_tests.get(module_path + "." + function_name)
-                        existing_tests = ""
-                        if test_files:
-                            for test_file in test_files:
-                                with open(test_file.test_file, "r", encoding="utf8") as f:
-                                    new_test = "".join(f.readlines())
-                                    if new_test not in existing_tests:
-                                        existing_tests += new_test
-
-                        check_create_pr(
-                            optimize_all=self.args.all,
-                            path=path,
-                            original_code=original_dependent_code | {path: original_code},
-                            new_code=new_dependent_code | {path: new_code},
-                            explanation=explanation_final,
-                            existing_tests_source=existing_tests,
-                            generated_original_test_source=generated_original_test_source,
+                    explanation_final = Explanation(
+                        raw_explanation_message=best_optimization[1],
+                        winning_test_results=winning_test_results,
+                        original_runtime_ns=original_runtime,
+                        best_runtime_ns=best_runtime,
+                        function_name=function_name,
+                        path=path,
+                    )
+                    logging.info(f"Explanation: \n{explanation_final.to_console_string()}")
+
+                    new_code = format_code(
+                        self.args.formatter_cmd,
+                        self.args.imports_sort_cmd,
+                        should_sort_imports,
+                        path,
+                    )
+                    new_dependent_code: dict[str, str] = {
+                        module_abspath: format_code(
+                            self.args.formatter_cmd,
+                            self.args.imports_sort_cmd,
+                            should_sort_imports,
+                            module_abspath,
                         )
-                        if self.args.all or env_utils.get_pr_number():
-                            # Reverting to original code, because optimizing functions in a sequence can lead to
-                            #  a) Error propagation, where error in one function can cause the next optimization to fail
-                            #  b) Performance estimates become unstable, as the runtime of an optimization might be
-                            #     dependent on the runtime of the previous optimization
-                            with open(path, "w", encoding="utf8") as f:
-                                f.write(original_code)
-                            for module_abspath in dependent_functions_by_module_abspath.keys():
-                                with open(module_abspath, "w", encoding="utf8") as f:
-                                    f.write(original_dependent_code[module_abspath])
-                    # Delete all the generated tests to not cause any clutter.
-                    pathlib.Path(generated_tests_path).unlink(missing_ok=True)
-                    for test_paths in instrumented_unittests_created_for_function:
-                        pathlib.Path(test_paths).unlink(missing_ok=True)
+                        for module_abspath in dependent_functions_by_module_abspath.keys()
+                    }
+                    logging.info(
+                        f"Optimization was validated for correctness by running the following tests - "
+                        f"\n{generated_original_test_source}",
+                    )
+
+                    logging.info(f"⚡️ Optimization successful! 📄 {function_name} in {path}")
+                    logging.info(f"📈 {explanation_final.perf_improvement_line}")
+
+                    ph(
+                        "cli-optimize-success",
+                        {
+                            "function_trace_id": function_trace_id,
+                            "speedup_x": explanation_final.speedup_x,
+                            "speedup_pct": explanation_final.speedup_pct,
+                            "best_runtime": explanation_final.best_runtime_ns,
+                            "original_runtime": explanation_final.original_runtime_ns,
+                            "winning_test_results": {
+                                tt.to_name(): v
+                                for tt, v in explanation_final.winning_test_results.get_test_pass_fail_report_by_type().items()
+                            },
+                        },
+                    )
+                    test_files = function_to_tests.get(module_path + "." + function_name)
+                    existing_tests = ""
+                    if test_files:
+                        for test_file in test_files:
+                            with open(test_file.test_file, encoding="utf8") as f:
+                                new_test = "".join(f.readlines())
+                                if new_test not in existing_tests:
+                                    existing_tests += new_test
+
+                    check_create_pr(
+                        optimize_all=self.args.all,
+                        path=path,
+                        original_code=original_dependent_code | {path: original_code},
+                        new_code=new_dependent_code | {path: new_code},
+                        explanation=explanation_final,
+                        existing_tests_source=existing_tests,
+                        generated_original_test_source=generated_original_test_source,
+                    )
+                    if self.args.all or env_utils.get_pr_number():
+                        # Reverting to original code, because optimizing functions in a sequence can lead to
+                        #  a) Error propagation, where error in one function can cause the next optimization to fail
+                        #  b) Performance estimates become unstable, as the runtime of an optimization might be
+                        #     dependent on the runtime of the previous optimization
+                        with open(path, "w", encoding="utf8") as f:
+                            f.write(original_code)
+                        for module_abspath in dependent_functions_by_module_abspath.keys():
+                            with open(module_abspath, "w", encoding="utf8") as f:
+                                f.write(original_dependent_code[module_abspath])
+                # Delete all the generated tests to not cause any clutter.
+                pathlib.Path(generated_tests_path).unlink(missing_ok=True)
+                for test_paths in instrumented_unittests_created_for_function:
+                    pathlib.Path(test_paths).unlink(missing_ok=True)
             ph("cli-optimize-run-finished", {"optimizations_found": optimizations_found})
             if optimizations_found == 0:
                 logging.info("❌ No optimizations found.")
             elif self.args.all:
                 logging.info("✨ All functions have been optimized! ✨")
         finally:
             # TODO: Also revert the file/function being optimized if the process did not succeed
@@ -534,15 +587,15 @@
                 )
                 with open(new_test_path, "w", encoding="utf8") as f:
                     f.write(injected_test)
                 unique_instrumented_test_files.add(new_test_path)
                 unique_original_test_files.add(tests_in_file.test_file)
             logging.info(
                 f"Discovered {relevant_test_files_count} existing unit test file"
-                f"{'s' if relevant_test_files_count != 1 else ''} for {full_module_function_path}"
+                f"{'s' if relevant_test_files_count != 1 else ''} for {full_module_function_path}",
             )
         return unique_instrumented_test_files
 
     def generate_tests_and_optimizations(
         self,
         code_to_optimize_with_dependents: str,
         function_to_optimize: FunctionToOptimize,
@@ -633,82 +686,88 @@
                 if generated_tests_elapsed_time > MAX_FUNCTION_TEST_SECONDS:
                     do_break = True
                     break
                 instrumented_existing_test_timing = []
                 original_test_results_iter = TestResults()
                 for test_file in instrumented_unittests_created_for_function:
                     unittest_results = self.run_and_parse_tests(
-                        test_env, test_file, TestType.EXISTING_UNIT_TEST, 0
+                        test_env,
+                        test_file,
+                        TestType.EXISTING_UNIT_TEST,
+                        0,
                     )
 
                     timing = unittest_results.total_passed_runtime()
                     original_test_results_iter.merge(unittest_results)
                     instrumented_existing_test_timing.append(timing)
                 if i == 0 and first_run:
                     logging.info(
-                        f"original code, existing unit test results -> {original_test_results_iter.get_test_pass_fail_report()}"
+                        f"original code, existing unit test results -> {original_test_results_iter.get_test_pass_fail_report()}",
                     )
 
                 original_gen_results = self.run_and_parse_tests(
-                    test_env, generated_tests_path, TestType.GENERATED_REGRESSION, 0
+                    test_env,
+                    generated_tests_path,
+                    TestType.GENERATED_REGRESSION,
+                    0,
                 )
 
                 # TODO: Implement the logic to disregard the timing info of the tests that errored out. That is remove test cases that failed to run.
 
                 if not original_gen_results and len(instrumented_existing_test_timing) == 0:
                     logging.warning(
-                        f"Couldn't run any tests for original function {function_name}. SKIPPING OPTIMIZING THIS FUNCTION."
+                        f"Couldn't run any tests for original function {function_name}. SKIPPING OPTIMIZING THIS FUNCTION.",
                     )
                     success = False
                     do_break = True
                     break
                 # TODO: Doing a simple sum of test runtime, Improve it by looking at test by test runtime, or a better scheme
                 # TODO: If the runtime is None, that happens in the case where an exception is expected and is successfully
                 #  caught by the test framework. This makes the test pass, but we can't find runtime because the exception caused
                 #  the execution to not reach the runtime measurement part. We are currently ignoring such tests, because the performance
                 #  for such a execution that raises an exception should not matter.
                 if i == 0 and first_run:
                     logging.info(
-                        f"original generated tests results -> {original_gen_results.get_test_pass_fail_report()}"
+                        f"original generated tests results -> {original_gen_results.get_test_pass_fail_report()}",
                     )
 
                 original_total_runtime_iter = original_gen_results.total_passed_runtime() + sum(
-                    instrumented_existing_test_timing
+                    instrumented_existing_test_timing,
                 )
                 if original_total_runtime_iter == 0:
                     logging.warning(
-                        "The overall test runtime of the original function is 0, couldn't run tests."
+                        "The overall test runtime of the original function is 0, couldn't run tests.",
                     )
                     logging.warning(original_gen_results.test_results)
                     do_break = True
                     break
                 original_test_results_iter.merge(original_gen_results)
                 if i == 0 and first_run:
                     logging.info(
-                        f"Original overall test results = {TestResults.report_to_string(original_test_results_iter.get_test_pass_fail_report_by_type())}"
+                        f"Original overall test results = {TestResults.report_to_string(original_test_results_iter.get_test_pass_fail_report_by_type())}",
                     )
                 if original_runtime is None or original_total_runtime_iter < original_runtime:
                     original_runtime = best_runtime = original_total_runtime_iter
                     overall_original_test_results = original_test_results_iter
                 cumulative_test_runs += 1
                 cumulative_test_runtime += original_total_runtime_iter
                 times_run += 1
             if first_run:
                 first_run = False
             if do_break:
                 break
 
         if times_run == 0:
             logging.warning(
-                "Failed to run the tests for the original function, skipping optimization"
+                "Failed to run the tests for the original function, skipping optimization",
             )
             success = False
         if success:
             logging.info(
-                f"Original code runtime measured over {times_run} run{'s' if times_run > 1 else ''}: {humanize_runtime(original_runtime)}"
+                f"Original code runtime measured over {times_run} run{'s' if times_run > 1 else ''}: {humanize_runtime(original_runtime)}",
             )
         return success, original_gen_results, overall_original_test_results, best_runtime
 
     def run_optimized_candidate(
         self,
         optimization_index: int,
         instrumented_unittests_created_for_function: set[str],
@@ -736,18 +795,18 @@
         do_break = False
         while (
             cumulative_test_runtime < MAX_CUMULATIVE_TEST_RUNTIME_NANOSECONDS
             and cumulative_test_runs < MAX_TEST_FUNCTION_RUNS
         ):
             for test_index in range(MAX_TEST_RUN_ITERATIONS):
                 pathlib.Path(
-                    get_run_tmp_file(f"test_return_values_{optimization_index}.bin")
+                    get_run_tmp_file(f"test_return_values_{optimization_index}.bin"),
                 ).unlink(missing_ok=True)
                 pathlib.Path(
-                    get_run_tmp_file(f"test_return_values_{optimization_index}.sqlite")
+                    get_run_tmp_file(f"test_return_values_{optimization_index}.sqlite"),
                 ).unlink(missing_ok=True)
                 if generated_tests_elapsed_time > MAX_FUNCTION_TEST_SECONDS:
                     do_break = True
                     break
 
                 optimized_test_results_iter = TestResults()
                 instrumented_test_timing = []
@@ -760,25 +819,25 @@
                     )
                     timing = unittest_results_optimized.total_passed_runtime()
                     optimized_test_results_iter.merge(unittest_results_optimized)
                     instrumented_test_timing.append(timing)
                 if first_run and test_index == 0:
                     equal_results = True
                     logging.info(
-                        f"optimized existing unit tests result -> {optimized_test_results_iter.get_test_pass_fail_report()}"
+                        f"optimized existing unit tests result -> {optimized_test_results_iter.get_test_pass_fail_report()}",
                     )
                     for test_invocation in optimized_test_results_iter:
                         if (
                             overall_original_test_results.get_by_id(test_invocation.id) is None
                             or test_invocation.did_pass
                             != overall_original_test_results.get_by_id(test_invocation.id).did_pass
                         ):
                             logging.info("Results did not match.")
                             logging.info(
-                                f"Test {test_invocation.id} failed on the optimized code. Skipping this optimization"
+                                f"Test {test_invocation.id} failed on the optimized code. Skipping this optimization",
                             )
                             equal_results = False
                             do_break = True
                             break
                     if not equal_results:
                         do_break = True
                         break
@@ -788,15 +847,15 @@
                     generated_tests_path,
                     TestType.GENERATED_REGRESSION,
                     optimization_index,
                 )
 
                 if first_run and test_index == 0:
                     logging.info(
-                        f"generated test_results optimized -> {test_results.get_test_pass_fail_report()}"
+                        f"generated test_results optimized -> {test_results.get_test_pass_fail_report()}",
                     )
                     if test_results:
                         if compare_results(original_gen_results, test_results):
                             equal_results = True
                             logging.info("Results matched!")
                         else:
                             logging.info("Results did not match.")
@@ -805,15 +864,15 @@
                     do_break = True
                     break
 
                 test_runtime = test_results.total_passed_runtime() + sum(instrumented_test_timing)
 
                 if test_runtime == 0:
                     logging.warning(
-                        "The overall test runtime of the optimized function is 0, couldn't run tests."
+                        "The overall test runtime of the optimized function is 0, couldn't run tests.",
                     )
                     do_break = True
                     break
                 if best_test_runtime is None or test_runtime < best_test_runtime:
                     optimized_test_results_iter.merge(test_results)
                     best_test_runtime = test_runtime
                     best_test_results = optimized_test_results_iter
@@ -827,18 +886,18 @@
                 # then it is not a good optimization. Early exit to save time.
                 success = True
                 do_break = True
             if do_break:
                 break
 
         pathlib.Path(get_run_tmp_file(f"test_return_values_{optimization_index}.bin")).unlink(
-            missing_ok=True
+            missing_ok=True,
         )
         pathlib.Path(get_run_tmp_file(f"test_return_values_{optimization_index}.sqlite")).unlink(
-            missing_ok=True
+            missing_ok=True,
         )
         if not (equal_results and times_run > 0):
             success = False
 
         return (
             success,
             times_run,
@@ -862,15 +921,15 @@
             verbose=True,
             test_env=test_env,
         )
         if run_result.returncode != 0:
             logging.debug(
                 f"Nonzero return code {run_result.returncode} when running tests in {test_file}.\n"
                 f"stdout: {run_result.stdout}\n"
-                f"stderr: {run_result.stderr}\n"
+                f"stderr: {run_result.stderr}\n",
             )
         unittest_results = parse_test_results(
             test_xml_path=result_file_path,
             test_py_path=test_file,
             test_config=self.test_cfg,
             test_type=test_type,
             run_result=run_result,
@@ -894,15 +953,15 @@
             test_cfg=self.test_cfg,
             test_timeout=INDIVIDUAL_TEST_TIMEOUT,
             use_cached_tests=self.args.use_cached_tests,
             function_trace_id=function_trace_id,
         )
         if tests is None:
             logging.error(
-                f"Failed to generate and instrument tests for {function_to_optimize.function_name}"
+                f"Failed to generate and instrument tests for {function_to_optimize.function_name}",
             )
             return None
 
         generated_original_test_source, instrumented_test_source = tests
 
         return generated_original_test_source, instrumented_test_source
```

### Comparing `codeflash-0.4.1/codeflash/optimization/function_context.py` & `codeflash-0.5.0/codeflash/optimization/function_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,178 +1,180 @@
 import ast
 import logging
 import os
-from typing import NoReturn, Union
+from typing import Union
 
 import jedi
 import tiktoken
 from jedi.api.classes import Name
 from pydantic.dataclasses import dataclass
 
-from codeflash.code_utils.code_extractor import get_code_no_skeleton, get_code
+from codeflash.code_utils.code_extractor import get_code, get_code_no_skeleton
 from codeflash.code_utils.code_utils import path_belongs_to_site_packages
-from codeflash.discovery.functions_to_optimize import FunctionToOptimize, FunctionParent
+from codeflash.discovery.functions_to_optimize import FunctionParent, FunctionToOptimize
 
 
 def belongs_to_class(name: Name, class_name: str) -> bool:
-    """
-    Check if the given name belongs to the specified class.
-    """
-    if name.full_name and name.full_name.startswith(name.module_name):
-        subname = name.full_name[len(name.module_name) + 1 :]
-        class_prefix = f"{class_name}."
-        return subname.startswith(class_prefix)
+    """Check if the given name belongs to the specified class."""
+    if name.full_name and name.full_name.startswith(f"{name.module_name}.{class_name}."):
+        return True
     return False
 
 
 def belongs_to_function(name: Name, function_name: str) -> bool:
-    """
-    Check if the given name belongs to the specified function
-    """
+    """Check if the given name belongs to the specified function"""
     if name.full_name and name.full_name.startswith(name.module_name):
-        subname = name.full_name.replace(name.module_name, "", 1)
+        subname: str = name.full_name.replace(name.module_name, "", 1)
     else:
         return False
     # The name is defined inside the function or is the function itself
     return f".{function_name}." in subname or f".{function_name}" == subname
 
 
 @dataclass(frozen=True, config={"arbitrary_types_allowed": True})
 class Source:
     full_name: str
     definition: Name
     source_code: str
 
 
 def get_type_annotation_context(
-    function: FunctionToOptimize, jedi_script: jedi.Script, project_root_path: str
+    function: FunctionToOptimize,
+    jedi_script: jedi.Script,
+    project_root_path: str,
 ) -> list[tuple[Source, str, str]]:
     function_name: str = function.function_name
     file_path: str = function.file_path
-    with open(file_path, "r", encoding="utf8") as file:
+    with open(file_path, encoding="utf8") as file:
         file_contents: str = file.read()
     try:
         module: ast.Module = ast.parse(file_contents)
     except SyntaxError as e:
-        logging.error(f"get_type_annotation_context - Syntax error in code: {e}")
+        logging.exception(f"get_type_annotation_context - Syntax error in code: {e}")
         return []
     sources: list[tuple[Source, str, str]] = []
-    ast_parents: list[str] = []
+    ast_parents: list[FunctionParent] = []
 
     def visit_children(
-        node: Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module], node_parents
-    ) -> NoReturn:
+        node: Union[ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module],
+        node_parents: list[FunctionParent],
+    ) -> None:
+        child: Union[ast.AST, ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module]
         for child in ast.iter_child_nodes(node):
             visit(child, node_parents)
 
     def visit(
         node: Union[ast.AST, ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef, ast.Module],
-        node_parents: list[Union[FunctionParent, str]],
-    ) -> NoReturn:
+        node_parents: list[FunctionParent],
+    ) -> None:
         if isinstance(node, (ast.Module, ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef)):
             if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
                 if node.name == function_name and node_parents == function.parents:
+                    arg: ast.arg
                     for arg in node.args.args:
                         if arg.annotation and hasattr(arg.annotation, "id"):
-                            name = arg.annotation.id
-                            line_no = arg.annotation.lineno
-                            col_no = arg.annotation.col_offset
+                            name: str = arg.annotation.id
+                            line_no: int = arg.annotation.lineno
+                            col_no: int = arg.annotation.col_offset
                             try:
                                 definition: list[Name] = jedi_script.goto(
                                     line=line_no,
                                     column=col_no,
                                     follow_imports=True,
                                     follow_builtin_imports=False,
                                 )
-                            except Exception as e:
+                            except Exception as ex:
                                 if hasattr(name, "full_name"):
-                                    logging.error(
-                                        f"Error while getting definition for {name.full_name}: {e}"
+                                    logging.exception(
+                                        f"Error while getting definition for {name.full_name}: {ex}",
                                     )
                                 else:
-                                    logging.error(f"Error while getting definition: {e}")
+                                    logging.exception(f"Error while getting definition: {ex}")
                                 definition = []
                             if definition:  # TODO can be multiple definitions
                                 definition_path = str(definition[0].module_path)
                                 # The definition is part of this project and not defined within the original function
                                 if (
                                     definition_path.startswith(project_root_path + os.sep)
                                     and definition[0].full_name
                                     and not path_belongs_to_site_packages(definition_path)
                                     and not belongs_to_function(definition[0], function_name)
                                 ):
                                     source_code = get_code(
-                                        FunctionToOptimize(
-                                            definition[0].name,
-                                            definition_path,
-                                            node_parents[:-1],
-                                        )
-                                    )
+                                        [
+                                            FunctionToOptimize(
+                                                definition[0].name,
+                                                definition_path,
+                                                node_parents[:-1],
+                                            ),
+                                        ],
+                                    )[0]
                                     if source_code:
                                         sources.append(
                                             (
                                                 Source(
                                                     definition[0].name,
                                                     definition[0],
                                                     source_code,
                                                 ),
                                                 definition_path,
                                                 definition[0].full_name.removeprefix(
-                                                    definition[0].module_name + "."
+                                                    definition[0].module_name + ".",
                                                 ),
-                                            )
+                                            ),
                                         )
             if not isinstance(node, ast.Module):
-                node_parents.append(node.name)
+                node_parents.append(FunctionParent(node.name, type(node).__name__))
             visit_children(node, node_parents)
             if not isinstance(node, ast.Module):
                 node_parents.pop()
 
     visit(module, ast_parents)
 
     return sources
 
 
 def get_function_variables_definitions(
-    function_to_optimize: FunctionToOptimize, project_root_path: str
+    function_to_optimize: FunctionToOptimize,
+    project_root_path: str,
 ) -> list[tuple[Source, str, str]]:
     function_name = function_to_optimize.function_name
     file_path = function_to_optimize.file_path
     script = jedi.Script(path=file_path, project=jedi.Project(path=project_root_path))
     sources: list[tuple[Source, str, str]] = []
     # TODO: The function name condition can be stricter so that it does not clash with other class names etc.
     # TODO: The function could have been imported as some other name,
     #  we should be checking for the translation as well. Also check for the original function name.
     names = []
     for ref in script.get_names(all_scopes=True, definitions=False, references=True):
         if ref.full_name:
             if function_to_optimize.parents:
                 # Check if the reference belongs to the specified class when FunctionParent is provided
                 if belongs_to_class(
-                    ref, function_to_optimize.parents[-1].name
+                    ref,
+                    function_to_optimize.parents[-1].name,
                 ) and belongs_to_function(ref, function_name):
                     names.append(ref)
-            else:
-                if belongs_to_function(ref, function_name):
-                    names.append(ref)
+            elif belongs_to_function(ref, function_name):
+                names.append(ref)
 
     for name in names:
         try:
             definitions: list[Name] = script.goto(
                 line=name.line,
                 column=name.column,
                 follow_imports=True,
                 follow_builtin_imports=False,
             )
         except Exception as e:
             try:
-                logging.error(f"Error while getting definition for {name.full_name}: {e}")
+                logging.exception(f"Error while getting definition for {name.full_name}: {e}")
             except Exception as e:
                 # name.full_name can also throw exceptions sometimes
-                logging.error(f"Error while getting definition: {e}")
+                logging.exception(f"Error while getting definition: {e}")
             definitions = []
         if definitions:
             # TODO: there can be multiple definitions, see how to handle such cases
             definition_path = str(definitions[0].module_path)
             # The definition is part of this project and not defined within the original function
             if (
                 definition_path.startswith(project_root_path + os.sep)
@@ -183,18 +185,20 @@
                 source_code = get_code_no_skeleton(definition_path, definitions[0].name)
                 if source_code:
                     sources.append(
                         (
                             Source(name.full_name, definitions[0], source_code),
                             definition_path,
                             name.full_name.removeprefix(name.module_name + "."),
-                        )
+                        ),
                     )
     annotation_sources = get_type_annotation_context(
-        function_to_optimize, script, project_root_path
+        function_to_optimize,
+        script,
+        project_root_path,
     )
     sources[:0] = annotation_sources  # prepend the annotation sources
     deduped_sources = []
     existing_full_names = set()
     for source in sources:
         if source[0].full_name not in existing_full_names:
             deduped_sources.append(source)
@@ -210,27 +214,39 @@
     project_root_path: str,
     code_to_optimize: str,
     max_tokens: int = MAX_PROMPT_TOKENS,
 ) -> tuple[str, list[tuple[Source, str, str]]]:
     # TODO: Not just do static analysis, but also find the datatypes of function arguments by running the existing
     #  unittests and inspecting the arguments to resolve the real definitions and dependencies.
     dependent_functions: list[tuple[Source, str, str]] = get_function_variables_definitions(
-        function_to_optimize, project_root_path
+        function_to_optimize,
+        project_root_path,
     )
     tokenizer = tiktoken.encoding_for_model("gpt-3.5-turbo")
     code_to_optimize_tokens = tokenizer.encode(code_to_optimize)
-    dependent_functions_sources = [function[0].source_code for function in dependent_functions]
+
+    if not function_to_optimize.parents:
+        dependent_functions_sources = [function[0].source_code for function in dependent_functions]
+    else:
+        dependent_functions_sources = [
+            function[0].source_code
+            for function in dependent_functions
+            if not function[2].count(".")
+            or function[2].split(".")[0] != function_to_optimize.parents[0].name
+        ]
     dependent_functions_tokens = [
         len(tokenizer.encode(function)) for function in dependent_functions_sources
     ]
+
     context_list = []
     context_len = len(code_to_optimize_tokens)
     logging.debug(f"ORIGINAL CODE TOKENS LENGTH: {context_len}")
     logging.debug(f"ALL DEPENDENCIES TOKENS LENGTH: {sum(dependent_functions_tokens)}")
     for function_source, source_len in zip(dependent_functions_sources, dependent_functions_tokens):
         if context_len + source_len <= max_tokens:
             context_list.append(function_source)
             context_len += source_len
         else:
             break
     logging.debug("FINAL OPTIMIZATION CONTEXT TOKENS LENGTH:", context_len)
-    return "\n".join(context_list) + "\n" + code_to_optimize, dependent_functions
+    dependent_code: str = "\n".join(context_list)
+    return dependent_code, dependent_functions
```

### Comparing `codeflash-0.4.1/codeflash/result/create_pr.py` & `codeflash-0.5.0/codeflash/result/create_pr.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/result/explanation.py` & `codeflash-0.5.0/codeflash/result/explanation.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/telemetry/posthog.py` & `codeflash-0.5.0/codeflash/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/telemetry/sentry.py` & `codeflash-0.5.0/codeflash/telemetry/sentry.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/tracing/replay_test.py` & `codeflash-0.5.0/codeflash/tracing/replay_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     imports = f"""import pickle
 import {test_framework}
 from codeflash.tracing.replay_test import get_next_arg_and_return
 from codeflash.validation.comparators import comparator
 """
 
+    # TODO: Module can have "-" character if the module-root is ".". Need to handle that case
     function_imports = [
         f"from {module} import {function_name} as {get_function_alias(module, function_name)}"
         for module, function_name in functions
     ]
     imports += "\n".join(function_imports)
 
     if test_framework == "unittest":
@@ -120,10 +121,10 @@
             test_function_body.format(
                 trace_file=trace_file,
                 function_name=function_name_alias,
                 orig_function_name=function_name,
             ),
             "    ",
         )
-        test_template += f"def test_{function_name_alias}():\n{formatted_test_body}\n"
+        test_template += f"\ndef test_{function_name_alias}():\n{formatted_test_body}\n"
 
     return test_template
```

### Comparing `codeflash-0.4.1/codeflash/tracing/tracer.py` & `codeflash-0.5.0/codeflash/tracing/tracer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,48 +2,49 @@
 import os
 import pathlib
 import pickle
 import sqlite3
 import sys
 import time
 from collections import defaultdict
-from typing import Any, Dict, List, Optional
-
-from codeflash.validation.validation_utils import get_test_file_path
+from typing import Any, Dict, Optional
 
 from codeflash.code_utils.code_utils import module_name_from_file_path
 from codeflash.code_utils.config_parser import parse_config_file
 from codeflash.tracing.replay_test import create_trace_replay_test
+from codeflash.verification.verification_utils import get_test_file_path
 
 
 class Tracer:
     """
     Use this class as a 'with' context manager to trace a function call,
     input arguments, and return value.
     """
 
     def __init__(
         self,
         output: str = "script.trace",
-        functions: List[str] = [],
+        functions=None,
         disable: bool = False,
         config_file_path: Optional[str] = None,
     ) -> None:
+        if functions is None:
+            functions = []
         self.disable = disable
         self.con = None
         self.flag = (
             False  # To ignore the first call to trace_callback due to return from trace_callback
         )
         self.output_file = os.path.abspath(output)
         self.functions = functions
         self.function_modules: Dict[str, str] = {}
         self.function_filenames: Dict[str, str] = {}
         self.function_count = defaultdict(int)
         self.max_function_count = 50
-        self.config = parse_config_file(config_file_path)
+        self.config, found_config_path = parse_config_file(config_file_path)
 
         assert (
             "test_framework" in self.config
         ), "Please specify 'test-framework' in pyproject.toml config file"
 
     def __enter__(self) -> None:
         if self.disable:
```

### Comparing `codeflash-0.4.1/codeflash/update_license_version.py` & `codeflash-0.5.0/codeflash/update_license_version.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/verification/comparator.py` & `codeflash-0.5.0/codeflash/verification/comparator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 import decimal
 import logging
 import math
 from typing import Any
 
+import sentry_sdk
+
 try:
     import numpy as np
 
     HAS_NUMPY = True
 except ImportError:
     HAS_NUMPY = False
 try:
@@ -28,114 +30,121 @@
 
     HAS_PANDAS = True
 except ImportError:
     HAS_PANDAS = False
 
 
 def comparator(orig: Any, new: Any) -> bool:
-    if HAS_SQLALCHEMY:
-        try:
-            insp = sqlalchemy.inspection.inspect(orig)
-            insp = sqlalchemy.inspection.inspect(new)
-            orig_keys = orig.__dict__
-            new_keys = new.__dict__
-            for key in list(orig_keys.keys()):
-                if key.startswith("_"):
-                    continue
-                if key not in new_keys or not comparator(orig_keys[key], new_keys[key]):
+    try:
+        if HAS_SQLALCHEMY:
+            try:
+                insp = sqlalchemy.inspection.inspect(orig)
+                insp = sqlalchemy.inspection.inspect(new)
+                orig_keys = orig.__dict__
+                new_keys = new.__dict__
+                for key in list(orig_keys.keys()):
+                    if key.startswith("_"):
+                        continue
+                    if key not in new_keys or not comparator(orig_keys[key], new_keys[key]):
+                        return False
+                return True
+
+            except sqlalchemy.exc.NoInspectionAvailable:
+                pass
+        if type(orig) != type(new):
+            return False
+        if isinstance(orig, (list, tuple)):
+            if len(orig) != len(new):
+                return False
+            for elem1, elem2 in zip(orig, new):
+                if not comparator(elem1, elem2):
                     return False
             return True
 
-        except sqlalchemy.exc.NoInspectionAvailable:
-            pass
-    if type(orig) != type(new):
-        return False
-    if isinstance(orig, (list, tuple)):
-        if len(orig) != len(new):
-            return False
-        for elem1, elem2 in zip(orig, new):
-            if not comparator(elem1, elem2):
+        if isinstance(orig, (str, int, bool, complex, type(None), decimal.Decimal, set)):
+            return orig == new
+        if isinstance(orig, float):
+            if math.isnan(orig) and math.isnan(new):
+                return True
+            return math.isclose(orig, new)
+        # scipy condition because dok_matrix type is also a instance of dict, but dict comparison doesn't work for it
+        if isinstance(orig, dict) and not (HAS_SCIPY and isinstance(orig, scipy.sparse.spmatrix)):
+            if len(orig) != len(new):
                 return False
-        return True
-
-    if isinstance(orig, (str, int, bool, complex, type(None), decimal.Decimal, set)):
-        return orig == new
-    if isinstance(orig, float):
-        if math.isnan(orig) and math.isnan(new):
+            for key in orig:
+                if key not in new:
+                    return False
+                if not comparator(orig[key], new[key]):
+                    return False
             return True
-        return math.isclose(orig, new)
-    # scipy condition because dok_matrix type is also a instance of dict, but dict comparison doesn't work for it
-    if isinstance(orig, dict) and not (HAS_SCIPY and isinstance(orig, scipy.sparse.spmatrix)):
-        if len(orig) != len(new):
-            return False
-        for key in orig:
-            if key not in new:
+
+        if HAS_NUMPY and isinstance(orig, np.ndarray):
+            if orig.dtype != new.dtype:
                 return False
-            if not comparator(orig[key], new[key]):
+            if orig.shape != new.shape:
                 return False
-        return True
-
-    if HAS_NUMPY and isinstance(orig, np.ndarray):
-        if orig.dtype != new.dtype:
-            return False
-        if orig.shape != new.shape:
-            return False
-        try:
-            return np.allclose(orig, new, equal_nan=True)
-        except Exception:
-            # fails at "ufunc 'isfinite' not supported for the input types"
-            return np.all([comparator(x, y) for x, y in zip(orig, new)])
-
-    if HAS_NUMPY and isinstance(orig, (np.floating, np.complex64, np.complex128)):
-        return np.isclose(orig, new)
+            try:
+                return np.allclose(orig, new, equal_nan=True)
+            except Exception:
+                # fails at "ufunc 'isfinite' not supported for the input types"
+                return np.all([comparator(x, y) for x, y in zip(orig, new)])
 
-    if HAS_NUMPY and isinstance(orig, (np.integer, np.bool_, np.byte)):
-        return orig == new
+        if HAS_NUMPY and isinstance(orig, (np.floating, np.complex64, np.complex128)):
+            return np.isclose(orig, new)
 
-    if HAS_SCIPY and isinstance(orig, scipy.sparse.spmatrix):
-        if orig.dtype != new.dtype:
-            return False
-        if orig.get_shape() != new.get_shape():
-            return False
-        return (orig != new).nnz == 0
-
-    if HAS_PANDAS and isinstance(
-        orig,
-        (
-            pandas.DataFrame,
-            pandas.Series,
-            pandas.Index,
-            pandas.Categorical,
-            pandas.arrays.SparseArray,
-        ),
-    ):
-        return orig.equals(new)
+        if HAS_NUMPY and isinstance(orig, (np.integer, np.bool_, np.byte)):
+            return orig == new
 
-    if HAS_PANDAS and isinstance(orig, (pandas.CategoricalDtype, pandas.Interval, pandas.Period)):
-        return orig == new
+        if HAS_SCIPY and isinstance(orig, scipy.sparse.spmatrix):
+            if orig.dtype != new.dtype:
+                return False
+            if orig.get_shape() != new.get_shape():
+                return False
+            return (orig != new).nnz == 0
 
-    # This should be at the end of all numpy checking
-    try:
-        if HAS_NUMPY and np.isnan(orig):
-            return np.isnan(new)
-    except Exception:
-        pass
-    try:
-        if HAS_NUMPY and np.isinf(orig):
-            return np.isinf(new)
-    except Exception:
-        pass
+        if HAS_PANDAS and isinstance(
+            orig,
+            (
+                pandas.DataFrame,
+                pandas.Series,
+                pandas.Index,
+                pandas.Categorical,
+                pandas.arrays.SparseArray,
+            ),
+        ):
+            return orig.equals(new)
+
+        if HAS_PANDAS and isinstance(
+            orig, (pandas.CategoricalDtype, pandas.Interval, pandas.Period)
+        ):
+            return orig == new
 
-    if isinstance(orig, (datetime.datetime, datetime.date, datetime.timedelta)):
-        return orig == new
+        # This should be at the end of all numpy checking
+        try:
+            if HAS_NUMPY and np.isnan(orig):
+                return np.isnan(new)
+        except Exception:
+            pass
+        try:
+            if HAS_NUMPY and np.isinf(orig):
+                return np.isinf(new)
+        except Exception:
+            pass
 
-    # If the object passed has a user defined __eq__ method, use that
-    # This could fail if the user defined __eq__ is defined with cython
-    try:
-        if hasattr(orig, "__eq__") and str(type(orig.__eq__)) == "<class 'method'>":
+        if isinstance(orig, (datetime.datetime, datetime.date, datetime.timedelta)):
             return orig == new
-    except Exception:
-        pass
 
-    # TODO : Add other types here
-    logging.warning(f"Unknown comparator input type: {type(orig)}")
-    return True
+        # If the object passed has a user defined __eq__ method, use that
+        # This could fail if the user defined __eq__ is defined with cython
+        try:
+            if hasattr(orig, "__eq__") and str(type(orig.__eq__)) == "<class 'method'>":
+                return orig == new
+        except Exception:
+            pass
+
+        # TODO : Add other types here
+        logging.warning(f"Unknown comparator input type: {type(orig)}")
+        return True
+    except RecursionError as e:
+        logging.error(f"RecursionError while comparing objects: {e}")
+        sentry_sdk.capture_exception(e)
+        return False
```

### Comparing `codeflash-0.4.1/codeflash/verification/parse_test_output.py` & `codeflash-0.5.0/codeflash/verification/parse_test_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,33 +33,36 @@
         return test_results
     with open(file_location, "rb") as file:
         while file:
             len_next = file.read(4)
             if not len_next:
                 return test_results
             len_next = int.from_bytes(len_next, byteorder="big")
-            encoded_invocation_id = file.read(len_next).decode("ascii")
+            encoded_test_name = file.read(len_next).decode("ascii")
             len_next = file.read(8)
             duration = int.from_bytes(len_next, byteorder="big")
             len_next = file.read(4)
             if not len_next:
                 return test_results
             len_next = int.from_bytes(len_next, byteorder="big")
             try:
                 test_pickle = pickle.loads(file.read(len_next))
             except Exception as e:
                 logging.error(f"Failed to load pickle file. Exception: {e}")
                 return test_results
+            len_next = file.read(4)
+            len_next = int.from_bytes(len_next, byteorder="big")
+            invocation_id = file.read(len_next).decode("ascii")
             # TODO : Remove the fully loaded unpickled object from the test_results.
             #  replace it with a link to the pickle object. Load it only on demand.
             #  The problem is that the unpickled object might be huge. This could cause codeflash to crash
             #  due to out-of-memory. Plus as we fill memory, the benchmarking results will get skewed.
             test_results.add(
                 FunctionTestInvocation(
-                    id=InvocationId.from_str_id(encoded_invocation_id),
+                    id=InvocationId.from_str_id(encoded_test_name, invocation_id),
                     file_name=test_file_path,
                     did_pass=True,
                     runtime=duration,
                     test_framework=test_framework,
                     test_type=test_type,
                     return_value=test_pickle,
                 )
```

### Comparing `codeflash-0.4.1/codeflash/verification/test_results.py` & `codeflash-0.5.0/codeflash/verification/test_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+import sys
 from enum import Enum
 from typing import Optional, Iterator, List
 
 from pydantic.dataclasses import dataclass
 
 from codeflash.verification.comparator import comparator
 
@@ -32,30 +33,30 @@
     iteration_id: Optional[str]
 
     # test_module_path:TestSuiteClass.test_function_name:function_tested:iteration_id
     def id(self):
         return f"{self.test_module_path}:{self.test_class_name or ''}.{self.test_function_name}:{self.function_getting_tested}:{self.iteration_id}"
 
     @staticmethod
-    def from_str_id(string_id: str):
+    def from_str_id(string_id: str, iteration_id: Optional[str] = None) -> "InvocationId":
         components = string_id.split(":")
         assert len(components) == 4
         second_components = components[1].split(".")
         if len(second_components) == 1:
             test_class_name = None
             test_function_name = second_components[0]
         else:
             test_class_name = second_components[0]
             test_function_name = second_components[1]
         return InvocationId(
             test_module_path=components[0],
             test_class_name=test_class_name,
             test_function_name=test_function_name,
             function_getting_tested=components[2],
-            iteration_id=components[3],
+            iteration_id=iteration_id if iteration_id else components[3],
         )
 
 
 @dataclass(frozen=True)
 class FunctionTestInvocation:
     id: InvocationId  # The fully qualified name of the function invocation (id)
     file_name: str  # The file where the test is defined
@@ -152,21 +153,27 @@
 
     def __eq__(self, other: TestResults):
         # Unordered comparison
         if type(self) != type(other):
             return False
         if len(self) != len(other):
             return False
+        original_recursion_limit = sys.getrecursionlimit()
         for test_result in self:
             other_test_result = other.get_by_id(test_result.id)
             if other_test_result is None:
                 return False
+
+            if original_recursion_limit < 5000:
+                sys.setrecursionlimit(5000)
             if (
                 test_result.file_name != other_test_result.file_name
                 or test_result.did_pass != other_test_result.did_pass
                 or test_result.runtime != other_test_result.runtime
                 or test_result.test_framework != other_test_result.test_framework
                 or test_result.test_type != other_test_result.test_type
                 or not comparator(test_result.return_value, other_test_result.return_value)
             ):
+                sys.setrecursionlimit(original_recursion_limit)
                 return False
+        sys.setrecursionlimit(original_recursion_limit)
         return True
```

### Comparing `codeflash-0.4.1/codeflash/verification/test_runner.py` & `codeflash-0.5.0/codeflash/verification/test_runner.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/verification/verification_utils.py` & `codeflash-0.5.0/codeflash/verification/verification_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/codeflash/verification/verifier.py` & `codeflash-0.5.0/codeflash/verification/verifier.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.4.1/pyproject.toml` & `codeflash-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "codeflash"
-version = "0.4.1" # Determined by poetry-dynamic-versioning during `poetry build`
+version = "0.5.0" # Determined by poetry-dynamic-versioning during `poetry build`
 description = "Client for codeflash.ai - automatic code performance optimization, powered by AI"
 license = "BSL-1.1"
 authors = ["CodeFlash Inc. <contact@codeflash.ai>"]
 homepage = "https://codeflash.ai"
 readme = "README.md"
 packages = [
     { include = "codeflash" },
@@ -30,67 +30,81 @@
 humanize = ">=4.0.0"
 posthog = ">=3.0.0"
 click = ">=8.1.0"
 inquirer = ">=3.0.0"
 sentry-sdk = "^1.40.6"
 parameterized = ">=0.9.0"
 returns = "^0.22.0"
+isort = "5.13.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.12.0"
 mypy = "^1.9.0"
+ruff = "^0.3.5"
 
 
 [tool.poetry.build]
 script = "codeflash/update_license_version.py"
 
 [tool.poetry.scripts]
 codeflash = "codeflash.main:main"
 
-
 [tool.mypy]
-disallow_any_decorated = true
-disallow_any_explicit = true
-disallow_any_expr = true
-disallow_any_unimported = true
-disallow_subclassing_any = true
 pretty = true
 show_absolute_path = true
 show_column_numbers = true
 show_error_context = true
 strict = true
-verbosity = 0
 warn_unreachable = true
 plugins = [
     "pydantic.mypy"
 ]
 
+[[tool.mypy.overrides]]
+module = [
+    "jedi",
+    "jedi.api.classes"
+]
+ignore_missing_imports = true
+
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 
-[tool.black]
-line-length = 100
-target-version = ['py312']
+[tool.ruff.lint]
+select = ["ALL"]
+unfixable = ["F401"]
+ignore = ["ANN101", "S101", "D103","G004", "FIX002"]
 
 [tool.ruff.lint.flake8-type-checking]
 strict = true
 runtime-evaluated-base-classes = ["pydantic.BaseModel"]
 runtime-evaluated-decorators = ["pydantic.validate_call"]
 
 [tool.ruff.lint.pep8-naming]
 classmethod-decorators = [
     # Allow Pydantic's `@validator` decorator to trigger class method treatment.
     "pydantic.validator",
 ]
 
+[tool.ruff]
+line-length = 110
+
+[tool.ruff.format]
+docstring-code-format = true
+
+
+[tool.black]
+line-length = 110
+target-version = ['py312']
+
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 vcs = "git"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["codeflash/version.py"]
@@ -103,15 +117,14 @@
   __version_tuple__ = (0, 0, 0)
 """
 
 
 [tool.codeflash]
 module-root = "codeflash"
 tests-root = "tests"
-test-framework = "unittest"
+test-framework = "pytest"
 ignore-paths = []
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.2.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
-
```

### Comparing `codeflash-0.4.1/PKG-INFO` & `codeflash-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeflash
-Version: 0.4.1
+Version: 0.5.0
 Summary: Client for codeflash.ai - automatic code performance optimization, powered by AI
 Home-page: https://codeflash.ai
 License: BSL-1.1
 Keywords: codeflash,performance,optimization,ai,code,machine learning,LLM
 Author: CodeFlash Inc.
 Author-email: contact@codeflash.ai
 Requires-Python: >=3.9,<4.0
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=22.3.0)
 Requires-Dist: click (>=8.1.0)
 Requires-Dist: gitpython (>=3.1.31)
 Requires-Dist: humanize (>=4.0.0)
 Requires-Dist: inquirer (>=3.0.0)
+Requires-Dist: isort (==5.13.2)
 Requires-Dist: jedi (>=0.19.0)
 Requires-Dist: junitparser (>=3.1.0)
 Requires-Dist: libcst (>=1.0.1)
 Requires-Dist: parameterized (>=0.9.0)
 Requires-Dist: posthog (>=3.0.0)
 Requires-Dist: pydantic (>=1.10.1)
 Requires-Dist: pytest (>=7.0.0)
```

