# Comparing `tmp/logfire-0.23.0.tar.gz` & `tmp/logfire-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfire-0.23.0.tar", max compression
+gzip compressed data, was "logfire-0.24.0.tar", max compression
```

## Comparing `logfire-0.23.0.tar` & `logfire-0.24.0.tar`

### file list

```diff
@@ -1,51 +1,55 @@
--rw-r--r--   0        0        0     1099 2024-03-25 15:35:47.637876 logfire-0.23.0/LICENSE
--rw-r--r--   0        0        0      111 2024-03-25 15:35:47.637876 logfire-0.23.0/README.md
--rw-r--r--   0        0        0     2348 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/__init__.py
--rw-r--r--   0        0        0       95 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/__main__.py
--rw-r--r--   0        0        0     4250 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_ast_utils.py
--rw-r--r--   0        0        0     4066 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_async.py
--rw-r--r--   0        0        0     3527 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_auth.py
--rw-r--r--   0        0        0     2954 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_auto_trace/__init__.py
--rw-r--r--   0        0        0     4595 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_auto_trace/import_hook.py
--rw-r--r--   0        0        0     6469 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_auto_trace/types.py
--rw-r--r--   0        0        0      578 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_collect_system_info.py
--rw-r--r--   0        0        0    53657 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_config.py
--rw-r--r--   0        0        0     8998 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_config_params.py
--rw-r--r--   0        0        0     4540 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_constants.py
--rw-r--r--   0        0        0     5704 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_formatter.py
--rw-r--r--   0        0        0     5732 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_instrument.py
--rw-r--r--   0        0        0     8422 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_json_encoder.py
--rw-r--r--   0        0        0    11648 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_json_formatter.py
--rw-r--r--   0        0        0    12342 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_json_schema.py
--rw-r--r--   0        0        0     2753 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_json_types.py
--rw-r--r--   0        0        0      313 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_limits.py
--rw-r--r--   0        0        0    47391 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_main.py
--rw-r--r--   0        0        0    12233 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_metrics.py
--rw-r--r--   0        0        0     8608 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_scrubbing.py
--rw-r--r--   0        0        0     2007 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_stack_info.py
--rw-r--r--   0        0        0    10587 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_tracer.py
--rw-r--r--   0        0        0     5852 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/_utils.py
--rw-r--r--   0        0        0     9083 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/backfill.py
--rw-r--r--   0        0        0    15925 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exceptions.py
--rw-r--r--   0        0        0       38 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exporters/__init__.py
--rw-r--r--   0        0        0     1041 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exporters/_fallback.py
--rw-r--r--   0        0        0     7438 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exporters/_file.py
--rw-r--r--   0        0        0     4066 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exporters/_otlp.py
--rw-r--r--   0        0        0     6979 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exporters/_processor_wrapper.py
--rw-r--r--   0        0        0     1812 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exporters/_remove_pending.py
--rw-r--r--   0        0        0      691 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exporters/_wrapper.py
--rw-r--r--   0        0        0    17080 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/exporters/console.py
--rw-r--r--   0        0        0       32 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     2666 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/integrations/_executors.py
--rw-r--r--   0        0        0     9420 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/integrations/_fastapi.py
--rw-r--r--   0        0        0     2261 2024-03-25 15:35:47.665876 logfire-0.23.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0    16385 2024-03-25 15:35:47.669876 logfire-0.23.0/logfire/integrations/pydantic_plugin.py
--rw-r--r--   0        0        0     1379 2024-03-25 15:35:47.669876 logfire-0.23.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0     2327 2024-03-25 15:35:47.669876 logfire-0.23.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2024-03-25 15:35:47.669876 logfire-0.23.0/logfire/py.typed
--rw-r--r--   0        0        0    10165 2024-03-25 15:35:47.669876 logfire-0.23.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2024-03-25 15:35:47.669876 logfire-0.23.0/logfire/version.py
--rw-r--r--   0        0        0     5216 2024-03-25 15:35:47.669876 logfire-0.23.0/pyproject.toml
--rw-r--r--   0        0        0     3865 1970-01-01 00:00:00.000000 logfire-0.23.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-04-11 13:44:34.633989 logfire-0.24.0/LICENSE
+-rw-r--r--   0        0        0      111 2024-04-11 13:44:34.633989 logfire-0.24.0/README.md
+-rw-r--r--   0        0        0     2787 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/__main__.py
+-rw-r--r--   0        0        0      183 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4247 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     2946 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6456 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0     9110 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    16459 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      570 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    54145 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0     8997 2024-04-11 13:44:34.657989 logfire-0.24.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     4535 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0       38 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    17141 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     6958 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0     5680 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0       46 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0     2634 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0     9435 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0     7732 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    12089 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0      313 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/limits.py
+-rw-r--r--   0        0        0    47334 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    12850 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8603 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     2007 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10566 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     5852 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0       53 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/exceptions.py
+-rw-r--r--   0        0        0       99 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     3718 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3242 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    16134 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1388 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0     2327 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/py.typed
+-rw-r--r--   0        0        0    10606 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2024-04-11 13:44:34.661989 logfire-0.24.0/logfire/version.py
+-rw-r--r--   0        0        0     5267 2024-04-11 13:44:34.661989 logfire-0.24.0/pyproject.toml
+-rw-r--r--   0        0        0     3905 1970-01-01 00:00:00.000000 logfire-0.24.0/PKG-INFO
```

### Comparing `logfire-0.23.0/LICENSE` & `logfire-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.23.0/logfire/__init__.py` & `logfire-0.24.0/logfire/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """**Logfire** is the observability tool focused on developer experience."""
+from __future__ import annotations
 
-from ._auto_trace import AutoTraceModule
-from ._auto_trace.rewrite_ast import no_auto_trace
-from ._config import METRICS_PREFERRED_TEMPORALITY, ConsoleOptions, PydanticPlugin, configure
-from ._main import LevelName, Logfire, LogfireSpan
-from ._scrubbing import ScrubMatch
-from .exporters._file import load_file as load_spans_from_file
+from typing import Any
+
+from ._internal.auto_trace import AutoTraceModule
+from ._internal.auto_trace.rewrite_ast import no_auto_trace
+from ._internal.config import METRICS_PREFERRED_TEMPORALITY, ConsoleOptions, PydanticPlugin, configure
+from ._internal.constants import LevelName
+from ._internal.exporters.file import load_file as load_spans_from_file
+from ._internal.main import Logfire, LogfireSpan
+from ._internal.scrubbing import ScrubMatch
 from .version import VERSION
 
 DEFAULT_LOGFIRE_INSTANCE = Logfire()
 with_tags = DEFAULT_LOGFIRE_INSTANCE.with_tags
 # with_trace_sample_rate = DEFAULT_LOGFIRE_INSTANCE.with_trace_sample_rate
 span = DEFAULT_LOGFIRE_INSTANCE.span
 instrument = DEFAULT_LOGFIRE_INSTANCE.instrument
@@ -35,14 +39,25 @@
 metric_histogram = DEFAULT_LOGFIRE_INSTANCE.metric_histogram
 metric_up_down_counter = DEFAULT_LOGFIRE_INSTANCE.metric_up_down_counter
 metric_counter_callback = DEFAULT_LOGFIRE_INSTANCE.metric_counter_callback
 metric_gauge_callback = DEFAULT_LOGFIRE_INSTANCE.metric_gauge_callback
 metric_up_down_counter_callback = DEFAULT_LOGFIRE_INSTANCE.metric_up_down_counter_callback
 
 
+def loguru_handler() -> dict[str, Any]:
+    """Create a **Logfire** handler for Loguru.
+
+    Returns:
+        A dictionary with the handler and format for Loguru.
+    """
+    from .integrations import loguru
+
+    return {'sink': loguru.LogfireHandler(), 'format': '{message}'}
+
+
 __version__ = VERSION
 
 __all__ = (
     'Logfire',
     'LogfireSpan',
     'LevelName',
     'ConsoleOptions',
@@ -64,8 +79,9 @@
     'AutoTraceModule',
     'with_tags',
     # 'with_trace_sample_rate',
     'load_spans_from_file',
     'no_auto_trace',
     'METRICS_PREFERRED_TEMPORALITY',
     'ScrubMatch',
+    'VERSION',
 )
```

### Comparing `logfire-0.23.0/logfire/_ast_utils.py` & `logfire-0.24.0/logfire/_internal/ast_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import ast
 from dataclasses import dataclass
 from typing import cast
 
 from opentelemetry.util import types as otel_types
 
-from ._constants import (
+from .constants import (
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SAMPLE_RATE_KEY,
     ATTRIBUTES_TAGS_KEY,
 )
-from ._stack_info import StackInfo, get_filepath_attribute
-from ._utils import uniquify_sequence
+from .stack_info import StackInfo, get_filepath_attribute
+from .utils import uniquify_sequence
 
 
 @dataclass(frozen=True)
 class LogfireArgs:
     """Values passed to `logfire.instrument` and/or values stored in a logfire instance as basic configuration.
 
     These determine the arguments passed to the method calls added by the AST transformer.
```

### Comparing `logfire-0.23.0/logfire/_async.py` & `logfire-0.24.0/logfire/_internal/async_.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import asyncio.events
 import asyncio.tasks
 import inspect
 from contextlib import contextmanager
 from types import CoroutineType
 from typing import TYPE_CHECKING, Any, ContextManager
 
-from logfire._constants import ONE_SECOND_IN_NANOSECONDS
-from logfire._stack_info import StackInfo, get_code_object_info, get_stack_info_from_frame
-from logfire._utils import safe_repr
+from .constants import ONE_SECOND_IN_NANOSECONDS
+from .stack_info import StackInfo, get_code_object_info, get_stack_info_from_frame
+from .utils import safe_repr
 
 if TYPE_CHECKING:
-    from logfire._main import Logfire
+    from .main import Logfire
 
 
 def log_slow_callbacks(logfire: Logfire, slow_duration: float) -> ContextManager[None]:
     """Log a warning whenever a function running in the asyncio event loop blocks for too long.
 
     See Logfire.log_slow_async_callbacks.
     Inspired by https://gitlab.com/quantlane/libs/aiodebug.
```

### Comparing `logfire-0.23.0/logfire/_auth.py` & `logfire-0.24.0/logfire/_internal/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import TypedDict
 from urllib.parse import urljoin
 
 import requests
 
-from ._utils import UnexpectedResponse
-from .exceptions import LogfireConfigError
+from logfire.exceptions import LogfireConfigError
+
+from .utils import UnexpectedResponse
 
 HOME_LOGFIRE = Path.home() / '.logfire'
 """Folder used to store global configuration, and user tokens."""
 DEFAULT_FILE = HOME_LOGFIRE / 'default.toml'
 """File used to store user tokens."""
```

### Comparing `logfire-0.23.0/logfire/_auto_trace/__init__.py` & `logfire-0.24.0/logfire/_internal/auto_trace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import inspect
 import sys
 import warnings
 from typing import TYPE_CHECKING, Callable, Literal, Sequence
 
-from .._constants import ONE_SECOND_IN_NANOSECONDS
+from ..constants import ONE_SECOND_IN_NANOSECONDS
 from .import_hook import LogfireFinder
 from .types import AutoTraceModule
 
 if TYPE_CHECKING:
-    from logfire._main import Logfire
+    from ..main import Logfire
 
 
 def install_auto_tracing(
     logfire: Logfire,
     modules: Sequence[str] | Callable[[AutoTraceModule], bool] | None = None,
     *,
     check_imported_modules: Literal['error', 'warn', 'ignore'] = 'error',
```

### Comparing `logfire-0.23.0/logfire/_auto_trace/import_hook.py` & `logfire-0.24.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from types import ModuleType
 from typing import TYPE_CHECKING, Callable, Iterator, Sequence
 
 from .rewrite_ast import exec_source
 from .types import AutoTraceModule
 
 if TYPE_CHECKING:
-    from logfire._main import Logfire
+    from ..main import Logfire
 
 
 @dataclass
 class LogfireFinder(MetaPathFinder):
     """The import hook entry point, inserted into `sys.meta_path` to apply AST rewriting to matching modules."""
 
     logfire: Logfire
```

### Comparing `logfire-0.23.0/logfire/_auto_trace/rewrite_ast.py` & `logfire-0.24.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import ast
 import uuid
 from dataclasses import dataclass
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, ContextManager, TypeVar
 
 import logfire
-from logfire._ast_utils import BaseTransformer, LogfireArgs
+
+from ..ast_utils import BaseTransformer, LogfireArgs
 
 if TYPE_CHECKING:
-    from logfire._main import Logfire
+    from ..main import Logfire
 
 
 def exec_source(
     source: str, filename: str, module_name: str, globs: dict[str, Any], logfire_instance: Logfire, min_duration: int
 ) -> None:
     """Execute a modified AST of the module's source code in the module's namespace.
```

### Comparing `logfire-0.23.0/logfire/_auto_trace/types.py` & `logfire-0.24.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.23.0/logfire/_collect_system_info.py` & `logfire-0.24.0/logfire/_internal/collect_system_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import importlib.metadata as metadata
 from functools import lru_cache
 
-from logfire._limits import filter_package_versions
+from .limits import filter_package_versions
 
 
 @lru_cache
 def collect_package_info() -> dict[str, str]:
     """Retrieve the package information for all installed packages.
 
     Returns:
```

### Comparing `logfire-0.23.0/logfire/_config.py` & `logfire-0.24.0/logfire/_internal/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import warnings
 from dataclasses import dataclass, field
 from functools import cached_property
 from pathlib import Path
 from threading import RLock
 from typing import Any, Callable, Literal, Sequence, cast
 from urllib.parse import urljoin
+from uuid import uuid4
 
 import requests
 from opentelemetry import metrics, trace
 from opentelemetry.context import attach, detach, set_value
 from opentelemetry.environment_variables import OTEL_TRACES_EXPORTER
 from opentelemetry.exporter.otlp.proto.http.metric_exporter import OTLPMetricExporter
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
@@ -40,41 +41,42 @@
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SimpleSpanProcessor, SpanExporter
 from opentelemetry.sdk.trace.id_generator import IdGenerator, RandomIdGenerator
 from opentelemetry.sdk.trace.sampling import ParentBasedTraceIdRatio
 from opentelemetry.semconv.resource import ResourceAttributes
 from rich.prompt import Confirm, Prompt
 from typing_extensions import Self
 
-from ._auth import DEFAULT_FILE, DefaultFile, is_logged_in
-from ._collect_system_info import collect_package_info
-from ._config_params import ParamManager, PydanticPluginRecordValues
-from ._constants import (
+from logfire.exceptions import LogfireConfigError
+from logfire.version import VERSION
+
+from .auth import DEFAULT_FILE, DefaultFile, is_logged_in
+from .collect_system_info import collect_package_info
+from .config_params import ParamManager, PydanticPluginRecordValues
+from .constants import (
     DEFAULT_FALLBACK_FILE_NAME,
     OTLP_MAX_BODY_SIZE,
     RESOURCE_ATTRIBUTES_PACKAGE_VERSIONS,
     SUPPRESS_INSTRUMENTATION_CONTEXT_KEY,
 )
-from ._metrics import ProxyMeterProvider, configure_metrics
-from ._scrubbing import Scrubber, ScrubCallback
-from ._tracer import PendingSpanProcessor, ProxyTracerProvider
-from ._utils import UnexpectedResponse, ensure_data_dir_exists, read_toml_file
-from .exceptions import LogfireConfigError
-from .exporters._fallback import FallbackSpanExporter
-from .exporters._file import FileSpanExporter
-from .exporters._otlp import OTLPExporterHttpSession, RetryFewerSpansSpanExporter
-from .exporters._processor_wrapper import SpanProcessorWrapper
-from .exporters._remove_pending import RemovePendingSpansExporter
 from .exporters.console import (
     ConsoleColorsValues,
     IndentedConsoleSpanExporter,
     ShowParentsConsoleSpanExporter,
     SimpleConsoleSpanExporter,
 )
-from .integrations._executors import instrument_executors
-from .version import VERSION
+from .exporters.fallback import FallbackSpanExporter
+from .exporters.file import FileSpanExporter
+from .exporters.otlp import OTLPExporterHttpSession, RetryFewerSpansSpanExporter
+from .exporters.processor_wrapper import SpanProcessorWrapper
+from .exporters.remove_pending import RemovePendingSpansExporter
+from .integrations.executors import instrument_executors
+from .metrics import ProxyMeterProvider, configure_metrics
+from .scrubbing import Scrubber, ScrubCallback
+from .tracer import PendingSpanProcessor, ProxyTracerProvider
+from .utils import UnexpectedResponse, ensure_data_dir_exists, read_toml_file
 
 CREDENTIALS_FILENAME = 'logfire_credentials.json'
 """Default base URL for the Logfire API."""
 COMMON_REQUEST_HEADERS = {'User-Agent': f'logfire/{VERSION}'}
 """Common request headers for requests to the Logfire API."""
 PROJECT_NAME_PATTERN = r'^[a-z0-9]+(?:-[a-z0-9]+)*$'
 
@@ -236,15 +238,15 @@
 class _LogfireConfigData:
     """Data-only parent class for LogfireConfig.
 
     This class can be pickled / copied and gives a nice repr,
     while allowing us to keep the ugly stuff only in LogfireConfig.
 
     In particular, using this dataclass as a base class of LogfireConfig allows us to use
-    `dataclasses.asdict` in `integrations/_executors.py` to get a dict with just the attributes from
+    `dataclasses.asdict` in `integrations/executors.py` to get a dict with just the attributes from
     `_LogfireConfigData`, and none of the attributes added in `LogfireConfig`.
     """
 
     base_url: str
     """The base URL of the Logfire API"""
 
     send_to_logfire: bool | Literal['if-token-present']
@@ -350,30 +352,30 @@
 
         # We save `scrubbing_patterns` and `scrubbing_callback` just so that they can be serialized and deserialized.
         self.scrubbing_patterns = scrubbing_patterns
         self.scrubbing_callback = scrubbing_callback
         self.scrubber = Scrubber(scrubbing_patterns, scrubbing_callback)
 
         if isinstance(console, dict):
-            # This is particularly for deserializing from a dict as in _executors.py
+            # This is particularly for deserializing from a dict as in executors.py
             console = ConsoleOptions(**console)  # type: ignore
         if console is not None:
             self.console = console
         elif param_manager.load_param('console') is False:
             self.console = False
         else:
             self.console = ConsoleOptions(
                 colors=param_manager.load_param('console_colors'),
                 span_style=param_manager.load_param('console_span_style'),
                 include_timestamps=param_manager.load_param('console_include_timestamp'),
                 verbose=param_manager.load_param('console_verbose'),
             )
 
         if isinstance(pydantic_plugin, dict):
-            # This is particularly for deserializing from a dict as in _executors.py
+            # This is particularly for deserializing from a dict as in executors.py
             pydantic_plugin = PydanticPlugin(**pydantic_plugin)  # type: ignore
         self.pydantic_plugin = pydantic_plugin or PydanticPlugin(
             record=param_manager.load_param('pydantic_plugin_record'),
             include=param_manager.load_param('pydantic_plugin_include'),
             exclude=param_manager.load_param('pydantic_plugin_exclude'),
         )
         self.fast_shutdown = fast_shutdown
@@ -395,15 +397,15 @@
     def _load_config_from_file(self, config_dir: Path) -> dict[str, Any]:
         config_file = config_dir / 'pyproject.toml'
         if not config_file.exists():
             return {}
         try:
             data = read_toml_file(config_file)
             return data.get('tool', {}).get('logfire', {})
-        except Exception as exc:  # pragma: no cover
+        except Exception as exc:
             raise LogfireConfigError(f'Invalid config file: {config_file}') from exc
 
 
 class LogfireConfig(_LogfireConfigData):
     def __init__(
         self,
         base_url: str | None = None,
@@ -533,28 +535,36 @@
             return self._tracer_provider
 
         backup_context = attach(set_value(SUPPRESS_INSTRUMENTATION_CONTEXT_KEY, True))
         try:
             otel_resource_attributes: dict[str, Any] = {
                 ResourceAttributes.SERVICE_NAME: self.service_name,
                 RESOURCE_ATTRIBUTES_PACKAGE_VERSIONS: json.dumps(collect_package_info(), separators=(',', ':')),
+                ResourceAttributes.PROCESS_PID: os.getpid(),
             }
             if self.service_version:
                 otel_resource_attributes[ResourceAttributes.SERVICE_VERSION] = self.service_version
             otel_resource_attributes_from_env = os.getenv(OTEL_RESOURCE_ATTRIBUTES)
             if otel_resource_attributes_from_env:
-                extra_resource_attributes = {}
                 for _field in otel_resource_attributes_from_env.split(','):
-                    key, value = _field.split('=')
-                    extra_resource_attributes[key.strip()] = value.strip()
-                otel_resource_attributes.update(
-                    self.scrubber.scrub(('otel_resource_attributes',), extra_resource_attributes)
-                )
+                    key, value = _field.split('=', maxsplit=1)
+                    otel_resource_attributes[key.strip()] = value.strip()
 
             resource = Resource.create(otel_resource_attributes)
+
+            # Set service instance ID to a random UUID if it hasn't been set already.
+            # Setting it above would have also mostly worked and allowed overriding via OTEL_RESOURCE_ATTRIBUTES,
+            # but doing it here means that resource detectors (checked in Resource.create) get priority.
+            # This attribute is currently experimental. The latest released docs about it are here:
+            # https://opentelemetry.io/docs/specs/semconv/resource/#service-experimental
+            # Currently there's a newer version with some differences here:
+            # https://github.com/open-telemetry/semantic-conventions/blob/e44693245eef815071402b88c3a44a8f7f8f24c8/docs/resource/README.md#service-experimental
+            # Both recommend generating a UUID.
+            resource = Resource({ResourceAttributes.SERVICE_INSTANCE_ID: uuid4().hex}).merge(resource)
+
             tracer_provider = SDKTracerProvider(
                 sampler=ParentBasedTraceIdRatio(self.trace_sample_rate),
                 resource=resource,
                 id_generator=self.id_generator,
             )
 
             self._tracer_provider.shutdown()
@@ -736,20 +746,20 @@
         We continue unless we get a 401 and allow OTel to take of storing data locally for back-fill.
 
         Raises:
             LogfireConfigError: If the token is invalid.
         """
         try:
             response = self.logfire_api_session.get(urljoin(self.base_url, '/v1/health'), timeout=10)
-        except requests.RequestException as e:  # pragma: no cover
+        except requests.RequestException as e:
             warnings.warn(f'Logfire API is unreachable, you may have trouble sending data. Error: {e}')
         else:
-            if response.status_code == 401:  # pragma: no cover
+            if response.status_code == 401:
                 raise LogfireConfigError('Invalid Logfire token.')
-            elif response.status_code != 200:  # pragma: no cover
+            elif response.status_code != 200:
                 # any other status code is considered unhealthy
                 warnings.warn(
                     f'Logfire API is unhealthy, you may have trouble sending data. Status code: {response.status_code}'
                 )
 
 
 def _get_default_span_processor(exporter: SpanExporter) -> SpanProcessor:
@@ -791,35 +801,33 @@
             LogfireConfigError: If the credentials file exists but is invalid.
         """
         path = _get_creds_file(creds_dir)
         if path.exists():
             try:
                 with path.open('rb') as f:
                     data = json.load(f)
-            except (ValueError, OSError) as e:  # pragma: no cover
+            except (ValueError, OSError) as e:
                 raise LogfireConfigError(f'Invalid credentials file: {path}') from e
 
             try:
                 # Handle legacy key
-                dashboard_url = data.get('dashboard_url')
-                if dashboard_url is not None:  # pragma: no cover
+                dashboard_url = data.pop('dashboard_url', None)
+                if dashboard_url is not None:
                     data.setdefault('project_url', dashboard_url)
                 return cls(**data)
-            except TypeError as e:  # pragma: no cover
+            except TypeError as e:
                 raise LogfireConfigError(f'Invalid credentials file: {path} - {e}') from e
 
     @classmethod
     def _get_user_token(cls, logfire_api_url: str) -> str:
         if DEFAULT_FILE.is_file():  # pragma: no branch
             data = cast(DefaultFile, read_toml_file(DEFAULT_FILE))
             if is_logged_in(data, logfire_api_url):  # pragma: no branch
                 return data['tokens'][logfire_api_url]['token']
-        raise LogfireConfigError(  # pragma: no cover
-            'You are not authenticated. Please run `logfire auth` to authenticate.'
-        )
+        raise LogfireConfigError('You are not authenticated. Please run `logfire auth` to authenticate.')
 
     @classmethod
     def get_user_projects(cls, session: requests.Session, logfire_api_url: str) -> list[dict[str, Any]]:
         """Get list of projects that user has access to them.
 
         Args:
             session: HTTP client session used to communicate with the Logfire API.
@@ -872,15 +880,15 @@
         user_token = cls._get_user_token(logfire_api_url=logfire_api_url)
         headers = {**COMMON_REQUEST_HEADERS, 'Authorization': user_token}
 
         # {1: (<organization_name1>, <project_name1>), 2: (<organization_name2>, <project_name2>)}
         projects_map = {str(index + 1): (p['organization_name'], p['project_name']) for index, p in enumerate(projects)}
 
         if (organization, project_name) not in projects_map.values():
-            if not projects_map:  # pragma: no cover
+            if not projects_map:
                 Prompt.ask('There is no project to use. Continue?', default=True)
                 return None
 
             project_choices_str = '\n'.join([f'{index}. {item[0]}/{item[1]}' for index, item in projects_map.items()])
             selected_project_key = Prompt.ask(
                 f'Please select one of the existing project number:\n' f'{project_choices_str}\n',
                 choices=list(projects_map.keys()),
@@ -893,15 +901,15 @@
         project_write_token_url = urljoin(
             logfire_api_url,
             f'/v1/organizations/{organization}/projects/{project_name}/write-tokens/',
         )
         try:
             response = session.post(project_write_token_url, headers=headers)
             UnexpectedResponse.raise_for_status(response)
-        except requests.RequestException as e:  # pragma: no cover
+        except requests.RequestException as e:
             raise LogfireConfigError('Error creating project write token.') from e
 
         return response.json()
 
     @classmethod
     def create_new_project(
         cls,
@@ -935,26 +943,26 @@
         headers = {**COMMON_REQUEST_HEADERS, 'Authorization': user_token}
 
         # Get user organizations
         organizations_url = urljoin(logfire_api_url, '/v1/organizations/')
         try:
             response = session.get(organizations_url, headers=headers)
             UnexpectedResponse.raise_for_status(response)
-        except requests.RequestException as e:  # pragma: no cover
+        except requests.RequestException as e:
             raise LogfireConfigError('Error retrieving list of organizations.') from e
         organizations = [item['organization_name'] for item in response.json()]
 
         if organization not in organizations:
             if len(organizations) > 1:
                 # Get user default organization
                 account_info_url = urljoin(logfire_api_url, '/v1/account/me')
                 try:
                     response = session.get(account_info_url, headers=headers)
                     UnexpectedResponse.raise_for_status(response)
-                except requests.RequestException as e:  # pragma: no cover
+                except requests.RequestException as e:
                     raise LogfireConfigError('Error retrieving user information.') from e
                 json_response = response.json()
                 user_default_organization_name = json_response.get('default_organization', {}).get('organization_name')
 
                 if default_organization and user_default_organization_name:
                     organization = user_default_organization_name
                 else:
@@ -1004,15 +1012,15 @@
                             f'\nThe project name you entered is invalid:\n'
                             f'{error["msg"]}\n'
                             f'Please enter a different project name'
                         )
                         project_name = None
                         continue
                 UnexpectedResponse.raise_for_status(response)
-            except requests.RequestException as e:  # pragma: no cover
+            except requests.RequestException as e:
                 raise LogfireConfigError('Error creating new project.') from e
             else:
                 return response.json()
 
     @classmethod
     def initialize_project(
         cls,
```

### Comparing `logfire-0.23.0/logfire/_config_params.py` & `logfire-0.24.0/logfire/_internal/config_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Literal, Set, TypeVar
 
 from opentelemetry.sdk.environment_variables import OTEL_EXPORTER_OTLP_ENDPOINT, OTEL_SERVICE_NAME
 from typing_extensions import get_args, get_origin
 
-from logfire.exporters.console import ConsoleColorsValues
+from logfire.exceptions import LogfireConfigError
 
-from ._constants import LOGFIRE_BASE_URL
-from .exceptions import LogfireConfigError
+from .constants import LOGFIRE_BASE_URL
+from .exporters.console import ConsoleColorsValues
 
 try:
     import opentelemetry.instrumentation.system_metrics  # noqa: F401 # type: ignore
 
     COLLECT_SYSTEM_METRICS_DEFAULT = True
 except ImportError:  # pragma: no cover
     COLLECT_SYSTEM_METRICS_DEFAULT = False  # type: ignore
```

### Comparing `logfire-0.23.0/logfire/_constants.py` & `logfire-0.24.0/logfire/_internal/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,37 @@
 """Level names for records."""
 
 LEVEL_NUMBERS = {
     'trace': 1,
     'debug': 5,
     'info': 9,
     'notice': 10,
-    'warn': 13,
     # warning is used by standard lib logging, has same meaning as "warn"
     'warning': 13,
+    'warn': 13,
     'error': 17,
     'fatal': 21,
 }
 
+NUMBER_TO_LEVEL = {v: k for k, v in LEVEL_NUMBERS.items()}
+
 ATTRIBUTES_LOG_LEVEL_NAME_KEY = f'{LOGFIRE_ATTRIBUTES_NAMESPACE}.level_name'
-"""The key within OTEL attributes where logfire puts the log level name."""
+"""Deprecated, use only ATTRIBUTES_LOG_LEVEL_NUM_KEY."""
 
 ATTRIBUTES_LOG_LEVEL_NUM_KEY = f'{LOGFIRE_ATTRIBUTES_NAMESPACE}.level_num'
 """The key within OTEL attributes where logfire puts the log level number."""
 
 
 # This is in this file to encourage using it instead of setting these attributes manually.
 def log_level_attributes(level: LevelName) -> dict[str, otel_types.AttributeValue]:
     if level not in LEVEL_NUMBERS:
         warnings.warn(f'Invalid log level name: {level!r}')
         level = 'error'
 
     return {
-        ATTRIBUTES_LOG_LEVEL_NAME_KEY: level,
         ATTRIBUTES_LOG_LEVEL_NUM_KEY: LEVEL_NUMBERS[level],
     }
 
 
 SpanTypeType = Literal['log', 'pending_span', 'span']
 
 ATTRIBUTES_SPAN_TYPE_KEY = f'{LOGFIRE_ATTRIBUTES_NAMESPACE}.span_type'
```

### Comparing `logfire-0.23.0/logfire/_formatter.py` & `logfire-0.24.0/logfire/_internal/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from string import Formatter
 from typing import Any, Final, Literal, Mapping
 
 from typing_extensions import NotRequired, TypedDict
 
 __all__ = 'chunks_formatter', 'LiteralChunk', 'ArgChunk', 'logfire_format'
 
-from logfire._constants import MESSAGE_FORMATTED_VALUE_LENGTH_LIMIT
-from logfire._scrubbing import Scrubber
-from logfire._utils import truncate_string
+from .constants import MESSAGE_FORMATTED_VALUE_LENGTH_LIMIT
+from .scrubbing import Scrubber
+from .utils import truncate_string
 
 
 class LiteralChunk(TypedDict):
     t: Literal['lit']
     v: str
```

### Comparing `logfire-0.23.0/logfire/_instrument.py` & `logfire-0.24.0/logfire/_internal/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from dataclasses import dataclass
 from functools import lru_cache, update_wrapper
 from types import CodeType, FunctionType
 from typing import TYPE_CHECKING, Callable, Iterator, TypeVar
 
 from typing_extensions import ParamSpec
 
-from logfire._ast_utils import BaseTransformer, LogfireArgs
+from .ast_utils import BaseTransformer, LogfireArgs
 
 if TYPE_CHECKING:
-    from logfire._main import Logfire
+    from .main import Logfire
 
 
 _PARAMS = ParamSpec('_PARAMS')
 _RETURN = TypeVar('_RETURN')
 
 
 def instrument(
```

### Comparing `logfire-0.23.0/logfire/_json_encoder.py` & `logfire-0.24.0/logfire/_internal/json_encoder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,26 @@
 from __future__ import annotations
 
+import contextlib
 import dataclasses
 import datetime
 import json
 from collections.abc import Mapping, Sequence
 from decimal import Decimal
 from enum import Enum
 from functools import lru_cache
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from itertools import chain
 from pathlib import PosixPath
 from re import Pattern
 from types import GeneratorType
-from typing import TYPE_CHECKING, Any, Callable
+from typing import Any, Callable
 from uuid import UUID
 
-from logfire._utils import JsonValue, safe_repr
-
-if TYPE_CHECKING:
-    from sqlalchemy.orm import DeclarativeBase, DeclarativeMeta
-else:
-    try:
-        from sqlalchemy.orm import DeclarativeBase, DeclarativeMeta
-    except ImportError:  # pragma: no cover
-        DeclarativeBase = type('DeclarativeBase', (), {})
-        DeclarativeMeta = type('DeclarativeMeta', (), {})
-
-try:
-    import pydantic
-except ModuleNotFoundError:  # pragma: no cover
-    # pydantic is not installed, possible since it's not a dependency
-    # don't add the types to the lookup logic
-    pydantic = None
-
-try:
-    import pandas
-except ModuleNotFoundError:  # pragma: no cover
-    pandas = None
-
-try:
-    import numpy
-except ModuleNotFoundError:  # pragma: no cover
-    numpy = None
-
-try:
-    import attrs
-except ModuleNotFoundError:  # pragma: no cover
-    attrs = None
-
-try:
-    import sqlalchemy
-    from sqlalchemy import inspect as sa_inspect
-except ModuleNotFoundError:  # pragma: no cover
-    sqlalchemy = None
-    sa_inspect = None
-
-__all__ = ('logfire_json_dumps',)
+from .utils import JsonValue, safe_repr
 
 NUMPY_DIMENSION_MAX_SIZE = 10
 """The maximum size of a dimension of a numpy array."""
 
 
 def _bytes_encoder(o: bytes) -> str:
     """Encode bytes using repr() to get a string representation of the bytes object.
@@ -153,46 +114,51 @@
         [1, 2, 4, 5],
         [2, 3, 8, 10],
         [4, 8, 16, 20],
         [5, 10, 20, 25],
     ]
     """
     # If we reach here, numpy is installed.
-    assert numpy and isinstance(o, numpy.ndarray)
+    import numpy
+
     shape = o.shape
     dimensions = o.ndim
 
     if isinstance(o, numpy.matrix):
         o = o.A  # type: ignore[reportUnknownMemberType]
 
     for dimension in range(dimensions):
         # In case of multiple dimensions, we limit the dimension size by the NUMPY_DIMENSION_MAX_SIZE.
         half = min(shape[dimension], NUMPY_DIMENSION_MAX_SIZE) // 2
         # Slicing and concatenating arrays along the specified axis
         slices = [slice(None)] * dimensions
         slices[dimension] = slice(0, half)
-        front = o[tuple(slices)]  # type: ignore[reportUnknownVariableType]
+        front = o[tuple(slices)]
 
         slices[dimension] = slice(-half, None)
-        end = o[tuple(slices)]  # type: ignore[reportUnknownVariableType]
-        o = numpy.concatenate((front, end), axis=dimension)  # type: ignore[reportUnknownVariableType]
+        end = o[tuple(slices)]
+        o = numpy.concatenate((front, end), axis=dimension)
 
     return to_json_value(o.tolist())
 
 
 def _pydantic_model_encoder(o: Any) -> JsonValue:
-    assert pydantic and isinstance(o, pydantic.BaseModel)
+    import pydantic
+
+    assert isinstance(o, pydantic.BaseModel)
     return to_json_value(o.model_dump())
 
 
 def _get_sqlalchemy_data(o: Any) -> JsonValue:
-    if sa_inspect is not None:  # pragma: no branch
+    try:
+        from sqlalchemy import inspect as sa_inspect
+
         state = sa_inspect(o)
         deferred = state.unloaded
-    else:  # pragma: no cover
+    except ModuleNotFoundError:  # pragma: no cover
         deferred = set()  # type: ignore
 
     return to_json_value(
         {field: getattr(o, field) if field not in deferred else '<deferred>' for field in o.__mapper__.attrs.keys()}
     )
 
 
@@ -220,43 +186,49 @@
         IPv6Interface: str,
         IPv6Network: str,
         PosixPath: str,
         Pattern: lambda o: to_json_value(o.pattern),
         UUID: str,
         Exception: str,
     }
-    if pydantic:  # pragma: no cover
+    with contextlib.suppress(ModuleNotFoundError):
+        import pydantic
+
         lookup.update(
             {
                 pydantic.AnyUrl: str,
                 pydantic.NameEmail: str,
                 pydantic.SecretBytes: str,
                 pydantic.SecretStr: str,
                 pydantic.BaseModel: _pydantic_model_encoder,
             }
         )
 
-    if pandas:  # pragma: no cover
+    with contextlib.suppress(ModuleNotFoundError):
+        import pandas
+
         lookup.update({pandas.DataFrame: _pandas_data_frame_encoder})
-    if numpy:  # pragma: no cover
+    with contextlib.suppress(ModuleNotFoundError):
+        import numpy
+
         lookup.update({numpy.ndarray: _numpy_array_encoder})
 
     return lookup
 
 
 def to_json_value(o: Any) -> JsonValue:
     try:
         if isinstance(o, (int, float, str, bool, type(None))):
             return o
         elif isinstance(o, Mapping):
             return {key if isinstance(key, str) else safe_repr(key): to_json_value(value) for key, value in o.items()}  # type: ignore
         elif dataclasses.is_dataclass(o):
             return {f.name: to_json_value(getattr(o, f.name)) for f in dataclasses.fields(o)}
-        elif attrs is not None and attrs.has(o.__class__):
-            return {f.name: to_json_value(getattr(o, f.name)) for f in attrs.fields(o.__class__)}
+        elif is_attrs(o):
+            return _get_attrs_data(o)
         elif is_sqlalchemy(o):
             return _get_sqlalchemy_data(o)
 
         # Check the class type and its superclasses for a matching encoder
         for base in o.__class__.__mro__[:-1]:
             try:
                 encoder = encoder_by_type()[base]
@@ -275,12 +247,30 @@
 
 
 def logfire_json_dumps(obj: Any) -> str:
     return json.dumps(to_json_value(obj), separators=(',', ':'))
 
 
 def is_sqlalchemy(obj: Any) -> bool:
-    if sqlalchemy is None:  # pragma: no cover
+    try:
+        from sqlalchemy.orm import DeclarativeBase, DeclarativeMeta
+
+        if isinstance(obj, DeclarativeBase):
+            return True
+        return isinstance(obj.__class__, DeclarativeMeta)
+    except ImportError:  # pragma: no cover
         return False
-    if isinstance(obj, DeclarativeBase):
-        return True
-    return isinstance(obj.__class__, DeclarativeMeta)
+
+
+def is_attrs(obj: Any) -> bool:
+    try:
+        import attrs
+
+        return attrs.has(obj.__class__)
+    except ModuleNotFoundError:  # pragma: no cover
+        return False
+
+
+def _get_attrs_data(o: Any) -> JsonValue:
+    import attrs
+
+    return {f.name: to_json_value(getattr(o, f.name)) for f in attrs.fields(o.__class__)}
```

### Comparing `logfire-0.23.0/logfire/_json_formatter.py` & `logfire-0.24.0/logfire/_internal/json_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import io
 from datetime import timedelta
 from functools import partial
 from typing import Any, Callable, cast
 
-from ._json_types import ArraySchema, DataType, JSONSchema
-from ._utils import safe_repr
+from .json_types import ArraySchema, DataType, JSONSchema
+from .utils import safe_repr
 
 
 class JsonArgsValueFormatter:
     """Format values recursively based on the information provided in value dict.
 
     When a custom format is identified, the `$__datatype__` key is always present.
     """
```

### Comparing `logfire-0.23.0/logfire/_json_schema.py` & `logfire-0.24.0/logfire/_internal/json_schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,66 +10,38 @@
 - `x-row-count`: The number of rows in the data frame. It is used to generate the Python type.
 - `x-shape`: The shape of the numpy array. It is used to generate the Python type.
 - `x-dtype`: The data type of the numpy array. It is used to generate the Python type.
 """
 
 from __future__ import annotations
 
+import contextlib
 import dataclasses
 import datetime
 import re
 import uuid
 from collections import deque
 from decimal import Decimal
 from enum import Enum
 from functools import lru_cache
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from pathlib import PosixPath
 from types import GeneratorType
 from typing import Any, Callable, Iterable, Mapping, NewType, Sequence, cast
 
-from logfire._json_encoder import is_sqlalchemy, to_json_value
-from logfire._stack_info import STACK_INFO_KEYS
-from logfire._utils import JsonDict, dump_json, safe_repr
+from .json_encoder import is_attrs, is_sqlalchemy, to_json_value
+from .stack_info import STACK_INFO_KEYS
+from .utils import JsonDict, dump_json, safe_repr
 
-try:
-    import pydantic
-    import pydantic_core
-except ModuleNotFoundError:  # pragma: no cover
-    pydantic = None
-    pydantic_core = None
-
-try:
-    import attrs
-except ModuleNotFoundError:  # pragma: no cover
-    attrs = None
-
-try:
-    import pandas
-except ModuleNotFoundError:  # pragma: no cover
-    pandas = None
-
-try:
-    import numpy
-except ModuleNotFoundError:  # pragma: no cover
-    numpy = None
-
-try:
-    import sqlalchemy
-    from sqlalchemy import inspect as sa_inspect
-except ModuleNotFoundError:  # pragma: no cover
-    sqlalchemy = None
-    sa_inspect = None
-
-__all__ = 'create_json_schema', 'attributes_json_schema_properties', 'attributes_json_schema'
+__all__ = 'create_json_schema', 'attributes_json_schema_properties', 'attributes_json_schema', 'JsonSchemaProperties'
 
 
 @lru_cache
 def type_to_schema() -> dict[type[Any], JsonDict | Callable[[Any], JsonDict]]:
-    return {
+    lookup: dict[type[Any], JsonDict | Callable[[Any], JsonDict]] = {
         bytes: _bytes_schema,
         bytearray: _bytearray_schema,
         Enum: _enum_schema,
         Decimal: {'type': 'string', 'format': 'decimal'},
         datetime.datetime: {'type': 'string', 'format': 'date-time'},
         datetime.date: {'type': 'string', 'format': 'date'},
         datetime.time: {'type': 'string', 'format': 'time'},
@@ -87,28 +59,42 @@
         IPv4Network: {'type': 'string', 'format': 'ipv4network'},
         IPv6Network: {'type': 'string', 'format': 'ipv6network'},
         re.Pattern: {'type': 'string', 'format': 'regex'},
         uuid.UUID: {'type': 'string', 'format': 'uuid'},
         range: {'type': 'array', 'x-python-datatype': 'range'},
         PosixPath: {'type': 'string', 'format': 'path', 'x-python-datatype': 'PosixPath'},
         Exception: _exception_schema,
-        **dict(
-            {}
-            if pydantic is None or pydantic_core is None
-            else {
-                pydantic_core.Url: {'type': 'string', 'x-python-datatype': 'Url'},
+    }
+    with contextlib.suppress(ModuleNotFoundError):
+        import pydantic
+
+        lookup.update(
+            {
                 pydantic.NameEmail: {'type': 'string', 'x-python-datatype': 'NameEmail'},
                 pydantic.SecretStr: {'type': 'string', 'x-python-datatype': 'SecretStr'},
                 pydantic.SecretBytes: {'type': 'string', 'x-python-datatype': 'SecretBytes'},
                 pydantic.BaseModel: _pydantic_model_schema,
             }
-        ),
-        **dict({} if pandas is None else {pandas.DataFrame: _pandas_schema}),
-        **dict({} if numpy is None else {numpy.ndarray: _numpy_schema}),
-    }
+        )
+
+    with contextlib.suppress(ModuleNotFoundError):
+        import pydantic_core
+
+        lookup.update({pydantic_core.Url: {'type': 'string', 'x-python-datatype': 'Url'}})
+
+    with contextlib.suppress(ModuleNotFoundError):
+        import numpy
+
+        lookup.update({numpy.ndarray: _numpy_schema})
+
+    with contextlib.suppress(ModuleNotFoundError):
+        import pandas
+
+        lookup.update({pandas.DataFrame: _pandas_schema})
+    return lookup
 
 
 _type_to_schema = None
 
 
 def create_json_schema(obj: Any) -> JsonDict:
     """Create a JSON Schema from the given object.
@@ -119,15 +105,15 @@
     Returns:
         The JSON Schema.
     """
     if dataclasses.is_dataclass(obj):
         return _dataclass_schema(obj)
     elif isinstance(obj, Mapping):
         return _mapping_schema(obj)
-    elif attrs and attrs.has(obj):
+    elif is_attrs(obj):
         return _attrs_schema(obj)
     elif is_sqlalchemy(obj):
         return _sqlalchemy_schema(obj)
 
     global _type_to_schema
     _type_to_schema = _type_to_schema or type_to_schema()
     for base in obj.__class__.__mro__[:-1]:
@@ -264,20 +250,24 @@
 
 
 def _exception_schema(obj: Exception) -> JsonDict:
     return {'type': 'object', 'title': obj.__class__.__name__, 'x-python-datatype': 'Exception'}
 
 
 def _pydantic_model_schema(obj: Any) -> JsonDict:
-    assert pydantic and isinstance(obj, pydantic.BaseModel)
+    import pydantic
+
+    assert isinstance(obj, pydantic.BaseModel)
     return _custom_object_schema(obj, 'PydanticModel', [*obj.model_fields, *(obj.model_extra or {})])
 
 
 def _pandas_schema(obj: Any) -> JsonDict:
-    assert pandas and isinstance(obj, pandas.DataFrame)
+    import pandas
+
+    assert isinstance(obj, pandas.DataFrame)
 
     row_count, column_count = obj.shape
 
     max_columns = pandas.get_option('display.max_columns')
     col_middle = min(max_columns, column_count) // 2
     columns = list(obj.columns[:col_middle]) + list(obj.columns[-col_middle:])  # type: ignore
 
@@ -312,15 +302,16 @@
     import attrs
 
     obj = cast(attrs.AttrsInstance, obj)
     return _custom_object_schema(obj, 'attrs', (key.name for key in obj.__attrs_attrs__))
 
 
 def _sqlalchemy_schema(obj: Any) -> JsonDict:
-    assert sqlalchemy and sa_inspect
+    from sqlalchemy import inspect as sa_inspect
+
     return _custom_object_schema(obj, 'sqlalchemy', sa_inspect(obj).attrs.keys())
 
 
 def _properties(properties: dict[str, Any]) -> JsonDict:
     schema_properties: JsonDict = {}
     for key, value in properties.items():
         if (value_schema := create_json_schema(value)) not in PLAIN_SCHEMAS:
```

### Comparing `logfire-0.23.0/logfire/_json_types.py` & `logfire-0.24.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.23.0/logfire/_main.py` & `logfire-0.24.0/logfire/_internal/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,46 +14,45 @@
 from opentelemetry.metrics import CallbackT, Counter, Histogram, UpDownCounter
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Tracer
 from opentelemetry.util import types as otel_types
 from typing_extensions import LiteralString, ParamSpec
 
-from logfire._config import GLOBAL_CONFIG, LogfireConfig
-from logfire._formatter import logfire_format
-from logfire._instrument import LogfireArgs, instrument
-from logfire.version import VERSION
-
-from . import AutoTraceModule, _async
-from ._auto_trace import install_auto_tracing
-from ._constants import (
+from ..version import VERSION
+from . import async_
+from .auto_trace import AutoTraceModule, install_auto_tracing
+from .config import GLOBAL_CONFIG, LogfireConfig
+from .constants import (
     ATTRIBUTES_JSON_SCHEMA_KEY,
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SAMPLE_RATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     ATTRIBUTES_TAGS_KEY,
     ATTRIBUTES_VALIDATION_ERROR_KEY,
     DISABLE_CONSOLE_KEY,
     NULL_ARGS_KEY,
     OTLP_MAX_INT_SIZE,
     LevelName,
     log_level_attributes,
 )
-from ._json_encoder import logfire_json_dumps
-from ._json_schema import (
+from .formatter import logfire_format
+from .instrument import LogfireArgs, instrument
+from .json_encoder import logfire_json_dumps
+from .json_schema import (
     JsonSchemaProperties,
     attributes_json_schema,
     attributes_json_schema_properties,
     create_json_schema,
 )
-from ._metrics import ProxyMeterProvider
-from ._stack_info import get_caller_stack_info
-from ._tracer import ProxyTracerProvider
-from ._utils import uniquify_sequence
+from .metrics import ProxyMeterProvider
+from .stack_info import get_caller_stack_info
+from .tracer import ProxyTracerProvider
+from .utils import uniquify_sequence
 
 if TYPE_CHECKING:
     from fastapi import FastAPI
     from starlette.requests import Request
     from starlette.websockets import WebSocket
 
 try:
@@ -630,15 +629,15 @@
         Returns:
             A context manager that will revert the patch when exited.
                 This context manager doesn't take into account threads or other concurrency.
                 Calling this method will immediately apply the patch
                 without waiting for the context manager to be opened,
                 i.e. it's not necessary to use this as a context manager.
         """
-        return _async.log_slow_callbacks(self, slow_duration)
+        return async_.log_slow_callbacks(self, slow_duration)
 
     def install_auto_tracing(
         self,
         modules: Sequence[str] | Callable[[AutoTraceModule], bool] | None = None,
         *,
         check_imported_modules: Literal['error', 'warn', 'ignore'] = 'error',
         min_duration: float = 0,
@@ -721,15 +720,15 @@
         Returns:
             A context manager that will revert the instrumentation when exited.
                 This context manager doesn't take into account threads or other concurrency.
                 Calling this method will immediately apply the instrumentation
                 without waiting for the context manager to be opened,
                 i.e. it's not necessary to use this as a context manager.
         """
-        from .integrations._fastapi import instrument_fastapi
+        from .integrations.fastapi import instrument_fastapi
 
         return instrument_fastapi(
             self,
             app,
             request_attributes_mapper=request_attributes_mapper,
             excluded_urls=excluded_urls,
             use_opentelemetry_instrumentation=use_opentelemetry_instrumentation,
@@ -1188,15 +1187,15 @@
     if exception is not sys.exc_info()[1]:
         # OTEL's record_exception uses `traceback.format_exc()` which is for the current exception,
         # ignoring the passed exception.
         # So we override the stacktrace attribute with the correct one.
         stacktrace = ''.join(traceback.format_exception(type(exception), exception, exception.__traceback__))
         attributes[SpanAttributes.EXCEPTION_STACKTRACE] = stacktrace
 
-    span.record_exception(cast(Exception, exception), attributes=attributes, timestamp=timestamp, escaped=escaped)
+    span.record_exception(exception, attributes=attributes, timestamp=timestamp, escaped=escaped)
 
 
 AttributesValueType = TypeVar('AttributesValueType', bound=Union[Any, otel_types.AttributeValue])
 
 
 def user_attributes(attributes: dict[str, Any]) -> dict[str, otel_types.AttributeValue]:
     """Prepare attributes for sending to OpenTelemetry.
```

### Comparing `logfire-0.23.0/logfire/_metrics.py` & `logfire-0.24.0/logfire/_internal/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,20 +24,30 @@
 
 try:
     # This only exists in opentelemetry-sdk>=1.23.0
     from opentelemetry.metrics import _Gauge as Gauge
 except ImportError:  # pragma: no cover
     Gauge = None
 
-# copied from opentelemetry/instrumentation/system_metrics/__init__.py
+# All the cpu_times fields provided by psutil (used by system_metrics) across all platforms,
+# except for 'guest' and 'guest_nice' which are included in 'user' and 'nice' in Linux (see psutil._cpu_tot_time).
+# Docs: https://psutil.readthedocs.io/en/latest/#psutil.cpu_times
+CPU_FIELDS = 'idle user system irq softirq nice iowait steal interrupt dpc'.split()
+
+# All the virtual_memory fields provided by psutil across all platforms,
+# except for 'percent' which can be calculated as `(total - available) / total * 100`.
+# Docs: https://psutil.readthedocs.io/en/latest/#psutil.virtual_memory
+MEMORY_FIELDS = 'total available used free active inactive buffers cached shared wired slab'.split()
+
+# Based on opentelemetry/instrumentation/system_metrics/__init__.py
 DEFAULT_CONFIG = {
-    'system.cpu.time': ['idle', 'user', 'system', 'irq'],
-    'system.cpu.utilization': ['idle', 'user', 'system', 'irq'],
-    'system.memory.usage': ['used', 'free', 'cached'],
-    'system.memory.utilization': ['used', 'free', 'cached'],
+    'system.cpu.time': CPU_FIELDS,
+    'system.cpu.utilization': CPU_FIELDS,
+    'system.memory.usage': MEMORY_FIELDS,
+    'system.memory.utilization': MEMORY_FIELDS,
     'system.swap.usage': ['used', 'free'],
     'system.swap.utilization': ['used', 'free'],
     'system.disk.io': ['read', 'write'],
     'system.disk.operations': ['read', 'write'],
     'system.disk.time': ['read', 'write'],
     'system.network.dropped.packets': ['transmit', 'receive'],
     'system.network.packets': ['transmit', 'receive'],
```

### Comparing `logfire-0.23.0/logfire/_scrubbing.py` & `logfire-0.24.0/logfire/_internal/scrubbing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import Any, Callable, Mapping, Sequence, cast
 
 from opentelemetry.attributes import BoundedAttributes
 from opentelemetry.sdk.trace import Event
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Link
 
-from logfire._constants import (
+from .constants import (
     ATTRIBUTES_JSON_SCHEMA_KEY,
     ATTRIBUTES_LOG_LEVEL_NAME_KEY,
     ATTRIBUTES_LOG_LEVEL_NUM_KEY,
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_PENDING_SPAN_REAL_PARENT_KEY,
     ATTRIBUTES_SAMPLE_RATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     ATTRIBUTES_TAGS_KEY,
     NULL_ARGS_KEY,
     RESOURCE_ATTRIBUTES_PACKAGE_VERSIONS,
 )
-from logfire._stack_info import STACK_INFO_KEYS
-from logfire._utils import ReadableSpanDict
+from .stack_info import STACK_INFO_KEYS
+from .utils import ReadableSpanDict
 
 DEFAULT_PATTERNS = [
     'password',
     'passwd',
     'mysql_pwd',
     'secret',
     'auth',
@@ -91,14 +91,15 @@
         SpanAttributes.HTTP_METHOD,
         SpanAttributes.HTTP_STATUS_CODE,
         SpanAttributes.HTTP_SCHEME,
         SpanAttributes.HTTP_URL,
         SpanAttributes.HTTP_TARGET,
         SpanAttributes.HTTP_ROUTE,
         SpanAttributes.DB_STATEMENT,
+        'db.plan',
     }
 
     def __init__(self, patterns: Sequence[str] | None, callback: ScrubCallback | None = None):
         # See scrubbing_patterns and scrubbing_callback in logfire.configure for more info on these parameters.
         patterns = [*DEFAULT_PATTERNS, *(patterns or [])]
         self._pattern = re.compile('|'.join(patterns), re.IGNORECASE | re.DOTALL)
         self._callback = callback
```

### Comparing `logfire-0.23.0/logfire/_stack_info.py` & `logfire-0.24.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.23.0/logfire/_tracer.py` & `logfire-0.24.0/logfire/_internal/tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 )
 from opentelemetry.sdk.trace.id_generator import IdGenerator
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.trace import Link, Span, SpanContext, SpanKind, Tracer, TracerProvider
 from opentelemetry.trace.status import Status, StatusCode
 from opentelemetry.util import types as otel_types
 
-from ._constants import (
+from .constants import (
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_PENDING_SPAN_REAL_PARENT_KEY,
     ATTRIBUTES_SAMPLE_RATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     PENDING_SPAN_NAME_SUFFIX,
 )
 
 if TYPE_CHECKING:
-    from logfire._config import LogfireConfig
+    from .config import LogfireConfig
 
 
 @dataclass
 class ProxyTracerProvider(TracerProvider):
     """A tracer provider that wraps another internal tracer provider allowing it to be re-assigned."""
 
     provider: TracerProvider
@@ -130,15 +130,15 @@
         status: Status | StatusCode,
         description: str | None = None,
     ) -> None:
         self.span.set_status(status, description)
 
     def record_exception(
         self,
-        exception: Exception,
+        exception: BaseException,
         attributes: otel_types.Attributes = None,
         timestamp: int | None = None,
         escaped: bool = False,
     ) -> None:
         timestamp = timestamp or self.ns_timestamp_generator()
         return self.span.record_exception(exception, attributes, timestamp, escaped)
 
@@ -202,15 +202,15 @@
         return _MaybeDeterministicTimestampSpan(
             span,
             ns_timestamp_generator=self.provider.config.ns_timestamp_generator,
         )
 
     # This means that `with start_as_current_span(...):`
     # is roughly equivalent to `with use_span(start_span(...)):`
-    start_as_current_span = SDKTracer.start_as_current_span  # type: ignore
+    start_as_current_span = SDKTracer.start_as_current_span
 
 
 @dataclass
 class PendingSpanProcessor(SpanProcessor):
     """Span processor that emits an extra pending span for each span as it starts.
 
     The pending span is emitted by calling `on_end` on all other processors.
```

### Comparing `logfire-0.23.0/logfire/_utils.py` & `logfire-0.24.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.23.0/logfire/backfill.py` & `logfire-0.24.0/logfire/_internal/backfill.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SimpleSpanProcessor
 from opentelemetry.sdk.trace.id_generator import RandomIdGenerator
 from opentelemetry.sdk.util.instrumentation import InstrumentationScope
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.trace import SpanContext, SpanKind, TraceFlags
 from opentelemetry.trace.status import Status, StatusCode
 
-from ._constants import (
-    ATTRIBUTES_LOG_LEVEL_NAME_KEY,
+from .constants import (
+    ATTRIBUTES_LOG_LEVEL_NUM_KEY,
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
+    LEVEL_NUMBERS,
     LevelName,
 )
-from ._formatter import logfire_format
-from ._main import user_attributes
-from ._scrubbing import Scrubber
-from .exporters._file import FileSpanExporter
+from .exporters.file import FileSpanExporter
+from .formatter import logfire_format
+from .main import user_attributes
+from .scrubbing import Scrubber
 
 try:
     from pydantic import BaseModel, ConfigDict, Field
 except ImportError as e:  # pragma: no cover
     raise ImportError('Pydantic is required to use `logfire.import`, run `pip install pydantic`.') from e
 
 
@@ -152,15 +153,15 @@
 
             if data.formatted_msg is None:  # pragma: no cover
                 formatted_message = logfire_format(data.msg_template, data.attributes, self.scrubber, stacklevel=2)
             else:
                 formatted_message = data.formatted_msg
             otlp_attributes: dict[str, Any] = {
                 ATTRIBUTES_SPAN_TYPE_KEY: 'log',
-                ATTRIBUTES_LOG_LEVEL_NAME_KEY: data.level,
+                ATTRIBUTES_LOG_LEVEL_NUM_KEY: LEVEL_NUMBERS[data.level],
                 ATTRIBUTES_MESSAGE_TEMPLATE_KEY: data.msg_template,
                 ATTRIBUTES_MESSAGE_KEY: formatted_message,
                 **otlp_attributes,
             }
             span = ReadableSpan(
                 name=data.msg_template,
                 context=SpanContext(
```

### Comparing `logfire-0.23.0/logfire/cli.py` & `logfire-0.24.0/logfire/_internal/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 """The CLI for Pydantic Logfire."""
-
 from __future__ import annotations
 
 import argparse
+import functools
 import importlib
 import importlib.util
+import logging
 import os
 import platform
 import shutil
 import sys
 import warnings
 import webbrowser
 from pathlib import Path
-from typing import Iterator, cast
+from typing import Any, Iterator, cast
 from urllib.parse import urljoin
 
 import requests
+from opentelemetry import trace
 from rich.console import Console
 from rich.progress import Progress
 from rich.table import Table
 
-import logfire._config
-from logfire._auth import DEFAULT_FILE, HOME_LOGFIRE, DefaultFile, is_logged_in, poll_for_token, request_device_code
-from logfire._config import LogfireCredentials
-from logfire._constants import LOGFIRE_BASE_URL
-from logfire._utils import read_toml_file
+import logfire
 from logfire.exceptions import LogfireConfigError
-from logfire.version import VERSION
+from logfire.propagate import ContextCarrier, get_context
+
+from ..version import VERSION
+from . import config as logfire_config
+from .auth import DEFAULT_FILE, HOME_LOGFIRE, DefaultFile, is_logged_in, poll_for_token, request_device_code
+from .config import LogfireCredentials
+from .constants import LOGFIRE_BASE_URL
+from .tracer import SDKTracerProvider
+from .utils import read_toml_file
 
 BASE_OTEL_INTEGRATION_URL = 'https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/'
 BASE_DOCS_URL = 'https://docs.logfire.dev'
 INTEGRATIONS_DOCS_URL = f'{BASE_DOCS_URL}/guide/integrations/'
 
+HOME_LOGFIRE.mkdir(exist_ok=True)
+
+LOGFIRE_LOG_FILE = HOME_LOGFIRE / 'log.txt'
+file_handler = logging.FileHandler(LOGFIRE_LOG_FILE)
+file_handler.setLevel(logging.DEBUG)
+logging.basicConfig(handlers=[file_handler], level=logging.DEBUG)
+
+logger = logging.getLogger(__name__)
+
 
 def version_callback() -> None:
     """Show the version and exit."""
     py_impl = platform.python_implementation()
     py_version = platform.python_version()
     system = platform.system()
     print(f'Running Logfire {VERSION} with {py_impl} {py_version} on {system}.')
@@ -52,23 +67,25 @@
     else:
         sys.stderr.write(f'Credentials loaded from data dir: {data_dir.resolve()}\n\n')
         credentials.print_token_summary()
 
 
 def parse_clean(args: argparse.Namespace) -> None:
     """Clean Logfire data."""
+    if args.logs and LOGFIRE_LOG_FILE.exists():
+        LOGFIRE_LOG_FILE.unlink()
+
     data_dir = Path(args.data_dir)
-    if not data_dir.exists():
+    if not data_dir.exists() or not data_dir.is_dir():
         sys.stderr.write(f'No Logfire data found in {data_dir.resolve()}\n')
         sys.exit(1)
 
     confirm = input(f'The folder {data_dir.resolve()} will be deleted. Are you sure? [N/y]')
     if confirm.lower() in ('yes', 'y'):
-        if data_dir.exists() and data_dir.is_dir():  # pragma: no branch
-            shutil.rmtree(data_dir)
+        shutil.rmtree(data_dir)
         sys.stderr.write('Cleaned Logfire data.\n')
     else:
         sys.stderr.write('Clean aborted.\n')
 
 
 # TODO(Marcelo): Add tests for this command.
 def parse_backfill(args: argparse.Namespace) -> None:  # pragma: no cover
@@ -82,15 +99,15 @@
     file = Path(args.file)
     if not file.exists():
         sys.stderr.write(f'No backfill file found at {file.resolve()}\n')
         sys.exit(1)
 
     logfire_url = cast(str, args.logfire_url)
     logfire.configure(data_dir=data_dir, base_url=logfire_url, collect_system_metrics=False)
-    config = logfire._config.GLOBAL_CONFIG
+    config = logfire_config.GLOBAL_CONFIG
     config.initialize()
     token = config.token
     assert token is not None  # if no token was available a new project should have been created
     console = Console(file=sys.stderr)
     with Progress(console=console) as progress:
         total = os.path.getsize(file)
         task = progress.add_task('Backfilling...', total=total)
@@ -175,16 +192,16 @@
         otel_package = OTEL_PACKAGE_LINK.get(name, name)
         otel_package_import = f'opentelemetry.instrumentation.{otel_package}'
 
         if importlib.util.find_spec(otel_package_import) is None:
             packages[name] = otel_package
 
     # Drop packages that are dependencies of other packages.
-    if packages.get('starlette') and packages.get('fastapi'):  # pragma: no branch
-        del packages['starlette']  # pragma: no cover
+    if packages.get('starlette') and packages.get('fastapi'):
+        del packages['starlette']
 
     for name, otel_package in sorted(packages.items()):
         package_name = otel_package.replace('.', '-')
         import_name = otel_package.replace('-', '_')
         link = f'[link={BASE_OTEL_INTEGRATION_URL}/{import_name}/{import_name}.html]opentelemetry-instrumentation-{package_name}[/link]'
         table.add_row(name, link)
 
@@ -208,41 +225,39 @@
     """Authenticate with Logfire.
 
     This command will authenticate you with Logfire, and store the credentials.
     """
     console = Console(file=sys.stderr)
     logfire_url = cast(str, args.logfire_url)
 
-    if DEFAULT_FILE.is_file():  # pragma: no cover
+    if DEFAULT_FILE.is_file():
         data = cast(DefaultFile, read_toml_file(DEFAULT_FILE))
-        if is_logged_in(data, logfire_url):
+        if is_logged_in(data, logfire_url):  # pragma: no branch
             console.print(f'You are already logged in. (Your credentials are stored in [bold]{DEFAULT_FILE}[/])')
             return
     else:
         data: DefaultFile = {'tokens': {}}
 
     console.print()
     console.print('Welcome to Logfire! :fire:')
     console.print('Before you can send data to Logfire, we need to authenticate you.')
     console.print()
 
-    with requests.Session() as session:
-        device_code, frontend_auth_url = request_device_code(session, logfire_url)
-        console.input('Press [bold]Enter[/] to open logfire.dev in your browser...')
-        try:
-            webbrowser.open(frontend_auth_url, new=2)
-        except webbrowser.Error:  # pragma: no cover
-            pass
-        console.print(f"Please open [bold]{frontend_auth_url}[/] in your browser to authenticate if it hasn't already.")
-        console.print('Waiting for you to authenticate with Logfire...')
+    device_code, frontend_auth_url = request_device_code(args._session, logfire_url)
+    console.input('Press [bold]Enter[/] to open logfire.dev in your browser...')
+    try:
+        webbrowser.open(frontend_auth_url, new=2)
+    except webbrowser.Error:
+        pass
+    console.print(f"Please open [bold]{frontend_auth_url}[/] in your browser to authenticate if it hasn't already.")
+    console.print('Waiting for you to authenticate with Logfire...')
 
-        data['tokens'][logfire_url] = poll_for_token(session, device_code, logfire_url)
-        console.print('Successfully authenticated!')
+    data['tokens'][logfire_url] = poll_for_token(args._session, device_code, logfire_url)
+    console.print('Successfully authenticated!')
 
-    HOME_LOGFIRE.mkdir(exist_ok=True)
     # There's no standard library package to write TOML files, so we'll write it manually.
     with DEFAULT_FILE.open('w') as f:
         for url, info in data['tokens'].items():
             f.write(f'[tokens."{url}"]\n')
             f.write(f'token = "{info["token"]}"\n')
             f.write(f'expiration = "{info["expiration"]}"\n')
 
@@ -251,80 +266,74 @@
     # TODO(Marcelo): Add a message to inform which commands can be used.
 
 
 def parse_list_projects(args: argparse.Namespace) -> None:
     """List user projects."""
     logfire_url = args.logfire_url
     console = Console(file=sys.stderr)
-    with requests.Session() as session:
-        projects = LogfireCredentials.get_user_projects(session=session, logfire_api_url=logfire_url)
-        # TODO(Marcelo): Add a test for this scenario.
-        if projects:  # pragma: no cover
-            table = Table()
-            table.add_column('Organization')
-            table.add_column('Project')
-            for project in projects:
-                table.add_row(project['organization_name'], project['project_name'])
-            console.print(table)
-        else:
-            console.print(
-                "No projects found for the current user. You can create a new project by 'logfire projects create' command"
-            )
+    projects = LogfireCredentials.get_user_projects(session=args._session, logfire_api_url=logfire_url)
+    if projects:
+        table = Table()
+        table.add_column('Organization')
+        table.add_column('Project')
+        for project in projects:
+            table.add_row(project['organization_name'], project['project_name'])
+        console.print(table)
+    else:
+        console.print(
+            "No projects found for the current user. You can create a new project by 'logfire projects create' command"
+        )
+
+
+def _write_credentials(project_info: dict[str, Any], data_dir: Path, logfire_api_url: str) -> LogfireCredentials:
+    try:
+        credentials = LogfireCredentials(**project_info, logfire_api_url=logfire_api_url)
+        credentials.write_creds_file(data_dir)
+        return credentials
+    except TypeError as e:
+        raise LogfireConfigError(f'Invalid credentials, when initializing project: {e}') from e
 
 
 def parse_create_new_project(args: argparse.Namespace) -> None:
     """Create a new project."""
     data_dir = Path(args.data_dir)
     logfire_url = args.logfire_url
     project_name = args.project_name
     organization = args.org
     default_organization = args.default_org
     console = Console(file=sys.stderr)
-    with requests.Session() as session:
-        project_info = LogfireCredentials.create_new_project(
-            session=session,
-            logfire_api_url=logfire_url,
-            organization=organization,
-            default_organization=default_organization,
-            project_name=project_name,
-        )
-    try:
-        credentials = LogfireCredentials(**project_info, logfire_api_url=logfire_url)
-        credentials.write_creds_file(data_dir)
-        console.print(f'Project created successfully. You will be able to view it at: {credentials.project_url}')
-    except TypeError as e:  # pragma: no cover
-        raise LogfireConfigError(f'Invalid credentials, when initializing project: {e}') from e
+    project_info = LogfireCredentials.create_new_project(
+        session=args._session,
+        logfire_api_url=logfire_url,
+        organization=organization,
+        default_organization=default_organization,
+        project_name=project_name,
+    )
+    credentials = _write_credentials(project_info, data_dir, logfire_url)
+    console.print(f'Project created successfully. You will be able to view it at: {credentials.project_url}')
 
 
 def parse_use_project(args: argparse.Namespace) -> None:
     """Use an existing project."""
     data_dir = Path(args.data_dir)
     logfire_url = args.logfire_url
     project_name = args.project_name
     organization = args.org
     console = Console(file=sys.stderr)
-    with requests.Session() as session:
-        projects = LogfireCredentials.get_user_projects(session=session, logfire_api_url=logfire_url)
-        project_info = LogfireCredentials.use_existing_project(
-            session=session,
-            logfire_api_url=logfire_url,
-            projects=projects,
-            organization=organization,
-            project_name=project_name,
-        )
-        # TODO(Marcelo): We should test when `project_info` is None, and maybe send a message to the user.
-        if project_info:  # pragma: no branch
-            try:
-                credentials = LogfireCredentials(**project_info, logfire_api_url=logfire_url)
-                credentials.write_creds_file(data_dir)
-                console.print(
-                    f'Project configured successfully. You will be able to view it at: {credentials.project_url}'
-                )
-            except TypeError as e:  # pragma: no cover
-                raise LogfireConfigError(f'Invalid credentials, when initializing project: {e}') from e
+    projects = LogfireCredentials.get_user_projects(session=args._session, logfire_api_url=logfire_url)
+    project_info = LogfireCredentials.use_existing_project(
+        session=args._session,
+        logfire_api_url=logfire_url,
+        projects=projects,
+        organization=organization,
+        project_name=project_name,
+    )
+    if project_info:
+        credentials = _write_credentials(project_info, data_dir, logfire_url)
+        console.print(f'Project configured successfully. You will be able to view it at: {credentials.project_url}')
 
 
 def main(args: list[str] | None = None) -> None:
     """Run the CLI."""
     parser = argparse.ArgumentParser(
         prog='logfire',
         description='The CLI for Pydantic Logfire.',
@@ -345,14 +354,15 @@
     cmd_backfill.add_argument('--data-dir', default='.logfire')
     cmd_backfill.add_argument('--file', default='logfire_spans.bin')
     cmd_backfill.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help=argparse.SUPPRESS)
     cmd_backfill.set_defaults(func=parse_backfill)
 
     cmd_clean = subparsers.add_parser('clean', help='Remove the contents of the Logfire data directory')
     cmd_clean.add_argument('--data-dir', default='.logfire')
+    cmd_clean.add_argument('--logs', action='store_true', default=False, help='Remove the Logfire logs.')
     cmd_clean.set_defaults(func=parse_clean)
 
     cmd_inspect = subparsers.add_parser(
         'inspect',
         help="Suggest opentelemetry instrumentations based on your environment's installed packages",
     )
     cmd_inspect.set_defaults(func=parse_inspect)
@@ -381,11 +391,25 @@
     cmd_projects_use.add_argument('project_name', help='Project name.')
     cmd_projects_use.add_argument('--org', help='Project organization.')
     cmd_projects_use.add_argument('--data-dir', default='.logfire')
     cmd_projects_use.add_argument('--logfire-url', default=LOGFIRE_BASE_URL, help='Logfire API URL.')
     cmd_projects_use.set_defaults(func=parse_use_project)
 
     namespace = parser.parse_args(args)
-    if namespace.version:
-        version_callback()
-    else:
-        namespace.func(namespace)
+
+    trace.set_tracer_provider(tracer_provider=SDKTracerProvider())
+    tracer = trace.get_tracer(__name__)
+
+    def log_trace_id(response: requests.Response, context: ContextCarrier, *args: Any, **kwargs: Any) -> None:
+        logger.debug('context=%s url=%s', context, response.url)
+
+    with tracer.start_as_current_span('logfire._internal.cli'):
+        with requests.Session() as session:
+            context = get_context()
+            session.hooks = {'response': functools.partial(log_trace_id, context=context)}
+            session.headers.update(context)
+            namespace._session = session
+
+            if namespace.version:
+                version_callback()
+            else:
+                namespace.func(namespace)
```

### Comparing `logfire-0.23.0/logfire/exporters/_fallback.py` & `logfire-0.24.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.23.0/logfire/exporters/_file.py` & `logfire-0.24.0/logfire/_internal/exporters/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from google.protobuf.json_format import MessageToJson
 from opentelemetry.exporter.otlp.proto.common.trace_encoder import encode_spans
 from opentelemetry.proto.collector.trace.v1.trace_service_pb2 import ExportTraceServiceRequest
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SpanExporter, SpanExportResult
 from typing_extensions import assert_never
 
-from .._constants import DEFAULT_FALLBACK_FILE_NAME
-from .._utils import ensure_data_dir_exists
+from ..constants import DEFAULT_FALLBACK_FILE_NAME
+from ..utils import ensure_data_dir_exists
 
 HEADER = b'LOGFIRE BACKUP FILE\n'
 VERSION = b'VERSION 1\n'
 
 
 class Writer:
     def write_header(self) -> bytes:
@@ -52,15 +52,15 @@
         writer = Writer()
         with self._lock:
             if not self._file:
                 if isinstance(self.file_path, Path):
                     ensure_data_dir_exists(self.file_path.parent)
                     if self._warn:
                         warnings.warn(
-                            f'Failed to export spans, writing to fallback file: {self.file_path}',
+                            f'Failed to export spans, writing to fallback file: {self.file_path.absolute()}',
                             WritingFallbackWarning,
                         )
                     self._file = self.file_path.open('ab')
                 else:
                     self._file = self.file_path
                 self._file.seek(0, os.SEEK_END)
                 if self._file.tell() == 0:
```

### Comparing `logfire-0.23.0/logfire/exporters/_otlp.py` & `logfire-0.24.0/logfire/_internal/exporters/otlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SpanExportResult
 from requests import Session
 from requests.models import PreparedRequest, Response
 
 import logfire
-from logfire._stack_info import STACK_INFO_KEYS
-from logfire._utils import truncate_string
-from logfire.exporters._wrapper import WrapperSpanExporter
+
+from ..stack_info import STACK_INFO_KEYS
+from ..utils import truncate_string
+from .wrapper import WrapperSpanExporter
 
 
 class OTLPExporterHttpSession(Session):
     """A requests.Session subclass that raises a BodyTooLargeError if the request body is too large."""
 
     def __init__(self, *args: Any, max_body_size: int, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
```

### Comparing `logfire-0.23.0/logfire/exporters/_processor_wrapper.py` & `logfire-0.24.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 from urllib.parse import urlparse
 
 from opentelemetry import context
 from opentelemetry.sdk.trace import ReadableSpan, Span, SpanProcessor
 from opentelemetry.semconv.trace import SpanAttributes
 
-from logfire._constants import (
+from ..constants import (
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     PENDING_SPAN_NAME_SUFFIX,
     log_level_attributes,
 )
-from logfire._scrubbing import Scrubber
-from logfire._utils import ReadableSpanDict, span_to_dict
+from ..scrubbing import Scrubber
+from ..utils import ReadableSpanDict, span_to_dict
 
 
 class SpanProcessorWrapper(SpanProcessor):
     """Wrapper around other processors to intercept starting and ending spans with our own global logic.
 
     Suppresses starting/ending if the current context has a `suppress_instrumentation` value.
     Tweaks the send/receive span names generated by the ASGI middleware.
```

### Comparing `logfire-0.23.0/logfire/exporters/_remove_pending.py` & `logfire-0.24.0/logfire/_internal/exporters/remove_pending.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Sequence
 
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SpanExportResult
 
-from logfire._constants import ATTRIBUTES_SPAN_TYPE_KEY
-from logfire.exporters._wrapper import WrapperSpanExporter
+from ..constants import ATTRIBUTES_SPAN_TYPE_KEY
+from .wrapper import WrapperSpanExporter
 
 
 class RemovePendingSpansExporter(WrapperSpanExporter):
     """An exporter that filters out pending spans if the corresponding final span is already in the same batch."""
 
     def export(self, spans: Sequence[ReadableSpan]) -> SpanExportResult:
         result: list[ReadableSpan] = []
```

### Comparing `logfire-0.23.0/logfire/exporters/_wrapper.py` & `logfire-0.24.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.23.0/logfire/exporters/console.py` & `logfire-0.24.0/logfire/_internal/exporters/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 from opentelemetry.sdk.trace.export import SpanExporter, SpanExportResult
 from opentelemetry.util import types as otel_types
 from rich.columns import Columns
 from rich.console import Console, Group
 from rich.syntax import Syntax
 from rich.text import Text
 
-from .._constants import (
+from ..constants import (
     ATTRIBUTES_JSON_SCHEMA_KEY,
-    ATTRIBUTES_LOG_LEVEL_NAME_KEY,
     ATTRIBUTES_LOG_LEVEL_NUM_KEY,
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_PENDING_SPAN_REAL_PARENT_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     ATTRIBUTES_TAGS_KEY,
     DISABLE_CONSOLE_KEY,
     LEVEL_NUMBERS,
+    NUMBER_TO_LEVEL,
     ONE_SECOND_IN_NANOSECONDS,
 )
-from .._json_formatter import json_args_value_formatter
+from ..json_formatter import json_args_value_formatter
 
 ConsoleColorsValues = Literal['auto', 'always', 'never']
 _WARN_LEVEL = LEVEL_NUMBERS['warn']
 _ERROR_LEVEL = LEVEL_NUMBERS['error']
 
 # A list of (text, style) pairs that can be passed to rich's `Text.assemble`.
 # When logging without colors, just the text is used in a plain `print`.
@@ -171,15 +171,16 @@
 
         file_location: str = span.attributes.get('code.filepath')  # type: ignore
         if file_location:
             lineno = span.attributes.get('code.lineno')
             if lineno:  # pragma: no branch
                 file_location += f':{lineno}'
 
-        log_level = span.attributes.get(ATTRIBUTES_LOG_LEVEL_NAME_KEY) or ''
+        log_level_num: int = span.attributes.get(ATTRIBUTES_LOG_LEVEL_NUM_KEY)  # type: ignore
+        log_level = NUMBER_TO_LEVEL.get(log_level_num, '')
 
         if file_location or log_level:
             return [
                 (indent_str, ''),
                 ('│', 'blue'),
                 (' ', ''),
                 (file_location, 'cyan'),
```

### Comparing `logfire-0.23.0/logfire/integrations/_executors.py` & `logfire-0.24.0/logfire/_internal/integrations/executors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import asdict
 from functools import partial
 from typing import Any, Callable
 
-from ..propagate import ContextCarrier, attach_context, get_context
+from logfire.propagate import ContextCarrier, attach_context, get_context
 
 try:
     # concurrent.futures does not work in pyodide
 
     from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
     submit_t_orig = ThreadPoolExecutor.submit
@@ -50,19 +50,19 @@
 except ImportError:  # pragma: no cover
 
     def instrument_executors() -> None:
         pass
 
 
 def serialize_config() -> dict[str, Any]:
-    from logfire import _config  # type: ignore
+    from ..config import GLOBAL_CONFIG
 
     # note: since `logfire.config._LogfireConfigData` is a dataclass
     # but `LogfireConfig` is not we only get the attributes from `_LogfireConfigData`
     # which is what we want here!
-    return asdict(_config.GLOBAL_CONFIG)
+    return asdict(GLOBAL_CONFIG)
 
 
 def deserialize_config(config: dict[str, Any]) -> None:
-    from logfire import _config  # type: ignore
+    from ..config import configure
 
-    _config.configure(**config)
+    configure(**config)
```

### Comparing `logfire-0.23.0/logfire/integrations/_fastapi.py` & `logfire-0.24.0/logfire/_internal/integrations/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.util.http import get_excluded_urls, parse_excluded_urls
 from starlette.requests import Request
 from starlette.websockets import WebSocket
 
 from logfire import Logfire
-from logfire._stack_info import StackInfo, get_code_object_info
+
+from ..stack_info import StackInfo, get_code_object_info
 
 
 def instrument_fastapi(
     logfire_instance: Logfire,
     app: FastAPI,
     *,
     request_attributes_mapper: Callable[
@@ -48,15 +49,15 @@
     if use_opentelemetry_instrumentation:
         FastAPIInstrumentor.instrument_app(app, excluded_urls=excluded_urls)  # type: ignore
 
     registry = patch_fastapi()
     if app in registry:  # pragma: no cover
         raise ValueError('This app has already been instrumented.')
 
-    registry[app] = Instrumentation(
+    registry[app] = FastAPIInstrumentation(
         logfire_instance,
         request_attributes_mapper or _default_request_attributes_mapper,
         excluded_urls,
     )
 
     @contextmanager
     def uninstrument_context():
@@ -72,15 +73,15 @@
 
     return uninstrument_context()
 
 
 @lru_cache  # only patch once
 def patch_fastapi():
     """Globally monkeypatch fastapi functions and return a dictionary for recording instrumentation config per app."""
-    registry: WeakKeyDictionary[FastAPI, Instrumentation] = WeakKeyDictionary()
+    registry: WeakKeyDictionary[FastAPI, FastAPIInstrumentation] = WeakKeyDictionary()
 
     async def patched_solve_dependencies(*, request: Request | WebSocket, **kwargs: Any):
         result = await original_solve_dependencies(request=request, **kwargs)
         if instrumentation := registry.get(request.app):
             return await instrumentation.solve_dependencies(request, result)
         else:
             return result
@@ -103,15 +104,15 @@
 
     original_run_endpoint_function = fastapi.routing.run_endpoint_function
     fastapi.routing.run_endpoint_function = patched_run_endpoint_function
 
     return registry
 
 
-class Instrumentation:
+class FastAPIInstrumentation:
     def __init__(
         self,
         logfire_instance: Logfire,
         request_attributes_mapper: Callable[
             [
                 Request | WebSocket,
                 dict[str, Any],
```

### Comparing `logfire-0.23.0/logfire/integrations/pydantic_plugin.py` & `logfire-0.24.0/logfire/integrations/pydantic.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Callable, Literal, TypedDict, TypeVar
 
 from typing_extensions import ParamSpec
 
 import logfire
 from logfire import LogfireSpan
-from logfire._config import GLOBAL_CONFIG
+
+from .._internal.config import GLOBAL_CONFIG
 
 if TYPE_CHECKING:  # pragma: no cover
     from pydantic import ValidationError
     from pydantic.plugin import (
         SchemaKind,
         SchemaTypePath,
     )
@@ -25,19 +26,19 @@
 METER = GLOBAL_CONFIG._meter_provider.get_meter('pydantic-plugin-meter')  # type: ignore
 validation_counter = METER.create_counter('pydantic.validations')
 
 
 class PluginSettings(TypedDict, total=False):
     """A typed dict for the Pydantic plugin settings.
 
-    This is how you can use the [`PluginSettings`][logfire.integrations.pydantic_plugin.PluginSettings]
+    This is how you can use the [`PluginSettings`][logfire.integrations.pydantic.PluginSettings]
     with a Pydantic model:
 
     ```py
-    from logfire.integrations.pydantic_plugin import PluginSettings
+    from logfire.integrations.pydantic import PluginSettings
     from pydantic import BaseModel
 
 
     class Model(BaseModel, plugin_settings=PluginSettings(logfire={'record': 'all'})):
         a: int
     ```
     """
@@ -252,16 +253,15 @@
         schema: The schema to get the name for.
 
     Returns:
         The name of the schema.
     """
     if schema['type'] in {'model', 'dataclass'}:
         return schema['cls'].__name__  # type: ignore
-    # TODO(Marcelo): This should be tested.
-    elif schema['type'] in {'function-after', 'function-before', 'function-wrap'}:  # pragma: no cover
+    elif schema['type'] in {'function-after', 'function-before', 'function-wrap'}:
         return get_schema_name(schema['schema'])  # type: ignore
     elif schema['type'] == 'definitions':
         inner_schema = schema['schema']
         if inner_schema['type'] == 'definition-ref':
             schema_ref: str = inner_schema['schema_ref']  # type: ignore
             [schema_definition] = [
                 definition
@@ -318,55 +318,49 @@
             record = logfire_settings['record']
         else:
             record = GLOBAL_CONFIG.pydantic_plugin.record
 
         if record == 'off':
             return None, None, None
 
-        if _include_model(schema, schema_type_path):
+        if _include_model(schema_type_path):
             _patch_build_wrapper()
             return (
                 _ValidateWrapper('validate_python', schema, config, plugin_settings, schema_type_path, record),
                 _ValidateWrapper('validate_json', schema, config, plugin_settings, schema_type_path, record),
                 _ValidateWrapper('validate_strings', schema, config, plugin_settings, schema_type_path, record),
             )
 
         return None, None, None
 
 
 plugin = LogfirePydanticPlugin()
 
-# set of modules to ignore completed
-IGNORED_MODULE_PREFIXES: tuple[str, ...] = 'fastapi.', 'logfire_backend.'
+# set of modules to ignore completely
+IGNORED_MODULES: tuple[str, ...] = 'fastapi', 'logfire_backend', 'fastui'
+IGNORED_MODULE_PREFIXES: tuple[str, ...] = tuple(f'{module}.' for module in IGNORED_MODULES)
 
 
-def _include_model(schema: CoreSchema, schema_type_path: SchemaTypePath) -> bool:
+def _include_model(schema_type_path: SchemaTypePath) -> bool:
     """Check whether a model should be instrumented."""
     include = GLOBAL_CONFIG.pydantic_plugin.include
     exclude = GLOBAL_CONFIG.pydantic_plugin.exclude
 
-    schema_type = schema['type']
-    if schema_type in {'function-after', 'function-before', 'function-wrap'}:  # pragma: no cover
-        return _include_model(schema['schema'])  # type: ignore
-
     # check if the model is in ignored model
-    if any(schema_type_path.module.startswith(prefix) for prefix in IGNORED_MODULE_PREFIXES):  # pragma: no cover
+    module = schema_type_path.module
+    if module.startswith(IGNORED_MODULE_PREFIXES) or module in IGNORED_MODULES:  # pragma: no cover
         return False
 
     # check if the model is in exclude models
-    if exclude and any(
-        re.search(f'{pattern}$', f'{schema_type_path.module}::{schema_type_path.name}') for pattern in exclude
-    ):
+    if exclude and any(re.search(f'{pattern}$', f'{module}::{schema_type_path.name}') for pattern in exclude):
         return False
 
     # check if the model is in include models
     if include:
-        return any(
-            re.search(f'{pattern}$', f'{schema_type_path.module}::{schema_type_path.name}') for pattern in include
-        )
+        return any(re.search(f'{pattern}$', f'{module}::{schema_type_path.name}') for pattern in include)
     return True
 
 
 @lru_cache  # only patch once
 def _patch_build_wrapper():
     """The old pydantic plugin API required managing state between event handler methods.
```

### Comparing `logfire-0.23.0/logfire/integrations/structlog.py` & `logfire-0.24.0/logfire/integrations/structlog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Logfire processor for structlog."""
 
 from structlog.types import EventDict, WrappedLogger
 
 import logfire
-from logfire.integrations.logging import RESERVED_ATTRS
+
+from .logging import RESERVED_ATTRS as LOGGING_RESERVED_ATTRS
 
 _STRUCTLOG_CALL_OFFSET = 5
 """The offset to the stack to find the caller of the structlog event."""
 
-_STRIP_FROM_EVENT = ('level', 'event', 'timestamp')
+RESERVED_ATTRS = LOGGING_RESERVED_ATTRS | {'level', 'event', 'timestamp'}
 """Attributes to strip from the event before sending to Logfire."""
 
 
 class LogfireProcessor:
     """Logfire processor for structlog."""
 
     def __init__(self, *, console_log: bool = False) -> None:
         self.console_log = console_log
 
     def __call__(self, logger: WrappedLogger, name: str, event_dict: EventDict) -> EventDict:
         """A middleware to process structlog event, and send it to **Logfire**."""
-        attributes = {k: v for k, v in event_dict.items() if k not in RESERVED_ATTRS + _STRIP_FROM_EVENT}
+        attributes = {k: v for k, v in event_dict.items() if k not in RESERVED_ATTRS}
         level = event_dict.get('level', 'info').lower()
         # NOTE: An event can be `None` in structlog. We may want to create a default msg in those cases.
         msg_template = event_dict.get('event') or 'structlog event'
         logfire.log(
             level=level,  # type: ignore
             msg_template=msg_template,
             attributes=attributes,
```

### Comparing `logfire-0.23.0/logfire/propagate.py` & `logfire-0.24.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.23.0/logfire/testing.py` & `logfire-0.24.0/logfire/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 """Testing utilities for Logfire."""
 from __future__ import annotations
 
+import os
 import random
+import re
 import sys
 from collections.abc import Sequence
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Mapping, cast
 
 import pytest
 from opentelemetry import trace
 from opentelemetry.sdk.metrics.export import InMemoryMetricReader
 from opentelemetry.sdk.trace import Event, ReadableSpan
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor, SpanExporter, SpanExportResult
 from opentelemetry.sdk.trace.id_generator import IdGenerator
+from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.semconv.trace import SpanAttributes
 from pydantic import BaseModel
 
 import logfire
-from logfire._constants import ATTRIBUTES_SPAN_TYPE_KEY, ONE_SECOND_IN_NANOSECONDS, RESOURCE_ATTRIBUTES_PACKAGE_VERSIONS
+
+from ._internal.constants import (
+    ATTRIBUTES_SPAN_TYPE_KEY,
+    ONE_SECOND_IN_NANOSECONDS,
+    RESOURCE_ATTRIBUTES_PACKAGE_VERSIONS,
+)
 
 
 class TestExporter(SpanExporter):
     """A SpanExporter that stores exported spans in a list for asserting in tests."""
 
     # NOTE: Avoid test discovery by pytest.
     __test__ = False
@@ -67,14 +75,20 @@
                 except ValueError:  # pragma: no cover
                     return value
             if name == 'code.lineno' and fixed_line_number is not None:
                 return fixed_line_number
             if name == 'code.function':
                 if sys.version_info >= (3, 11) and _strip_function_qualname:
                     return value.split('.')[-1]
+            if name == ResourceAttributes.PROCESS_PID:
+                assert value == os.getpid()
+                return 1234
+            if name == ResourceAttributes.SERVICE_INSTANCE_ID:
+                if re.match(r'^[0-9a-f]{32}$', value):
+                    return '0' * 32
             return value
 
         def build_attributes(attributes: Mapping[str, Any] | None) -> dict[str, Any] | None:
             if attributes is None:  # pragma: no branch
                 return None  # pragma: no cover
             attributes = {
                 k: process_attribute(k, v)
@@ -122,16 +136,17 @@
                 'start_time': span.start_time,
                 'end_time': span.end_time,
                 'attributes': build_attributes(span.attributes),
             }
             if span.events:
                 res['events'] = [build_event(event) for event in span.events]
             if include_resources:
+                resource_attributes = build_attributes(span.resource.attributes)
                 res['resource'] = {
-                    'attributes': build_attributes(span.resource.attributes),
+                    'attributes': resource_attributes,
                 }
             return res
 
         spans = [build_span(span) for span in self.exported_spans]
         return [
             span
             for span in spans
```

### Comparing `logfire-0.23.0/pyproject.toml` & `logfire-0.24.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # TODO revert this file to hatchling using https://github.com/pydantic/platform/pull/264/commits/01e4d2258776f98284d019d5040eceeb5e9af42f
 # when we move it to a new repo
 
 [tool.poetry]
 name = "logfire"
-version = "0.23.0"
+version = "0.24.0"
 description = "Coming soon..."
 authors = [
     "Pydantic Team <engineering@pydantic.dev>",
     "Samuel Colvin <samuel@pydantic.dev>",
     "Hasan Ramezani <hasan@pydantic.dev>",
     "Adrian Garcia Badaracco <adrian@pydantic.dev>",
     "David Montague <david@pydantic.dev>",
@@ -60,14 +60,15 @@
 gitpython = { version = ">=3.1.40", optional = true }
 devtools = { version = "^0.12.2", optional = true }
 requests-mock = { version = "*", optional = true }
 inline-snapshot = { version = ">=0", optional = true }
 eval-type-backport = { version = "^0.1.3", optional = true }
 pytest-django = { version = "^4.8.0", optional = true }
 structlog = { version = ">=21.1.0", optional = true }
+loguru = { version = "*", optional = true }
 
 [tool.poetry.extras]
 system-metrics = ["opentelemetry-instrumentation-system-metrics"]
 aiohttp = ["opentelemetry-instrumentation-aiohttp-client"]
 celery = ["opentelemetry-instrumentation-celery"]
 django = ["opentelemetry-instrumentation-django"]
 fastapi = ["opentelemetry-instrumentation-fastapi"]
@@ -107,21 +108,22 @@
     "opentelemetry-instrumentation-system-metrics",
     "gitpython",
     "devtools",
     "eval-type-backport",
     "requests-mock",
     "inline-snapshot",
     "structlog",
+    "loguru",
 ]
 
 [tool.poetry.scripts]
 logfire = "logfire.cli:main"
 
 [tool.poetry.plugins."pydantic"]
-logfire-plugin = "logfire.integrations.pydantic_plugin:plugin"
+logfire-plugin = "logfire.integrations.pydantic:plugin"
 
 [tool.poetry.plugins."pytest11"]
 logfire = "logfire.testing"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `logfire-0.23.0/PKG-INFO` & `logfire-0.24.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfire
-Version: 0.23.0
+Version: 0.24.0
 Summary: Coming soon...
 License: MIT
 Author: Pydantic Team
 Author-email: engineering@pydantic.dev
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,15 @@
 Requires-Dist: dirty-equals (>=0.6.0) ; extra == "test"
 Requires-Dist: django (>=3.2.0) ; extra == "test"
 Requires-Dist: eval-type-backport (>=0.1.3,<0.2.0) ; extra == "test"
 Requires-Dist: fastapi (>=0.68.0) ; extra == "test"
 Requires-Dist: gitpython (>=3.1.40) ; extra == "test"
 Requires-Dist: httpx (>=0.22.0) ; extra == "test"
 Requires-Dist: inline-snapshot (>=0) ; extra == "test"
+Requires-Dist: loguru ; extra == "test"
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.21.0)
 Requires-Dist: opentelemetry-instrumentation (>=0.41b0)
 Requires-Dist: opentelemetry-instrumentation-aiohttp-client (>=0.42b0) ; extra == "aiohttp" or extra == "test"
 Requires-Dist: opentelemetry-instrumentation-asgi (>=0.42b0) ; extra == "test"
 Requires-Dist: opentelemetry-instrumentation-celery (>=0.42b0) ; extra == "celery"
 Requires-Dist: opentelemetry-instrumentation-django (>=0.42b0) ; extra == "django" or extra == "test"
 Requires-Dist: opentelemetry-instrumentation-fastapi (>=0.42b0) ; extra == "fastapi" or extra == "test"
```

