# Comparing `tmp/composio_langchain-0.1.84.tar.gz` & `tmp/composio_langchain-0.1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.84.tar", last modified: Sun Apr  7 19:52:58 2024, max compression
+gzip compressed data, was "composio_langchain-0.1.87.tar", last modified: Thu Apr 11 12:40:29 2024, max compression
```

## Comparing `composio_langchain-0.1.84.tar` & `composio_langchain-0.1.87.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:52:58.127309 composio_langchain-0.1.84/
--rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-02 18:29:17.000000 composio_langchain-0.1.84/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-07 19:52:58.127113 composio_langchain-0.1.84/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2591 2024-04-02 18:29:17.000000 composio_langchain-0.1.84/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:52:58.126016 composio_langchain-0.1.84/composio_langchain/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       88 2024-04-02 18:29:17.000000 composio_langchain-0.1.84/composio_langchain/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     5405 2024-04-07 18:28:35.000000 composio_langchain-0.1.84/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-02 18:29:17.000000 composio_langchain-0.1.84/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 19:52:58.126905 composio_langchain-0.1.84/composio_langchain.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-07 19:52:58.000000 composio_langchain-0.1.84/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      363 2024-04-07 19:52:58.000000 composio_langchain-0.1.84/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 19:52:58.000000 composio_langchain-0.1.84/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      149 2024-04-07 19:52:58.000000 composio_langchain-0.1.84/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       19 2024-04-07 19:52:58.000000 composio_langchain-0.1.84/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      455 2024-04-07 19:52:16.000000 composio_langchain-0.1.84/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 19:52:58.127352 composio_langchain-0.1.84/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      839 2024-04-07 19:52:16.000000 composio_langchain-0.1.84/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:29.395492 composio_langchain-0.1.87/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-02 18:29:17.000000 composio_langchain-0.1.87/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-11 12:40:29.395303 composio_langchain-0.1.87/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2591 2024-04-02 18:29:17.000000 composio_langchain-0.1.87/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:29.394062 composio_langchain-0.1.87/composio_langchain/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       88 2024-04-02 18:29:17.000000 composio_langchain-0.1.87/composio_langchain/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5405 2024-04-07 18:28:35.000000 composio_langchain-0.1.87/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2804 2024-04-02 18:29:17.000000 composio_langchain-0.1.87/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:29.395062 composio_langchain-0.1.87/composio_langchain.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3334 2024-04-11 12:40:29.000000 composio_langchain-0.1.87/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      363 2024-04-11 12:40:29.000000 composio_langchain-0.1.87/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 12:40:29.000000 composio_langchain-0.1.87/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      149 2024-04-11 12:40:29.000000 composio_langchain-0.1.87/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       19 2024-04-11 12:40:29.000000 composio_langchain-0.1.87/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      455 2024-04-11 12:39:53.000000 composio_langchain-0.1.87/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 12:40:29.395535 composio_langchain-0.1.87/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      839 2024-04-11 12:39:53.000000 composio_langchain-0.1.87/setup.py
```

### Comparing `composio_langchain-0.1.84/PKG-INFO` & `composio_langchain-0.1.87/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.84
+Version: 0.1.87
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.84
+Requires-Dist: composio_core===0.1.87
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.84/README.md` & `composio_langchain-0.1.87/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.84/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.1.87/composio_langchain/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.84/composio_langchain/pydantic_utils.py` & `composio_langchain-0.1.87/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.84/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.1.87/composio_langchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.84
+Version: 0.1.87
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.84
+Requires-Dist: composio_core===0.1.87
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.84/setup.py` & `composio_langchain-0.1.87/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.1.84",
+    version="0.1.87",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

