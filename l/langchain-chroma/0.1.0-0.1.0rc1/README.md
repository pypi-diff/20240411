# Comparing `tmp/langchain_chroma-0.1.0.tar.gz` & `tmp/langchain_chroma-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_chroma-0.1.0.tar", max compression
+gzip compressed data, was "langchain_chroma-0.1.0rc1.tar", max compression
```

## Comparing `langchain_chroma-0.1.0.tar` & `langchain_chroma-0.1.0rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-04-11 19:40:18.241277 langchain_chroma-0.1.0/LICENSE
--rw-r--r--   0        0        0      373 2024-04-11 19:40:18.241277 langchain_chroma-0.1.0/README.md
--rw-r--r--   0        0        0       78 2024-04-11 19:40:18.241277 langchain_chroma-0.1.0/langchain_chroma/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 19:40:18.241277 langchain_chroma-0.1.0/langchain_chroma/py.typed
--rw-r--r--   0        0        0    31062 2024-04-11 19:40:18.241277 langchain_chroma-0.1.0/langchain_chroma/vectorstores.py
--rw-r--r--   0        0        0     2831 2024-04-11 19:40:18.241277 langchain_chroma-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1262 1970-01-01 00:00:00.000000 langchain_chroma-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0      373 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/README.md
+-rw-r--r--   0        0        0       78 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/langchain_chroma/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/langchain_chroma/py.typed
+-rw-r--r--   0        0        0    31062 2024-04-11 18:30:01.144052 langchain_chroma-0.1.0rc1/langchain_chroma/vectorstores.py
+-rw-r--r--   0        0        0     2834 2024-04-11 18:30:01.148052 langchain_chroma-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1265 1970-01-01 00:00:00.000000 langchain_chroma-0.1.0rc1/PKG-INFO
```

### Comparing `langchain_chroma-0.1.0/LICENSE` & `langchain_chroma-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_chroma-0.1.0/langchain_chroma/vectorstores.py` & `langchain_chroma-0.1.0rc1/langchain_chroma/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_chroma-0.1.0/pyproject.toml` & `langchain_chroma-0.1.0rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-chroma"
-version = "0.1.0"
+version = "0.1.0rc1"
 description = "An integration package connecting Chroma and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_chroma-0.1.0/PKG-INFO` & `langchain_chroma-0.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-chroma
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: An integration package connecting Chroma and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

