# Comparing `tmp/uagents_ai_engine-0.1.5.tar.gz` & `tmp/uagents_ai_engine-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_ai_engine-0.1.5.tar", max compression
+gzip compressed data, was "uagents_ai_engine-0.1.6.tar", max compression
```

## Comparing `uagents_ai_engine-0.1.5.tar` & `uagents_ai_engine-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      209 2024-03-15 19:58:48.912304 uagents_ai_engine-0.1.5/README.md
--rw-r--r--   0        0        0      394 2024-04-04 08:59:10.091291 uagents_ai_engine-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       89 2024-03-15 19:58:57.112803 uagents_ai_engine-0.1.5/src/ai_engine/__init__.py
--rw-r--r--   0        0        0     4487 2024-04-04 04:31:33.596581 uagents_ai_engine-0.1.5/src/ai_engine/chitchat.py
--rw-r--r--   0        0        0     2284 2024-04-04 04:31:33.596720 uagents_ai_engine-0.1.5/src/ai_engine/dialogue.py
--rw-r--r--   0        0        0     2967 2024-04-04 08:59:10.091701 uagents_ai_engine-0.1.5/src/ai_engine/messages.py
--rw-r--r--   0        0        0      765 2024-03-15 19:58:48.914653 uagents_ai_engine-0.1.5/src/ai_engine/types.py
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 uagents_ai_engine-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-03-15 19:58:48.912304 uagents_ai_engine-0.1.6/README.md
+-rw-r--r--   0        0        0      394 2024-04-11 12:32:46.289573 uagents_ai_engine-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-03-15 19:58:57.112803 uagents_ai_engine-0.1.6/src/ai_engine/__init__.py
+-rw-r--r--   0        0        0     4487 2024-04-04 04:31:33.596581 uagents_ai_engine-0.1.6/src/ai_engine/chitchat.py
+-rw-r--r--   0        0        0     2302 2024-04-11 12:32:46.290062 uagents_ai_engine-0.1.6/src/ai_engine/dialogue.py
+-rw-r--r--   0        0        0     2967 2024-04-04 08:59:10.091701 uagents_ai_engine-0.1.6/src/ai_engine/messages.py
+-rw-r--r--   0        0        0      765 2024-03-15 19:58:48.914653 uagents_ai_engine-0.1.6/src/ai_engine/types.py
+-rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 uagents_ai_engine-0.1.6/PKG-INFO
```

### Comparing `uagents_ai_engine-0.1.5/src/ai_engine/chitchat.py` & `uagents_ai_engine-0.1.6/src/ai_engine/chitchat.py`

 * *Files identical despite different names*

### Comparing `uagents_ai_engine-0.1.5/src/ai_engine/dialogue.py` & `uagents_ai_engine-0.1.6/src/ai_engine/dialogue.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     terminal: bool = False
 
 
 class EdgeMetadata(BaseModel):
     """Metadata for the edges"""
 
     # what is the target of this transition, user means direct message to the user, ai, system involves AI Engine processing
-    target: Literal["user", "ai", "system"]
+    target: Literal["user", "ai", "system", "agent"]
 
     # can the AI Engine observe this transition, and process the information
     observable: bool
 
 
 class NodeDescription(BaseModel):
     """Temporary type to add structure to the node description"""
@@ -71,15 +71,15 @@
         description=description.json(),
     )
 
 
 def create_edge(
     name: str,
     description: str,
-    target: Literal["user", "ai", "system"],
+    target: Literal["user", "ai", "system", "agent"],
     observable: bool,
     parent: Node,
     child: Node,
 ):
     """Create an edge with metadata"""
 
     # create the metadata
```

### Comparing `uagents_ai_engine-0.1.5/src/ai_engine/messages.py` & `uagents_ai_engine-0.1.6/src/ai_engine/messages.py`

 * *Files identical despite different names*

### Comparing `uagents_ai_engine-0.1.5/src/ai_engine/types.py` & `uagents_ai_engine-0.1.6/src/ai_engine/types.py`

 * *Files identical despite different names*

### Comparing `uagents_ai_engine-0.1.5/PKG-INFO` & `uagents_ai_engine-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents-ai-engine
-Version: 0.1.5
+Version: 0.1.6
 Summary: Integrating AI-Engine with UAgents
 License: Apache 2.0
 Keywords: uagents,agents,ai,ai-engine,fetch.ai
 Author: Fetch.AI Limited
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

