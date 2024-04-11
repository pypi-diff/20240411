# Comparing `tmp/scrapegraphai-0.1.4.tar.gz` & `tmp/scrapegraphai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.1.4.tar", max compression
+gzip compressed data, was "scrapegraphai-0.1.5.tar", max compression
```

## Comparing `scrapegraphai-0.1.4.tar` & `scrapegraphai-0.1.5.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.1.4/LICENSE
--rw-r--r--   0        0        0     6999 2024-04-10 07:49:00.999641 scrapegraphai-0.1.4/README.md
--rw-r--r--   0        0        0     1621 2024-04-10 10:20:50.478712 scrapegraphai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.1.4/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.1.4/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.1.4/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      205 2024-04-06 12:46:22.006551 scrapegraphai-0.1.4/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     3212 2024-04-09 19:38:23.615281 scrapegraphai-0.1.4/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     3041 2024-04-08 20:24:28.569893 scrapegraphai-0.1.4/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2161 2024-04-09 11:20:43.625882 scrapegraphai-0.1.4/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2264 2024-04-09 08:20:31.578158 scrapegraphai-0.1.4/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3000 2024-04-09 09:44:17.066614 scrapegraphai-0.1.4/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.1.4/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      732 2024-04-09 11:47:11.921274 scrapegraphai-0.1.4/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.1.4/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.1.4/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      252 2024-04-08 16:13:44.453206 scrapegraphai-0.1.4/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.1.4/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.1.4/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.1.4/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.1.4/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.1.4/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.1.4/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      448 2024-04-06 12:46:22.007377 scrapegraphai-0.1.4/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.1.4/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.1.4/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3209 2024-04-09 09:44:17.067983 scrapegraphai-0.1.4/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     5602 2024-04-08 16:13:44.455773 scrapegraphai-0.1.4/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     4023 2024-03-27 19:54:31.570449 scrapegraphai-0.1.4/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1592 2024-04-08 16:13:44.455987 scrapegraphai-0.1.4/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3337 2024-04-08 20:26:19.442517 scrapegraphai-0.1.4/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4728 2024-04-10 07:49:01.005389 scrapegraphai-0.1.4/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     4521 2024-04-09 08:22:49.561048 scrapegraphai-0.1.4/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     1635 2024-04-08 20:27:04.824493 scrapegraphai-0.1.4/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.1.4/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.1.4/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.1.4/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.1.4/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      767 2024-04-06 12:43:33.712605 scrapegraphai-0.1.4/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.1.4/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.1.4/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.1.4/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     8586 1970-01-01 00:00:00.000000 scrapegraphai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.1.5/LICENSE
+-rw-r--r--   0        0        0     6999 2024-04-11 16:23:21.991624 scrapegraphai-0.1.5/README.md
+-rw-r--r--   0        0        0     1621 2024-04-11 20:59:57.776276 scrapegraphai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.1.5/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.1.5/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.1.5/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      205 2024-04-06 12:46:22.006551 scrapegraphai-0.1.5/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     3635 2024-04-11 20:59:48.392539 scrapegraphai-0.1.5/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     4644 2024-04-11 17:29:53.798493 scrapegraphai-0.1.5/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2191 2024-04-11 17:29:53.798710 scrapegraphai-0.1.5/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2380 2024-04-11 17:29:53.798934 scrapegraphai-0.1.5/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3120 2024-04-11 17:29:53.799158 scrapegraphai-0.1.5/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.1.5/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-09 11:47:11.921274 scrapegraphai-0.1.5/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-04-09 11:20:43.626222 scrapegraphai-0.1.5/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2363 2024-04-08 20:25:15.266957 scrapegraphai-0.1.5/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      290 2024-04-11 20:59:48.392874 scrapegraphai-0.1.5/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-04-09 11:20:43.626608 scrapegraphai-0.1.5/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-08 20:25:27.931161 scrapegraphai-0.1.5/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      839 2024-04-11 20:59:48.393159 scrapegraphai-0.1.5/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-04-08 20:25:35.475199 scrapegraphai-0.1.5/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-04-08 20:25:42.545477 scrapegraphai-0.1.5/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-04-08 20:25:31.195250 scrapegraphai-0.1.5/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-04-08 20:25:37.349894 scrapegraphai-0.1.5/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      448 2024-04-06 12:46:22.007377 scrapegraphai-0.1.5/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-08 20:25:53.786578 scrapegraphai-0.1.5/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.1.5/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3209 2024-04-09 09:44:17.067983 scrapegraphai-0.1.5/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5602 2024-04-11 20:59:43.888685 scrapegraphai-0.1.5/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     4023 2024-03-27 19:54:31.570449 scrapegraphai-0.1.5/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-08 16:13:44.455987 scrapegraphai-0.1.5/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-08 20:26:19.442517 scrapegraphai-0.1.5/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4939 2024-04-11 20:59:48.393720 scrapegraphai-0.1.5/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     4520 2024-04-11 17:29:53.800171 scrapegraphai-0.1.5/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     1635 2024-04-08 20:27:04.824493 scrapegraphai-0.1.5/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      242 2024-04-11 17:29:53.800438 scrapegraphai-0.1.5/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.1.5/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.1.5/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.1.5/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0     1504 2024-04-11 17:29:53.800583 scrapegraphai-0.1.5/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      767 2024-04-06 12:43:33.712605 scrapegraphai-0.1.5/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.1.5/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.1.5/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.1.5/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     8586 1970-01-01 00:00:00.000000 scrapegraphai-0.1.5/PKG-INFO
```

### Comparing `scrapegraphai-0.1.4/LICENSE` & `scrapegraphai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/README.md` & `scrapegraphai-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/pyproject.toml` & `scrapegraphai-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.1.4"
+version = "0.1.5"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `scrapegraphai-0.1.4/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.1.5/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.1.5/scrapegraphai/graphs/abstract_graph.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-""" 
+"""
 Module having abstract class for creating all the graphs
 """
 from abc import ABC, abstractmethod
 from typing import Optional
-from ..models import OpenAI, Gemini, Ollama, AzureOpenAI
+from ..models import OpenAI, Gemini, Ollama, AzureOpenAI, HuggingFace
 from ..helpers import models_tokens
 
-
 class AbstractGraph(ABC):
     """
     Abstract class representing a generic graph-based tool.
     """
 
     def __init__(self, prompt: str, config: dict, source: Optional[str] = None):
         """
@@ -19,22 +18,25 @@
         self.prompt = prompt
         self.source = source
         self.config = config
         self.llm_model = self._create_llm(config["llm"])
         self.embedder_model = None if "embeddings" not in config else self._create_llm(
             config["embeddings"])
         self.graph = self._create_graph()
+        
+        self.final_state = None
+        self.execution_info = None
 
     def _create_llm(self, llm_config: dict):
         """
         Creates an instance of the language model (OpenAI or Gemini) based on configuration.
         """
         llm_defaults = {
             "temperature": 0,
-            "streaming": True
+            "streaming": False
         }
         llm_params = {**llm_defaults, **llm_config}
 
         # Instantiate the language model based on the model name
         if "gpt-" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["openai"][llm_params["model"]]
@@ -42,50 +44,55 @@
                 raise ValueError("Model not supported")
             return OpenAI(llm_params)
 
         elif "azure" in llm_params["model"]:
             # take the model after the last dash
             llm_params["model"] = llm_params["model"].split("/")[-1]
             try:
-                self.model_token = models_tokens["openai"][llm_params["model"]]
+                self.model_token = models_tokens["azure"][llm_params["model"]]
             except KeyError:
                 raise ValueError("Model not supported")
             return AzureOpenAI(llm_params)
 
         elif "gemini" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["gemini"][llm_params["model"]]
             except KeyError:
                 raise ValueError("Model not supported")
             return Gemini(llm_params)
 
         elif "ollama" in llm_params["model"]:
-            """ 
-            Avaiable models:
-            - llama2
-            - mistral
-            - codellama
-            - dolphin-mixtral
-            - mistral-openorca
-            """
             llm_params["model"] = llm_params["model"].split("/")[-1]
 
             # allow user to set model_tokens in config
             if "model_tokens" in llm_params:
                 self.model_token = llm_params["model_tokens"]
             elif llm_params["model"] in models_tokens["ollama"]:
-                self.model_token = models_tokens["ollama"][llm_params["model"]]
-            else:
-                 raise ValueError("Model not supported")
+                try:
+                    self.model_token = models_tokens["ollama"][llm_params["model"]]
+                except KeyError:
+                    raise ValueError("Model not supported")
 
             return Ollama(llm_params)
-
+        elif "hugging_face" in llm_params["model"]:
+            try:
+                self.model_token = models_tokens["hugging_face"][llm_params["model"]]
+            except KeyError:
+                raise ValueError("Model not supported")
+            return HuggingFace(llm_params)
         else:
-            raise ValueError("Model not supported")
+            raise ValueError(
+                "Model provided by the configuration not supported")
 
+    def get_execution_info(self):
+        """
+        Returns the execution information of the graph.
+        """
+        return self.execution_info
+    
     @abstractmethod
     def _create_graph(self):
         """
         Abstract method to create a graph representation.
         """
         pass
```

### Comparing `scrapegraphai-0.1.4/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.1.5/scrapegraphai/graphs/search_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 from .abstract_graph import AbstractGraph
 
-
 class SearchGraph(AbstractGraph):
     """ 
     Module for searching info on the internet
     """
 
     def _create_graph(self):
         """
@@ -67,10 +66,10 @@
         )
 
     def run(self) -> str:
         """
         Executes the web scraping and searching process.
         """
         inputs = {"user_prompt": self.prompt}
-        final_state = self.graph.execute(inputs)
+        self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.1.4/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.1.5/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     FetchNode,
     ParseNode,
     RAGNode,
     GenerateAnswerNode
 )
 from .abstract_graph import AbstractGraph
 
-
 class SmartScraperGraph(AbstractGraph):
     """
     SmartScraper is a comprehensive web scraping tool that automates the process of extracting
     information from web pages using a natural language model to interpret and answer prompts.
     """
 
     def __init__(self, prompt: str, source: str, config: dict):
@@ -37,15 +36,18 @@
             input="doc",
             output=["parsed_doc"],
             node_config={"chunk_size": self.model_token}
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
-            node_config={"llm": self.llm_model},
+            node_config={
+                "llm": self.llm_model,
+                "embedder_model": self.embedder_model
+            }
         )
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={"llm": self.llm_model},
         )
 
@@ -64,11 +66,11 @@
             entry_point=fetch_node
         )
 
     def run(self) -> str:
         """
         Executes the web scraping process and returns the answer to the prompt.
         """
-        inputs = {"user_prompt": self.prompt, self.input_key: self.source}
-        final_state = self.graph.execute(inputs)
+        inputs = {"user_prompt": self.prompt, self.input_key: self.source}  
+        self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        return final_state.get("answer", "No answer found.")
+        return self.final_state.get("answer", "No answer found.")
```

### Comparing `scrapegraphai-0.1.4/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.1.5/scrapegraphai/graphs/speech_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,15 +40,18 @@
             input="doc",
             output=["parsed_doc"],
             node_config={"chunk_size": self.model_token}
         )
         rag_node = RAGNode(
             input="user_prompt & (parsed_doc | doc)",
             output=["relevant_chunks"],
-            node_config={"llm": self.llm_model},
+            node_config={
+                "llm": self.llm_model,
+                "embedder_model": self.embedder_model
+            }
         )
         generate_answer_node = GenerateAnswerNode(
             input="user_prompt & (relevant_chunks | parsed_doc | doc)",
             output=["answer"],
             node_config={"llm": self.llm_model},
         )
         text_to_speech_node = TextToSpeechNode(
@@ -76,17 +79,17 @@
         )
 
     def run(self) -> str:
         """
         Executes the web scraping, summarization, and text-to-speech process.
         """
         inputs = {"user_prompt": self.prompt, self.input_key: self.source}
-        final_state = self.graph.execute(inputs)
+        self.final_state, self.execution_info = self.graph.execute(inputs)
 
-        audio = final_state.get("audio", None)
+        audio = self.final_state.get("audio", None)
         if not audio:
             raise ValueError("No audio generated from the text.")
         save_audio_from_bytes(audio, self.config.get(
             "output_path", "output.mp3"))
         print(f"Audio saved to {self.config.get('output_path', 'output.mp3')}")
 
-        return final_state
+        return self.final_state
```

### Comparing `scrapegraphai-0.1.4/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.1.5/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.1.5/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.1.5/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.1.5/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/models/gemini.py` & `scrapegraphai-0.1.5/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/models/ollama.py` & `scrapegraphai-0.1.5/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/models/openai.py` & `scrapegraphai-0.1.5/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.1.5/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.1.5/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/rag_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 """
 
 from typing import List
 from langchain.docstore.document import Document
 from langchain.retrievers import ContextualCompressionRetriever
 from langchain.retrievers.document_compressors import EmbeddingsFilter, DocumentCompressorPipeline
 from langchain_community.document_transformers import EmbeddingsRedundantFilter
+from langchain_community.embeddings import HuggingFaceHubEmbeddings
 from langchain_community.vectorstores import FAISS
 from langchain_openai import OpenAIEmbeddings, AzureOpenAIEmbeddings
-from ..models import OpenAI, Ollama, AzureOpenAI
+from ..models import OpenAI, Ollama, AzureOpenAI, HuggingFace
 from langchain_community.embeddings import OllamaEmbeddings
 from .base_node import BaseNode
 
 
 class RAGNode(BaseNode):
     """
     A node responsible for compressing the input tokens and storing the document
@@ -22,43 +23,43 @@
     It allows scraping of big documents without exceeding the token limit of the language model.
 
     Attributes:
         node_name (str): The unique identifier name for the node, defaulting to "ParseHTMLNode".
         node_type (str): The type of the node, set to "node" indicating a standard operational node.
 
     Args:
-        node_name (str, optional): The unique identifier name for the node. 
+        node_name (str, optional): The unique identifier name for the node.
         Defaults to "ParseHTMLNode".
 
     Methods:
-        execute(state): Parses the HTML document contained within the state using 
+        execute(state): Parses the HTML document contained within the state using
         the specified tags, if provided, and updates the state with the parsed content.
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict, node_name: str = "RAG"):
         """
         Initializes the ParseHTMLNode with a node name.
         """
         super().__init__(node_name, "node", input, output, 2, node_config)
         self.llm_model = node_config["llm"]
         self.embedder_model = node_config.get("embedder_model", None)
 
     def execute(self, state):
         """
-        Executes the node's logic to implement RAG (Retrieval-Augmented Generation) 
+        Executes the node's logic to implement RAG (Retrieval-Augmented Generation)
         The method updates the state with relevant chunks of the document.
 
         Args:
             state (dict): The state containing the 'document' key with the HTML content
 
         Returns:
             dict: The updated state containing the 'relevant_chunks' key with the relevant chunks.
 
         Raises:
-            KeyError: If 'document' is not found in the state, indicating that the necessary 
+            KeyError: If 'document' is not found in the state, indicating that the necessary
                       information for parsing is missing.
         """
 
         print(f"--- Executing {self.node_name} Node ---")
 
         # Interpret input keys based on the provided input expression
         input_keys = self.get_input_keys(state)
@@ -88,14 +89,16 @@
         if isinstance(embedding_model, OpenAI):
             embeddings = OpenAIEmbeddings(
                 api_key=embedding_model.openai_api_key)
         elif isinstance(embedding_model, AzureOpenAI):
             embeddings = AzureOpenAIEmbeddings()
         elif isinstance(embedding_model, Ollama):
             embeddings = OllamaEmbeddings(model=embedding_model.model)
+        elif isinstance(embedding_model, HuggingFace):
+            embeddings = HuggingFaceHubEmbeddings(model=embedding_model.model)
         else:
             raise ValueError("Embedding Model missing or not supported")
 
         retriever = FAISS.from_documents(
             chunked_docs, embeddings).as_retriever()
 
         redundant_filter = EmbeddingsRedundantFilter(embeddings=embeddings)
```

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/search_internet_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 from typing import List
 from langchain.output_parsers import CommaSeparatedListOutputParser
 from langchain.prompts import PromptTemplate
 from ..utils.research_web import search_on_web
 from .base_node import BaseNode
 
-
 class SearchInternetNode(BaseNode):
     """
     A node that generates an answer by querying a language model (LLM) based on the user's input
     and the content extracted from a webpage. It constructs a prompt from the user's input
     and the scraped content, feeds it to the LLM, and parses the LLM's response to produce
     an answer.
```

### Comparing `scrapegraphai-0.1.4/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.1.5/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.1.5/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.1.5/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.1.5/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/utils/remover.py` & `scrapegraphai-0.1.5/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.1.5/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.1.5/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.1.5/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.1.4/PKG-INFO` & `scrapegraphai-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.1.4
+Version: 0.1.5
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >3.9,<4.0
```

