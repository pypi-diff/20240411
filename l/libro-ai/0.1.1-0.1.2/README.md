# Comparing `tmp/libro_ai-0.1.1.tar.gz` & `tmp/libro_ai-0.1.2.tar.gz`

## Comparing `libro_ai-0.1.1.tar` & `libro_ai-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 libro_ai-0.1.1/.python-version
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/_version.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/extensions.py
--rwxr-xr-x   0        0        0      852 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/chat_message.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/chat_record.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/executor.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/item.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/langchain_variable.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/langchain_variable_executor.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/object.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/object_manager.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/openai.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/openai_chat_executor.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/provider.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/source.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/chat/utils.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/flow/__init__.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/flow/libro_client.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/flow/nb_args.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/magics/__init__.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/magics/exception.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/magics/prompt_magic.py
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/utils/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/utils/base.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/utils/inspector.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 libro_ai-0.1.1/src/libro_ai/utils/langchain.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 libro_ai-0.1.1/.gitignore
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 libro_ai-0.1.1/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 libro_ai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 libro_ai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 libro_ai-0.1.2/.python-version
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/_version.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/extensions.py
+-rwxr-xr-x   0        0        0      852 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/chat_message.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/chat_record.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/executor.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/item.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/langchain_variable.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/langchain_variable_executor.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/object.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/object_manager.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/openai.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/openai_chat_executor.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/provider.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/source.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/chat/utils.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/flow/__init__.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/flow/libro_client.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/flow/nb_args.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/magics/__init__.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/magics/exception.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/magics/prompt_magic.py
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/utils/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/utils/base.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/utils/inspector.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 libro_ai-0.1.2/src/libro_ai/utils/langchain.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 libro_ai-0.1.2/.gitignore
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 libro_ai-0.1.2/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 libro_ai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 libro_ai-0.1.2/PKG-INFO
```

### Comparing `libro_ai-0.1.1/src/libro_ai/__init__.py` & `libro_ai-0.1.2/src/libro_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/extensions.py` & `libro_ai-0.1.2/src/libro_ai/extensions.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/__init__.py` & `libro_ai-0.1.2/src/libro_ai/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/chat_record.py` & `libro_ai-0.1.2/src/libro_ai/chat/chat_record.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/executor.py` & `libro_ai-0.1.2/src/libro_ai/chat/executor.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/item.py` & `libro_ai-0.1.2/src/libro_ai/chat/item.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/langchain_variable.py` & `libro_ai-0.1.2/src/libro_ai/chat/langchain_variable.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/langchain_variable_executor.py` & `libro_ai-0.1.2/src/libro_ai/chat/langchain_variable_executor.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/object.py` & `libro_ai-0.1.2/src/libro_ai/chat/object.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/object_manager.py` & `libro_ai-0.1.2/src/libro_ai/chat/object_manager.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/openai.py` & `libro_ai-0.1.2/src/libro_ai/chat/openai.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/openai_chat_executor.py` & `libro_ai-0.1.2/src/libro_ai/chat/openai_chat_executor.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/chat/provider.py` & `libro_ai-0.1.2/src/libro_ai/chat/provider.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/flow/libro_client.py` & `libro_ai-0.1.2/src/libro_ai/flow/libro_client.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/flow/nb_args.py` & `libro_ai-0.1.2/src/libro_ai/flow/nb_args.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/magics/exception.py` & `libro_ai-0.1.2/src/libro_ai/magics/exception.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/magics/prompt_magic.py` & `libro_ai-0.1.2/src/libro_ai/magics/prompt_magic.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/utils/base.py` & `libro_ai-0.1.2/src/libro_ai/utils/base.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/utils/inspector.py` & `libro_ai-0.1.2/src/libro_ai/utils/inspector.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/src/libro_ai/utils/langchain.py` & `libro_ai-0.1.2/src/libro_ai/utils/langchain.py`

 * *Files identical despite different names*

### Comparing `libro_ai-0.1.1/pyproject.toml` & `libro_ai-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libro-ai"
-version = "0.1.1"
+version = "0.1.2"
 description = "Add your description here"
 authors = [
     { name = "brokun", email = "brokun0128@gmail.com" },
     { name = "zhanba", email = "c5e1856@gmail.com" }
 ]
 dependencies = [
     "langchain>=0.1.0",
```

