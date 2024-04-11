# Comparing `tmp/LiteLLMJson-0.0.5.tar.gz` & `tmp/LiteLLMJson-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiteLLMJson-0.0.5.tar", last modified: Sat Mar 23 06:52:55 2024, max compression
+gzip compressed data, was "LiteLLMJson-0.0.6.tar", last modified: Thu Apr 11 09:15:24 2024, max compression
```

## Comparing `LiteLLMJson-0.0.5.tar` & `LiteLLMJson-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 06:52:55.825424 LiteLLMJson-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-03-23 06:52:55.819427 LiteLLMJson-0.0.5/LiteLLMJson.egg-info/
--rw-rw-rw-   0        0        0     1726 2024-03-23 06:52:55.000000 LiteLLMJson-0.0.5/LiteLLMJson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-03-23 06:52:55.000000 LiteLLMJson-0.0.5/LiteLLMJson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 06:52:55.000000 LiteLLMJson-0.0.5/LiteLLMJson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-03-23 06:52:55.000000 LiteLLMJson-0.0.5/LiteLLMJson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-23 06:52:55.000000 LiteLLMJson-0.0.5/LiteLLMJson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1726 2024-03-23 06:52:55.824440 LiteLLMJson-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1235 2023-12-10 08:02:17.000000 LiteLLMJson-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 06:52:55.823456 LiteLLMJson-0.0.5/lite_llm_json/
--rw-rw-rw-   0        0        0       41 2024-03-23 06:29:14.000000 LiteLLMJson-0.0.5/lite_llm_json/__init__.py
--rw-rw-rw-   0        0        0     2730 2024-03-23 06:51:29.000000 LiteLLMJson-0.0.5/lite_llm_json/lite_llm_json.py
--rw-rw-rw-   0        0        0     4324 2024-03-23 06:44:02.000000 LiteLLMJson-0.0.5/lite_llm_json/test.py
--rw-rw-rw-   0        0        0       42 2024-03-23 06:52:55.825424 LiteLLMJson-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      830 2024-03-23 06:52:45.000000 LiteLLMJson-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:15:24.867054 LiteLLMJson-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:15:24.852083 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/
+-rw-rw-rw-   0        0        0     1726 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 09:15:24.000000 LiteLLMJson-0.0.6/LiteLLMJson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1726 2024-04-11 09:15:24.866053 LiteLLMJson-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1235 2023-12-10 08:02:17.000000 LiteLLMJson-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 09:15:24.864535 LiteLLMJson-0.0.6/lite_llm_json/
+-rw-rw-rw-   0        0        0       41 2024-03-23 06:29:14.000000 LiteLLMJson-0.0.6/lite_llm_json/__init__.py
+-rw-rw-rw-   0        0        0     2770 2024-04-11 09:14:02.000000 LiteLLMJson-0.0.6/lite_llm_json/lite_llm_json.py
+-rw-rw-rw-   0        0        0     4495 2024-04-11 09:13:19.000000 LiteLLMJson-0.0.6/lite_llm_json/test.py
+-rw-rw-rw-   0        0        0       42 2024-04-11 09:15:24.867054 LiteLLMJson-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      830 2024-04-11 09:14:30.000000 LiteLLMJson-0.0.6/setup.py
```

### Comparing `LiteLLMJson-0.0.5/LiteLLMJson.egg-info/PKG-INFO` & `LiteLLMJson-0.0.6/LiteLLMJson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiteLLMJson
-Version: 0.0.5
+Version: 0.0.6
 Summary: This library offers functionality to cleanly extract JSON from LLM responses and generate prompts for LLM that return JSON. It features a simple implementation while maintaining high versatility.
 Home-page: https://github.com/HawkClaws/lite_llm_json
 Author: HawkClaws
 License: MIT
 Project-URL: Source Code, https://github.com/HawkClaws/lite_llm_json
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `LiteLLMJson-0.0.5/PKG-INFO` & `LiteLLMJson-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiteLLMJson
-Version: 0.0.5
+Version: 0.0.6
 Summary: This library offers functionality to cleanly extract JSON from LLM responses and generate prompts for LLM that return JSON. It features a simple implementation while maintaining high versatility.
 Home-page: https://github.com/HawkClaws/lite_llm_json
 Author: HawkClaws
 License: MIT
 Project-URL: Source Code, https://github.com/HawkClaws/lite_llm_json
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `LiteLLMJson-0.0.5/README.md` & `LiteLLMJson-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `LiteLLMJson-0.0.5/lite_llm_json/lite_llm_json.py` & `LiteLLMJson-0.0.6/lite_llm_json/lite_llm_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 class LiteLLMJson:
     BASE_PROMPT = """{query_prompt}
 
 ## Response Format:
 
 Respond strictly in **JSON**. The response should adhere to the following JSON schema:
-```
+
+```JSON schema
 {json_schema}
 ```
 
 """
 
     def __init__(self, json_schema: dict) -> None:
         """
@@ -82,12 +83,13 @@
             json_pattern = r"\s*(\[.*?\]|{.*?}|\\[.*?\\]|\\{.*?\\})\s*"
             match = re.search(json_pattern, response_content, re.DOTALL)
             if match:
                 response_content = match.group(1)
             else:
                 return {}
         try:
-            data = json.loads(response_content)
+            data = json.loads(response_content, strict=False)
             return data
-        except (ValueError, TypeError):
+        except Exception as e:
+            print(e)
             return {}
```

### Comparing `LiteLLMJson-0.0.5/lite_llm_json/test.py` & `LiteLLMJson-0.0.6/lite_llm_json/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -72,22 +72,40 @@
         self.assertEqual(data, expected_data)
 
     def test_extract_data_from_invalid_json(self):
         response_content = "invalid json"
         expected_data = {}
         data = self.llm_json._extract_data_from_response(response_content)
         self.assertEqual(data, expected_data)
-    
+
     def test_extract_data_with_extra_whitespace(self):
-        response_content = "   {\"key\": \"value\"}   "
+        response_content = '   {"key": "value"}   '
         expected_data = {"key": "value"}
         data = self.llm_json._extract_data_from_response(response_content)
         self.assertEqual(data, expected_data)
 
-    def test_extract_data_with_code_block_and_extra_text(self):
-        response_content = "```json { \"sentence\": \"An ornate wooden coffin, its surface etched with ancient runes and adorned with intricate carvings, holds the remains of a fallen hero, his body preserved in a state of suspended animation by the miasma that permeates the air around it.\" } ```"
-        expected_data = {"sentence": "An ornate wooden coffin, its surface etched with ancient runes and adorned with intricate carvings, holds the remains of a fallen hero, his body preserved in a state of suspended animation by the miasma that permeates the air around it."}
+    def test_extract_data_with_simple_json(self):
+        response_content = (
+            '{"sentence": "The quick brown fox jumps over the lazy dog."}'
+        )
+        expected_data = {"sentence": "The quick brown fox jumps over the lazy dog."}
         data = self.llm_json._extract_data_from_response(response_content)
         self.assertEqual(data, expected_data)
 
+    def test_extract_data_newline_text(self):
+        response_content = """
+        {
+            "answer_impossible": false, 
+            "text": "# Introduction
+This is a simple example of a markdown-formatted text response."
+        }
+        """
+        expected_data = {
+            "answer_impossible": False,
+            "text": "# Introduction\nThis is a simple example of a markdown-formatted text response.",
+        }
+        data = self.llm_json._extract_data_from_response(response_content)
+        self.assertEqual(data, expected_data)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `LiteLLMJson-0.0.5/setup.py` & `LiteLLMJson-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fp:
     readme = fp.read()
 
 DESCRIPTION = "This library offers functionality to cleanly extract JSON from LLM responses and generate prompts for LLM that return JSON. It features a simple implementation while maintaining high versatility."
 
 setup(
     name="LiteLLMJson",
-    version="0.0.5",
+    version="0.0.6",
     author="HawkClaws",
     packages=find_packages(),
     install_requires=[
         "jsonschema>=4.19.2"
     ],
     python_requires=">=3.6",
     include_package_data=True,
```

