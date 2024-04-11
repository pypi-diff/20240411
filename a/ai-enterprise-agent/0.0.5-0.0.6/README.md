# Comparing `tmp/ai-enterprise-agent-0.0.5.tar.gz` & `tmp/ai-enterprise-agent-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-enterprise-agent-0.0.5.tar", last modified: Thu Apr 11 18:05:16 2024, max compression
+gzip compressed data, was "ai-enterprise-agent-0.0.6.tar", last modified: Thu Apr 11 20:58:45 2024, max compression
```

## Comparing `ai-enterprise-agent-0.0.5.tar` & `ai-enterprise-agent-0.0.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.730979 ai-enterprise-agent-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-11 18:05:16.730979 ai-enterprise-agent-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.722978 ai-enterprise-agent-0.0.5/ai_enterprise_agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.722978 ai-enterprise-agent-0.0.5/ai_enterprise_agent/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/interface/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/interface/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/interface/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/interface/vector_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.722978 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.726979 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/open_api_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/orchestrator_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/sequential_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/simple_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/sql_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/vector_store_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.726979 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chat_history/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chat_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chat_history/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chat_history/memory_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.726979 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/llm/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/llm/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/llm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.726979 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/vector_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.726979 ai-enterprise-agent-0.0.5/ai_enterprise_agent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent/utils/fetch_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:05:16.730979 ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-11 18:05:16.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-11 18:05:16.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:05:16.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-11 18:05:16.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 18:05:16.000000 ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:05:16.730979 ai-enterprise-agent-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-11 18:05:12.000000 ai-enterprise-agent-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.209381 ai-enterprise-agent-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-11 20:58:45.209381 ai-enterprise-agent-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.201381 ai-enterprise-agent-0.0.6/ai_enterprise_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.201381 ai-enterprise-agent-0.0.6/ai_enterprise_agent/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/interface/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/interface/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/interface/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/interface/vector_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.201381 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.201381 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/open_api_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/orchestrator_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/sequential_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/simple_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/sql_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/vector_store_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.205381 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chat_history/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chat_history/memory_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chat_history/memory_chat_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.205381 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/llm/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/llm/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/llm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.205381 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/vector_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.205381 ai-enterprise-agent-0.0.6/ai_enterprise_agent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent/utils/fetch_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:58:45.205381 ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-04-11 20:58:45.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-11 20:58:45.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:58:45.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-11 20:58:45.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 20:58:45.000000 ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:58:45.209381 ai-enterprise-agent-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-11 20:58:40.000000 ai-enterprise-agent-0.0.6/setup.py
```

### Comparing `ai-enterprise-agent-0.0.5/LICENSE` & `ai-enterprise-agent-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/PKG-INFO` & `ai-enterprise-agent-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-enterprise-agent
-Version: 0.0.5
+Version: 0.0.6
 Summary: AI Agent simplifies the implementation and use of generative AI with LangChain.
 Author: Author
 Author-email: autor@autor.com.br
 License: Apache 2.0 License
 Keywords: ai ai-agent agent assistant enterprise
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -78,15 +78,15 @@
 Requires-Dist: pyasn1-modules==0.3.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydantic_core==2.16.3
 Requires-Dist: PyJWT==2.8.0
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: pywin32==306
+Requires-Dist: pypiwin32==223
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: redis==5.0.3
 Requires-Dist: regex==2023.12.25
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-oauthlib==2.0.0
 Requires-Dist: rsa==4.9
 Requires-Dist: s3transfer==0.10.1
```

### Comparing `ai-enterprise-agent-0.0.5/README.md` & `ai-enterprise-agent-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/agent.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/agent.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/interface/chat_history.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/interface/chat_history.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/interface/settings.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/interface/settings.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/chain.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/open_api_chain.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/open_api_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/orchestrator_chain.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/orchestrator_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/sequential_chain.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/sequential_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/simple_chain.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/simple_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/sql_chain.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/sql_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chains/vector_store_chain.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chains/vector_store_chain.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chat_history/memory.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chat_history/memory.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chat_history/memory_chat_history.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chat_history/memory_chat_history.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/chat_history/memory_chat_redis.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/chat_history/memory_chat_redis.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/llm/azure.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/llm/azure.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/llm/google.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/llm/google.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/llm/model.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/llm/model.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/aws.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/aws.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/azure.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/azure.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/embedding.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/embedding.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/pinecone.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/pinecone.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/services/vector_store/vector_store.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/services/vector_store/vector_store.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent/utils/fetch_helper.py` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent/utils/fetch_helper.py`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/PKG-INFO` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-enterprise-agent
-Version: 0.0.5
+Version: 0.0.6
 Summary: AI Agent simplifies the implementation and use of generative AI with LangChain.
 Author: Author
 Author-email: autor@autor.com.br
 License: Apache 2.0 License
 Keywords: ai ai-agent agent assistant enterprise
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -78,15 +78,15 @@
 Requires-Dist: pyasn1-modules==0.3.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pydantic_core==2.16.3
 Requires-Dist: PyJWT==2.8.0
 Requires-Dist: pypdf==4.2.0
 Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: pywin32==306
+Requires-Dist: pypiwin32==223
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: redis==5.0.3
 Requires-Dist: regex==2023.12.25
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-oauthlib==2.0.0
 Requires-Dist: rsa==4.9
 Requires-Dist: s3transfer==0.10.1
```

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/SOURCES.txt` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-enterprise-agent-0.0.5/ai_enterprise_agent.egg-info/requires.txt` & `ai-enterprise-agent-0.0.6/ai_enterprise_agent.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 pyasn1-modules==0.3.0
 pycparser==2.21
 pydantic==2.6.4
 pydantic_core==2.16.3
 PyJWT==2.8.0
 pypdf==4.2.0
 python-dateutil==2.9.0.post0
-pywin32==306
+pypiwin32==223
 PyYAML==6.0.1
 redis==5.0.3
 regex==2023.12.25
 requests==2.31.0
 requests-oauthlib==2.0.0
 rsa==4.9
 s3transfer==0.10.1
```

### Comparing `ai-enterprise-agent-0.0.5/setup.py` & `ai-enterprise-agent-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='ai-enterprise-agent',
-    version='0.0.5',
+    version='0.0.6',
     license='Apache 2.0 License',
     author='Author',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='autor@autor.com.br',
     keywords='ai ai-agent agent assistant enterprise',
     description='AI Agent simplifies the implementation and use of generative AI with LangChain.',
@@ -85,15 +85,15 @@
       'pyasn1-modules==0.3.0',
       'pycparser==2.21',
       'pydantic==2.6.4',
       'pydantic_core==2.16.3',
       'PyJWT==2.8.0',
       'pypdf==4.2.0',
       'python-dateutil==2.9.0.post0',
-      'pywin32==306',
+      'pypiwin32==223',
       'PyYAML==6.0.1',
       'redis==5.0.3',
       'regex==2023.12.25',
       'requests==2.31.0',
       'requests-oauthlib==2.0.0',
       'rsa==4.9',
       's3transfer==0.10.1',
```

