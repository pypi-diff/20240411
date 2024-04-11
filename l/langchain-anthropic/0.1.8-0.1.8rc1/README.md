# Comparing `tmp/langchain_anthropic-0.1.8.tar.gz` & `tmp/langchain_anthropic-0.1.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_anthropic-0.1.8.tar", max compression
+gzip compressed data, was "langchain_anthropic-0.1.8rc1.tar", max compression
```

## Comparing `langchain_anthropic-0.1.8.tar` & `langchain_anthropic-0.1.8rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/LICENSE
--rw-r--r--   0        0        0     1215 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/README.md
--rw-r--r--   0        0        0      225 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/langchain_anthropic/__init__.py
--rw-r--r--   0        0        0    26903 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/langchain_anthropic/chat_models.py
--rw-r--r--   0        0        0     4908 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/langchain_anthropic/experimental.py
--rw-r--r--   0        0        0    11687 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/langchain_anthropic/llms.py
--rw-r--r--   0        0        0     2493 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/langchain_anthropic/output_parsers.py
--rw-r--r--   0        0        0        0 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/langchain_anthropic/py.typed
--rw-r--r--   0        0        0     2677 2024-04-11 16:20:24.392875 langchain_anthropic-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/LICENSE
+-rw-r--r--   0        0        0     1215 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/README.md
+-rw-r--r--   0        0        0      225 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/__init__.py
+-rw-r--r--   0        0        0    26903 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/chat_models.py
+-rw-r--r--   0        0        0     4908 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/experimental.py
+-rw-r--r--   0        0        0    11687 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/llms.py
+-rw-r--r--   0        0        0     2493 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/output_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/py.typed
+-rw-r--r--   0        0        0     2723 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.8rc1/PKG-INFO
```

### Comparing `langchain_anthropic-0.1.8/LICENSE` & `langchain_anthropic-0.1.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8/README.md` & `langchain_anthropic-0.1.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8/langchain_anthropic/chat_models.py` & `langchain_anthropic-0.1.8rc1/langchain_anthropic/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8/langchain_anthropic/experimental.py` & `langchain_anthropic-0.1.8rc1/langchain_anthropic/experimental.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8/langchain_anthropic/llms.py` & `langchain_anthropic-0.1.8rc1/langchain_anthropic/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8/langchain_anthropic/output_parsers.py` & `langchain_anthropic-0.1.8rc1/langchain_anthropic/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8/pyproject.toml` & `langchain_anthropic-0.1.8rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-anthropic"
-version = "0.1.8"
+version = "0.1.8rc1"
 description = "An integration package connecting AnthropicMessages and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.42"
+langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
 anthropic = ">=0.23.0,<1"
 defusedxml = { version = "^0.7.1", optional = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_anthropic-0.1.8/PKG-INFO` & `langchain_anthropic-0.1.8rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-anthropic
-Version: 0.1.8
+Version: 0.1.8rc1
 Summary: An integration package connecting AnthropicMessages and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.23.0,<1)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic
 Description-Content-Type: text/markdown
 
 # langchain-anthropic
 
 This package contains the LangChain integration for Anthropic's generative models.
```

