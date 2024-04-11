# Comparing `tmp/llama_index_llms_predibase-0.1.2.tar.gz` & `tmp/llama_index_llms_predibase-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_predibase-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_llms_predibase-0.1.3.tar", max compression
```

## Comparing `llama_index_llms_predibase-0.1.2.tar` & `llama_index_llms_predibase-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       41 2024-02-13 13:53:01.687558 llama_index_llms_predibase-0.1.2/README.md
--rw-r--r--   0        0        0       85 2024-02-13 13:53:01.687756 llama_index_llms_predibase-0.1.2/llama_index/llms/predibase/__init__.py
--rw-r--r--   0        0        0     4295 2024-02-13 13:53:01.687831 llama_index_llms_predibase-0.1.2/llama_index/llms/predibase/base.py
--rw-r--r--   0        0        0     1436 2024-02-21 18:02:24.223451 llama_index_llms_predibase-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 llama_index_llms_predibase-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-11 16:20:38.185894 llama_index_llms_predibase-0.1.3/README.md
+-rw-r--r--   0        0        0       85 2024-04-11 16:20:38.185894 llama_index_llms_predibase-0.1.3/llama_index/llms/predibase/__init__.py
+-rw-r--r--   0        0        0     6739 2024-04-11 16:20:38.185894 llama_index_llms_predibase-0.1.3/llama_index/llms/predibase/base.py
+-rw-r--r--   0        0        0     1436 2024-04-11 16:20:38.185894 llama_index_llms_predibase-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 llama_index_llms_predibase-0.1.3/PKG-INFO
```

### Comparing `llama_index_llms_predibase-0.1.2/pyproject.toml` & `llama_index_llms_predibase-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms predibase integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-predibase"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_llms_predibase-0.1.2/PKG-INFO` & `llama_index_llms_predibase-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-predibase
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index llms predibase integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Predibase
```

