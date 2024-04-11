# Comparing `tmp/retried-6.4.0.tar.gz` & `tmp/retried-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retried-6.4.0.tar", last modified: Wed Mar 27 00:50:03 2024, max compression
+gzip compressed data, was "retried-7.0.0.tar", last modified: Thu Apr 11 16:54:20 2024, max compression
```

## Comparing `retried-6.4.0.tar` & `retried-7.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      102 2024-03-27 00:49:47.767948 retried-6.4.0/README.md
--rw-r--r--   0        0        0     1036 2024-03-27 00:50:03.564142 retried-6.4.0/pyproject.toml
--rw-r--r--   0        0        0      162 2024-03-27 00:49:47.767948 retried-6.4.0/src/retried/__init__.py
--rw-r--r--   0        0        0       18 2024-03-27 00:49:47.767948 retried-6.4.0/src/retried/__version__.py
--rw-r--r--   0        0        0     2290 2024-03-27 00:49:47.767948 retried-6.4.0/src/retried/aretry.py
--rw-r--r--   0        0        0     3274 2024-03-27 00:49:47.767948 retried-6.4.0/src/retried/retry.py
--rw-r--r--   0        0        0        0 2024-03-27 00:49:47.767948 retried-6.4.0/tests/__init__.py
--rw-r--r--   0        0        0      657 2024-03-27 00:49:47.767948 retried-6.4.0/tests/test_aretry.py
--rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 retried-6.4.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2024-04-11 16:54:03.856699 retried-7.0.0/README.md
+-rw-r--r--   0        0        0     1061 2024-04-11 16:54:20.036707 retried-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2024-04-11 16:54:03.856699 retried-7.0.0/src/retried/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-11 16:54:03.856699 retried-7.0.0/src/retried/__version__.py
+-rw-r--r--   0        0        0     2290 2024-04-11 16:54:03.856699 retried-7.0.0/src/retried/aretry.py
+-rw-r--r--   0        0        0     3270 2024-04-11 16:54:03.856699 retried-7.0.0/src/retried/retry.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:54:03.856699 retried-7.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-11 16:54:03.856699 retried-7.0.0/tests/test_aretry.py
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-7.0.0/PKG-INFO
```

### Comparing `retried-6.4.0/pyproject.toml` & `retried-7.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 [project]
 name = "retried"
-version = "6.4.0"
+version = "7.0.0"
 requires-python = ">=3.9"
 description = "A simple and powerful retrying library for Python"
 readme = "README.md"
-dependencies = [
-    "typing-extensions>=4.10.0",
-]
+dependencies = []
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
@@ -36,14 +34,17 @@
 
 [tool.ruff]
 line-length = 100
 fix = true
 show-fixes = true
 output-format = "full"
 
+[tool.ruff.format]
+quote-style = "single"
+
 [tool.ruff.lint]
 extend-select = [
     "W",
     "I",
     "N",
     "S",
     "PTH",
@@ -58,11 +59,13 @@
     "S311",
 ]
 
 [tool.ruff.lint.isort]
 lines-after-imports = 2
 force-single-line = true
 force-sort-within-sections = true
-known-local-folder = []
+known-local-folder = [
+    "retried",
+]
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `retried-6.4.0/src/retried/aretry.py` & `retried-7.0.0/src/retried/aretry.py`

 * *Files identical despite different names*

### Comparing `retried-6.4.0/src/retried/retry.py` & `retried-7.0.0/src/retried/retry.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,80 +3,83 @@
 from itertools import cycle
 from itertools import repeat
 import logging
 import time
 import typing as t
 
 
-try:
-    from typing import ParamSpec
-except ImportError:
-    from typing_extensions import ParamSpec  # type: ignore[assignment]
+# try:
+#     from typing import ParamSpec
+# except ImportError:
+#     from typing_extensions import ParamSpec  # type: ignore[assignment]
+# P = ParamSpec('P')  # https://docs.python.org/zh-tw/3/library/typing.html#typing.ParamSpec
+# R = t.TypeVar('R')
+FuncT = t.Callable  # [P, R]
 
 
 logger = logging.getLogger(__package__)
 
 
-P = ParamSpec('P')  # https://docs.python.org/zh-tw/3/library/typing.html#typing.ParamSpec
-T = t.TypeVar('T')
-SingleOrTuple = t.Union[T, tuple[T, ...]]
-SingleOrIterable = t.Union[T, t.Iterable[T]]
+_T = t.TypeVar('_T')
+SingleOrTuple = t.Union[_T, tuple[_T, ...]]
+SingleOrIterable = t.Union[_T, t.Iterable[_T]]
 
+
+SleepT = t.Callable[[float], None]
 DelayT = float
 RetriesT = t.Optional[int]
+LogfT = t.Callable[[t.Any], None]
 
 
 class DummyLogger(logging.Logger):
-    def __init__(self, f: t.Callable):
-        self._f = f
+    def __init__(self, logf: LogfT):
+        self._logf = logf
         super().__init__(__package__)
 
     def _log(self, level, msg, *args, **kwargs):
-        self._f(msg)
+        self._logf(msg)
 
 
 def retry(
     retries: RetriesT = None,
     *,
     exceptions: SingleOrTuple[t.Type[Exception]] = Exception,
-    error_callback: t.Optional[
-        t.Callable[[int, Exception, DelayT, RetriesT, t.Callable[P, T]], None]
-    ] = None,
-    sleep: t.Callable[[float], None] = time.sleep,
+    error_callback: t.Optional[t.Callable[[int, Exception, DelayT, RetriesT, FuncT], None]] = None,
+    sleep: SleepT = time.sleep,
     delays: SingleOrIterable[DelayT] = 0,
     first_delay: t.Optional[DelayT] = None,
     chain_exception: bool = False,
-    logger: t.Union[logging.Logger, t.Callable[[t.Any], None]] = logger,
+    logger: t.Union[logging.Logger, LogfT] = logger,
 ):
     if not isinstance(delays, t.Iterable):
         delays = repeat(delays)
     delays = cycle(delays)
     if first_delay is None:
         first_delay = next(delays)
     if not isinstance(logger, logging.Logger):
         logger = DummyLogger(logger)
 
-    def _default_error_callback(i: int, e: Exception, d: DelayT, r: RetriesT, f: t.Callable[P, T]):
+    def _default_error_callback(i: int, e: Exception, d: DelayT, r: RetriesT, f: FuncT):
         log_prefix = f'tried {i} of {r}: {f.__code__.co_filename}:{f.__code__.co_firstlineno} {e!r}'
         is_last = i == r
         if not is_last:
             logger.info(f'{log_prefix} -> sleep {d} seconds')
         else:
             logger.warning(log_prefix)
 
     error_callback = error_callback or _default_error_callback
 
-    def callback(i: int, e: Exception, d: DelayT, r: RetriesT, f: t.Callable[P, T]):
+    def callback(i: int, e: Exception, d: DelayT, r: RetriesT, f: FuncT):
         error_callback(i, e, d, r, f)
         if i != r:
             sleep(d)
 
-    def decorator(f: t.Callable[P, T]) -> t.Callable[P, T]:
+    def decorator(f):
         @wraps(f)
-        def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+        def wrapper(*args, **kwargs):
             function_retrying = partial(f, *args, **kwargs)
             try:
                 # execute once
                 result = function_retrying()
             except exceptions as e:
                 # start retrying
                 i = 0
```

### Comparing `retried-6.4.0/tests/test_aretry.py` & `retried-7.0.0/tests/test_aretry.py`

 * *Files identical despite different names*

