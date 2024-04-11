# Comparing `tmp/neurowave_logger-0.2.2b0.tar.gz` & `tmp/neurowave_logger-0.2.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurowave_logger-0.2.2b0.tar", max compression
+gzip compressed data, was "neurowave_logger-0.2.3b0.tar", max compression
```

## Comparing `neurowave_logger-0.2.2b0.tar` & `neurowave_logger-0.2.3b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       62 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/README.md
--rw-r--r--   0        0        0        0 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/__init__.py
--rw-r--r--   0        0        0     7126 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/langchain_tracer.py
--rw-r--r--   0        0        0     4150 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/tracer.py
--rw-r--r--   0        0        0        0 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/utils/__init__.py
--rw-r--r--   0        0        0     4878 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/utils/openai_info.py
--rw-r--r--   0        0        0     1105 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/nwlogger/utils/text_print.py
--rw-r--r--   0        0        0      501 2024-04-10 00:33:46.886082 neurowave_logger-0.2.2b0/pyproject.toml
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 neurowave_logger-0.2.2b0/PKG-INFO
+-rw-r--r--   0        0        0       62 2024-04-11 06:18:56.858797 neurowave_logger-0.2.3b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/__init__.py
+-rw-r--r--   0        0        0     7115 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/langchain_tracer.py
+-rw-r--r--   0        0        0     4150 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/tracer.py
+-rw-r--r--   0        0        0        0 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/utils/__init__.py
+-rw-r--r--   0        0        0     4878 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/utils/openai_info.py
+-rw-r--r--   0        0        0     1105 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/nwlogger/utils/text_print.py
+-rw-r--r--   0        0        0      501 2024-04-11 06:18:56.862797 neurowave_logger-0.2.3b0/pyproject.toml
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 neurowave_logger-0.2.3b0/PKG-INFO
```

### Comparing `neurowave_logger-0.2.2b0/nwlogger/langchain_tracer.py` & `neurowave_logger-0.2.3b0/nwlogger/langchain_tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,18 +120,17 @@
         item = {
             "content": question,
             "role": "user",
             "index": len(self.conversation["messages"]),
         }
         self.conversation["messages"].append(item)
 
-    def log_context(self, context: str) -> None:
-
+    def log_verbose(self, info: Dict) -> None:
         if len(self.conversation["messages"]) > 0 and self.conversation["messages"][-1].get("role") == "assistant":
-            self.conversation["messages"][-1]["context"] = context
+            self.conversation["messages"][-1].update(info)
         else:
             pass
 
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> None:
         """Collect token usage."""
 
         if response.llm_output is None:
```

### Comparing `neurowave_logger-0.2.2b0/nwlogger/tracer.py` & `neurowave_logger-0.2.3b0/nwlogger/tracer.py`

 * *Files identical despite different names*

### Comparing `neurowave_logger-0.2.2b0/nwlogger/utils/openai_info.py` & `neurowave_logger-0.2.3b0/nwlogger/utils/openai_info.py`

 * *Files identical despite different names*

### Comparing `neurowave_logger-0.2.2b0/nwlogger/utils/text_print.py` & `neurowave_logger-0.2.3b0/nwlogger/utils/text_print.py`

 * *Files identical despite different names*

### Comparing `neurowave_logger-0.2.2b0/PKG-INFO` & `neurowave_logger-0.2.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurowave-logger
-Version: 0.2.2b0
+Version: 0.2.3b0
 Summary: Log agent for Neurowave
 License: MIT
 Author: Neurowave AI
 Author-email: it@neurowave.ai
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

