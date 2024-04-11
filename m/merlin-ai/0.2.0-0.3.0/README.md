# Comparing `tmp/merlin_ai-0.2.0.tar.gz` & `tmp/merlin_ai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin_ai-0.2.0.tar", max compression
+gzip compressed data, was "merlin_ai-0.3.0.tar", max compression
```

## Comparing `merlin_ai-0.2.0.tar` & `merlin_ai-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      231 2024-01-16 12:17:42.787631 merlin_ai-0.2.0/merlin_ai/__init__.py
--rw-r--r--   0        0        0    13747 2024-01-16 12:17:42.792630 merlin_ai-0.2.0/merlin_ai/ai_classes.py
--rw-r--r--   0        0        0     4566 2024-01-16 12:17:42.798167 merlin_ai-0.2.0/merlin_ai/data_classes.py
--rw-r--r--   0        0        0     1262 2024-01-16 12:17:42.803168 merlin_ai-0.2.0/merlin_ai/decorators.py
--rw-r--r--   0        0        0     1396 2023-11-16 08:52:02.636762 merlin_ai-0.2.0/merlin_ai/llm_classes.py
--rw-r--r--   0        0        0      164 2023-11-16 08:52:02.636762 merlin_ai-0.2.0/merlin_ai/settings.py
--rw-r--r--   0        0        0     2830 2024-01-15 20:21:40.161659 merlin_ai-0.2.0/merlin_ai/test.py
--rw-r--r--   0        0        0      486 2024-01-16 12:17:42.807668 merlin_ai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      283 2023-11-16 08:52:02.634765 merlin_ai-0.2.0/README.md
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 merlin_ai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      254 2024-04-11 08:55:45.766906 merlin_ai-0.3.0/merlin_ai/__init__.py
+-rw-r--r--   0        0        0    13921 2024-04-11 08:55:45.771910 merlin_ai-0.3.0/merlin_ai/ai_classes.py
+-rw-r--r--   0        0        0     4566 2024-01-16 12:17:42.798167 merlin_ai-0.3.0/merlin_ai/data_classes.py
+-rw-r--r--   0        0        0     1262 2024-01-16 12:22:03.201080 merlin_ai-0.3.0/merlin_ai/decorators.py
+-rw-r--r--   0        0        0     1514 2024-04-11 08:55:45.776909 merlin_ai-0.3.0/merlin_ai/llm_classes.py
+-rw-r--r--   0        0        0     5993 2024-04-11 08:55:45.781907 merlin_ai-0.3.0/merlin_ai/llm_client.py
+-rw-r--r--   0        0        0      164 2023-11-16 08:52:02.636762 merlin_ai-0.3.0/merlin_ai/settings.py
+-rw-r--r--   0        0        0      530 2024-04-11 09:01:45.007727 merlin_ai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-11-16 08:52:02.634765 merlin_ai-0.3.0/README.md
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 merlin_ai-0.3.0/PKG-INFO
```

### Comparing `merlin_ai-0.2.0/merlin_ai/ai_classes.py` & `merlin_ai-0.3.0/merlin_ai/ai_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,15 @@
         Generate LLM prompt from provided value
         :param value:
         :return:
         """
         raise NotImplementedError()
 
     def _get_base_llm_settings(
-        self,
-        function_call_model_settings: Optional[dict] = None
+        self, function_call_model_settings: Optional[dict] = None
     ) -> dict:
         """
         Get base LLM settings
         """
         settings = default_model_settings
         if self._model_settings:
             settings.update(self._model_settings)
@@ -316,20 +315,37 @@
 class OpenAIEnumModel(OpenAIEnum):
     """
     OpenAI-based AI Enum implemented as a model (parser)
     """
 
     def __init__(self, data_class: Type, model_settings: Optional[dict] = None):
         super().__init__(data_class, model_settings)
-        fields = [("category", data_class,
-                   field(metadata={"description": data_class.__doc__} if data_class.__doc__ else None)),
-                  ("explanation", str,
-                   field(metadata={"description": "Explain your categorization in a short and concise manner."}))
-                  ]
-        data_class_wrapper = dataclasses.make_dataclass(f"{data_class.__name__}_wrapper", fields)
+        fields = [
+            (
+                "category",
+                data_class,
+                field(
+                    metadata={"description": data_class.__doc__}
+                    if data_class.__doc__
+                    else None
+                ),
+            ),
+            (
+                "explanation",
+                str,
+                field(
+                    metadata={
+                        "description": "Explain your categorization in a short and concise manner."
+                    }
+                ),
+            ),
+        ]
+        data_class_wrapper = dataclasses.make_dataclass(
+            f"{data_class.__name__}_wrapper", fields
+        )
         if data_class.__doc__:
             data_class_wrapper.__doc__ = data_class.__doc__
         self._data_class_wrapper = data_class_wrapper
 
     def __str__(self):
         return f"OpenAIEnumExplained: {self._data_class.__name__}"
 
@@ -367,20 +383,15 @@
         system_prompt += (
             "The user will provide text to classify, you will use your expertise "
             "to choose the best category below based on it.\n"
             f"To submit your categorization result, you must call the `{function_name}` function.\n"
             "Use the provided text and context to infer the category and explanation "
             f"needed to call `{function_name}`.\n"
             "The following categories are available to choose from:\n"
-            + "\n".join(
-                [
-                    f"* {option.name}"
-                    for idx, option in enumerate(enum_options)
-                ]
-            )
+            + "\n".join([f"* {option.name}" for idx, option in enumerate(enum_options)])
         )
 
         return OpenAIPrompt(
             model_settings,
             messages=[
                 {
                     "role": "system",
```

### Comparing `merlin_ai-0.2.0/merlin_ai/data_classes.py` & `merlin_ai-0.3.0/merlin_ai/data_classes.py`

 * *Files identical despite different names*

### Comparing `merlin_ai-0.2.0/merlin_ai/decorators.py` & `merlin_ai-0.3.0/merlin_ai/decorators.py`

 * *Files identical despite different names*

### Comparing `merlin_ai-0.2.0/merlin_ai/llm_classes.py` & `merlin_ai-0.3.0/merlin_ai/llm_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 LLM classes
 """
 import os
 from typing import Optional
 
 import openai
 
+from merlin_ai.llm_client import MerlinChatCompletion
+
 
 class PromptBase:
     """
     Base class for creating Prompts
     """
 
     def as_dict(self) -> dict:
@@ -54,8 +56,9 @@
         return {
             **self._model_settings,
             "messages": self._messages,
         }
 
     def get_llm_response(self):
         openai.api_key = os.environ.get("OPENAI_API_KEY")
-        return openai.ChatCompletion.create(**self.as_dict())
+        return MerlinChatCompletion.create(**self.as_dict())
+        # return openai.ChatCompletion.create(**self.as_dict())
```

### Comparing `merlin_ai-0.2.0/PKG-INFO` & `merlin_ai-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: merlin-ai
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/matevzpoljanc/merlin-ai
 License: MIT
 Author: Matevz Poljanc
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: anthropic (>=0.25.0,<0.26.0)
 Requires-Dist: openai (>=0.28.1,<0.29.0)
 Requires-Dist: tiktoken (>=0.5.1,<0.6.0)
 Project-URL: Repository, https://github.com/matevzpoljanc/merlin-ai
 Description-Content-Type: text/markdown
 
 # Merlin AI
 ## The AI engineering framework
```

