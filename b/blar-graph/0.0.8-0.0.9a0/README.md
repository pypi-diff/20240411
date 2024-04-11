# Comparing `tmp/blar_graph-0.0.8.tar.gz` & `tmp/blar_graph-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blar_graph-0.0.8.tar", max compression
+gzip compressed data, was "blar_graph-0.0.9a0.tar", max compression
```

## Comparing `blar_graph-0.0.8.tar` & `blar_graph-0.0.9a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2024-03-28 15:41:58.920589 blar_graph-0.0.8/LICENSE
--rw-r--r--   0        0        0     4882 2024-04-03 20:54:57.651698 blar_graph-0.0.8/README.md
--rw-r--r--   0        0        0      911 2024-04-03 20:54:57.655698 blar_graph-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-28 15:41:58.928588 blar_graph-0.0.8/src/blar_graph/__init__.py
--rw-r--r--   0        0        0     1871 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/agents_tools/agents_examples/debug.py
--rw-r--r--   0        0        0     1962 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/agents_tools/agents_examples/unit_test.py
--rw-r--r--   0        0        0      360 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/agents_tools/tools/BaseCypherModel.py
--rw-r--r--   0        0        0     1094 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/agents_tools/tools/KeywordSearchTool.py
--rw-r--r--   0        0        0      121 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/db_managers/__init__.py
--rw-r--r--   0        0        0      131 2024-03-29 13:04:27.168034 blar_graph-0.0.8/src/blar_graph/db_managers/base_manager.py
--rw-r--r--   0        0        0      523 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/db_managers/json_manager.py
--rw-r--r--   0        0        0     8041 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/db_managers/neo4j_manager.py
--rw-r--r--   0        0        0   605302 2024-04-03 20:54:57.655698 blar_graph-0.0.8/src/blar_graph/examples/Debugger.ipynb
--rw-r--r--   0        0        0   578289 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/examples/UnitTest.ipynb
--rw-r--r--   0        0        0        0 2024-03-28 15:41:58.928588 blar_graph-0.0.8/src/blar_graph/graph_construction/__init__.py
--rw-r--r--   0        0        0     6406 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/core/base_parser.py
--rw-r--r--   0        0        0    11221 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/core/graph_builder.py
--rw-r--r--   0        0        0     5987 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/languages/python/python_parser.py
--rw-r--r--   0        0        0        0 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/utils/__init__.py
--rw-r--r--   0        0        0     1783 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/utils/format_nodes.py
--rw-r--r--   0        0        0     4252 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/graph_construction/utils/tree_parser.py
--rw-r--r--   0        0        0      327 2024-04-03 20:54:57.659699 blar_graph-0.0.8/src/blar_graph/run.py
--rw-r--r--   0        0        0     6231 1970-01-01 00:00:00.000000 blar_graph-0.0.8/setup.py
--rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 blar_graph-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-28 15:41:58.920589 blar_graph-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0     4882 2024-04-03 20:54:57.651698 blar_graph-0.0.9a0/README.md
+-rw-r--r--   0        0        0      916 2024-04-04 17:43:04.263317 blar_graph-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-28 15:41:58.928588 blar_graph-0.0.9a0/src/blar_graph/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-04 17:37:35.060451 blar_graph-0.0.9a0/src/blar_graph/agents_tools/agents_examples/debug.py
+-rw-r--r--   0        0        0     1962 2024-04-04 17:37:35.060451 blar_graph-0.0.9a0/src/blar_graph/agents_tools/agents_examples/unit_test.py
+-rw-r--r--   0        0        0      360 2024-04-03 20:54:57.655698 blar_graph-0.0.9a0/src/blar_graph/agents_tools/tools/BaseCypherModel.py
+-rw-r--r--   0        0        0     1094 2024-04-03 20:54:57.655698 blar_graph-0.0.9a0/src/blar_graph/agents_tools/tools/KeywordSearchTool.py
+-rw-r--r--   0        0        0      121 2024-04-03 20:54:57.655698 blar_graph-0.0.9a0/src/blar_graph/db_managers/__init__.py
+-rw-r--r--   0        0        0      131 2024-03-29 13:04:27.168034 blar_graph-0.0.9a0/src/blar_graph/db_managers/base_manager.py
+-rw-r--r--   0        0        0      523 2024-04-03 20:54:57.655698 blar_graph-0.0.9a0/src/blar_graph/db_managers/json_manager.py
+-rw-r--r--   0        0        0     8041 2024-04-03 20:54:57.655698 blar_graph-0.0.9a0/src/blar_graph/db_managers/neo4j_manager.py
+-rw-r--r--   0        0        0   605302 2024-04-03 20:54:57.655698 blar_graph-0.0.9a0/src/blar_graph/examples/Debugger.ipynb
+-rw-r--r--   0        0        0   578289 2024-04-03 20:54:57.659699 blar_graph-0.0.9a0/src/blar_graph/examples/UnitTest.ipynb
+-rw-r--r--   0        0        0        0 2024-03-28 15:41:58.928588 blar_graph-0.0.9a0/src/blar_graph/graph_construction/__init__.py
+-rw-r--r--   0        0        0     6406 2024-04-04 17:37:35.064451 blar_graph-0.0.9a0/src/blar_graph/graph_construction/core/base_parser.py
+-rw-r--r--   0        0        0    11221 2024-04-03 20:54:57.659699 blar_graph-0.0.9a0/src/blar_graph/graph_construction/core/graph_builder.py
+-rw-r--r--   0        0        0     5987 2024-04-03 20:54:57.659699 blar_graph-0.0.9a0/src/blar_graph/graph_construction/languages/python/python_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:54:57.659699 blar_graph-0.0.9a0/src/blar_graph/graph_construction/utils/__init__.py
+-rw-r--r--   0        0        0     1783 2024-04-03 20:54:57.659699 blar_graph-0.0.9a0/src/blar_graph/graph_construction/utils/format_nodes.py
+-rw-r--r--   0        0        0     4252 2024-04-04 17:37:35.064451 blar_graph-0.0.9a0/src/blar_graph/graph_construction/utils/tree_parser.py
+-rw-r--r--   0        0        0      327 2024-04-04 17:37:35.064451 blar_graph-0.0.9a0/src/blar_graph/run.py
+-rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 blar_graph-0.0.9a0/setup.py
+-rw-r--r--   0        0        0     5865 1970-01-01 00:00:00.000000 blar_graph-0.0.9a0/PKG-INFO
```

### Comparing `blar_graph-0.0.8/LICENSE` & `blar_graph-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/README.md` & `blar_graph-0.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/pyproject.toml` & `blar_graph-0.0.9a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 line-length = 119
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "blar-graph"
-version = "0.0.8"
+version = "0.0.9-alpha"
 description = "Llm agent to search within a graph"
 authors = ["Benjamín Errazuriz <benjamin@blar.io>", "José Domínguez <jose@blar.io>"]
 readme = "README.md"
 homepage = "https://blar.io"
 repository = "https://github.com/blarApp/code-base-agent"
 license = "MIT"
 packages = [{include = "blar_graph", from = "src"}]
 exclude = [
   {path = "src/blar_graph/examples"}
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.8,<3.12"
 llama-index-packs-code-hierarchy = "^0.1.1"
 llama-index = "^0.10.20"
 python-dotenv = "^1.0.1"
 tree-sitter-languages = "^1.10.2"
 langchain = "^0.1.13"
 langchain-openai = "^0.1.1"
 neo4j = "^5.18.0"
```

### Comparing `blar_graph-0.0.8/src/blar_graph/agents_tools/agents_examples/debug.py` & `blar_graph-0.0.9a0/src/blar_graph/agents_tools/agents_examples/debug.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/agents_tools/agents_examples/unit_test.py` & `blar_graph-0.0.9a0/src/blar_graph/agents_tools/agents_examples/unit_test.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/agents_tools/tools/KeywordSearchTool.py` & `blar_graph-0.0.9a0/src/blar_graph/agents_tools/tools/KeywordSearchTool.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/db_managers/json_manager.py` & `blar_graph-0.0.9a0/src/blar_graph/db_managers/json_manager.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/db_managers/neo4j_manager.py` & `blar_graph-0.0.9a0/src/blar_graph/db_managers/neo4j_manager.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/examples/Debugger.ipynb` & `blar_graph-0.0.9a0/src/blar_graph/examples/Debugger.ipynb`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/examples/UnitTest.ipynb` & `blar_graph-0.0.9a0/src/blar_graph/examples/UnitTest.ipynb`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/graph_construction/core/base_parser.py` & `blar_graph-0.0.9a0/src/blar_graph/graph_construction/core/base_parser.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/graph_construction/core/graph_builder.py` & `blar_graph-0.0.9a0/src/blar_graph/graph_construction/core/graph_builder.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/graph_construction/languages/python/python_parser.py` & `blar_graph-0.0.9a0/src/blar_graph/graph_construction/languages/python/python_parser.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/graph_construction/utils/format_nodes.py` & `blar_graph-0.0.9a0/src/blar_graph/graph_construction/utils/format_nodes.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/src/blar_graph/graph_construction/utils/tree_parser.py` & `blar_graph-0.0.9a0/src/blar_graph/graph_construction/utils/tree_parser.py`

 * *Files identical despite different names*

### Comparing `blar_graph-0.0.8/setup.py` & `blar_graph-0.0.9a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,24 +24,24 @@
  'llama-index>=0.10.20,<0.11.0',
  'neo4j>=5.18.0,<6.0.0',
  'python-dotenv>=1.0.1,<2.0.0',
  'tree-sitter-languages>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'blar-graph',
-    'version': '0.0.8',
+    'version': '0.0.9a0',
     'description': 'Llm agent to search within a graph',
     'long_description': '# code-base-agent\n\n## Introduction\n\nThis repo introduces a method to represent a local code repository as a graph structure. The objective is to allow an LLM to traverse this graph to understand the code logic and flow. Providing the LLM with the power to debug, refactor, and optimize queries. However, several tasks are yet unexplored.\n\n## Technology Stack\n\nWe used a combination of `llama-index`, `CodeHierarchy` module, and `tree-sitter-languages` for parsing code into a graph structure, `Neo4j` for storing and querying the graph data, and `langchain` to create the agents.\n\n## Installation\n\n**Install the package:**\n\n```shell\npip install blar-graph\n```\n\nSet the env variables\n\n```.env\nNEO4J_URI=neo4j+s://YOUR_NEO4J.databases.neo4j.io\nNEO4J_USERNAME=neo4j\nNEO4J_PASSWORD=YOUR_NEO4J_PASSWORD\nOPENAI_API_KEY=YOUR_OPEN_AI_KEY\n```\n\nIf you are new to Neo4j you can deploy a free instance of neo4j with [Aura](https://login.neo4j.com/u/signup/identifier?state=hKFo2SBIWW01eGl6SEhHVTVZQ2g1VU9rSk1BZlVVblJPd2FzSqFur3VuaXZlcnNhbC1sb2dpbqN0aWTZIFNSUXR5UEtwZThoQTBlOWs0ck1hN0ZTekFOY3JfWkNho2NpZNkgV1NMczYwNDdrT2pwVVNXODNnRFo0SnlZaElrNXpZVG8). Also you can host your own version in [AWS](https://aws.amazon.com/marketplace/seller-profile?id=23ec694a-d2af-4641-b4d3-b7201ab2f5f9) or [GCP](https://console.cloud.google.com/marketplace/product/endpoints/prod.n4gcp.neo4j.io?rapt=AEjHL4O-iQH8W8STKpH0_zwz8HEyQqA9XFkpnFUkJotAt2wAT0Zmjhraww8X6covdYdzJdUi_LwtQtG8qDChLOLYHeEG4x1kZyhfzukM2WkabnwQlQpu5ws&project=direct-album-395214)\n\n### Quick start guide\n\nTo build the graph, you have to instantiate the graph manager and constructor. The graph manager handles the connection with Neo4j, and the graph constructor processes the directory input to create the graph.\n\n```python\nfrom blar_graph.graph_construction.graph_builder import GraphConstructor\nfrom blar_graph.graph_construction.neo4j_manager import Neo4jManager\n\ngraph_manager = Neo4jManager()\ngraph_constructor = GraphConstructor(graph_manager)\ngraph_constructor.build_graph("YOUR_LOCAL_DIRECTORY", "python")\ngraph_manager.close()\n```\n\nNow you can use our agent tools, or build your own, to create agents that resolves specific tasks. In the folder \'agents_tools\' you will find all our tools (for now is just the Keyword search) and examples of agent implementations. For example, for a debugger agent you could do:\n\n```python\nfrom langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder\nfrom langchain.agents.format_scratchpad.openai_tools import (\n    format_to_openai_tool_messages,\n)\nfrom langchain.agents.output_parsers.openai_tools import (\n    OpenAIToolsAgentOutputParser,\n)\nfrom blar_graph.agents_tools.tools.KeywordSearchTool import KeywordSearchTool\nfrom blar_graph.db_managers.base_manager import BaseDBManager\nfrom langchain.agents import AgentExecutor\nfrom langchain_openai import ChatOpenAI\n\nllm = ChatOpenAI(model="gpt-4-turbo-preview", temperature=0)\n\nsystem_prompt = """\n    You are a code debugger, Given a problem description and an initial function, you need to find the bug in the code.\n    You are given a graph of code functions,\n    We purposly omited some code If the code has the comment \'# Code replaced for brevity. See node_id ..... \'.\n    You can traverse the graph by calling the function keword_search.\n    Prefer calling the function keword_search with query = node_id, only call it with starting nodes or neighbours.\n    Explain why your solution solves the bug. Extensivley traverse the graph before giving an answer\n"""\n\n\nprompt = ChatPromptTemplate.from_messages(\n    [\n        (\n            "system",\n            system_prompt,\n        ),\n        ("user", "{input}"),\n        MessagesPlaceholder(variable_name="agent_scratchpad"),\n    ]\n)\n\ntools = [KeywordSearchTool(db_manager=graph_manager)]\nllm_with_tools = llm.bind_tools(tools)\n\nagent = (\n    {\n        "input": lambda x: x["input"],\n        "agent_scratchpad": lambda x: format_to_openai_tool_messages(\n            x["intermediate_steps"]\n        ),\n    }\n    | prompt\n    | llm_with_tools\n    | OpenAIToolsAgentOutputParser()\n)\n```\n\nNow you can ask yur agent to perform a debugging process.\n\n```python\nlist(\n    agent.stream(\n        {\n            "input": """\n            The directory nodes generates multiples conections,\n            it doesn\'t distinguish betweem different directories, can you fix it?\n            The initial functions is run\n            """\n        }\n    )\n)\n```\n\nYou can find more examples in the folder \'examples\'. They are comprehensive jupiter notebooks that guide you from creating the graph to deploying the agent.\n\n*Note: The supported language for now is python, we are going to include Typescript (or other language) if you ask for it enough. So don\'t hesitate to reach out through the [issues](https://github.com/blarApp/code-base-agent/issues) or directly to benjamin@blar.io or jose@blar.io*\n',
     'author': 'Benjamín Errazuriz',
     'author_email': 'benjamin@blar.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://blar.io',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<3.12',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `blar_graph-0.0.8/PKG-INFO` & `blar_graph-0.0.9a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: blar-graph
-Version: 0.0.8
+Version: 0.0.9a0
 Summary: Llm agent to search within a graph
 Home-page: https://blar.io
 License: MIT
 Author: Benjamín Errazuriz
 Author-email: benjamin@blar.io
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: langchain (>=0.1.13,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.1,<0.2.0)
 Requires-Dist: llama-index (>=0.10.20,<0.11.0)
 Requires-Dist: llama-index-packs-code-hierarchy (>=0.1.1,<0.2.0)
 Requires-Dist: neo4j (>=5.18.0,<6.0.0)
```

