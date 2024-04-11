# Comparing `tmp/crawlee-0.0.1.tar.gz` & `tmp/crawlee-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.1.tar", max compression
+gzip compressed data, was "crawlee-0.0.2.tar", max compression
```

## Comparing `crawlee-0.0.1.tar` & `crawlee-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,65 @@
--rw-r--r--   0        0        0    11355 2024-01-15 10:43:27.602910 crawlee-0.0.1/LICENSE
--rw-r--r--   0        0        0       17 2024-01-14 07:30:15.307605 crawlee-0.0.1/README.md
--rw-r--r--   0        0        0     5313 2024-01-30 14:56:03.876980 crawlee-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-30 14:30:04.982947 crawlee-0.0.1/src/crawlee/__init__.py
--rw-r--r--   0        0        0       77 2024-01-29 07:45:35.113027 crawlee-0.0.1/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 10:09:02.893258 crawlee-0.0.1/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0     4198 2024-01-30 14:30:04.982947 crawlee-0.0.1/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0    10458 2024-01-30 14:30:04.982947 crawlee-0.0.1/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0       40 2024-01-30 10:12:23.385226 crawlee-0.0.1/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     6967 2024-01-30 10:12:18.710274 crawlee-0.0.1/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0        0 2024-01-30 10:09:02.909258 crawlee-0.0.1/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1245 2024-01-30 10:17:55.564860 crawlee-0.0.1/src/crawlee/events/types.py
--rw-r--r--   0        0        0     4802 2024-01-30 10:10:33.743337 crawlee-0.0.1/src/crawlee/log_config.py
--rw-r--r--   0        0        0        0 2024-01-30 10:09:02.909258 crawlee-0.0.1/src/crawlee/py.typed
--rw-r--r--   0        0        0      630 2024-01-30 14:30:04.982947 crawlee-0.0.1/src/crawlee/utils.py
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 crawlee-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-01-15 10:43:27.602910 crawlee-0.0.2/LICENSE
+-rw-r--r--   0        0        0       17 2024-01-14 07:30:15.307605 crawlee-0.0.2/README.md
+-rw-r--r--   0        0        0     5913 2024-04-11 07:59:00.206388 crawlee-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-18 16:55:10.812444 crawlee-0.0.2/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 15:21:38.269919 crawlee-0.0.2/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0     3341 2024-04-05 11:38:44.800791 crawlee-0.0.2/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-04-04 15:33:46.940733 crawlee-0.0.2/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3376 2024-04-04 15:33:46.940733 crawlee-0.0.2/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1950 2024-04-04 15:33:46.940733 crawlee-0.0.2/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     4668 2024-04-04 15:33:46.941733 crawlee-0.0.2/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     2056 2024-04-04 15:33:46.941733 crawlee-0.0.2/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-04-05 11:38:44.800791 crawlee-0.0.2/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-03-08 15:21:38.269919 crawlee-0.0.2/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0     1835 2024-03-08 15:28:15.522918 crawlee-0.0.2/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-04-04 15:33:46.941733 crawlee-0.0.2/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-04-05 11:38:44.800791 crawlee-0.0.2/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-03-08 15:21:38.270919 crawlee-0.0.2/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15881 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9174 2024-03-18 16:55:10.813444 crawlee-0.0.2/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      186 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    12621 2024-04-10 16:34:23.951009 crawlee-0.0.2/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     4026 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2279 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0      420 2024-04-10 16:02:45.061422 crawlee-0.0.2/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0     1245 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/configuration.py
+-rw-r--r--   0        0        0       91 2024-04-10 13:42:23.139187 crawlee-0.0.2/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7169 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     3004 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-03-08 15:21:38.271919 crawlee-0.0.2/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1264 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/events/types.py
+-rw-r--r--   0        0        0       38 2024-04-10 08:51:04.114008 crawlee-0.0.2/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     2481 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      261 2024-04-11 07:59:09.550307 crawlee-0.0.2/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-03-30 20:24:08.426839 crawlee-0.0.2/src/crawlee/log_config.py
+-rw-r--r--   0        0        0        0 2024-03-08 15:21:38.271919 crawlee-0.0.2/src/crawlee/py.typed
+-rw-r--r--   0        0        0     5512 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/request.py
+-rw-r--r--   0        0        0      365 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/resource_clients/__init__.py
+-rw-r--r--   0        0        0     5693 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/resource_clients/base_resource_client.py
+-rw-r--r--   0        0        0     3436 2024-04-05 13:50:29.284761 crawlee-0.0.2/src/crawlee/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0        0        0    19760 2024-04-05 13:50:29.284761 crawlee-0.0.2/src/crawlee/resource_clients/dataset_client.py
+-rw-r--r--   0        0        0     1545 2024-04-05 13:50:29.284761 crawlee-0.0.2/src/crawlee/resource_clients/dataset_collection_client.py
+-rw-r--r--   0        0        0    20509 2024-04-05 13:50:29.284761 crawlee-0.0.2/src/crawlee/resource_clients/key_value_store_client.py
+-rw-r--r--   0        0        0     1660 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/resource_clients/key_value_store_collection_client.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/resource_clients/py.typed
+-rw-r--r--   0        0        0    22531 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/resource_clients/request_queue_client.py
+-rw-r--r--   0        0        0     1635 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/resource_clients/request_queue_collection_client.py
+-rw-r--r--   0        0        0     1645 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      106 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/storage_clients/__init__.py
+-rw-r--r--   0        0        0     1577 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/storage_clients/base_storage_client.py
+-rw-r--r--   0        0        0    11486 2024-04-08 10:23:01.757507 crawlee-0.0.2/src/crawlee/storage_clients/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:50:29.285761 crawlee-0.0.2/src/crawlee/storage_clients/py.typed
+-rw-r--r--   0        0        0      150 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     7240 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15488 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     5123 2024-04-11 07:59:09.551307 crawlee-0.0.2/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0        0 2024-04-04 15:33:46.944733 crawlee-0.0.2/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2611 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2741 2024-04-10 08:51:04.115008 crawlee-0.0.2/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25804 2024-04-10 16:39:44.067022 crawlee-0.0.2/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0     3989 2024-04-10 08:51:04.116008 crawlee-0.0.2/src/crawlee/storages/types.py
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 crawlee-0.0.2/PKG-INFO
```

### Comparing `crawlee-0.0.1/LICENSE` & `crawlee-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.1/pyproject.toml` & `crawlee-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.1"
+version = "0.0.2"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://todo.com/"
-repository = "https://github.com/apify/crawlee-py"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -32,51 +30,66 @@
     "headless",
     "scraper",
     "scraping",
 ]
 
 [tool.poetry.urls]
 "Homepage" = "https://todo.com/"
-"Documentation" = "https://todo.com/"
-"Source" = "https://github.com/apify/crawlee-py"
-"Issue tracker" = "https://github.com/apify/crawlee-py/issues"
-"Changelog" = "https://github.com/apify/crawlee-py/blob/master/CHANGELOG.md"
 "Apify Homepage" = "https://apify.com"
+"Changelog" = "https://github.com/apify/crawlee-py/blob/master/CHANGELOG.md"
+"Documentation" = "https://todo.com/"
+"Issue Tracker" = "https://github.com/apify/crawlee-py/issues"
+"Repository" = "https://github.com/apify/crawlee-py"
 
-# We use inclusive ordered comparison clause for external packages intentionally in order to enhance the Crawlee's
+# We use inclusive ordered comparison clauses for external packages intentionally in order to enhance Crawlee's
 # compatibility with external packages. This decision was discussed in detail in the following PR:
 # https://github.com/apify/apify-sdk-python/pull/154.
 [tool.poetry.dependencies]
 python = "^3.9"
+aiofiles = "^23.2.1"
+aioshutil = "^1.3"
 colorama = "^0.4.6"
+docutils = "^0.20.1" # HACK - prevent poetry from resolving version to 0.21.post1 which does not exist
+eval-type-backport = "^0.1.3"
+httpx = "^0.27.0"
 more_itertools = "^10.2.0"
+psutil = "^5.9.8"
+pydantic = "^2.6.3"
+pydantic-settings = "^2.2.1"
 pyee = "^11.1.0"
+sortedcollections = "^2.1.0"
 typing-extensions = "^4.1.0"
 
 [tool.poetry.group.dev.dependencies]
-build = "~1.0.3"
+build = "~1.2.0"
 filelock = "~3.13.1"
-mypy = "~1.8.0"
-pre-commit = "~3.4.0"
+mypy = "~1.9.0"
+pre-commit = "~3.7.0"
 pydoc-markdown = "~4.8.2"
-pytest = "~7.4.4"
-pytest-asyncio = "~0.23.4"
-pytest-cov = "~4.1.0"
-pytest-only = "~2.0.0"
-pytest-timeout = "~2.2.0"
+pytest = "~8.1.0"
+pytest-asyncio = "~0.23.5"
+pytest-cov = "~5.0.0"
+pytest-only = "~2.1.0"
+pytest-timeout = "~2.3.0"
 pytest-xdist = "~3.5.0"
-respx = "~0.20.1"
-ruff = "~0.1.13"
-twine = "~4.0.2"
+respx = "~0.21.0"
+ruff = "~0.3.0"
+twine = "~5.0.0"
+types-aiofiles = "^23.2.0.20240106"
 types-colorama = "~0.4.15.20240106"
+types-psutil = "~5.9.5.20240205"
 
 [tool.ruff]
 line-length = 120
+
+[tool.ruff.lint]
 select = ["ALL"]
 ignore = [
+    "ANN101",  # Missing type annotation for `{name}` in method
+    "ANN102",  # Missing type annotation for `{name}` in classmethod
     "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in {filename}
     "BLE001",  # Do not catch blind exception
     "C901",    # `{name}` is too complex
     "COM812",  # This rule may cause conflicts when used with the formatter
     "D100",    # Missing docstring in public module
     "D104",    # Missing docstring in public package
     "D107",    # Missing docstring in `__init__`
@@ -116,26 +129,34 @@
     "T20",     # flake8-print
 ]
 "**/{tests}/*" = [
     "D",       # Everything from the pydocstyle
     "INP001",  # File {filename} is part of an implicit namespace package, add an __init__.py
     "PLR2004", # Magic value used in comparison, consider replacing {value} with a constant variable
     "S101",    # Use of assert detected
+    "SLF001",  # Private member accessed: `{name}`
     "T20",     # flake8-print
     "TRY301",  # Abstract `raise` to an inner function
 ]
 
 [tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 inline-quotes = "single"
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.pytest]
+[tool.ruff.lint.isort]
+known-local-folder = ["crawlee"]
+
+[tool.ruff.lint.pylint]
+max-branches = 18
+
+[tool.pytest.ini_options]
+addopts = "-ra"
 asyncio_mode = "auto"
 timeout = 1200
 
 [tool.mypy]
 python_version = "3.9"
 files = ["scripts", "src", "tests"]
 check_untyped_defs = true
```

### Comparing `crawlee-0.0.1/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.2/src/crawlee/autoscaling/system_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,237 +1,199 @@
+# Inspiration: https://github.com/apify/crawlee/blob/v3.7.3/packages/core/src/autoscaling/system_status.ts
+
 from __future__ import annotations
 
-from dataclasses import dataclass
+from datetime import timedelta
 from logging import getLogger
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING
 
 from more_itertools import pairwise
 
-from crawlee.utils import weighted_avg
+from crawlee._utils.math import compute_weighted_avg
+from crawlee.autoscaling.types import LoadRatioInfo, Snapshot, SystemInfo
 
 if TYPE_CHECKING:
-    from datetime import datetime
-
-    from crawlee.autoscaling.snapshotter import Snapshot, Snapshotter
+    from crawlee.autoscaling.snapshotter import Snapshotter
 
 logger = getLogger(__name__)
 
 
-@dataclass
-class LoadRatioInfo:
-    """Represents the load ratio of a resource."""
-
-    is_overloaded: bool
-    limit_ratio: float
-    actual_ratio: float
-
-
-@dataclass
-class SystemInfo:
-    """Represents the current status of the system."""
-
-    is_system_idle: bool  # Indicates whether the system is currently idle or overloaded
-    mem_info: LoadRatioInfo
-    event_loop_info: LoadRatioInfo
-    cpu_info: LoadRatioInfo
-    client_info: LoadRatioInfo
-    mem_current_bytes: int | None = None  # Platform only property
-    cpu_current_usage: int | None = None  # Platform only property
-    is_cpu_overloaded: bool | None = None  # Platform only property
-    created_at: datetime | None = None
-
-
-@dataclass
-class FinalStatistics:
-    """Represents final statistics."""
-
-    requests_finished: int
-    requests_failed: int
-    retry_histogram: list[int]
-    request_avg_failed_duration_millis: float
-    request_avg_finished_duration_millis: float
-    requests_finished_per_minute: float
-    requests_failed_per_minute: float
-    request_total_duration_millis: float
-    requests_total: int
-    crawler_runtime_millis: float
-
-
 class SystemStatus:
-    """Provides a simple interface to reading system status from a `Snapshotter` instance.
-
-    It only exposes two functions `SystemStatus.get_current_status` and `SystemStatus.get_historical_status`.
-    The system status is calculated using a weighted average of overloaded messages in the snapshots, with the weights
-    being the time intervals between the snapshots. Each resource is calculated separately, and the system
-    is overloaded whenever at least one resource is overloaded. The class is used by the `AutoscaledPool` class.
+    """Provides a simple interface for evaluating system resource usage from snapshots collected by `Snapshotter`.
 
-    `SystemStatus.get_current_status` returns a boolean that represents the current status of the system. The length
-    of the current timeframe in seconds is configurable by the `currentHistorySecs` option and represents the max age
-    of snapshots to be considered for the calculation.
+    This class aggregates and interprets snapshots from a Snapshotter instance to evaluate the current and historical
+    status of system resources like CPU, memory, event loop, and client API usage. It exposes two methods
+    `get_current_system_info` and `get_historical_system_info`. The system information is computed using a weighted
+    average of overloaded messages in the snapshots, with the weights being the time intervals between the snapshots.
+    Each resource is computed separately, and the system is considered as overloaded whenever at least one resource
+    is overloaded.
+
+    `get_current_system_info` returns a `SystemInfo` data structure that represents the current status
+    of the system. The length of the current timeframe in seconds is configurable by the `max_snapshot_age` option
+    and represents the max age of snapshots to be considered for the computation.
 
-    `SystemStatus.get_historical_status` returns a boolean that represents the long-term status of the system. It
-    considers the full snapshot history available in the `Snapshotter` instance.
+    `SystemStatus.get_historical_system_info` returns a `SystemInfo` that represents the long-term status of the system.
+    It considers the full snapshot history available in the `Snapshotter` instance.
+    """
 
-    Attributes:
-        snapshotter: The `Snapshotter` instance to be queried for `SystemStatus`.
+    def __init__(
+        self,
+        snapshotter: Snapshotter,
+        *,
+        max_snapshot_age: timedelta = timedelta(seconds=5),
+        cpu_overload_threshold: float = 0.4,
+        memory_overload_threshold: float = 0.2,
+        event_loop_overload_threshold: float = 0.6,
+        client_overload_threshold: float = 0.3,
+    ) -> None:
+        """Creates a new instance.
 
-        current_history_secs: Defines max age of snapshots used in the `SystemStatus.get_current_status` measurement.
+        Args:
+            snapshotter: The `Snapshotter` instance to be queried for `SystemStatus`.
 
-        max_memory_overloaded_ratio: Sets the maximum ratio of overloaded snapshots in a memory sample.
-            If the sample exceeds this ratio, the system will be overloaded.
+            max_snapshot_age: Defines max age of snapshots used in the `SystemStatus.get_current_system_info`
+                measurement.
 
-        max_event_loop_overloaded_ratio: Sets the maximum ratio of overloaded snapshots in an event loop sample.
-            If the sample exceeds this ratio, the system will be overloaded.
+            cpu_overload_threshold: Sets the threshold of overloaded snapshots in the CPU sample.
+                If the sample exceeds this threshold, the system will be considered overloaded.
 
-        max_cpu_overloaded_ratio: Sets the maximum ratio of overloaded snapshots in a CPU sample. If the sample
-            exceeds this ratio, the system will be overloaded.
+            memory_overload_threshold: Sets the threshold of overloaded snapshots in the memory sample.
+                If the sample exceeds this threshold, the system will be considered overloaded.
 
-        max_client_overloaded_ratio: Sets the maximum ratio of overloaded snapshots in a Client sample.
-            If the sample exceeds this ratio, the system will be overloaded.
-    """
+            event_loop_overload_threshold: Sets the threshold of overloaded snapshots in the event loop sample.
+                If the sample exceeds this threshold, the system will be considered overloaded.
 
-    def __init__(
-        self: SystemStatus,
-        snapshotter: Snapshotter,
-        current_history_secs: int = 5,
-        max_memory_overloaded_ratio: float = 0.2,
-        max_event_loop_overloaded_ratio: float = 0.6,
-        max_cpu_overloaded_ratio: float = 0.4,
-        max_client_overloaded_ratio: float = 0.3,
-    ) -> None:
-        self.snapshotter = snapshotter
-        self.current_history_secs = current_history_secs
-        self.max_memory_overloaded_ratio = max_memory_overloaded_ratio
-        self.max_event_loop_overloaded_ratio = max_event_loop_overloaded_ratio
-        self.max_cpu_overloaded_ratio = max_cpu_overloaded_ratio
-        self.max_client_overloaded_ratio = max_client_overloaded_ratio
+            client_overload_threshold: Sets the threshold of overloaded snapshots in the Client sample.
+                If the sample exceeds this threshold, the system will be considered overloaded.
+        """
+        self._snapshotter = snapshotter
+        self._max_snapshot_age = max_snapshot_age
+        self._cpu_overload_threshold = cpu_overload_threshold
+        self._memory_overload_threshold = memory_overload_threshold
+        self._event_loop_overload_threshold = event_loop_overload_threshold
+        self._client_overload_threshold = client_overload_threshold
 
-    def get_current_status(self: SystemStatus) -> SystemInfo:
-        """Get the current system status.
+    def get_current_system_info(self) -> SystemInfo:
+        """Retrieves and evaluates the current status of system resources.
 
-        Returns a `SystemInfo` object where the `is_system_idle` property is `False` if the system has been overloaded
-        in the last `current_history_secs` seconds, and `True` otherwise.
+        Considers snapshots within the `_max_snapshot_age` timeframe and determines if the system is currently
+        overloaded based on predefined thresholds for each resource type.
 
         Returns:
             An object representing the current system status.
         """
-        return self._is_system_idle(self.current_history_secs)
+        return self._get_system_info(self._max_snapshot_age)
 
-    def get_historical_status(self: SystemStatus) -> SystemInfo:
-        """Get the historical system status.
+    def get_historical_system_info(self) -> SystemInfo:
+        """Retrieves and evaluates the historical status of system resources.
 
-        Returns a `SystemInfo` where the `is_system_idle` property is set to `False` if the system has been overloaded
-        in the full history of the `Snapshotter` (which is configurable in the `Snapshotter`, and `True` otherwise.
+        Considers the entire history of snapshots from the Snapshotter to assess long-term system performance and
+        determines if the system has been historically overloaded.
 
         Returns:
             An object representing the historical system status.
         """
-        return self._is_system_idle()
+        return self._get_system_info()
 
-    def _is_system_idle(self: SystemStatus, sample_duration_millis: int | None = None) -> SystemInfo:
-        """Determine if the system is currently idle or overloaded.
+    def _get_system_info(self, sample_duration: timedelta | None = None) -> SystemInfo:
+        """Get system information based on the overload state of different resources within a specified duration.
 
         Args:
-            sample_duration_millis: The duration (in milliseconds) within which to analyze system status.
+            sample_duration: Specific duration for which to evaluate the system status. If None, evaluates across
+                the entire history available in the snapshotter.
 
         Returns:
-            An object representing the system status with an `is_system_idle` property set to `True` if the system
-            has not been overloaded within the specified time duration, and `False` otherwise.
+            Aggregated system status indicating whether the system is idle or overloaded.
         """
-        mem_info = self._is_memory_overloaded(sample_duration_millis)
-        event_loop_info = self._is_event_loop_overloaded(sample_duration_millis)
-        cpu_info = self._is_cpu_overloaded(sample_duration_millis)
-        client_info = self._is_client_overloaded(sample_duration_millis)
+        mem_info = self._is_memory_overloaded(sample_duration)
+        event_loop_info = self._is_event_loop_overloaded(sample_duration)
+        cpu_info = self._is_cpu_overloaded(sample_duration)
+        client_info = self._is_client_overloaded(sample_duration)
 
         return SystemInfo(
-            is_system_idle=(
-                not mem_info.is_overloaded
-                and not event_loop_info.is_overloaded
-                and not cpu_info.is_overloaded
-                and not client_info.is_overloaded
-            ),
-            mem_info=mem_info,
+            memory_info=mem_info,
             event_loop_info=event_loop_info,
             cpu_info=cpu_info,
             client_info=client_info,
         )
 
-    def _is_memory_overloaded(self: SystemStatus, sample_duration_millis: int | None = None) -> LoadRatioInfo:
-        """Determine if memory has been overloaded within a specified time duration.
+    def _is_cpu_overloaded(self, sample_duration: timedelta | None = None) -> LoadRatioInfo:
+        """Determine if the CPU has been overloaded within a specified time duration.
 
         Args:
-            sample_duration_millis: The duration (in milliseconds) within which to analyze memory snapshots.
+            sample_duration: The duration within which to analyze CPU snapshots. If None, evaluates across
+                the entire history available in the snapshotter.
 
         Returns:
-            An object with an `is_overloaded` property set to `True` if memory has been overloaded within the specified
-            time duration. Otherwise, `is_overloaded` is set to `False`.
+            CPU load ratio information.
         """
-        sample = self.snapshotter.get_memory_sample(sample_duration_millis)
-        return self._is_sample_overloaded(sample, self.max_memory_overloaded_ratio)
+        sample = self._snapshotter.get_cpu_sample(sample_duration)
+        return self._is_sample_overloaded(sample, self._cpu_overload_threshold)
 
-    def _is_event_loop_overloaded(self: SystemStatus, sample_duration_millis: int | None = None) -> LoadRatioInfo:
-        """Determine if the event loop has been overloaded within a specified time duration.
+    def _is_memory_overloaded(self, sample_duration: timedelta | None = None) -> LoadRatioInfo:
+        """Determine if memory has been overloaded within a specified time duration.
 
         Args:
-            sample_duration_millis: The duration (in milliseconds) within which to analyze event loop snapshots.
+            sample_duration: The duration within which to analyze memory snapshots. If None, evaluates across
+                the entire history available in the snapshotter.
 
         Returns:
-            An object with an `is_overloaded` property set to `True` if the event loop has been overloaded within
-            the specified time duration. Otherwise, `is_overloaded` is set to `False`.
+            Memory load ratio information.
         """
-        sample = self.snapshotter.get_event_loop_sample(sample_duration_millis)
-        return self._is_sample_overloaded(sample, self.max_event_loop_overloaded_ratio)
+        sample = self._snapshotter.get_memory_sample(sample_duration)
+        return self._is_sample_overloaded(sample, self._memory_overload_threshold)
 
-    def _is_cpu_overloaded(self: SystemStatus, sample_duration_millis: int | None = None) -> LoadRatioInfo:
-        """Determine if the CPU has been overloaded within a specified time duration.
+    def _is_event_loop_overloaded(self, sample_duration: timedelta | None = None) -> LoadRatioInfo:
+        """Determine if the event loop has been overloaded within a specified time duration.
 
         Args:
-            sample_duration_millis: The duration (in milliseconds) within which to analyze CPU snapshots.
+            sample_duration: The duration within which to analyze event loop snapshots. If None, evaluates across
+                the entire history available in the snapshotter.
 
         Returns:
-            An object with an `is_overloaded` property set to `True` if the CPU has been overloaded within
-            the specified time duration. Otherwise, `is_overloaded` is set to `False`.
+            Event loop load ratio information.
         """
-        sample = self.snapshotter.get_cpu_sample(sample_duration_millis)
-        return self._is_sample_overloaded(sample, self.max_cpu_overloaded_ratio)
+        sample = self._snapshotter.get_event_loop_sample(sample_duration)
+        return self._is_sample_overloaded(sample, self._event_loop_overload_threshold)
 
-    def _is_client_overloaded(self: SystemStatus, sample_duration_millis: int | None = None) -> LoadRatioInfo:
+    def _is_client_overloaded(self, sample_duration: timedelta | None = None) -> LoadRatioInfo:
         """Determine if the client has been overloaded within a specified time duration.
 
         Args:
-            sample_duration_millis: The duration (in milliseconds) within which to analyze client snapshots.
+            sample_duration: The duration within which to analyze client snapshots. If None, evaluates across
+                the entire history available in the snapshotter.
 
         Returns:
-            An object with an `is_overloaded` property set to `True` if the client has been overloaded within
-            the specified time duration. Otherwise, `is_overloaded` is set to `False`.
+            Client load ratio information.
         """
-        sample = self.snapshotter.get_client_sample(sample_duration_millis)
-        return self._is_sample_overloaded(sample, self.max_client_overloaded_ratio)
+        sample = self._snapshotter.get_client_sample(sample_duration)
+        return self._is_sample_overloaded(sample, self._client_overload_threshold)
 
-    def _is_sample_overloaded(self: SystemStatus, sample: Sequence[Snapshot], ratio: float) -> LoadRatioInfo:
+    def _is_sample_overloaded(self, sample: list[Snapshot], threshold: float) -> LoadRatioInfo:
         """Determine if a sample of snapshot data is overloaded based on a specified ratio.
 
         Args:
-            sample: A sequence of snapshot data to analyze.
-            ratio: The ratio threshold to consider the sample as overloaded.
+            sample: A list of snapshot data to analyze.
+            threshold: The threshold ratio to use for determining if the sample is overloaded.
 
         Returns:
             An object with an `is_overloaded` property set to `True` if the sample is considered overloaded based
-            on the specified ratio. Otherwise, `is_overloaded` is set to `False`.
+            on the specified threshold ratio. Otherwise, `is_overloaded` is set to `False`.
         """
         if not sample:
-            return LoadRatioInfo(is_overloaded=False, limit_ratio=ratio, actual_ratio=0)
+            return LoadRatioInfo(limit_ratio=threshold, actual_ratio=0)
 
         weights, values = [], []
 
         for previous, current in pairwise(sample):
             weight = (current.created_at - previous.created_at).total_seconds() or 0.001  # Avoid zero
+            value = float(current.is_overloaded)
             weights.append(weight)
-            values.append(float(current.is_overloaded))
+            values.append(value)
 
-        w_avg = values[0] if len(sample) == 1 else weighted_avg(values, weights)
+        try:
+            weighted_avg = compute_weighted_avg(values, weights)
+        except ValueError:
+            logger.warning('Total weight cannot be zero')
+            return LoadRatioInfo(limit_ratio=threshold, actual_ratio=0)
 
-        return LoadRatioInfo(
-            is_overloaded=w_avg > ratio,
-            limit_ratio=ratio,
-            actual_ratio=round(w_avg, 3),
-        )
+        return LoadRatioInfo(limit_ratio=threshold, actual_ratio=round(weighted_avg, 3))
```

### Comparing `crawlee-0.0.1/src/crawlee/events/event_manager.py` & `crawlee-0.0.2/src/crawlee/events/event_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+# Inspiration: https://github.com/apify/crawlee/blob/v3.7.3/packages/core/src/events/event_manager.ts
+
 from __future__ import annotations
 
 import asyncio
 from collections import defaultdict
 from contextlib import suppress
 from functools import wraps
-from inspect import iscoroutinefunction
 from logging import getLogger
 from typing import TYPE_CHECKING
 
 from pyee.asyncio import AsyncIOEventEmitter
 
 if TYPE_CHECKING:
     from datetime import timedelta
@@ -19,122 +20,124 @@
 
 
 class EventManager:
     """Event manager for registering, emitting, and managing event listeners.
 
     Event manager allows you to register event listeners, emit events, and wait for event listeners to complete
     their execution. It is built on top of the `pyee.asyncio.AsyncIOEventEmitter` class.
-
-    Attributes:
-        _event_emitter: The event emitter which is used to emit events and call the event listeners.
-
-        _listener_tasks: The set of asyncio tasks which are currently executing the event listeners.
-
-        _listeners_to_wrappers: The mapping between events and listeners, and the wrapped listeners which are
-            registered with the event emitter.
     """
 
-    def __init__(self: EventManager) -> None:
-        logger.debug('Calling LocalEventManager.__init__()...')
+    def __init__(self) -> None:
+        logger.debug('Calling EventManager.__init__()...')
+
+        # Asynchronous event emitter for handle events and invoke the event listeners.
         self._event_emitter = AsyncIOEventEmitter()
 
-        # Listeners are wrapped in a asyncio.Task, store their references here so that we can wait for them to finish
+        # Listeners are wrapped inside asyncio.Task. Store their references here so that we can wait for them to finish.
         self._listener_tasks: set[asyncio.Task] = set()
 
-        # Store the mapping between events and listeners like this:
+        # Store the mapping between events, listeners and their wrappers in the following way:
         #   event -> listener -> [wrapped_listener_1, wrapped_listener_2, ...]
         self._listeners_to_wrappers: dict[Event, dict[Listener, list[WrappedListener]]] = defaultdict(
             lambda: defaultdict(list),
         )
 
-    async def close(self: EventManager, *, timeout: timedelta | None = None) -> None:
-        """Close the event manager.
-
-        This will stop listening for the events, and it will wait for all the event listeners to finish.
-
-        Args:
-            timeout: Optional timeout after which the pending event listeners are canceled.
-        """
-        logger.debug('Calling LocalEventManager.close()...')
-        await self.wait_for_all_listeners_to_complete(timeout=timeout)
-        self._event_emitter.remove_all_listeners()
-
-    def on(self: EventManager, *, event: Event, listener: Listener) -> None:
+    def on(self, *, event: Event, listener: Listener) -> None:
         """Add an event listener to the event manager.
 
         Args:
             event: The Actor event for which to listen to.
             listener: The function (sync or async) which is to be called when the event is emitted.
         """
-        logger.debug('Calling LocalEventManager.on()...')
+        logger.debug('Calling EventManager.on()...')
 
         @wraps(listener)
         async def listener_wrapper(event_data: EventData) -> None:
-            logger.debug('Calling LocalEventManager.on.listener_wrapper()...')
+            logger.debug('Calling EventManager.on.listener_wrapper()...')
 
             # If the listener is a coroutine function, just call it, otherwise, run it in a separate thread
             # to avoid blocking the event loop
-            coroutine = (
-                listener(event_data) if iscoroutinefunction(listener) else asyncio.to_thread(listener, event_data)
+            coro = (
+                listener(event_data)
+                if asyncio.iscoroutinefunction(listener)
+                else asyncio.to_thread(listener, event_data)
             )
+            # Note: use `asyncio.iscoroutinefunction` rather then `inspect.iscoroutinefunction` since it works with
+            # unittests.mock.AsyncMock. See https://github.com/python/cpython/issues/84753.
 
-            listener_task = asyncio.create_task(coroutine, name=f'Task-{event.value}-{listener.__name__}')
+            listener_task = asyncio.create_task(coro, name=f'Task-{event.value}-{listener.__name__}')
             self._listener_tasks.add(listener_task)
 
             try:
+                logger.debug('LocalEventManager.on.listener_wrapper(): Awaiting listener task...')
                 await listener_task
+                logger.debug('LocalEventManager.on.listener_wrapper(): Listener task completed.')
             except Exception:
                 # We need to swallow the exception and just log it here, otherwise it could break the event emitter
                 logger.exception(
                     'Exception in the event listener',
                     extra={'event_name': event.value, 'listener_name': listener.__name__},
                 )
             finally:
                 logger.debug('LocalEventManager.on.listener_wrapper(): Removing listener task from the set...')
                 self._listener_tasks.remove(listener_task)
 
         self._listeners_to_wrappers[event][listener].append(listener_wrapper)
         self._event_emitter.add_listener(event.value, listener_wrapper)
 
-    def off(self: EventManager, *, event: Event, listener: Listener | None = None) -> None:
+    def off(self, *, event: Event, listener: Listener | None = None) -> None:
         """Remove a listener, or all listeners, from an Actor event.
 
         Args:
             event: The Actor event for which to remove listeners.
             listener: The listener which is supposed to be removed. If not passed, all listeners of this event
                 are removed.
         """
-        logger.debug('Calling LocalEventManager.off()...')
+        logger.debug('Calling EventManager.off()...')
 
         if listener:
             for listener_wrapper in self._listeners_to_wrappers[event][listener]:
                 self._event_emitter.remove_listener(event.value, listener_wrapper)
             self._listeners_to_wrappers[event][listener] = []
         else:
             self._listeners_to_wrappers[event] = defaultdict(list)
             self._event_emitter.remove_all_listeners(event.value)
 
-    def emit(self: EventManager, *, event: Event, event_data: EventData) -> None:
+    def emit(self, *, event: Event, event_data: EventData) -> None:
         """Emit an event.
 
         Args:
             event: The event which will be emitted.
             event_data: The data which will be passed to the event listeners.
         """
-        logger.debug('Calling LocalEventManager.emit()...')
+        logger.debug('Calling EventManager.emit()...')
         self._event_emitter.emit(event.value, event_data)
 
-    async def wait_for_all_listeners_to_complete(self: EventManager, *, timeout: timedelta | None = None) -> None:
+    async def close(self, *, timeout: timedelta | None = None) -> None:
+        """Close the event manager.
+
+        This will stop listening for the events, and it will wait for all the event listeners to finish.
+
+        Args:
+            timeout: Optional timeout after which the pending event listeners are canceled.
+        """
+        logger.debug('Calling EventManager.close()...')
+        await self._wait_for_all_listeners_to_complete(timeout=timeout)
+        self._event_emitter.remove_all_listeners()
+        self._listener_tasks.clear()
+        self._listeners_to_wrappers.clear()
+
+    async def _wait_for_all_listeners_to_complete(self, *, timeout: timedelta | None = None) -> None:
         """Wait for all currently executing event listeners to complete.
 
         Args:
             timeout: The maximum time to wait for the event listeners to finish. If they do not complete within
                 the specified timeout, they will be canceled.
         """
-        logger.debug('Calling LocalEventManager.wait_for_all_listeners_to_complete()...')
+        logger.debug('Calling EventManager.wait_for_all_listeners_to_complete()...')
 
         async def wait_for_listeners() -> None:
             """Gathers all listener tasks and awaits their completion, logging any exceptions encountered."""
             results = await asyncio.gather(*self._listener_tasks, return_exceptions=True)
             for result in results:
                 if isinstance(result, Exception):
                     logger.exception('Event listener raised an exception.', exc_info=result)
```

### Comparing `crawlee-0.0.1/src/crawlee/events/types.py` & `crawlee-0.0.2/src/crawlee/events/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import Callable, Coroutine
 from dataclasses import dataclass
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Union
 
 if TYPE_CHECKING:
-    from crawlee.autoscaling.system_status import SystemInfo
+    from crawlee._utils.system import CpuInfo, MemoryInfo
 
 
 class Event(Enum):
     """Enum of all possible events that can be emitted."""
 
     PERSIST_STATE = 'persistState'
     SYSTEM_INFO = 'systemInfo'
@@ -26,15 +26,16 @@
     is_migrating: bool
 
 
 @dataclass
 class EventSystemInfoData:
     """Data for the system info event."""
 
-    system_info: SystemInfo
+    cpu_info: CpuInfo
+    memory_info: MemoryInfo
 
 
 @dataclass
 class EventMigratingData:
     """Data for the migrating event."""
```

### Comparing `crawlee-0.0.1/src/crawlee/log_config.py` & `crawlee-0.0.2/src/crawlee/log_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,38 +44,38 @@
     # The fields that are added to the log record with `logger.log(..., extra={...})` are just merged in the log record
     # with the other log record properties, and you can't get them in some nice, isolated way. So, to get the extra
     # fields, we just compare all the properties present in the log record with properties present in an empty log
     # record, and extract all the extra ones not present in the empty log record.
     empty_record = logging.LogRecord('dummy', 0, 'dummy', 0, 'dummy', None, None)
 
     def __init__(
-        self: CrawleeLogFormatter,
-        include_logger_name: bool = False,  # noqa: FBT001, FBT002
+        self,
+        include_logger_name: bool = True,  # noqa: FBT001, FBT002
         *args: Any,
         **kwargs: Any,
     ) -> None:
         """Create a new instance.
 
         Args:
-            include_logger_name: Include logger name at the beginning of the log line. Defaults to False.
+            include_logger_name: Include logger name at the beginning of the log line.
             args: Arguments passed to the parent class.
             kwargs: Keyword arguments passed to the parent class.
         """
         super().__init__(*args, **kwargs)
         self.include_logger_name = include_logger_name
 
-    def _get_extra_fields(self: CrawleeLogFormatter, record: logging.LogRecord) -> dict[str, Any]:
+    def _get_extra_fields(self, record: logging.LogRecord) -> dict[str, Any]:
         extra_fields: dict[str, Any] = {}
         for key, value in record.__dict__.items():
             if key not in self.empty_record.__dict__:
                 extra_fields[key] = value
 
         return extra_fields
 
-    def format(self: CrawleeLogFormatter, record: logging.LogRecord) -> str:
+    def format(self, record: logging.LogRecord) -> str:
         """Format the log record nicely.
 
         This formats the log record so that it:
             - starts with the level (colorized, and padded to 5 chars so that it is nicely aligned)
             - then has the actual log message, if it's multiline then it's nicely indented
             - then has the stringified extra log fields
             - then, if an exception is a part of the log record, prints the formatted exception.
```

### Comparing `crawlee-0.0.1/PKG-INFO` & `crawlee-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.1
+Version: 0.0.2
 Summary: Crawlee for Python
-Home-page: https://todo.com/
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
+Requires-Dist: aioshutil (>=1.3,<2.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: docutils (>=0.20.1,<0.21.0)
+Requires-Dist: eval-type-backport (>=0.1.3,<0.2.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: more_itertools (>=10.2.0,<11.0.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
+Requires-Dist: pydantic (>=2.6.3,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pyee (>=11.1.0,<12.0.0)
+Requires-Dist: sortedcollections (>=2.1.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
 Project-URL: Apify Homepage, https://apify.com
 Project-URL: Changelog, https://github.com/apify/crawlee-py/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://todo.com/
-Project-URL: Issue tracker, https://github.com/apify/crawlee-py/issues
+Project-URL: Homepage, https://todo.com/
+Project-URL: Issue Tracker, https://github.com/apify/crawlee-py/issues
 Project-URL: Repository, https://github.com/apify/crawlee-py
-Project-URL: Source, https://github.com/apify/crawlee-py
 Description-Content-Type: text/markdown
 
 # Crawlee Python
```

