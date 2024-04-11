# Comparing `tmp/chaturbate_poller-0.3.6.tar.gz` & `tmp/chaturbate_poller-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.3.6.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.3.7.tar", max compression
```

## Comparing `chaturbate_poller-0.3.6.tar` & `chaturbate_poller-0.3.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2024-04-10 21:12:06.650014 chaturbate_poller-0.3.6/LICENSE
--rw-r--r--   0        0        0     2692 2024-04-10 21:12:06.650014 chaturbate_poller-0.3.6/README.md
--rw-r--r--   0        0        0     3129 2024-04-10 21:12:17.306099 chaturbate_poller-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      573 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     3889 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      669 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     4017 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/format_messages.py
--rw-r--r--   0        0        0     2211 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     5578 2024-04-10 21:12:06.654013 chaturbate_poller-0.3.6/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-11 01:45:30.220776 chaturbate_poller-0.3.7/LICENSE
+-rw-r--r--   0        0        0     2692 2024-04-11 01:45:30.220776 chaturbate_poller-0.3.7/README.md
+-rw-r--r--   0        0        0     3129 2024-04-11 01:45:41.280784 chaturbate_poller-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      573 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     4027 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0      895 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     4017 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/format_messages.py
+-rw-r--r--   0        0        0     1564 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     5578 2024-04-11 01:45:30.224776 chaturbate_poller-0.3.7/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.7/PKG-INFO
```

### Comparing `chaturbate_poller-0.3.6/LICENSE` & `chaturbate_poller-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.6/README.md` & `chaturbate_poller-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.6/pyproject.toml` & `chaturbate_poller-0.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.3.6"
+version = "0.3.7"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.3.6/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.3.7/src/chaturbate_poller/__init__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.6/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.3.7/src/chaturbate_poller/chaturbate_poller.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from logging.config import dictConfig
 from types import TracebackType
 
 import backoff
 import httpx
 from httpx import HTTPStatusError, RequestError
 
-from chaturbate_poller.constants import BASE_URL, ERROR_RANGE_END, ERROR_RANGE_START
+from chaturbate_poller.constants import BASE_URL, HttpStatusCode
 from chaturbate_poller.logging_config import LOGGING_CONFIG
 from chaturbate_poller.models import EventsAPIResponse
 
 dictConfig(LOGGING_CONFIG)
 """Use the logging configuration from LOGGING_CONFIG."""
 
 logger = logging.getLogger(__name__)
@@ -119,9 +119,14 @@
         exception (Exception): The exception raised.
 
     Returns:
         bool: True if the request should be retried.
     """
     if isinstance(exception, HTTPStatusError):
         status_code = exception.response.status_code
-        return ERROR_RANGE_START <= status_code < ERROR_RANGE_END
+        return status_code in (
+            HttpStatusCode.INTERNAL_SERVER_ERROR,
+            HttpStatusCode.BAD_GATEWAY,
+            HttpStatusCode.SERVICE_UNAVAILABLE,
+            HttpStatusCode.GATEWAY_TIMEOUT,
+        )
     return False
```

### Comparing `chaturbate_poller-0.3.6/src/chaturbate_poller/format_messages.py` & `chaturbate_poller-0.3.7/src/chaturbate_poller/format_messages.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.6/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.3.7/src/chaturbate_poller/logging_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-"""Logging configuration for the Chaturbate poller."""
+"""Logging configuration for the application."""
 
 import logging
 
-CRITICAL_LEVEL = 50
-"""int: Custom level for CRITICAL events."""
-logging.addLevelName(CRITICAL_LEVEL, "CRITICAL")
-"""str: Name for the custom CRITICAL level."""
-
 
 class CustomFormatter(logging.Formatter):
-    """Custom formatter for including module and function names."""
+    """Custom log formatter.
+
+    Args:
+        logging.Formatter: The logging formatter class.
+    """
+
+    def format(self, record: logging.LogRecord) -> str:
+        """Format the log record.
 
-    def format(
-        self,
-        record: logging.LogRecord,
-    ) -> str:
-        """Format the log record."""
+        Args:
+            record (logging.LogRecord): The log record to format.
+
+        Returns:
+            str: The formatted log record.
+        """
         record.module = record.module.split(".")[-1]
-        record.funcName = record.funcName or ""
         return super().format(record)
 
 
 LOGGING_CONFIG = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
         "standard": {
-            "format": "%(message)s",
+            "format": "%(asctime)s - %(levelname)s - %(name)s - %(message)s",
             "datefmt": "%Y-%m-%d %H:%M:%S",
         },
         "detailed": {
             "()": CustomFormatter,
-            "format": "%(asctime)s - %(name)s - %(levelname)s - %(module)s - %(message)s",  # noqa: E501
+            "format": "%(asctime)s - %(levelname)s - %(name)s - %(module)s - %(funcName)s - %(message)s",  # noqa: E501
             "datefmt": "%Y-%m-%d %H:%M:%S",
         },
     },
     "handlers": {
         "console": {
             "class": "logging.StreamHandler",
             "formatter": "standard",
@@ -43,39 +45,16 @@
         },
         "file": {
             "class": "logging.handlers.TimedRotatingFileHandler",
             "filename": "app.log",
             "formatter": "detailed",
             "level": "DEBUG",
             "when": "midnight",
-            "backupCount": 7,
         },
     },
     "loggers": {
         "": {
             "handlers": ["console", "file"],
             "level": "INFO",
-            "propagate": True,
-        },
-        "chaturbate_poller": {
-            "handlers": ["file"],
-            "level": "INFO",
-            "propagate": False,
-        },
-        "httpx": {
-            "handlers": ["file"],
-            "level": "CRITICAL",
-            "propagate": False,
-        },
-        "httpcore": {
-            "handlers": ["file"],
-            "level": "CRITICAL",
-            "propagate": False,
-        },
-        "backoff": {
-            "handlers": ["file"],
-            "level": "CRITICAL",
-            "propagate": False,
         },
     },
 }
-"""dict: Logging configuration for the Chaturbate poller."""
```

### Comparing `chaturbate_poller-0.3.6/src/chaturbate_poller/models.py` & `chaturbate_poller-0.3.7/src/chaturbate_poller/models.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.6/PKG-INFO` & `chaturbate_poller-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.3.6
+Version: 0.3.7
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

