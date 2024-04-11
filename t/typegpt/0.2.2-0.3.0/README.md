# Comparing `tmp/typegpt-0.2.2.tar.gz` & `tmp/typegpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegpt-0.2.2.tar", last modified: Thu Feb  1 22:13:43 2024, max compression
+gzip compressed data, was "typegpt-0.3.0.tar", last modified: Thu Apr 11 17:01:10 2024, max compression
```

## Comparing `typegpt-0.2.2.tar` & `typegpt-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.990694 typegpt-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-01 22:13:35.000000 typegpt-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-02-01 22:13:43.986694 typegpt-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-02-01 22:13:35.000000 typegpt-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 22:13:43.990694 typegpt-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-01 22:13:35.000000 typegpt-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.982694 typegpt-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-02-01 22:13:35.000000 typegpt-0.2.2/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-02-01 22:13:35.000000 typegpt-0.2.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18714 2024-02-01 22:13:35.000000 typegpt-0.2.2/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-02-01 22:13:35.000000 typegpt-0.2.2/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-02-01 22:13:35.000000 typegpt-0.2.2/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-02-01 22:13:35.000000 typegpt-0.2.2/tests/test_response_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.986694 typegpt-0.2.2/typegpt/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/example_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/message_collection_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.986694 typegpt-0.2.2/typegpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.986694 typegpt-0.2.2/typegpt/openai/_async/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/_async/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/_async/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.986694 typegpt-0.2.2/typegpt/openai/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/_sync/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/base_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/openai/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/prompt_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.986694 typegpt-0.2.2/typegpt/prompt_definition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/prompt_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/prompt_definition/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.986694 typegpt-0.2.2/typegpt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/utils/internal_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/utils/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-01 22:13:35.000000 typegpt-0.2.2/typegpt/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:13:43.986694 typegpt-0.2.2/typegpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-02-01 22:13:43.000000 typegpt-0.2.2/typegpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-01 22:13:43.000000 typegpt-0.2.2/typegpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:13:43.000000 typegpt-0.2.2/typegpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-01 22:13:43.000000 typegpt-0.2.2/typegpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-01 22:13:43.000000 typegpt-0.2.2/typegpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.826071 typegpt-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-11 17:01:07.000000 typegpt-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-11 17:01:10.826071 typegpt-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-11 17:01:07.000000 typegpt-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:01:10.826071 typegpt-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 17:01:07.000000 typegpt-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.818071 typegpt-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_fewshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/example_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/example_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/message_collection_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/openai/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_async/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_async/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/openai/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_sync/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/base_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/prompt_definition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_definition/few_shot_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_definition/prompt_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_definition/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.826071 typegpt-0.3.0/typegpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/utils/internal_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/utils/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.826071 typegpt-0.3.0/typegpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/top_level.txt
```

### Comparing `typegpt-0.2.2/LICENSE` & `typegpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/PKG-INFO` & `typegpt-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-Metadata-Version: 2.1
-Name: typegpt
-Version: 0.2.2
-Summary: TypeGPT - Make GPT safe for production
-Home-page: https://github.com/alexeichhorn/typegpt
-Author: Alexander Eichhorn
-Author-email: 
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: typing_extensions>=4.1.0
-Requires-Dist: inflect>=7.0.0
-Requires-Dist: tiktoken>=0.5.0
-Requires-Dist: openai>=1.1.0
-
 # TypeGPT - Making GPT Safe for Production
 
 It is inherently difficult to produce outputs from LLMs in a consistent structure. TypeGPT simplifies this process to be as easy as defining a class in Python.
 
-Powering our own projects, such as [BoostSEO](https://boostseo.ai)
+Powering our own projects, such as [Spexia](https://getspexia.com)
 
 
 ## Installation
 
 ```bash
 pip install typegpt
 ```
@@ -189,17 +171,60 @@
 ```python
 prompt = ExamplePrompt(...)
 output = client.chat.completions.generate_output(model="gpt-4", prompt=prompt, output_type=ExamplePrompt.Output, ...)
 ```
 This parameter is not merely a type decorator. It can also be used to overwrite the actual output type that GPT attempts to predict.
 
 
+### Few-Shot Prompting
+
+Give examples to the model to explain tasks that are hard to explain:
+
+```python
+class ExamplePrompt(PromptTemplate):
+
+    class Output(BaseLLMResponse):
+        class Ingredient(BaseLLMResponse):
+            name: str
+            quantity: int
+
+        ingredients: list[Ingredient]
+
+    def system_prompt(self) -> str:
+        return "Given a recipe, extract the ingredients."
+
+    def few_shot_examples(self) -> list[FewShotExample[Output]]:
+        return [
+            FewShotExample(
+                input="Let's take two apples, three bananas, and four oranges.",
+                output=self.Output(ingredients=[
+                    self.Output.Ingredient(name="apple", quantity=2),
+                    self.Output.Ingredient(name="banana", quantity=3),
+                    self.Output.Ingredient(name="orange", quantity=4),
+                ])
+            ),
+            FewShotExample(
+                input="My recipe requires five eggs and two cups of flour.",
+                output=self.Output(ingredients=[
+                    self.Output.Ingredient(name="egg", quantity=5),
+                    self.Output.Ingredient(name="flour cups", quantity=2),
+                ])
+            )
+        ]
+
+    def user_prompt(self) -> str:
+        ...
+```
+
+
+
+
 ### Azure
 
-e sure to use the `AzureChatModel` as the model when generating the output, which consists of the deployment_id and the corresponding base model (this is used for automatically reducing prompts if needed).
+Make sure to use the `AzureChatModel` as the model when generating the output, which consists of the deployment_id and the corresponding base model (this is used for automatically reducing prompts if needed).
 ```python
 from typegpt.openai import AzureChatModel, TypeAzureOpenAI
 
 client = TypeAzureOpenAI(
     azure_endpoint="<your azure endpoint>",
     api_key="<your api key>",
     api_version="2023-05-15",
```

### Comparing `typegpt-0.2.2/README.md` & `typegpt-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+Metadata-Version: 2.1
+Name: typegpt
+Version: 0.3.0
+Summary: TypeGPT - Make GPT safe for production
+Home-page: https://github.com/alexeichhorn/typegpt
+Author: Alexander Eichhorn
+Author-email: 
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: typing_extensions>=4.1.0
+Requires-Dist: inflect>=7.0.0
+Requires-Dist: tiktoken>=0.5.0
+Requires-Dist: openai>=1.1.0
+
 # TypeGPT - Making GPT Safe for Production
 
 It is inherently difficult to produce outputs from LLMs in a consistent structure. TypeGPT simplifies this process to be as easy as defining a class in Python.
 
-Powering our own projects, such as [BoostSEO](https://boostseo.ai)
+Powering our own projects, such as [Spexia](https://getspexia.com)
 
 
 ## Installation
 
 ```bash
 pip install typegpt
 ```
@@ -171,17 +189,60 @@
 ```python
 prompt = ExamplePrompt(...)
 output = client.chat.completions.generate_output(model="gpt-4", prompt=prompt, output_type=ExamplePrompt.Output, ...)
 ```
 This parameter is not merely a type decorator. It can also be used to overwrite the actual output type that GPT attempts to predict.
 
 
+### Few-Shot Prompting
+
+Give examples to the model to explain tasks that are hard to explain:
+
+```python
+class ExamplePrompt(PromptTemplate):
+
+    class Output(BaseLLMResponse):
+        class Ingredient(BaseLLMResponse):
+            name: str
+            quantity: int
+
+        ingredients: list[Ingredient]
+
+    def system_prompt(self) -> str:
+        return "Given a recipe, extract the ingredients."
+
+    def few_shot_examples(self) -> list[FewShotExample[Output]]:
+        return [
+            FewShotExample(
+                input="Let's take two apples, three bananas, and four oranges.",
+                output=self.Output(ingredients=[
+                    self.Output.Ingredient(name="apple", quantity=2),
+                    self.Output.Ingredient(name="banana", quantity=3),
+                    self.Output.Ingredient(name="orange", quantity=4),
+                ])
+            ),
+            FewShotExample(
+                input="My recipe requires five eggs and two cups of flour.",
+                output=self.Output(ingredients=[
+                    self.Output.Ingredient(name="egg", quantity=5),
+                    self.Output.Ingredient(name="flour cups", quantity=2),
+                ])
+            )
+        ]
+
+    def user_prompt(self) -> str:
+        ...
+```
+
+
+
+
 ### Azure
 
-e sure to use the `AzureChatModel` as the model when generating the output, which consists of the deployment_id and the corresponding base model (this is used for automatically reducing prompts if needed).
+Make sure to use the `AzureChatModel` as the model when generating the output, which consists of the deployment_id and the corresponding base model (this is used for automatically reducing prompts if needed).
 ```python
 from typegpt.openai import AzureChatModel, TypeAzureOpenAI
 
 client = TypeAzureOpenAI(
     azure_endpoint="<your azure endpoint>",
     api_key="<your api key>",
     api_version="2023-05-15",
```

### Comparing `typegpt-0.2.2/setup.py` & `typegpt-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="typegpt",
-    version="0.2.2",
+    version="0.3.0",
     author="Alexander Eichhorn",
     author_email="",
     description="TypeGPT - Make GPT safe for production",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alexeichhorn/typegpt",
     install_requires=[
```

### Comparing `typegpt-0.2.2/tests/test_fields.py` & `typegpt-0.3.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/tests/test_helpers.py` & `typegpt-0.3.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/tests/test_openai.py` & `typegpt-0.3.0/tests/test_openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def test_token_counter(self):
         test_messages = [
             {"role": "system", "content": "This is a system message"},
             {"role": "user", "content": "This is a user message 🧑🏾"},
         ]
 
         # check if test covers all models (increase if new models are added)
-        assert len(OpenAIChatModel.__args__) == 17  #  type: ignore
+        assert len(OpenAIChatModel.__args__) == 19  #  type: ignore
 
         client = AsyncTypeOpenAI(api_key="mock")
 
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-3.5-turbo") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-3.5-turbo-0301") == 29
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-3.5-turbo-0613") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-3.5-turbo-1106") == 27
@@ -43,18 +43,20 @@
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-32k") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-32k-0314") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-32k-0613") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-turbo-preview") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-1106-preview") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-0125-preview") == 27
         assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-vision-preview") == 27
+        assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-turbo") == 27
+        assert client.chat.completions.num_tokens_from_messages(test_messages, model="gpt-4-turbo-2024-04-09") == 27
 
     def test_max_token_counter(self):
         # check if test covers all models (increase if new models are added)
-        assert len(OpenAIChatModel.__args__) == 17  #  type: ignore
+        assert len(OpenAIChatModel.__args__) == 19  #  type: ignore
 
         client = AsyncTypeOpenAI(api_key="mock")
 
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo") == 4096
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-0301") == 4096
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-0613") == 4096
         assert client.chat.completions.max_tokens_of_model("gpt-3.5-turbo-1106") == 16384
@@ -67,14 +69,16 @@
         assert client.chat.completions.max_tokens_of_model("gpt-4-32k") == 32768
         assert client.chat.completions.max_tokens_of_model("gpt-4-32k-0314") == 32768
         assert client.chat.completions.max_tokens_of_model("gpt-4-32k-0613") == 32768
         assert client.chat.completions.max_tokens_of_model("gpt-4-turbo-preview") == 128_000
         assert client.chat.completions.max_tokens_of_model("gpt-4-1106-preview") == 128_000
         assert client.chat.completions.max_tokens_of_model("gpt-4-0125-preview") == 128_000
         assert client.chat.completions.max_tokens_of_model("gpt-4-vision-preview") == 128_000
+        assert client.chat.completions.max_tokens_of_model("gpt-4-turbo") == 128_000
+        assert client.chat.completions.max_tokens_of_model("gpt-4-turbo-2024-04-09") == 128_000
 
     # -
 
     @pytest.fixture
     def mock_openai_completion(self, mocker):
         async def async_mock(*args, **kwargs):
             return ChatCompletion(
```

### Comparing `typegpt-0.2.2/tests/test_parser.py` & `typegpt-0.3.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/tests/test_prompt.py` & `typegpt-0.3.0/tests/test_prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -128,27 +128,62 @@
 STRING 1: <Put the first string here>
 STRING 2: <Put the second string here>
 ...
 
 ITEM 1 SUBTITLE: <Put the first subtitle here>
 ITEM 1 DESCRIPTION: <Put the first item description here>
 ITEM 1 ABSTRACT: <Some instruction>
+
 ITEM 2 SUBTITLE: <Put the second subtitle here>
 ITEM 2 DESCRIPTION: <Put the second item description here>
 ITEM 2 ABSTRACT: <Some instruction>
+
 ...
 
 SUBITEM TITLE: <Put the title here>
 
 OPTIONAL SUBITEM TITLE: <Put the title here>
 \"""
 """.strip()
 
         assert prompt == expected_prompt
 
+    # -
+
+    class SubtypeOnlyTestOutput(BaseLLMResponse):
+        class Item(BaseLLMArrayElement):
+            title: str
+            subtitles: list[str]
+
+        items: list[Item]
+
+    def test_subtype_only_output_fields(self):
+        fields = list(self.SubtypeOnlyTestOutput.__fields__.values())
+        prompt = OutputPromptFactory(fields).generate()
+        expected_prompt = f"""
+Always return the answer in the following format:
+\"""
+ITEM 1 TITLE: <Put the first title here>
+ITEM 1 SUBTITLE 1: <Put the first subtitle here>
+ITEM 1 SUBTITLE 2: <Put the second subtitle here>
+...
+
+ITEM 2 TITLE: <Put the second title here>
+ITEM 2 SUBTITLE 1: <Put the first subtitle here>
+ITEM 2 SUBTITLE 2: <Put the second subtitle here>
+...
+
+...
+\"""
+""".strip()
+
+        assert prompt == expected_prompt
+
+    # -
+
     class UltraSubtypeTestOutput(BaseLLMResponse):
         class Item(BaseLLMArrayElement):
             class InnerItem(BaseLLMResponse):
                 title: str
                 description: str
 
             class InnerElement(BaseLLMArrayElement):
@@ -165,14 +200,15 @@
                 subtitle: str
 
             title: str
             x: list[InnerDirectElement]
 
         title: str
         subitem: DirectItem
+        middle_int: int
         items: list[Item]
 
     def test_ultra_subtype_output_fields(self):
         fields = list(self.UltraSubtypeTestOutput.__fields__.values())
         prompt = OutputPromptFactory(fields).generate()
         expected_prompt = f"""
 Always return the answer in the following format:
@@ -180,30 +216,34 @@
 TITLE: <Put the title here>
 
 SUBITEM TITLE: <Put the title here>
 SUBITEM X 1 SUBTITLE: <Put the first subtitle here>
 SUBITEM X 2 SUBTITLE: <Put the second subtitle here>
 ...
 
+MIDDLE INT: <Put the middle int here>
+
 ITEM 1 SUBTITLE: <Put the first subtitle here>
 ITEM 1 DESCRIPTION: <Put the first description here>
 ITEM 1 ABSTRACT: <Put the first abstract here>
 
 ITEM 1 INNER ITEM TITLE: <Put the title here>
 ITEM 1 INNER ITEM DESCRIPTION: <Put the description here>
 
 ITEM 1 INNER ELEMENT 1 VALUE: <Put the first value here>
 ITEM 1 INNER ELEMENT 2 VALUE: <Put the second value here>
+
 ITEM 2 SUBTITLE: <Put the second subtitle here>
 ITEM 2 DESCRIPTION: <Put the second description here>
 ITEM 2 ABSTRACT: <Put the second abstract here>
 
 ITEM 2 INNER ITEM TITLE: <Put the title here>
 ITEM 2 INNER ITEM DESCRIPTION: <Put the description here>
 
 ITEM 2 INNER ELEMENT 1 VALUE: <Put the first value here>
 ITEM 2 INNER ELEMENT 2 VALUE: <Put the second value here>
+
 ...
 \"""
 """.strip()
 
         assert prompt == expected_prompt
```

### Comparing `typegpt-0.2.2/tests/test_response_object.py` & `typegpt-0.3.0/tests/test_response_object.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/base.py` & `typegpt-0.3.0/typegpt/base.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/example_formatter.py` & `typegpt-0.3.0/typegpt/example_formatter.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/fields.py` & `typegpt-0.3.0/typegpt/fields.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/helper.py` & `typegpt-0.3.0/typegpt/helper.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/message_collection_builder.py` & `typegpt-0.3.0/tests/test_settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-from __future__ import annotations
+import os
+import sys
 
-import copy
-from typing import TYPE_CHECKING, Callable, Generic, TypeVar
+myPath = os.path.dirname(os.path.abspath(__file__))
+sys.path.insert(0, myPath + "/../")
 
-from .exceptions import LLMTokenLimitExceeded
-from .prompt_builder import OutputPromptFactory
+import pytest
 
-Prompt = TypeVar("Prompt", bound="PromptTemplate")
+from typegpt import BaseLLMResponse, LLMArrayElementOutput, LLMArrayOutput, LLMOutput, PromptSettings, PromptTemplate
 
-# EncodedMessage = dict[str, dict[str, str] | str | None]
-EncodedMessage = dict[str, str]
 
+class TestSettings:
+    class InjectableSimplePrompt(PromptTemplate):
+        class Output(BaseLLMResponse):
+            title: str
 
-class MessageCollectionFactory(Generic[Prompt]):
-    def __init__(self, prompt: Prompt, token_counter: Callable[[list[EncodedMessage]], int]):
-        self.prompt = prompt
-        self.token_counter = token_counter
-        self.output_prompt_factory = OutputPromptFactory(
-            list(prompt.Output.__fields__.values())
-        )  #  TODO: add config for `threaten` and more
+        def __init__(self, settings: PromptSettings):
+            self.settings = settings
 
-    def _generate_messages_from_prompt(self, prompt: Prompt) -> list[EncodedMessage]:
-        system_prompt = prompt.system_prompt()
-        system_prompt += "\n\n"
-        system_prompt += self.output_prompt_factory.generate()
+        def system_prompt(self) -> str:
+            return "Some system prompt"
 
-        result: list[EncodedMessage] = [{"role": "system", "content": system_prompt}]
+        def user_prompt(self) -> str:
+            return "Some user prompt"
 
-        result.append({"role": "user", "content": prompt.user_prompt()})
+    class NoDirectFormattingInstructionPrompt(PromptTemplate):
+        class Output(BaseLLMResponse):
+            title: str
 
-        return result
+        settings = PromptSettings(disable_formatting_instructions=True)
 
-    def generate_messages(self, token_limit: int):
-        """
-        Generates messages dictionary that can be sent to any OpenAI equivalent API, ensuring that the total number of tokens is below the specified limit
-        Messages that do not fit in are removed inside the object permanently
-        """
+        def system_prompt(self) -> str:
+            return "Some system prompt"
 
-        generated_messages = self._generate_messages_from_prompt(self.prompt)
+        def user_prompt(self) -> str:
+            return "Some user prompt"
 
-        num_tokens = self.token_counter(generated_messages)
-        if num_tokens <= token_limit:
-            return generated_messages
+    def test_disable_formatting_instructions(self):
+        enabled_settings = PromptSettings(disable_formatting_instructions=False)
+        disabled_settings = PromptSettings(disable_formatting_instructions=True)
 
-        # try to reduce the length of the prompt
-        prompt = copy.deepcopy(self.prompt)
-        while prompt.reduce_if_possible():
-            generated_messages = self._generate_messages_from_prompt(prompt)
+        enabled_messages = self.InjectableSimplePrompt(settings=enabled_settings).generate_messages(
+            token_limit=1000, token_counter=lambda x: 0
+        )
+        disabled_messages = self.InjectableSimplePrompt(settings=disabled_settings).generate_messages(
+            token_limit=1000, token_counter=lambda x: 0
+        )
+        direct_disabled_messages = self.NoDirectFormattingInstructionPrompt().generate_messages(token_limit=1000, token_counter=lambda x: 0)
 
-            num_tokens = self.token_counter(generated_messages)
-            if num_tokens <= token_limit:
-                self.prompt = prompt  # update the prompt if successful
-                return generated_messages
+        assert len(enabled_messages) == 2
+        assert enabled_messages[0]["role"] == "system"
+        assert enabled_messages[0]["content"].count("Always return the answer in the following format:") == 1
 
-        raise LLMTokenLimitExceeded(f"Prompt can't be reduced to fit within the token limit ({token_limit})")
+        assert disabled_messages == [
+            {"role": "system", "content": "Some system prompt"},
+            {"role": "user", "content": "Some user prompt"},
+        ]
 
-
-if TYPE_CHECKING:
-    from .prompt_definition.prompt_template import PromptTemplate
+        assert direct_disabled_messages == disabled_messages
```

### Comparing `typegpt-0.2.2/typegpt/meta.py` & `typegpt-0.3.0/typegpt/meta.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/openai/_async/chat_completion.py` & `typegpt-0.3.0/typegpt/openai/_async/chat_completion.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/openai/_async/client.py` & `typegpt-0.3.0/typegpt/openai/_async/client.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/openai/_sync/chat_completion.py` & `typegpt-0.3.0/typegpt/openai/_sync/chat_completion.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/openai/_sync/client.py` & `typegpt-0.3.0/typegpt/openai/_sync/client.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/openai/base_chat_completion.py` & `typegpt-0.3.0/typegpt/openai/base_chat_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,22 @@
                 return 4096
             case "gpt-3.5-turbo-16k" | "gpt-3.5-turbo-16k-0613" | "gpt-3.5-turbo-1106" | "gpt-3.5-turbo-0125":
                 return 16384
             case "gpt-4" | "gpt-4-0314" | "gpt-4-0613":
                 return 8192
             case "gpt-4-32k" | "gpt-4-32k-0314" | "gpt-4-32k-0613":
                 return 32768
-            case "gpt-4-turbo-preview" | "gpt-4-1106-preview" | "gpt-4-0125-preview" | "gpt-4-vision-preview":
+            case (
+                "gpt-4-turbo-preview"
+                | "gpt-4-1106-preview"
+                | "gpt-4-0125-preview"
+                | "gpt-4-vision-preview"
+                | "gpt-4-turbo"
+                | "gpt-4-turbo-2024-04-09"
+            ):
                 return 128_000
 
     # copied from OpenAI: https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     @classmethod
     def num_tokens_from_messages(cls, messages: list[EncodedMessage], model: OpenAIChatModel | None = None) -> int:
         """Returns the number of tokens used by a list of messages."""
         if model is None:
@@ -50,14 +57,16 @@
             "gpt-3.5-turbo-16k-0613",
             "gpt-4-32k-0314",
             "gpt-4-32k-0613",
             "gpt-4-turbo-preview",
             "gpt-4-0125-preview",
             "gpt-4-1106-preview",
             "gpt-4-vision-preview",
+            "gpt-4-turbo",
+            "gpt-4-turbo-2024-04-09",
         ):
             tokens_per_message = 3
             tokens_per_name = 1
         else:
             raise NotImplementedError(
                 f"""num_tokens_from_messages() is not implemented for model {model}. See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens."""
             )
```

### Comparing `typegpt-0.2.2/typegpt/openai/views.py` & `typegpt-0.3.0/typegpt/openai/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,20 @@
     "gpt-3.5-turbo-16k-0613",
     "gpt-4",  # gpt-4
     "gpt-4-0314",
     "gpt-4-0613",
     "gpt-4-32k",  # gpt-4 32k
     "gpt-4-32k-0314",
     "gpt-4-32k-0613",
-    "gpt-4-turbo-preview",  # gpt-4 turbo
+    "gpt-4-turbo",  # gpt-4 turbo
+    "gpt-4-turbo-2024-04-09",
+    "gpt-4-turbo-preview",  # gpt-4 turbo (preview)
     "gpt-4-1106-preview",
     "gpt-4-0125-preview",
-    "gpt-4-vision-preview",  # gpt-4 vision
+    "gpt-4-vision-preview",  # gpt-4 vision (preview)
 ]
 
 
 @dataclass
 class AzureChatModel:
     deployment_id: str
     base_model: OpenAIChatModel  # only used for token counting
```

### Comparing `typegpt-0.2.2/typegpt/parser.py` & `typegpt-0.3.0/typegpt/parser.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt/prompt_builder.py` & `typegpt-0.3.0/typegpt/prompt_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typegpt.utils.utils import limit_newlines
 from .example_formatter import LimitedExampleListFormatter
 from .fields import ExamplePosition, LLMArrayElementOutputInfo, LLMArrayOutputInfo, LLMFieldInfo, LLMOutputInfo
 from .utils.type_checker import if_array_element_list_type, if_response_type
 
 
 class OutputPromptFactory:
     def __init__(self, fields: list[LLMFieldInfo], threaten: bool = False, name_prefixes: list[str] = []):
@@ -17,14 +18,19 @@
             subfields = list(element_type.__fields__.values())
             # subprompt_factory = OutputPromptFactory(subfields, name_prefixes=self.name_prefixes + [field.name])
             # examples = [subprompt_factory._generate_schema(offset=i + 1) for i in range(max_count)]
             examples = [
                 OutputPromptFactory(subfields, name_prefixes=self.name_prefixes + [field.name + f" {i+1}"])._generate_schema(offset=i + 1)
                 for i in range(max_count)
             ]
+            # append newline for each example that is complex enough (i.e. contains multiple lines)
+            if max_count > 0 and "\n" in examples[0]:
+                for i in range(len(examples)):
+                    examples[i] += "\n"
+                examples[0] = "\n" + examples[0]  # prepend newline to first example
         else:
             field_name = " ".join(self.name_prefixes + [field.name])
             examples = [f"{field_name} {i+1}: <{info.instruction(ExamplePosition(i+1))}>" for i in range(max_count)]
 
         if is_unlimited:
             return LimitedExampleListFormatter(max_count, "\n").format(examples) + "\n...\n"
         else:
@@ -65,22 +71,22 @@
                     prompt += field_prompt
 
             elif isinstance(field.info, LLMArrayOutputInfo):
                 prompt += self._generate_array(field, field.info)
 
             prompt += "\n"
 
-        return prompt.rstrip()
+        return limit_newlines(prompt.rstrip())
 
     def generate(self) -> str:
         if self.threaten:
             prompt = "Always return the answer in the following format, otherwise people might die and you are the only one to blame:"
         else:
             prompt = "Always return the answer in the following format:"
 
         prompt += '\n"""\n'
 
-        prompt += self._generate_schema() + "\n"
+        prompt += self._generate_schema().strip() + "\n"
 
         prompt += '"""'
 
         return prompt
```

### Comparing `typegpt-0.2.2/typegpt/prompt_definition/prompt_template.py` & `typegpt-0.3.0/typegpt/prompt_definition/prompt_template.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, ClassVar, Generic, Protocol, TypeVar
 
+from typegpt.prompt_definition.few_shot_example import FewShotExample
+from typegpt.prompt_definition.prompt_settings import PromptSettings
+
 from ..base import BaseLLMResponse
 from ..fields import LLMArrayOutput
 from ..message_collection_builder import EncodedMessage, MessageCollectionFactory
 
 # _Output = TypeVar("_Output", bound=BaseLLMResponse)
 
 
 class PromptTemplate(Protocol):  # , Generic[_Output]):
     def system_prompt(self) -> str:
+        """System prompt for the LLM (required)"""
         ...
 
     def user_prompt(self) -> str:
+        """User prompt for the LLM (required)"""
         ...
 
     def reduce_if_possible(self) -> bool:
         """
         Override this method to reduce the parameters of the prompt, which gets called when the token limit is exceeded
         @returns: whether the parameters could be further reduced
         """
         return False
 
+    def few_shot_examples(self) -> list[FewShotExample[BaseLLMResponse]]:  # list[FewShotExample[_Output]]:
+        """
+        Override this method to provide few shot examples
+        """
+        return []
+
     Output: type[BaseLLMResponse]  # type[_Output]
 
+    settings: PromptSettings = PromptSettings()
+
     def generate_messages(self, token_limit: int, token_counter: Callable[[list[EncodedMessage]], int]):
         """
         Generates messages dictionary that can be sent to any OpenAI equivalent API, ensuring that the total number of tokens is below the specified limit
         Messages that do not fit in are removed inside the object permanently
         """
         return MessageCollectionFactory(self, token_counter=token_counter).generate_messages(token_limit=token_limit)
```

### Comparing `typegpt-0.2.2/typegpt/utils/type_checker.py` & `typegpt-0.3.0/typegpt/utils/type_checker.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.2.2/typegpt.egg-info/PKG-INFO` & `typegpt-0.3.0/typegpt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typegpt
-Version: 0.2.2
+Version: 0.3.0
 Summary: TypeGPT - Make GPT safe for production
 Home-page: https://github.com/alexeichhorn/typegpt
 Author: Alexander Eichhorn
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: tiktoken>=0.5.0
 Requires-Dist: openai>=1.1.0
 
 # TypeGPT - Making GPT Safe for Production
 
 It is inherently difficult to produce outputs from LLMs in a consistent structure. TypeGPT simplifies this process to be as easy as defining a class in Python.
 
-Powering our own projects, such as [BoostSEO](https://boostseo.ai)
+Powering our own projects, such as [Spexia](https://getspexia.com)
 
 
 ## Installation
 
 ```bash
 pip install typegpt
 ```
@@ -189,17 +189,60 @@
 ```python
 prompt = ExamplePrompt(...)
 output = client.chat.completions.generate_output(model="gpt-4", prompt=prompt, output_type=ExamplePrompt.Output, ...)
 ```
 This parameter is not merely a type decorator. It can also be used to overwrite the actual output type that GPT attempts to predict.
 
 
+### Few-Shot Prompting
+
+Give examples to the model to explain tasks that are hard to explain:
+
+```python
+class ExamplePrompt(PromptTemplate):
+
+    class Output(BaseLLMResponse):
+        class Ingredient(BaseLLMResponse):
+            name: str
+            quantity: int
+
+        ingredients: list[Ingredient]
+
+    def system_prompt(self) -> str:
+        return "Given a recipe, extract the ingredients."
+
+    def few_shot_examples(self) -> list[FewShotExample[Output]]:
+        return [
+            FewShotExample(
+                input="Let's take two apples, three bananas, and four oranges.",
+                output=self.Output(ingredients=[
+                    self.Output.Ingredient(name="apple", quantity=2),
+                    self.Output.Ingredient(name="banana", quantity=3),
+                    self.Output.Ingredient(name="orange", quantity=4),
+                ])
+            ),
+            FewShotExample(
+                input="My recipe requires five eggs and two cups of flour.",
+                output=self.Output(ingredients=[
+                    self.Output.Ingredient(name="egg", quantity=5),
+                    self.Output.Ingredient(name="flour cups", quantity=2),
+                ])
+            )
+        ]
+
+    def user_prompt(self) -> str:
+        ...
+```
+
+
+
+
 ### Azure
 
-e sure to use the `AzureChatModel` as the model when generating the output, which consists of the deployment_id and the corresponding base model (this is used for automatically reducing prompts if needed).
+Make sure to use the `AzureChatModel` as the model when generating the output, which consists of the deployment_id and the corresponding base model (this is used for automatically reducing prompts if needed).
 ```python
 from typegpt.openai import AzureChatModel, TypeAzureOpenAI
 
 client = TypeAzureOpenAI(
     azure_endpoint="<your azure endpoint>",
     api_key="<your api key>",
     api_version="2023-05-15",
```

### Comparing `typegpt-0.2.2/typegpt.egg-info/SOURCES.txt` & `typegpt-0.3.0/typegpt.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 LICENSE
 README.md
 setup.py
+tests/test_fewshot.py
 tests/test_fields.py
 tests/test_helpers.py
 tests/test_openai.py
 tests/test_parser.py
 tests/test_prompt.py
 tests/test_response_object.py
+tests/test_settings.py
 typegpt/__init__.py
 typegpt/base.py
+typegpt/example_builder.py
 typegpt/example_formatter.py
 typegpt/exceptions.py
 typegpt/fields.py
 typegpt/helper.py
 typegpt/message_collection_builder.py
 typegpt/meta.py
 typegpt/parser.py
@@ -29,12 +32,14 @@
 typegpt/openai/_async/__init__.py
 typegpt/openai/_async/chat_completion.py
 typegpt/openai/_async/client.py
 typegpt/openai/_sync/__init__.py
 typegpt/openai/_sync/chat_completion.py
 typegpt/openai/_sync/client.py
 typegpt/prompt_definition/__init__.py
+typegpt/prompt_definition/few_shot_example.py
+typegpt/prompt_definition/prompt_settings.py
 typegpt/prompt_definition/prompt_template.py
 typegpt/utils/__init__.py
 typegpt/utils/internal_types.py
 typegpt/utils/type_checker.py
 typegpt/utils/utils.py
```

