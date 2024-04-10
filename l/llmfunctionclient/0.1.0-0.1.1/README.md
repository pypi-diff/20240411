# Comparing `tmp/llmfunctionclient-0.1.0.tar.gz` & `tmp/llmfunctionclient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmfunctionclient-0.1.0.tar", max compression
+gzip compressed data, was "llmfunctionclient-0.1.1.tar", max compression
```

## Comparing `llmfunctionclient-0.1.0.tar` & `llmfunctionclient-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     3778 2024-04-10 21:55:19.591756 llmfunctionclient-0.1.0/README.md
--rw-r--r--   0        0        0       19 2024-04-10 21:56:35.425094 llmfunctionclient-0.1.0/llmfunctionclient/__init__.py
--rw-r--r--   0        0        0     3366 2024-04-10 21:30:37.649873 llmfunctionclient-0.1.0/llmfunctionclient/main.py
--rw-r--r--   0        0        0      321 2024-04-10 21:30:19.012299 llmfunctionclient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4476 1970-01-01 00:00:00.000000 llmfunctionclient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     4328 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/README.md
+-rw-r--r--   0        0        0       19 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/llmfunctionclient/__init__.py
+-rw-r--r--   0        0        0     3936 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/llmfunctionclient/main.py
+-rw-r--r--   0        0        0      321 2024-04-10 22:42:50.361950 llmfunctionclient-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5026 1970-01-01 00:00:00.000000 llmfunctionclient-0.1.1/PKG-INFO
```

### Comparing `llmfunctionclient-0.1.0/README.md` & `llmfunctionclient-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Python LLM Function Client
 
 The purpose of this library is to simplify using function calling with OpenAI-like API clients. Traditionally, you would have to rewrite your functions into JSON Schema and write logic to handle tool calls in responses. With this library, you can convert python functions into JSON schema by simply calling `to_tool(func)` or you can create a client that will handle those tool calls for you and simply pass back a response once the tool call chain is finished by creating an instance of `FunctionClient`.
 
+## Installation
+
+To install simply run:
+`pip install llmfunctionclient`
+
 ## Requirements for Functions
 
 Functions used with this library must have type annotations for each parameter. You do not have to have an annotation for the return type of the function.
 Currently, the supported types are string, int, StrEnum and IntEnum.
 If the type is a StrEnum or IntEnum, the valid values will be included as part of the function tool spec.
 
 Optionally, you can include a docstring to add descriptions. The first line of the docstring will be considered the description of the function. Subsequent lines should be of the format `<parameter_name>: <description>`
@@ -49,14 +54,18 @@
 1. The two message specified here will be submitted to the LLM Client
 2. The LLM Client responds with a tool call for "get_weather"
 3. The get_weather function is called and the result is appended as a message
 4. The LLM Client is called again with the function result.
 5. The LLM Client Responds with an informed answer.
 6. This response text is passed back.
 
+You can pass functions into the constructor of the client to create the default set of tools for every message as well as pass in the `functions` kwarg to `send_message` to specify a specific set of functions for that portion of the conversation.
+
+To force the LLM to use a specific function, you can pass the `force_function` kwarg with the function (or its name) you want the LLM to use and it will be provided as the tool_choice parameter for the chat completion endpoint.
+
 ## to_tool
 
 If you want to continue using any other LLM clients and just want the ability to convert python functions into JSON Schema compatible with the function calling spec, you can simply import the function to_tool and call that on the function.
 
 Example:
 ```python
 def get_weather(location: str):
```

### Comparing `llmfunctionclient-0.1.0/llmfunctionclient/main.py` & `llmfunctionclient-0.1.1/llmfunctionclient/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -64,42 +64,57 @@
   }
   if top_description:
     tool['description'] = top_description
   return tool
 
 class FunctionClient:
   def __init__(self, client, model, functions, messages=None):
-     self.tools = [to_tool(func) for func in functions]
-     print(self.tools)
-     self.tools_map = {func.__name__: func for func in functions}
      self.messages = messages or []
      self.model = model
      self.client = client
+     self.functions = functions
+
+  @staticmethod
+  def funcs_to_tools(funcs):
+    return [to_tool(func) for func in funcs], {func.__name__: func for func in funcs}
 
   def add_message(self, content, role='user'):
     self.messages.append({'role': role, 'content': content})
 
-  def internal_send_message(self):
+  def internal_send_message(self, functions, force_function = None):
+    tools, tools_map = self.funcs_to_tools(functions)
+    args = {
+      'model': self.model,
+      'messages': self.messages,
+      'tools': tools,
+    }
+    if force_function:
+       args['tool_choice'] = {"type": "function", "function": {"name": force_function}}
     response = self.client.chat.completions.create(
       model=self.model,
       messages=self.messages,
-      tools=self.tools
+      tools=tools,
     )
     message = response.choices[0].message
     if message.tool_calls:
       for tool_call in message.tool_calls:
         args = json.loads(tool_call.function.arguments)
-        result = self.tools_map[tool_call.function.name](**args)
+        result = tools_map[tool_call.function.name](**args)
         print(f'Function call: {tool_call.function.name}({args})')
         self.messages.append({"role": "function", "tool_call_id": tool_call.id, "name": tool_call.function.name, "content": result})
       return False
     else:
       self.messages.append({"role": "assistant", "content": message.content})
       return True
 
-  def send_message(self, role=None, content=None):
+  def send_message(self, content=None, role=None, functions=None, force_function=None):
     if content:
       self.add_message(content, role)
+    if not functions:
+       functions = self.functions
+    if isinstance(force_function, callable):
+       force_function = force_function.__name__
     done = False
+    done = self.internal_send_message(functions, force_function)
     while not done:
-      done = self.internal_send_message()
+      done = self.internal_send_message(functions)
     return self.messages[-1]['content']
```

### Comparing `llmfunctionclient-0.1.0/PKG-INFO` & `llmfunctionclient-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfunctionclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: James Mills
 Author-email: jimmyemills@gmail.com
 Requires-Python: >=3.4,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -17,14 +17,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Python LLM Function Client
 
 The purpose of this library is to simplify using function calling with OpenAI-like API clients. Traditionally, you would have to rewrite your functions into JSON Schema and write logic to handle tool calls in responses. With this library, you can convert python functions into JSON schema by simply calling `to_tool(func)` or you can create a client that will handle those tool calls for you and simply pass back a response once the tool call chain is finished by creating an instance of `FunctionClient`.
 
+## Installation
+
+To install simply run:
+`pip install llmfunctionclient`
+
 ## Requirements for Functions
 
 Functions used with this library must have type annotations for each parameter. You do not have to have an annotation for the return type of the function.
 Currently, the supported types are string, int, StrEnum and IntEnum.
 If the type is a StrEnum or IntEnum, the valid values will be included as part of the function tool spec.
 
 Optionally, you can include a docstring to add descriptions. The first line of the docstring will be considered the description of the function. Subsequent lines should be of the format `<parameter_name>: <description>`
@@ -68,14 +73,18 @@
 1. The two message specified here will be submitted to the LLM Client
 2. The LLM Client responds with a tool call for "get_weather"
 3. The get_weather function is called and the result is appended as a message
 4. The LLM Client is called again with the function result.
 5. The LLM Client Responds with an informed answer.
 6. This response text is passed back.
 
+You can pass functions into the constructor of the client to create the default set of tools for every message as well as pass in the `functions` kwarg to `send_message` to specify a specific set of functions for that portion of the conversation.
+
+To force the LLM to use a specific function, you can pass the `force_function` kwarg with the function (or its name) you want the LLM to use and it will be provided as the tool_choice parameter for the chat completion endpoint.
+
 ## to_tool
 
 If you want to continue using any other LLM clients and just want the ability to convert python functions into JSON Schema compatible with the function calling spec, you can simply import the function to_tool and call that on the function.
 
 Example:
 ```python
 def get_weather(location: str):
```

