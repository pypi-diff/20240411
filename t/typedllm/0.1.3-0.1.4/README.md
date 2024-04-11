# Comparing `tmp/typedllm-0.1.3.tar.gz` & `tmp/typedllm-0.1.4.tar.gz`

## Comparing `typedllm-0.1.3.tar` & `typedllm-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.3/HISTORY.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 typedllm-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 typedllm-0.1.3/tests/test_client.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.1.3/tests/test_interop.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 typedllm-0.1.3/tests/test_langchain.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedllm-0.1.3/tests/test_tool.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.1.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.1.3/LICENSE
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.1.3/README.md
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 typedllm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 typedllm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.4/HISTORY.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/test_client.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/test_interop.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 typedllm-0.1.4/tests/test_tool.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 typedllm-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 typedllm-0.1.4/LICENSE
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 typedllm-0.1.4/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 typedllm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 typedllm-0.1.4/PKG-INFO
```

### Comparing `typedllm-0.1.3/tests/conftest.py` & `typedllm-0.1.4/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pytest
 
-from typedllm import LLMModel, TypedPrompt, LLMSession, LLMRequest
+from typedllm import LLMModel, TypedPrompt, LLMSession, LLMRequest, Tool
 from typedtemplate import JinjaTemplateEngine
 from pydantic import Field
 
 
 @pytest.fixture(name="openai_key")
 def get_openai_key() -> str:
     return os.getenv("OPENAI_API_KEY")
@@ -54,7 +54,16 @@
         verbose=True,
     )
 
 
 @pytest.fixture(name="llmrequest")
 def get_request():
     return LLMRequest(force_text_response=True)
+
+
+@pytest.fixture(name="llmtool")
+def get_tool():
+    class CityFoundingTool(Tool):
+        """A tool to collect a city and its founding year."""
+        city_name: str = Field(description="The name of the city")
+        founded_year: int = Field(description="The year a city was founded")
+    return CityFoundingTool
```

### Comparing `typedllm-0.1.3/tests/test_client.py` & `typedllm-0.1.4/tests/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from typing import Type
+
 import pytest
 
 from pydantic import BaseModel, Field
 
 from typedllm import (
     LLMModel,
     LLMSession,
     LLMRequest,
     LLMUserMessage,
     llm_request,
     async_llm_request,
-    create_tool_from_function
+    create_tool_from_function,
+    Tool
 )
 
 
 @pytest.mark.asyncio
 async def test_basic_request(openai_key: str):
     model = LLMModel(
         name="gpt-4-0125-preview",
@@ -40,40 +43,41 @@
 
 def get_city_founding_history(city: FoundingYear) -> str:
     return (f"Historical weather for {city.city} since its founding in {city.year}. "
             f"The weather is very nice. Average 80 degrees F.")
 
 
 def test_make_tool_from_function():
-    tool = create_tool_from_function(get_city_founding_history)
-    assert tool.name == "get_city_founding_history"
-    assert tool.parameter_type == FoundingYear
+    Tool = create_tool_from_function(get_city_founding_history)
+    assert Tool.__name__ == "get_city_founding_history"
+    assert "city" in Tool.model_fields
+    assert Tool.model_fields["city"].annotation == FoundingYear
 
 
 @pytest.mark.asyncio
 async def test_basic_tools_request(openai_key: str):
     model = LLMModel(
         name="gpt-4",
         api_key=openai_key,
     )
-    tool = create_tool_from_function(get_city_founding_history)
+    tool: Type[Tool] = create_tool_from_function(get_city_founding_history)
     session = LLMSession(
         model=model,
         tools=[tool]
     )
     request = LLMRequest(
         message=LLMUserMessage(
             content="What is the founding story of New York City?",
         ),
         required_tool=tool,
     )
     session, response = await async_llm_request(session, request)
     assert session
     assert response
-    assert response.tool_calls[0].tool.name == "get_city_founding_history"
-    assert response.tool_calls[0].arguments.city.index("New York") > -1
-    assert response.tool_calls[0].arguments.year == 1624
+    assert response.tool_calls[0].tool.__class__.__name__ == "get_city_founding_history"
+    assert response.tool_calls[0].tool.city.city.index("New York") > -1
+    assert response.tool_calls[0].tool.city.year == 1624
 
 
 @pytest.mark.asyncio
 async def test_basic_lvm_request(openai_key: str):
     pass
```

### Comparing `typedllm-0.1.3/tests/test_interop.py` & `typedllm-0.1.4/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.3/.gitignore` & `typedllm-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.3/LICENSE` & `typedllm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `typedllm-0.1.3/pyproject.toml` & `typedllm-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 [project]
 name = "typedllm"
 description = "A Pydantic LLM Interface that sparks Joy"
 authors = [
     {name = "Todd Cullen", email = "todd@100-x.ai"},
 ]
 dependencies = [
-    "pydantic>=2.6.3",
+    "pydantic>=2.1.0",
     "httpx>=0.27.0",
     "litellm>=1.34.25",
-    "typedtemplate>=0.1.6",
+    "typedtemplate>=0.1.6"
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {text = "MIT"}
 dynamic = ["version"]
 
-[project.optional-dependencies]
-langchain = [
-    "langchain-core>=0.1.33",
-    "typedtemplate>=0.1.5",
-]
-
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 path = 'src/typedllm/version.py'
 
@@ -42,12 +36,11 @@
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.0.2",
     "pytest-asyncio>=0.23.5.post1",
-    "langchain-core>=0.1.33",
 ]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
```

