# Comparing `tmp/rigging-0.2.0.tar.gz` & `tmp/rigging-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigging-0.2.0.tar", max compression
+gzip compressed data, was "rigging-0.2.1.tar", max compression
```

## Comparing `rigging-0.2.0.tar` & `rigging-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1066 2024-03-29 20:55:17.686656 rigging-0.2.0/LICENSE
--rw-r--r--   0        0        0     6791 2024-03-29 20:55:17.686656 rigging-0.2.0/README.md
--rw-r--r--   0        0        0     1841 2024-03-29 20:55:17.686656 rigging-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      375 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/__init__.py
--rw-r--r--   0        0        0    11947 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/chat.py
--rw-r--r--   0        0        0      457 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/error.py
--rw-r--r--   0        0        0     5068 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/generator.py
--rw-r--r--   0        0        0     1501 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/logging.py
--rw-r--r--   0        0        0     6593 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/message.py
--rw-r--r--   0        0        0     8638 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/model.py
--rw-r--r--   0        0        0      984 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/prompt.py
--rw-r--r--   0        0        0        0 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/py.typed
--rw-r--r--   0        0        0     8455 2024-03-29 20:55:17.686656 rigging-0.2.0/rigging/tool.py
--rw-r--r--   0        0        0     7523 1970-01-01 00:00:00.000000 rigging-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-10 22:37:42.924340 rigging-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6803 2024-04-10 22:37:42.924340 rigging-0.2.1/README.md
+-rw-r--r--   0        0        0     1841 2024-04-10 22:37:42.924340 rigging-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      375 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/__init__.py
+-rw-r--r--   0        0        0    12752 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/chat.py
+-rw-r--r--   0        0        0      457 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/error.py
+-rw-r--r--   0        0        0     5068 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/generator.py
+-rw-r--r--   0        0        0     1501 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/logging.py
+-rw-r--r--   0        0        0     6593 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/message.py
+-rw-r--r--   0        0        0     8638 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/model.py
+-rw-r--r--   0        0        0     1090 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/py.typed
+-rw-r--r--   0        0        0     8455 2024-04-10 22:37:42.924340 rigging-0.2.1/rigging/tool.py
+-rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 rigging-0.2.1/PKG-INFO
```

### Comparing `rigging-0.2.0/LICENSE` & `rigging-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rigging-0.2.0/README.md` & `rigging-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 chat = (
     rg.get_generator("mistral/mistral-tiny")
     .chat(
         [
             {"role": "user", "content": "What is the weather in London?"},
         ]
     )
-    .using(WeatherTool())
+    .using(WeatherTool(), force=True)
     .run()
 )
 
 # [=] get_for_city('London')
 
 print(chat.last.content)
```

### Comparing `rigging-0.2.0/pyproject.toml` & `rigging-0.2.1/pyproject.toml`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rigging"
-version = "0.2.0"
+version = "0.2.1"
 description = "LLM Interaction Framework"
 authors = ["Nick Landers <monoxgas@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/dreadnode/rigging"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `rigging-0.2.0/rigging/chat.py` & `rigging-0.2.1/rigging/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         self.chat: Chat = Chat(messages, pending=self)
 
         # (callback, attempt_recovery, drop_dialog, max_rounds)
         self.until_callbacks: list[tuple[UntilCallback, bool, bool, int]] = []
         self.until_types: list[type[Model]] = []
         self.until_tools: list[Tool] = []
         self.inject_tool_prompt: bool = True
+        self.force_tool: bool = False
 
         self.params = params
 
     def overload(self, **kwargs: t.Any) -> "PendingChat":
         from rigging.generator import GenerateParams
 
         return self.with_params(GenerateParams(**kwargs))
@@ -176,23 +177,32 @@
         self.until_callbacks.append((callback, attempt_recovery, drop_dialog, max_rounds))
         return self
 
     def using(
         self,
         tool: Tool | t.Sequence[Tool],
         *,
+        force: bool = False,
         attempt_recovery: bool = True,
         drop_dialog: bool = False,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
         inject_prompt: bool | None = None,
     ) -> "PendingChat":
         self.until_tools += tool if isinstance(tool, t.Sequence) else [tool]
         self.inject_tool_prompt = inject_prompt or self.inject_tool_prompt
+        self.force_tool = force
         if next((c for c in self.until_callbacks if c[0] == self._until_tools_callback), None) is None:
-            self.until_callbacks.append((self._until_tools_callback, attempt_recovery, drop_dialog, max_rounds))
+            self.until_callbacks.append(
+                (
+                    self._until_tools_callback,
+                    attempt_recovery,
+                    drop_dialog,
+                    max_rounds,
+                )
+            )
         return self
 
     def until_parsed_as(
         self,
         types: type[ModelT] | t.Sequence[type[ModelT]],
         *,
         attempt_recovery: bool = False,
@@ -211,16 +221,22 @@
         try:
             tool_calls = message.try_parse(ToolCalls)
         except ValidationError as e:
             next_messages.append(Message.from_model(ValidationErrorModel(content=e)))
             return (True, next_messages)
 
         if tool_calls is None:
-            logger.debug("No tool calls or types, returning message")
-            return (False, next_messages)
+            if self.force_tool:
+                logger.debug("No tool calls or types, returning error")
+                next_messages.append(Message.from_model(SystemErrorModel(content="You must use a tool")))
+            else:
+                logger.debug("No tool calls or types, returning message")
+            return (self.force_tool, next_messages)
+
+        self.force_tool = False
 
         tool_results: list[ToolResult] = []
         errors: list[SystemErrorModel] = []
         for call in tool_calls.calls:
             if call.tool not in [tool.name for tool in self.until_tools]:
                 errors.append(SystemErrorModel(content=f"Tool '{call.tool}' does not exist"))
                 continue
@@ -294,15 +310,21 @@
                 running_messages += step_messages
 
         logger.warning(f"Exhausted max rounds ({max_rounds})")
         raise ExhaustedMaxRoundsError(max_rounds)
 
     def _execute(self) -> list[Message]:
         if self.until_tools:
-            self.params.stop = [ToolCalls.xml_end_tag()]
+            # TODO: This can cause issues when certain APIs do not return
+            # the stop sequence as part of the response. This behavior
+            # seems like a larger issue than the model continuining after
+            # requesting a tool call, so we'll remove it for now.
+            #
+            # self.params.stop = [ToolCalls.xml_end_tag()]
+
             if self.inject_tool_prompt:
                 self.chat.inject_tool_prompt(self.until_tools)
 
         new_messages: list[Message] = [self.generator.complete(self.chat.all, self.params)]
 
         for callback, reset_between, drop_internal, max_rounds in self.until_callbacks:
             next_messages = self._until(
```

### Comparing `rigging-0.2.0/rigging/generator.py` & `rigging-0.2.1/rigging/generator.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.0/rigging/logging.py` & `rigging-0.2.1/rigging/logging.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.0/rigging/message.py` & `rigging-0.2.1/rigging/message.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.0/rigging/model.py` & `rigging-0.2.1/rigging/model.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.0/rigging/tool.py` & `rigging-0.2.1/rigging/tool.py`

 * *Files identical despite different names*

### Comparing `rigging-0.2.0/PKG-INFO` & `rigging-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigging
-Version: 0.2.0
+Version: 0.2.1
 Summary: LLM Interaction Framework
 Home-page: https://github.com/dreadnode/rigging
 License: MIT
 Author: Nick Landers
 Author-email: monoxgas@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -167,15 +167,15 @@
 chat = (
     rg.get_generator("mistral/mistral-tiny")
     .chat(
         [
             {"role": "user", "content": "What is the weather in London?"},
         ]
     )
-    .using(WeatherTool())
+    .using(WeatherTool(), force=True)
     .run()
 )
 
 # [=] get_for_city('London')
 
 print(chat.last.content)
```

