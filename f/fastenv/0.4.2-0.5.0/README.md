# Comparing `tmp/fastenv-0.4.2.tar.gz` & `tmp/fastenv-0.5.0.tar.gz`

## Comparing `fastenv-0.4.2.tar` & `fastenv-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastenv-0.4.2/fastenv/__init__.py
--rw-r--r--   0        0        0     8709 2020-02-02 00:00:00.000000 fastenv-0.4.2/fastenv/dotenv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastenv-0.4.2/fastenv/py.typed
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 fastenv-0.4.2/fastenv/types.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastenv-0.4.2/fastenv/utilities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastenv-0.4.2/fastenv/cloud/__init__.py
--rw-r--r--   0        0        0    40262 2020-02-02 00:00:00.000000 fastenv-0.4.2/fastenv/cloud/object_storage.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 fastenv-0.4.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastenv-0.4.2/LICENSE
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 fastenv-0.4.2/README.md
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 fastenv-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 fastenv-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastenv-0.5.0/fastenv/__init__.py
+-rw-r--r--   0        0        0     8709 2020-02-02 00:00:00.000000 fastenv-0.5.0/fastenv/dotenv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastenv-0.5.0/fastenv/py.typed
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 fastenv-0.5.0/fastenv/types.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastenv-0.5.0/fastenv/utilities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastenv-0.5.0/fastenv/cloud/__init__.py
+-rw-r--r--   0        0        0    40262 2020-02-02 00:00:00.000000 fastenv-0.5.0/fastenv/cloud/object_storage.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 fastenv-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastenv-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 fastenv-0.5.0/README.md
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 fastenv-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fastenv-0.5.0/PKG-INFO
```

### Comparing `fastenv-0.4.2/fastenv/__init__.py` & `fastenv-0.5.0/fastenv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     "ObjectStorageClient",
     "ObjectStorageConfig",
     "dotenv_values",
     "dump_dotenv",
     "find_dotenv",
     "load_dotenv",
 )
-__version__ = "0.4.2"
+__version__ = "0.5.0"
```

### Comparing `fastenv-0.4.2/fastenv/dotenv.py` & `fastenv-0.5.0/fastenv/dotenv.py`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.2/fastenv/types.py` & `fastenv-0.5.0/fastenv/types.py`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.2/fastenv/cloud/object_storage.py` & `fastenv-0.5.0/fastenv/cloud/object_storage.py`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.2/.gitignore` & `fastenv-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.2/LICENSE` & `fastenv-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastenv-0.4.2/README.md` & `fastenv-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -53,14 +53,49 @@
 # {'EXAMPLE_VARIABLE': 'example_value', 'I_THINK_FASTENV_IS': 'awesome'}
 # save the DotEnv instance to a file
 import anyio
 anyio.run(fastenv.dump_dotenv, dotenv)
 # Path('/path/to/this/dir/.env')
 ```
 
+Use fastenv in your FastAPI app:
+
+```py
+from contextlib import asynccontextmanager
+from typing import AsyncIterator, TypedDict
+
+import fastenv
+from fastapi import FastAPI, Request
+
+
+class LifespanState(TypedDict):
+    settings: fastenv.DotEnv
+
+
+@asynccontextmanager
+async def lifespan(_: FastAPI) -> AsyncIterator[LifespanState]:
+    """Configure app lifespan.
+
+    https://fastapi.tiangolo.com/advanced/events/
+    https://www.starlette.io/lifespan/
+    """
+    settings = await fastenv.load_dotenv(".env")
+    lifespan_state: LifespanState = {"settings": settings}
+    yield lifespan_state
+
+
+app = FastAPI(lifespan=lifespan)
+
+
+@app.get("/settings")
+async def get_settings(request: Request) -> dict[str, str]:
+    settings = request.state.settings
+    return dict(settings)
+```
+
 ## Documentation
 
 Documentation is built with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/), deployed on [Vercel](https://vercel.com/), and available at [fastenv.bws.bio](https://fastenv.bws.bio) and [fastenv.vercel.app](https://fastenv.vercel.app).
 
 [Vercel build configuration](https://vercel.com/docs/build-step):
 
 - Build command: `python3 -m pip install mkdocs-material && mkdocs build --site-dir public`
```

### Comparing `fastenv-0.4.2/pyproject.toml` & `fastenv-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
   "Topic :: System :: Installation/Setup",
   "Topic :: System :: Systems Administration",
   "Topic :: Utilities",
   "Typing :: Typed",
 ]
@@ -43,17 +44,18 @@
   "mkdocs-material>=9,<10",
 ]
 httpx = [
   "httpx>=0.23,<1",
 ]
 tests = [
   "coverage[toml]>=7,<8",
+  "fastapi>=0.110.1,<0.111",
   "freezegun>=1,<2",
   "httpx>=0.23,<1",
-  "pytest>=7,<8",
+  "pytest>=8.1.1,<9",
   "pytest-mock>=3,<4",
 ]
 
 [project.urls]
 Documentation = "https://fastenv.bws.bio"
 Homepage = "https://github.com/br3ndonland/fastenv"
 Repository = "https://github.com/br3ndonland/fastenv"
```

### Comparing `fastenv-0.4.2/PKG-INFO` & `fastenv-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastenv
-Version: 0.4.2
+Version: 0.5.0
 Summary: Unified environment variable and settings management for FastAPI and beyond.
 Project-URL: Documentation, https://fastenv.bws.bio
 Project-URL: Homepage, https://github.com/br3ndonland/fastenv
 Project-URL: Repository, https://github.com/br3ndonland/fastenv
 Author-email: Brendon Smith <bws@bws.bio>
 License-Expression: MIT
 License-File: LICENSE
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.8.1
@@ -32,18 +33,19 @@
 Requires-Dist: httpx<1,>=0.23; extra == 'cloud'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material<10,>=9; extra == 'docs'
 Provides-Extra: httpx
 Requires-Dist: httpx<1,>=0.23; extra == 'httpx'
 Provides-Extra: tests
 Requires-Dist: coverage[toml]<8,>=7; extra == 'tests'
+Requires-Dist: fastapi<0.111,>=0.110.1; extra == 'tests'
 Requires-Dist: freezegun<2,>=1; extra == 'tests'
 Requires-Dist: httpx<1,>=0.23; extra == 'tests'
 Requires-Dist: pytest-mock<4,>=3; extra == 'tests'
-Requires-Dist: pytest<8,>=7; extra == 'tests'
+Requires-Dist: pytest<9,>=8.1.1; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # ⚙️ fastenv 🚀
 
 _Unified environment variable and settings management for FastAPI and beyond_
 
 [![PyPI](https://img.shields.io/pypi/v/fastenv?color=success)](https://pypi.org/project/fastenv/)
@@ -97,14 +99,49 @@
 # {'EXAMPLE_VARIABLE': 'example_value', 'I_THINK_FASTENV_IS': 'awesome'}
 # save the DotEnv instance to a file
 import anyio
 anyio.run(fastenv.dump_dotenv, dotenv)
 # Path('/path/to/this/dir/.env')
 ```
 
+Use fastenv in your FastAPI app:
+
+```py
+from contextlib import asynccontextmanager
+from typing import AsyncIterator, TypedDict
+
+import fastenv
+from fastapi import FastAPI, Request
+
+
+class LifespanState(TypedDict):
+    settings: fastenv.DotEnv
+
+
+@asynccontextmanager
+async def lifespan(_: FastAPI) -> AsyncIterator[LifespanState]:
+    """Configure app lifespan.
+
+    https://fastapi.tiangolo.com/advanced/events/
+    https://www.starlette.io/lifespan/
+    """
+    settings = await fastenv.load_dotenv(".env")
+    lifespan_state: LifespanState = {"settings": settings}
+    yield lifespan_state
+
+
+app = FastAPI(lifespan=lifespan)
+
+
+@app.get("/settings")
+async def get_settings(request: Request) -> dict[str, str]:
+    settings = request.state.settings
+    return dict(settings)
+```
+
 ## Documentation
 
 Documentation is built with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/), deployed on [Vercel](https://vercel.com/), and available at [fastenv.bws.bio](https://fastenv.bws.bio) and [fastenv.vercel.app](https://fastenv.vercel.app).
 
 [Vercel build configuration](https://vercel.com/docs/build-step):
 
 - Build command: `python3 -m pip install mkdocs-material && mkdocs build --site-dir public`
```

