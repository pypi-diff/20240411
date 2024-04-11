# Comparing `tmp/safe_init-1.0.0.tar.gz` & `tmp/safe_init-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_init-1.0.0.tar", max compression
+gzip compressed data, was "safe_init-1.0.1.tar", max compression
```

## Comparing `safe_init-1.0.0.tar` & `safe_init-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2024-03-25 11:18:57.731103 safe_init-1.0.0/LICENSE
--rw-r--r--   0        0        0    11769 2024-03-25 11:18:57.731103 safe_init-1.0.0/README.md
--rw-r--r--   0        0        0     3152 2024-03-25 11:18:57.731103 safe_init-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      736 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/__init__.py
--rw-r--r--   0        0        0     7428 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/decorator.py
--rw-r--r--   0        0        0     4240 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/dlq.py
--rw-r--r--   0        0        0      751 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/errors.py
--rw-r--r--   0        0        0     5422 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/handler.py
--rw-r--r--   0        0        0        0 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/py.typed
--rw-r--r--   0        0        0     3909 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/safe_logging.py
--rw-r--r--   0        0        0     1339 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/sentry.py
--rw-r--r--   0        0        0     5620 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/slack.py
--rw-r--r--   0        0        0     5479 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/timeout.py
--rw-r--r--   0        0        0     3918 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/tracer.py
--rw-r--r--   0        0        0     3237 2024-03-25 11:18:57.735103 safe_init-1.0.0/safe_init/utils.py
--rw-r--r--   0        0        0    13203 1970-01-01 00:00:00.000000 safe_init-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-11 09:07:19.830757 safe_init-1.0.1/LICENSE
+-rw-r--r--   0        0        0    11999 2024-04-11 09:07:19.830757 safe_init-1.0.1/README.md
+-rw-r--r--   0        0        0     3205 2024-04-11 09:07:19.834757 safe_init-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      736 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/__init__.py
+-rw-r--r--   0        0        0     7429 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/decorator.py
+-rw-r--r--   0        0        0     4240 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/dlq.py
+-rw-r--r--   0        0        0      751 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/errors.py
+-rw-r--r--   0        0        0     5422 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/handler.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/py.typed
+-rw-r--r--   0        0        0     3909 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/safe_logging.py
+-rw-r--r--   0        0        0     1339 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/sentry.py
+-rw-r--r--   0        0        0     5621 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/slack.py
+-rw-r--r--   0        0        0     5895 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/timeout.py
+-rw-r--r--   0        0        0     3918 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/tracer.py
+-rw-r--r--   0        0        0     3237 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/utils.py
+-rw-r--r--   0        0        0    13484 1970-01-01 00:00:00.000000 safe_init-1.0.1/PKG-INFO
```

### Comparing `safe_init-1.0.0/LICENSE` & `safe_init-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.0/README.md` & `safe_init-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# Safe Init
+# Safe Init: Simplifying AWS Lambda Error Handling and Monitoring
 
 [![PyPI version](https://badge.fury.io/py/safe-init.svg)](https://badge.fury.io/py/safe-init)
 [![Documentation Status](https://readthedocs.org/projects/safe-init/badge/?version=latest)](https://safe-init.readthedocs.io/en/latest/?badge=latest)
 [![Python versions](https://img.shields.io/pypi/pyversions/safe-init.svg)](https://pypi.org/project/safe-init/)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Safe Init is a Python library that provides a comprehensive set of tools for initializing AWS Lambda functions safely and handling errors and exceptions gracefully. It is designed to make your Lambda functions more robust, easier to debug, and less prone to unexpected failures. With Safe Init, you can focus on writing your core Lambda function logic while the library takes care of error handling, logging, notifications, and more.
 
+[Read the Docs](https://safe-init.readthedocs.io/en/latest/) | [GitHub Repository](https://github.com/Kalepa/safe-init) | [PyPI Package](https://pypi.org/project/safe-init/) 
+
 ## Features
 
 ### Error Handling and Logging
 - **Error Handling**: Safe Init wraps your Lambda handler with robust error handling and logging, ensuring that any unhandled exceptions are captured and logged for easy debugging.
 - **Execution Time Tracing**: Traces the execution time of all function calls within the Lambda handler, helping you identify performance bottlenecks and optimize your code.
 
 ### Monitoring and Alerting
```

### Comparing `safe_init-1.0.0/pyproject.toml` & `safe_init-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "safe-init"
-version = "1.0.0"
+version = "1.0.1"
 description = "Safe Init is a Python library that enhances AWS Lambda functions with advanced error handling, logging, monitoring, and resilience features, providing comprehensive observability and reliability for serverless applications."
 license = "MIT"
 authors = ["Maciej Wilczyński <maciej@lupine.software>"]
 repository = "https://github.com/kalepa/safe-init"
 readme = "README.md"
 packages = [{ include = "safe_init" }]
 include = ["safe_init/py.typed"]
+documentation = "https://safe-init.readthedocs.io/en/latest/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
@@ -26,16 +27,16 @@
 python = "~3.11"
 structlog = "^24.1.0"
 sentry-sdk = "<2.0.0"
 requests = "^2.31.0"
 awslambdaric = ">=2.0.10"
 boto3 = ">=1.20.0"
 boto3-type-annotations = ">=0.3.1"
-datadog-lambda = "5.91.0"
-ddtrace = "2.7.4"
+datadog-lambda = "*"
+ddtrace = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 mypy = "^1.4.1"
 types-ujson = ">=5.8.0.0"
 types-colorama = ">=0.4.15.11"
 types-urllib3 = ">=1.26.25.13,<2.0.0"
```

### Comparing `safe_init-1.0.0/safe_init/__init__.py` & `safe_init-1.0.1/safe_init/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-__VERSION__ = "1.0.0"
+__VERSION__ = "1.0.1"
 
 _wrapped_handler = None
 
 
 class LazyHandler:
     @staticmethod
     def _init_handler() -> None:
```

### Comparing `safe_init-1.0.0/safe_init/decorator.py` & `safe_init-1.0.1/safe_init/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
                 else LONG_NOTIFY_SEC_BEFORE_TIMEOUT
             )
 
         self.timeout_thread = TimeoutThread(
             remaining_exec_time / 1000.0 - notify_sec_before_timeout,
             timeout_message=(
                 f"Impending Lambda execution timeout detected — less than {notify_sec_before_timeout} seconds left to"
-                f" configured timeout ({timeout_value}s)"
+                f" configured timeout ({timeout_value}s)."
             ),
             call_args=args,
             call_kwargs=kwargs,
             execution_fingerprint=["TimeoutWarning", lambda_ctx.function_name],
         )
 
         # Start the thread to raise timeout warning exception
```

### Comparing `safe_init-1.0.0/safe_init/dlq.py` & `safe_init-1.0.1/safe_init/dlq.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.0/safe_init/errors.py` & `safe_init-1.0.1/safe_init/errors.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.0/safe_init/handler.py` & `safe_init-1.0.1/safe_init/handler.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.0/safe_init/safe_logging.py` & `safe_init-1.0.1/safe_init/safe_logging.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.0/safe_init/sentry.py` & `safe_init-1.0.1/safe_init/sentry.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.0/safe_init/slack.py` & `safe_init-1.0.1/safe_init/slack.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             {
                 "type": "section",
                 "text": {
                     "type": "plain_text",
                     "text": (
                         ":rage: There also was an error sending the event to Sentry."
                         if not sentry_capture_result
-                        else ":pepeok: The error has been sent to Sentry."
+                        else ":ok_hand: The error has been sent to Sentry."
                     ),
                 },
             },
         )
 
     slack_message = {
         "text": f"[{env}] Safe Init — {message_title} :pleading_face:",
```

### Comparing `safe_init-1.0.0/safe_init/timeout.py` & `safe_init-1.0.1/safe_init/timeout.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,36 +99,48 @@
         log_debug("Timeout thread processing data before raising")
 
         if context_has_dlq():
             log_debug("Pushing to DLQ")
             push_event_to_dlq(*self.call_args, **self.call_kwargs)
             log_debug("Pushed to DLQ")
 
-        calls_by_time = []
+        include_lambda_data = is_lambda_handler(self.call_args)
 
+        calls_by_time = []
         # Check if execution was traced to optionally include the trace in timeout warnings
-        if is_lambda_handler(self.call_args):
+        if include_lambda_data:
             log_debug("Checking for traces")
             if tracer.is_traced():
                 log_debug("Tracer is active")
                 fn_calls = tracer.get_function_calls()
                 aggregated_calls = aggregate_traced_fn_calls(fn_calls)
                 log_debug("Got aggregated calls", aggregated_calls=aggregated_calls)
                 calls_by_time = sorted(aggregated_calls, key=lambda x: x[2], reverse=True)
                 log_debug("Sorted calls by time", calls_by_time=calls_by_time)
 
         exc = SafeInitTimeoutWarning(self.timeout_message)
         exc.traces = calls_by_time
 
         sentry_result = sentry_capture(exc, fingerprint=self.execution_fingerprint)
         log_debug("Sentry capture result", sentry_capture_result=sentry_result)
+
+        additional_log_data: dict[str, Any] = {}
+        if calls_by_time:
+            additional_log_data["longest_calls"] = calls_by_time[:40]
+        if include_lambda_data:
+            additional_log_data["lambda_name"] = os.environ.get(
+                "AWS_LAMBDA_FUNCTION_NAME",
+                self.call_args[1].function_name,
+            )
+
         log_error(
             self.timeout_message,
             sentry_capture_result=sentry_result,
-            longest_calls=calls_by_time[:40],
+            exc_info=exc,
+            **additional_log_data,
         )
 
         if not os.getenv("SAFE_INIT_NO_SLACK_TIMEOUT_NOTIFICATIONS"):
             slack_notify(
                 str(exc),
                 exc,
                 lambda_context=self.call_args[1] if is_lambda_handler(self.call_args) else None,
```

### Comparing `safe_init-1.0.0/safe_init/tracer.py` & `safe_init-1.0.1/safe_init/tracer.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.0/safe_init/utils.py` & `safe_init-1.0.1/safe_init/utils.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.0/PKG-INFO` & `safe_init-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-init
-Version: 1.0.0
+Version: 1.0.1
 Summary: Safe Init is a Python library that enhances AWS Lambda functions with advanced error handling, logging, monitoring, and resilience features, providing comprehensive observability and reliability for serverless applications.
 Home-page: https://github.com/kalepa/safe-init
 License: MIT
 Author: Maciej Wilczyński
 Author-email: maciej@lupine.software
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,31 +18,34 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Monitoring
 Classifier: Typing :: Typed
 Requires-Dist: awslambdaric (>=2.0.10)
 Requires-Dist: boto3 (>=1.20.0)
 Requires-Dist: boto3-type-annotations (>=0.3.1)
-Requires-Dist: datadog-lambda (==5.91.0)
-Requires-Dist: ddtrace (==2.7.4)
+Requires-Dist: datadog-lambda
+Requires-Dist: ddtrace
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sentry-sdk (<2.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
+Project-URL: Documentation, https://safe-init.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/kalepa/safe-init
 Description-Content-Type: text/markdown
 
-# Safe Init
+# Safe Init: Simplifying AWS Lambda Error Handling and Monitoring
 
 [![PyPI version](https://badge.fury.io/py/safe-init.svg)](https://badge.fury.io/py/safe-init)
 [![Documentation Status](https://readthedocs.org/projects/safe-init/badge/?version=latest)](https://safe-init.readthedocs.io/en/latest/?badge=latest)
 [![Python versions](https://img.shields.io/pypi/pyversions/safe-init.svg)](https://pypi.org/project/safe-init/)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 Safe Init is a Python library that provides a comprehensive set of tools for initializing AWS Lambda functions safely and handling errors and exceptions gracefully. It is designed to make your Lambda functions more robust, easier to debug, and less prone to unexpected failures. With Safe Init, you can focus on writing your core Lambda function logic while the library takes care of error handling, logging, notifications, and more.
 
+[Read the Docs](https://safe-init.readthedocs.io/en/latest/) | [GitHub Repository](https://github.com/Kalepa/safe-init) | [PyPI Package](https://pypi.org/project/safe-init/) 
+
 ## Features
 
 ### Error Handling and Logging
 - **Error Handling**: Safe Init wraps your Lambda handler with robust error handling and logging, ensuring that any unhandled exceptions are captured and logged for easy debugging.
 - **Execution Time Tracing**: Traces the execution time of all function calls within the Lambda handler, helping you identify performance bottlenecks and optimize your code.
 
 ### Monitoring and Alerting
```

