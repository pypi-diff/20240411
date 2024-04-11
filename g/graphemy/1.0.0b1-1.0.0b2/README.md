# Comparing `tmp/graphemy-1.0.0b1.tar.gz` & `tmp/graphemy-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphemy-1.0.0b1.tar", max compression
+gzip compressed data, was "graphemy-1.0.0b2.tar", max compression
```

## Comparing `graphemy-1.0.0b1.tar` & `graphemy-1.0.0b2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      174 2024-03-02 04:18:14.613391 graphemy-1.0.0b1/graphemy/__init__.py
--rw-r--r--   0        0        0     5632 2024-03-03 14:45:13.570971 graphemy-1.0.0b1/graphemy/database/operations.py
--rw-r--r--   0        0        0     1394 2024-03-02 04:18:14.625389 graphemy-1.0.0b1/graphemy/database/utils.py
--rw-r--r--   0        0        0     2227 2024-03-03 14:45:12.700973 graphemy-1.0.0b1/graphemy/dl.py
--rw-r--r--   0        0        0     1356 2024-03-03 14:45:39.241519 graphemy-1.0.0b1/graphemy/models.py
--rw-r--r--   0        0        0     5357 2024-03-03 14:45:13.541973 graphemy-1.0.0b1/graphemy/router.py
--rw-r--r--   0        0        0     6744 2024-03-02 05:21:19.332121 graphemy-1.0.0b1/graphemy/schemas/generators.py
--rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0b1/graphemy/schemas/models.py
--rw-r--r--   0        0        0     2699 2024-03-03 14:44:06.277319 graphemy-1.0.0b1/graphemy/setup.py
--rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     2120 2024-03-21 16:21:24.994384 graphemy-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0b1/README.md
--rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 graphemy-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      174 2024-03-02 04:18:14.613391 graphemy-1.0.0b2/graphemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0b2/graphemy/database/__init__.py
+-rw-r--r--   0        0        0     5632 2024-03-03 14:45:13.570971 graphemy-1.0.0b2/graphemy/database/operations.py
+-rw-r--r--   0        0        0     1394 2024-03-02 04:18:14.625389 graphemy-1.0.0b2/graphemy/database/utils.py
+-rw-r--r--   0        0        0     2227 2024-03-03 14:45:12.700973 graphemy-1.0.0b2/graphemy/dl.py
+-rw-r--r--   0        0        0     1356 2024-03-03 14:45:39.241519 graphemy-1.0.0b2/graphemy/models.py
+-rw-r--r--   0        0        0     5359 2024-04-03 15:55:25.323324 graphemy-1.0.0b2/graphemy/router.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0b2/graphemy/schemas/__init__.py
+-rw-r--r--   0        0        0     6806 2024-04-10 15:08:41.241347 graphemy-1.0.0b2/graphemy/schemas/generators.py
+-rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0b2/graphemy/schemas/models.py
+-rw-r--r--   0        0        0     2699 2024-03-03 14:44:06.277319 graphemy-1.0.0b2/graphemy/setup.py
+-rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     2123 2024-04-10 15:10:15.725351 graphemy-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0b2/README.md
+-rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 graphemy-1.0.0b2/PKG-INFO
```

### Comparing `graphemy-1.0.0b1/graphemy/database/operations.py` & `graphemy-1.0.0b2/graphemy/database/operations.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b1/graphemy/database/utils.py` & `graphemy-1.0.0b2/graphemy/database/utils.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b1/graphemy/dl.py` & `graphemy-1.0.0b2/graphemy/dl.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b1/graphemy/models.py` & `graphemy-1.0.0b2/graphemy/models.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b1/graphemy/router.py` & `graphemy-1.0.0b2/graphemy/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         context_getter: Callable | None = None,
         permission_getter: Callable | None = None,
         dl_filter: Callable | None = None,
         query_filter: Callable | None = None,
         engine: Engine | Dict[str, Engine] = None,
         extensions: list = [],
         enable_queries: bool = True,
-        enable_put_mutations: bool = True,
-        enable_delete_mutations: bool = True,
+        enable_put_mutations: bool = False,
+        enable_delete_mutations: bool = False,
         **kwargs,
     ):
         functions: Dict[str, tuple] = {}
         Setup.setup(
             engine=engine,
             get_perm=permission_getter,
             query_filter=query_filter,
```

### Comparing `graphemy-1.0.0b1/graphemy/schemas/generators.py` & `graphemy-1.0.0b2/graphemy/schemas/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,17 @@
     # Define the return type using Strawberry's lazy type resolution
     return_type = Annotated[
         f'{class_type}Schema',
         strawberry.lazy('graphemy.router'),
     ]
     if is_list:
         return_type = list[return_type]
+    
+    else:
+        return_type = Optional[return_type]
 
     async def loader_func(
         self,
         info: Info,
         filters: Annotated[
             f'{class_type}Filter',
             strawberry.lazy('graphemy.router'),
```

### Comparing `graphemy-1.0.0b1/graphemy/setup.py` & `graphemy-1.0.0b2/graphemy/setup.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b1/LICENSE` & `graphemy-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b1/pyproject.toml` & `graphemy-1.0.0b2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphemy"
-version = "1.0.0-beta.1"
+version = "1.0.0-beta.2"
 description = "A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions."
 authors = ["Matheus Doreto <matheusdoreto.md@gmail.com>"]
 readme = "README.md"
 packages = [{include = "graphemy"}]
 homepage = "https://github.com/MDoreto/graphemy"
 documentation = "https://graphemy.readthedocs.io/en/latest/"
 repository = "https://github.com/MDoreto/graphemy"
@@ -60,13 +60,13 @@
 
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.taskipy.tasks]
-example = "uvicorn examples.music.main:app --reload --port 8001"
+example = "uvicorn examples.tutorial.main:app --reload --port 8001"
 lint = "blue . && isort ."
 docs = "mkdocs serve"
 pre_test = "task lint"
 test = "pytest -s -x --cov=graphemy -vv -W ignore::DeprecationWarning"
 post_test = "coverage html"
```

### Comparing `graphemy-1.0.0b1/README.md` & `graphemy-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b1/PKG-INFO` & `graphemy-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphemy
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions.
 Home-page: https://github.com/MDoreto/graphemy
 License: MIT
 Author: Matheus Doreto
 Author-email: matheusdoreto.md@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
```

