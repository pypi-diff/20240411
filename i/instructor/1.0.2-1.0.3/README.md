# Comparing `tmp/instructor-1.0.2.tar.gz` & `tmp/instructor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.0.2.tar", max compression
+gzip compressed data, was "instructor-1.0.3.tar", max compression
```

## Comparing `instructor-1.0.2.tar` & `instructor-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-04-05 03:42:44.643954 instructor-1.0.2/LICENSE
--rw-r--r--   0        0        0     8979 2024-04-05 03:42:44.643954 instructor-1.0.2/README.md
--rw-r--r--   0        0        0     1185 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6494 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/cli/usage.py
--rw-r--r--   0        0        0     9586 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/client.py
--rw-r--r--   0        0        0     1712 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/client_anthropic.py
--rw-r--r--   0        0        0     1335 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/client_groq.py
--rw-r--r--   0        0        0     8968 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2642 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11016 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1733 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4381 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/exceptions.py
--rw-r--r--   0        0        0     7339 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/function_calls.py
--rw-r--r--   0        0        0      818 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/mode.py
--rw-r--r--   0        0        0     4820 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/patch.py
--rw-r--r--   0        0        0    12534 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/py.typed
--rw-r--r--   0        0        0     6171 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/retry.py
--rw-r--r--   0        0        0      266 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/test.py
--rw-r--r--   0        0        0     4373 2024-04-05 03:42:44.707954 instructor-1.0.2/instructor/utils.py
--rw-r--r--   0        0        0     2151 2024-04-05 03:42:44.711954 instructor-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    10659 1970-01-01 00:00:00.000000 instructor-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-05 13:30:03.247179 instructor-1.0.3/LICENSE
+-rw-r--r--   0        0        0     8979 2024-04-05 13:30:03.247179 instructor-1.0.3/README.md
+-rw-r--r--   0        0        0     1185 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3792 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/files.py
+-rw-r--r--   0        0        0     5348 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8255 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6494 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/usage.py
+-rw-r--r--   0        0        0     9586 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/client.py
+-rw-r--r--   0        0        0     1712 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     1335 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/client_groq.py
+-rw-r--r--   0        0        0     8968 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     7929 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2165 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2642 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11016 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1733 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4381 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/exceptions.py
+-rw-r--r--   0        0        0     7339 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/function_calls.py
+-rw-r--r--   0        0        0      818 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/mode.py
+-rw-r--r--   0        0        0     4820 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/patch.py
+-rw-r--r--   0        0        0    12534 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/py.typed
+-rw-r--r--   0        0        0     6171 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/retry.py
+-rw-r--r--   0        0        0     4373 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/utils.py
+-rw-r--r--   0        0        0     2154 2024-04-05 13:30:03.315180 instructor-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10662 1970-01-01 00:00:00.000000 instructor-1.0.3/PKG-INFO
```

### Comparing `instructor-1.0.2/LICENSE` & `instructor-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/README.md` & `instructor-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/__init__.py` & `instructor-1.0.3/instructor/__init__.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/_types/_alias.py` & `instructor-1.0.3/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/cli/cli.py` & `instructor-1.0.3/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/cli/files.py` & `instructor-1.0.3/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/cli/hub.py` & `instructor-1.0.3/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/cli/jobs.py` & `instructor-1.0.3/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/cli/usage.py` & `instructor-1.0.3/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/client.py` & `instructor-1.0.3/instructor/client.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/client_anthropic.py` & `instructor-1.0.3/instructor/client_anthropic.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/client_groq.py` & `instructor-1.0.3/instructor/client_groq.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/distil.py` & `instructor-1.0.3/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/dsl/citation.py` & `instructor-1.0.3/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/dsl/iterable.py` & `instructor-1.0.3/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/dsl/maybe.py` & `instructor-1.0.3/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/dsl/parallel.py` & `instructor-1.0.3/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/dsl/partial.py` & `instructor-1.0.3/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/dsl/simple_type.py` & `instructor-1.0.3/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/dsl/validators.py` & `instructor-1.0.3/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/function_calls.py` & `instructor-1.0.3/instructor/function_calls.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/mode.py` & `instructor-1.0.3/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/patch.py` & `instructor-1.0.3/instructor/patch.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/process_response.py` & `instructor-1.0.3/instructor/process_response.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/retry.py` & `instructor-1.0.3/instructor/retry.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/instructor/utils.py` & `instructor-1.0.3/instructor/utils.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.2/pyproject.toml` & `instructor-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "instructor"
-version = "1.0.2"
+version = "1.0.3"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^1.1.0"
-pydantic = "^2.0.2"
+pydantic = "^2.7.0b01"
 docstring-parser = "^0.15"
 typer = "^0.9.0"
 rich = "^13.7.0"
 aiohttp = "^3.9.1"
 tenacity = "^8.2.3"
 pydantic-core = "^2.18.0"
```

### Comparing `instructor-1.0.2/PKG-INFO` & `instructor-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.0.2
+Version: 1.0.3
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Requires-Dist: diskcache (>=5.6.3,<6.0.0) ; extra == "test-docs"
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0) ; extra == "test-docs"
 Requires-Dist: groq (>=0.4.2,<0.5.0) ; extra == "groq" or extra == "test-docs"
 Requires-Dist: litellm (>=1.0.0,<2.0.0) ; extra == "test-docs"
 Requires-Dist: openai (>=1.1.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "test-docs"
-Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic (>=2.7.0b01,<3.0.0)
 Requires-Dist: pydantic-core (>=2.18.0,<3.0.0)
 Requires-Dist: pydantic_extra_types (>=2.6.0,<3.0.0) ; extra == "test-docs"
 Requires-Dist: redis (>=5.0.1,<6.0.0) ; extra == "test-docs"
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "test-docs"
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
```

