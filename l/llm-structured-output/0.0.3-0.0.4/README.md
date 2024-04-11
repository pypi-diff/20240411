# Comparing `tmp/llm_structured_output-0.0.3.tar.gz` & `tmp/llm_structured_output-0.0.4.tar.gz`

## Comparing `llm_structured_output-0.0.3.tar` & `llm_structured_output-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0      467 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/_/_eval.sh
--rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/_/_mistral_schema.sh
--rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/_/_server.sh
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/_/x.py
--rw-r--r--   0        0        0    17802 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/examples/llm_schema.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/examples/requirements.txt
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/examples/server.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/__init__.py
--rw-r--r--   0        0        0    24601 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/acceptor.py
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/json_acceptor.py
--rw-r--r--   0        0        0    21187 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/json_schema_acceptor.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/util/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/util/bitmap.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/util/output.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/util/tokenization.py
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/llm_structured_output/util/tokentrie.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/tests/eval.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/src/tests/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/LICENSE
--rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      467 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/_/_eval.sh
+-rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/_/_mistral_schema.sh
+-rwxr-xr-x   0        0        0      219 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/_/_server.sh
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/_/x.py
+-rw-r--r--   0        0        0    17802 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/examples/llm_schema.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/examples/requirements.txt
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/examples/server.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/__init__.py
+-rw-r--r--   0        0        0    24601 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/acceptor.py
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/json_acceptor.py
+-rw-r--r--   0        0        0    21187 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/json_schema_acceptor.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/util/__init__.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/util/bitmap.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/util/output.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/util/tokenization.py
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/llm_structured_output/util/tokentrie.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/tests/eval.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/src/tests/requirements.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/LICENSE
+-rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    14495 2020-02-02 00:00:00.000000 llm_structured_output-0.0.4/PKG-INFO
```

### Comparing `llm_structured_output-0.0.3/_/_mistral_schema.sh` & `llm_structured_output-0.0.4/_/_mistral_schema.sh`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/_/x.py` & `llm_structured_output-0.0.4/_/x.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/examples/llm_schema.py` & `llm_structured_output-0.0.4/src/examples/llm_schema.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/examples/server.py` & `llm_structured_output-0.0.4/src/examples/server.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/llm_structured_output/acceptor.py` & `llm_structured_output-0.0.4/src/llm_structured_output/acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/llm_structured_output/json_acceptor.py` & `llm_structured_output-0.0.4/src/llm_structured_output/json_acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/llm_structured_output/json_schema_acceptor.py` & `llm_structured_output-0.0.4/src/llm_structured_output/json_schema_acceptor.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/llm_structured_output/util/bitmap.py` & `llm_structured_output-0.0.4/src/llm_structured_output/util/bitmap.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/llm_structured_output/util/output.py` & `llm_structured_output-0.0.4/src/llm_structured_output/util/output.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/llm_structured_output/util/tokenization.py` & `llm_structured_output-0.0.4/src/llm_structured_output/util/tokenization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Tokenizer utils.
 """
 
-from typing import Iterable, Union
+from typing import Union
 
 SPIECE_UNDERLINE = "▁"
 
 
 class HuggingfaceTokenizerHelper:
     """
     Helper to use Huggingface tokenizers effectively.
@@ -40,15 +40,15 @@
         """
         fragment = self.tokenizer.decode(tokens)
         if self.token_has_space_prefix[tokens[0]]:
             return f" {fragment}"
         else:
             return fragment
 
-    def extract_vocabulary(self) -> tuple[Iterable[tuple[int, str]], int]:
+    def extract_vocabulary(self) -> tuple[list[tuple[int, str]], int]:
         """
         Extract the vocabulary and eos_token_id from a Huggingface PreTrainedTokenizer.
         """
         return (
-            ((i, self.no_strip_decode([i])) for _, i in self.tokenizer.vocab.items()),
+            [(i, self.no_strip_decode([i])) for _, i in self.tokenizer.vocab.items()],
             self.tokenizer.eos_token_id,
         )
```

### Comparing `llm_structured_output-0.0.3/src/llm_structured_output/util/tokentrie.py` & `llm_structured_output-0.0.4/src/llm_structured_output/util/tokentrie.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/src/tests/eval.py` & `llm_structured_output-0.0.4/src/tests/eval.py`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/LICENSE` & `llm_structured_output-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/README.md` & `llm_structured_output-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `llm_structured_output-0.0.3/pyproject.toml` & `llm_structured_output-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llm_structured_output"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Oscar D.P. Triscon", email="github@triscon.com" },
 ]
 description = "Constrain LLM generation to structured output, such as function calling a.k.a. tool use"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `llm_structured_output-0.0.3/PKG-INFO` & `llm_structured_output-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: llm_structured_output
-Version: 0.0.3
+Version: 0.0.4
 Summary: Constrain LLM generation to structured output, such as function calling a.k.a. tool use
 Project-URL: Homepage, https://github.com/otriscon/llm-structured-output
 Project-URL: Issues, https://github.com/otriscon/llm-structured-output/issues
 Author-email: "Oscar D.P. Triscon" <github@triscon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

