# Comparing `tmp/py-llm-core-2.8.2.tar.gz` & `tmp/py-llm-core-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-llm-core-2.8.2.tar", last modified: Wed Jan 10 12:46:59 2024, max compression
+gzip compressed data, was "py-llm-core-2.8.4.tar", last modified: Thu Apr 11 20:26:51 2024, max compression
```

## Comparing `py-llm-core-2.8.2.tar` & `py-llm-core-2.8.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-01-10 12:46:59.739705 py-llm-core-2.8.2/
--rw-r--r--   0 pas        (501) staff       (20)     1082 2023-09-25 09:08:19.000000 py-llm-core-2.8.2/LICENSE
--rw-r--r--   0 pas        (501) staff       (20)       26 2023-11-28 09:08:27.000000 py-llm-core-2.8.2/MANIFEST.in
--rw-r--r--   0 pas        (501) staff       (20)    27642 2024-01-10 12:46:59.739477 py-llm-core-2.8.2/PKG-INFO
--rw-r--r--   0 pas        (501) staff       (20)    27148 2024-01-10 12:44:27.000000 py-llm-core-2.8.2/README.md
--rw-r--r--   0 pas        (501) staff       (20)       88 2023-11-28 09:02:40.000000 py-llm-core-2.8.2/requirements.txt
--rw-r--r--   0 pas        (501) staff       (20)       38 2024-01-10 12:46:59.739748 py-llm-core-2.8.2/setup.cfg
--rw-r--r--   0 pas        (501) staff       (20)      785 2024-01-10 12:44:13.000000 py-llm-core-2.8.2/setup.py
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-01-10 12:46:59.732646 py-llm-core-2.8.2/src/
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-01-10 12:46:59.734717 py-llm-core-2.8.2/src/llm_core/
--rw-r--r--   0 pas        (501) staff       (20)       73 2023-10-05 20:44:56.000000 py-llm-core-2.8.2/src/llm_core/__init__.py
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-01-10 12:46:59.737477 py-llm-core-2.8.2/src/llm_core/assistants/
--rw-r--r--   0 pas        (501) staff       (20)      535 2023-10-05 20:44:56.000000 py-llm-core-2.8.2/src/llm_core/assistants/__init__.py
--rw-r--r--   0 pas        (501) staff       (20)      993 2023-10-05 20:44:56.000000 py-llm-core-2.8.2/src/llm_core/assistants/analysts.py
--rw-r--r--   0 pas        (501) staff       (20)     1369 2024-01-09 11:26:24.000000 py-llm-core-2.8.2/src/llm_core/assistants/base.py
--rw-r--r--   0 pas        (501) staff       (20)     3744 2023-10-05 20:44:56.000000 py-llm-core-2.8.2/src/llm_core/assistants/summarizers.py
--rw-r--r--   0 pas        (501) staff       (20)     1851 2023-10-05 20:44:56.000000 py-llm-core-2.8.2/src/llm_core/assistants/verifiers.py
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-01-10 12:46:59.738362 py-llm-core-2.8.2/src/llm_core/llm/
--rw-r--r--   0 pas        (501) staff       (20)      164 2023-11-08 21:02:18.000000 py-llm-core-2.8.2/src/llm_core/llm/__init__.py
--rw-r--r--   0 pas        (501) staff       (20)     2392 2024-01-08 12:14:32.000000 py-llm-core-2.8.2/src/llm_core/llm/base.py
--rw-r--r--   0 pas        (501) staff       (20)     5019 2023-11-28 06:20:33.000000 py-llm-core-2.8.2/src/llm_core/llm/llama_cpp_compatible.py
--rw-r--r--   0 pas        (501) staff       (20)     3550 2024-01-10 12:45:57.000000 py-llm-core-2.8.2/src/llm_core/llm/openai.py
--rw-r--r--   0 pas        (501) staff       (20)     2635 2023-10-10 20:41:06.000000 py-llm-core-2.8.2/src/llm_core/parsers.py
--rw-r--r--   0 pas        (501) staff       (20)     7185 2024-01-09 17:57:38.000000 py-llm-core-2.8.2/src/llm_core/schema.py
--rw-r--r--   0 pas        (501) staff       (20)      568 2024-01-10 12:45:52.000000 py-llm-core-2.8.2/src/llm_core/settings.py
--rw-r--r--   0 pas        (501) staff       (20)     1019 2023-11-03 16:04:40.000000 py-llm-core-2.8.2/src/llm_core/splitters.py
--rw-r--r--   0 pas        (501) staff       (20)     2312 2023-11-06 20:48:15.000000 py-llm-core-2.8.2/src/llm_core/token_codecs.py
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-01-10 12:46:59.739162 py-llm-core-2.8.2/src/py_llm_core.egg-info/
--rw-r--r--   0 pas        (501) staff       (20)    27642 2024-01-10 12:46:59.000000 py-llm-core-2.8.2/src/py_llm_core.egg-info/PKG-INFO
--rw-r--r--   0 pas        (501) staff       (20)      703 2024-01-10 12:46:59.000000 py-llm-core-2.8.2/src/py_llm_core.egg-info/SOURCES.txt
--rw-r--r--   0 pas        (501) staff       (20)        1 2024-01-10 12:46:59.000000 py-llm-core-2.8.2/src/py_llm_core.egg-info/dependency_links.txt
--rw-r--r--   0 pas        (501) staff       (20)       88 2024-01-10 12:46:59.000000 py-llm-core-2.8.2/src/py_llm_core.egg-info/requires.txt
--rw-r--r--   0 pas        (501) staff       (20)        9 2024-01-10 12:46:59.000000 py-llm-core-2.8.2/src/py_llm_core.egg-info/top_level.txt
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.293892 py-llm-core-2.8.4/
+-rw-r--r--   0 pas        (501) staff       (20)     1082 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/LICENSE
+-rw-r--r--   0 pas        (501) staff       (20)       26 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/MANIFEST.in
+-rw-r--r--   0 pas        (501) staff       (20)    27667 2024-04-11 20:26:51.293631 py-llm-core-2.8.4/PKG-INFO
+-rw-r--r--   0 pas        (501) staff       (20)    27148 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/README.md
+-rw-r--r--   0 pas        (501) staff       (20)       98 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/requirements.txt
+-rw-r--r--   0 pas        (501) staff       (20)       38 2024-04-11 20:26:51.293931 py-llm-core-2.8.4/setup.cfg
+-rw-r--r--   0 pas        (501) staff       (20)      785 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/setup.py
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.288203 py-llm-core-2.8.4/src/
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.290189 py-llm-core-2.8.4/src/llm_core/
+-rw-r--r--   0 pas        (501) staff       (20)       73 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/__init__.py
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.291635 py-llm-core-2.8.4/src/llm_core/assistants/
+-rw-r--r--   0 pas        (501) staff       (20)      591 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/assistants/__init__.py
+-rw-r--r--   0 pas        (501) staff       (20)      993 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/assistants/analysts.py
+-rw-r--r--   0 pas        (501) staff       (20)     1646 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/assistants/base.py
+-rw-r--r--   0 pas        (501) staff       (20)     3744 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/assistants/summarizers.py
+-rw-r--r--   0 pas        (501) staff       (20)     1851 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/assistants/verifiers.py
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.292402 py-llm-core-2.8.4/src/llm_core/llm/
+-rw-r--r--   0 pas        (501) staff       (20)      239 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/llm/__init__.py
+-rw-r--r--   0 pas        (501) staff       (20)     2674 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/llm/base.py
+-rw-r--r--   0 pas        (501) staff       (20)     5019 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/llm/llama_cpp_compatible.py
+-rw-r--r--   0 pas        (501) staff       (20)     2848 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/llm/mistralai.py
+-rw-r--r--   0 pas        (501) staff       (20)     3542 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/llm/openai.py
+-rw-r--r--   0 pas        (501) staff       (20)     3377 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/parsers.py
+-rw-r--r--   0 pas        (501) staff       (20)     7185 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/schema.py
+-rw-r--r--   0 pas        (501) staff       (20)      986 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/settings.py
+-rw-r--r--   0 pas        (501) staff       (20)     1019 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/splitters.py
+-rw-r--r--   0 pas        (501) staff       (20)     2455 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/token_codecs.py
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.293306 py-llm-core-2.8.4/src/py_llm_core.egg-info/
+-rw-r--r--   0 pas        (501) staff       (20)    27667 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/PKG-INFO
+-rw-r--r--   0 pas        (501) staff       (20)      733 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/SOURCES.txt
+-rw-r--r--   0 pas        (501) staff       (20)        1 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/dependency_links.txt
+-rw-r--r--   0 pas        (501) staff       (20)       98 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/requires.txt
+-rw-r--r--   0 pas        (501) staff       (20)        9 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/top_level.txt
```

### Comparing `py-llm-core-2.8.2/LICENSE` & `py-llm-core-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.2/PKG-INFO` & `py-llm-core-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: py-llm-core
-Version: 2.8.2
+Version: 2.8.4
 Summary: PyLLMCore provides a light-weighted interface with LLMs
 Home-page: https://github.com/paschembri/py-llm-core
 Author: P.A. SCHEMBRI
 Author-email: pa.schembri@advanced-stack.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai<2,>=1.3.5
 Requires-Dist: tiktoken
 Requires-Dist: jsonschema
 Requires-Dist: dirtyjson
 Requires-Dist: llama-cpp-python>=0.2.20
 Requires-Dist: python-decouple
+Requires-Dist: mistralai
 
 # PyLLMCore
 
 ## Overview
 
 PyLLMCore is a light-weighted structured interface with Large Language Models 
 with native support for [llama.cpp](http://github.com/ggerganov/llama.cpp) and OpenAI API.
```

### Comparing `py-llm-core-2.8.2/README.md` & `py-llm-core-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.2/setup.py` & `py-llm-core-2.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 main_package = packages[0]
 long_description = (here / "README.md").read_text()
 requirements = (here / "requirements.txt").read_text().splitlines()
 
 
 setup(
     name="py-llm-core",
-    version="2.8.2",
+    version="2.8.4",
     license="MIT",
     description="PyLLMCore provides a light-weighted interface with LLMs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="P.A. SCHEMBRI",
     author_email="pa.schembri@advanced-stack.com",
     url="https://github.com/paschembri/py-llm-core",
```

### Comparing `py-llm-core-2.8.2/src/llm_core/assistants/analysts.py` & `py-llm-core-2.8.4/src/llm_core/assistants/analysts.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.2/src/llm_core/assistants/base.py` & `py-llm-core-2.8.4/src/llm_core/assistants/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # -*- coding: utf-8 -*-
-from ..parsers import BaseParser, OpenAIParser, LLaMACPPParser
+from ..parsers import (
+    BaseParser,
+    OpenAIParser,
+    LLaMACPPParser,
+    MistralAILargeParser,
+)
 
 
 class BaseAssistant(BaseParser):
     def __init__(self, target_cls, *args, **kwargs):
         super().__init__(target_cls, *args, **kwargs)
         self.system_prompt = getattr(self.target_cls, "system_prompt", "")
         self.prompt = getattr(self.target_cls, "prompt", "")
@@ -38,7 +43,14 @@
         super().__init__(
             target_cls,
             model=model,
             llama_cpp_kwargs=llama_cpp_kwargs,
             *args,
             **kwargs
         )
+
+
+class MistralAILargeAssistant(BaseAssistant, MistralAILargeParser):
+    def __init__(
+        self, target_cls, model="mistral-large-latest", *args, **kwargs
+    ):
+        super().__init__(target_cls, model=model, *args, **kwargs)
```

### Comparing `py-llm-core-2.8.2/src/llm_core/assistants/summarizers.py` & `py-llm-core-2.8.4/src/llm_core/assistants/summarizers.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.2/src/llm_core/assistants/verifiers.py` & `py-llm-core-2.8.4/src/llm_core/assistants/verifiers.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.2/src/llm_core/llm/base.py` & `py-llm-core-2.8.4/src/llm_core/llm/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,19 +12,20 @@
         prompt,
         history=None,
         schema=None,
     ):
         schema_prompt = ""
 
         if schema:
-            schema_prompt = json.dumps(schema_prompt)
+            schema_prompt = json.dumps(schema)
 
         complete_prompt = [
             self.system_prompt,
             prompt,
+            str(history) if history else "",
             schema_prompt,
         ]
 
         complete_prompt = "\n".join(complete_prompt)
 
         required_ctx_size = len(codecs.encode(complete_prompt, self.name))
         if required_ctx_size > self.ctx_size:
@@ -44,14 +45,15 @@
 
 @dataclass
 class Message:
     role: str
     content: str
     function_call: dict = None
     tool_calls: dict = None
+    name: str = None
 
 
 @dataclass
 class ChatCompletionChoice:
     index: int
     message: Message
     finish_reason: str
@@ -61,18 +63,23 @@
         for item in iterable:
             message_attrs = item["message"]
 
             # To ensure compatibility with other models, we stuff
             # function calling in the message content.
 
             function_call = message_attrs.get("function_call")
+            tool_calls = message_attrs.get("tool_calls")
             if function_call:
                 message_attrs["content"] = message_attrs["function_call"][
                     "arguments"
                 ]
+            elif tool_calls:
+                message_attrs["content"] = message_attrs["tool_calls"][0][
+                    "function"
+                ]["arguments"]
 
             message = Message(**item["message"])
             index = item["index"]
             finish_reason = item["finish_reason"]
             yield cls(
                 index=index, message=message, finish_reason=finish_reason
             )
```

### Comparing `py-llm-core-2.8.2/src/llm_core/llm/llama_cpp_compatible.py` & `py-llm-core-2.8.4/src/llm_core/llm/llama_cpp_compatible.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.2/src/llm_core/llm/openai.py` & `py-llm-core-2.8.4/src/llm_core/llm/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     model, messages, temperature, max_tokens=1000, **kwargs
 ):
     default_timeout = httpx.Timeout(DEFAULT_TIMEOUT, write=10.0, connect=2.0)
 
     if USE_AZURE_OPENAI:
         # gets the API Key from environment variable AZURE_OPENAI_API_KEY
         client = AzureOpenAI(
-            api_version="2023-09-01-preview",
+            api_version="2024-02-01",
             azure_endpoint=AZURE_OPENAI_ENDPOINT,
             timeout=default_timeout,
         )
 
         # Here we are using the following convention:
         # Every model name is mapped to an Azure deployment where we remove the
         # dot sign.
```

### Comparing `py-llm-core-2.8.2/src/llm_core/parsers.py` & `py-llm-core-2.8.4/src/llm_core/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 import dirtyjson
 
-from .llm import OpenAIChatModel, LLaMACPPModel
+from .llm import OpenAIChatModel, LLaMACPPModel, MistralAILarge
 from .schema import to_json_schema, from_dict
 
 
 class BaseParser:
     def __init__(self, target_cls, *args, **kwargs):
         self.target_cls = target_cls
         self.target_json_schema = to_json_schema(self.target_cls)
@@ -86,7 +86,32 @@
 
     def __enter__(self):
         self.model_wrapper.load_model()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.model_wrapper.release_model()
+
+
+class MistralAILargeParser(BaseParser):
+    def __init__(
+        self,
+        target_cls,
+        model="mistral-large-latest",
+        completion_kwargs=None,
+        *args,
+        **kwargs
+    ):
+        super().__init__(target_cls, *args, **kwargs)
+        self.completion_kwargs = (
+            {} if completion_kwargs is None else completion_kwargs
+        )
+
+        self.model_wrapper = MistralAILarge(
+            name=model,
+            system_prompt=(
+                "Act as a powerful AI able to extract, parse and process "
+                "information from unstructured content."
+            ),
+        )
+        self.ctx_size = self.model_wrapper.ctx_size
+        self.model_name = self.model_wrapper.name
```

### Comparing `py-llm-core-2.8.2/src/llm_core/schema.py` & `py-llm-core-2.8.4/src/llm_core/schema.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.2/src/llm_core/splitters.py` & `py-llm-core-2.8.4/src/llm_core/splitters.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.2/src/llm_core/token_codecs.py` & `py-llm-core-2.8.4/src/llm_core/token_codecs.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
             "gpt_3.5_turbo_0613",
             "gpt_3.5_turbo_16k",
             "gpt_3.5_turbo_16k_0613",
             "gpt_4",
             "gpt_4_0613",
             "gpt_4_1106_preview",
             "gpt_4_32k",
+            "mistral_large_latest",  #: dirty hack to quickly support mistral
+            "azureai",  #: dirty hack to quickly support mistral
         )
 
     def __init__(self, codec_name):
         # Map everything to gpt-3.5-turbo
         self.token_encoder = tiktoken.encoding_for_model("gpt-3.5-turbo")
```

### Comparing `py-llm-core-2.8.2/src/py_llm_core.egg-info/PKG-INFO` & `py-llm-core-2.8.4/src/py_llm_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: py-llm-core
-Version: 2.8.2
+Version: 2.8.4
 Summary: PyLLMCore provides a light-weighted interface with LLMs
 Home-page: https://github.com/paschembri/py-llm-core
 Author: P.A. SCHEMBRI
 Author-email: pa.schembri@advanced-stack.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai<2,>=1.3.5
 Requires-Dist: tiktoken
 Requires-Dist: jsonschema
 Requires-Dist: dirtyjson
 Requires-Dist: llama-cpp-python>=0.2.20
 Requires-Dist: python-decouple
+Requires-Dist: mistralai
 
 # PyLLMCore
 
 ## Overview
 
 PyLLMCore is a light-weighted structured interface with Large Language Models 
 with native support for [llama.cpp](http://github.com/ggerganov/llama.cpp) and OpenAI API.
```

### Comparing `py-llm-core-2.8.2/src/py_llm_core.egg-info/SOURCES.txt` & `py-llm-core-2.8.4/src/py_llm_core.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,13 +13,14 @@
 src/llm_core/assistants/analysts.py
 src/llm_core/assistants/base.py
 src/llm_core/assistants/summarizers.py
 src/llm_core/assistants/verifiers.py
 src/llm_core/llm/__init__.py
 src/llm_core/llm/base.py
 src/llm_core/llm/llama_cpp_compatible.py
+src/llm_core/llm/mistralai.py
 src/llm_core/llm/openai.py
 src/py_llm_core.egg-info/PKG-INFO
 src/py_llm_core.egg-info/SOURCES.txt
 src/py_llm_core.egg-info/dependency_links.txt
 src/py_llm_core.egg-info/requires.txt
 src/py_llm_core.egg-info/top_level.txt
```

