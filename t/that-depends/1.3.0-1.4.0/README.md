# Comparing `tmp/that_depends-1.3.0.tar.gz` & `tmp/that_depends-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.3.0.tar", max compression
+gzip compressed data, was "that_depends-1.4.0.tar", max compression
```

## Comparing `that_depends-1.3.0.tar` & `that_depends-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3794 2024-03-20 20:02:14.016047 that_depends-1.3.0/README.md
--rw-r--r--   0        0        0     1157 2024-03-20 20:15:06.819698 that_depends-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.3.0/that_depends/__init__.py
--rw-r--r--   0        0        0      655 2024-03-20 08:12:29.710111 that_depends-1.3.0/that_depends/container.py
--rw-r--r--   0        0        0     1016 2024-03-18 09:24:54.496625 that_depends-1.3.0/that_depends/injection.py
--rw-r--r--   0        0        0     4841 2024-03-20 20:06:58.946302 that_depends-1.3.0/that_depends/providers.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.3.0/that_depends/py.typed
--rw-r--r--   0        0        0     4274 1970-01-01 00:00:00.000000 that_depends-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3794 2024-03-20 20:02:14.016047 that_depends-1.4.0/README.md
+-rw-r--r--   0        0        0     1482 2024-04-11 11:53:40.084417 that_depends-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.4.0/that_depends/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.4.0/that_depends/container.py
+-rw-r--r--   0        0        0     1016 2024-03-18 09:24:54.496625 that_depends-1.4.0/that_depends/injection.py
+-rw-r--r--   0        0        0     4915 2024-04-11 11:51:20.009689 that_depends-1.4.0/that_depends/providers.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.4.0/that_depends/py.typed
+-rw-r--r--   0        0        0     4274 1970-01-01 00:00:00.000000 that_depends-1.4.0/PKG-INFO
```

### Comparing `that_depends-1.3.0/README.md` & `that_depends-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `that_depends-1.3.0/pyproject.toml` & `that_depends-1.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.3.0"
+version = "1.4.0"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
@@ -17,14 +17,15 @@
 litestar = "*"
 httpx = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 ruff = "*"
 mypy = "*"
+typing-extensions = "*"
 
 [tool.mypy]
 python_version = "3.12"
 strict = true
 
 [tool.ruff]
 fix = true
@@ -37,20 +38,27 @@
 ignore = [
     "D1", # allow missing docstrings
     "S101", # allow asserts
     "TCH", # ignore flake8-type-checking
     "FBT", # allow boolean args
     "ANN101", # missing-type-self
     "ANN102", # missing-type-cls
+    "D203", # "one-blank-line-before-class" conflicting with D211
+    "D213", # "multi-line-summary-second-line" conflicting with D212
+    "COM812", # flake8-commas "Trailing comma missing"
+    "ISC001", # flake8-implicit-str-concat
 ]
 
 [tool.ruff.lint.isort]
 lines-after-imports = 2
 no-lines-before = ["standard-library", "local-folder"]
 
 [tool.pytest.ini_options]
 addopts = "--cov=. --cov-report term-missing"
 asyncio_mode = "auto"
 
+[tool.coverage.report]
+exclude_also = ["if typing.TYPE_CHECKING:"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `that_depends-1.3.0/that_depends/injection.py` & `that_depends-1.4.0/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.3.0/that_depends/providers.py` & `that_depends-1.4.0/that_depends/providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     async def tear_down(self) -> None:
         """Tear down dependency."""
 
 
 class Resource(AbstractResource[T]):
     def __init__(
         self,
-        creator: typing.Callable[[], typing.Iterator[typing.Any]],
+        creator: typing.Callable[[], typing.Iterator[T]],
         *args: typing.Any,  # noqa: ANN401
         **kwargs: typing.Any,  # noqa: ANN401
     ) -> None:
         if not inspect.isgeneratorfunction(creator):
             msg = "Resource must be generator function"
             raise RuntimeError(msg)
 
@@ -70,15 +70,15 @@
             )
         return self._instance
 
 
 class AsyncResource(AbstractResource[T]):
     def __init__(
         self,
-        creator: typing.Callable[[], typing.AsyncIterator[typing.Any]],
+        creator: typing.Callable[[], typing.AsyncIterator[T]],
         *args: typing.Any,  # noqa: ANN401
         **kwargs: typing.Any,  # noqa: ANN401
     ) -> None:
         if not inspect.isasyncgenfunction(creator):
             msg = "AsyncResource must be async generator function"
             raise RuntimeError(msg)
 
@@ -123,15 +123,15 @@
         return self._factory(
             *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
             **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
         )
 
 
 class List(AbstractProvider[T]):
-    def __init__(self, *providers: AbstractProvider[typing.Any]) -> None:
+    def __init__(self, *providers: AbstractProvider[T]) -> None:
         self._providers = providers
 
     async def resolve(self) -> list[T]:  # type: ignore[override]
         return [await x.resolve() for x in self._providers]
 
     async def __call__(self) -> list[T]:  # type: ignore[override]
         return await self.resolve()
@@ -151,7 +151,11 @@
 
         if not self._instance:
             self._instance = self._factory(
                 *[await x() if isinstance(x, AbstractProvider) else x for x in self._args],
                 **{k: await v() if isinstance(v, AbstractProvider) else v for k, v in self._kwargs.items()},
             )
         return self._instance
+
+    async def tear_down(self) -> None:
+        if self._instance:
+            self._instance = None
```

### Comparing `that_depends-1.3.0/PKG-INFO` & `that_depends-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.3.0
+Version: 1.4.0
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

