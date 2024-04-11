# Comparing `tmp/basicbedrock-0.1.0.tar.gz` & `tmp/basicbedrock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.1.0.tar", last modified: Tue Apr  9 15:23:28 2024, max compression
+gzip compressed data, was "basicbedrock-0.1.1.tar", last modified: Thu Apr 11 00:28:17 2024, max compression
```

## Comparing `basicbedrock-0.1.0.tar` & `basicbedrock-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.613340 basicbedrock-0.1.0/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.0/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     2899 2024-04-09 15:23:28.613119 basicbedrock-0.1.0/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)     1002 2024-04-09 15:09:01.000000 basicbedrock-0.1.0/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-09 15:21:30.000000 basicbedrock-0.1.0/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-09 15:23:28.613391 basicbedrock-0.1.0/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.605822 basicbedrock-0.1.0/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.607010 basicbedrock-0.1.0/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-09 15:11:23.000000 basicbedrock-0.1.0/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    13220 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/basicbedrock.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.611953 basicbedrock-0.1.0/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     2782 2024-04-09 15:10:38.000000 basicbedrock-0.1.0/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4880 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     6477 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4804 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4379 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3020 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2589 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.612845 basicbedrock-0.1.0/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     2899 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      554 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-09 15:23:28.000000 basicbedrock-0.1.0/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-09 15:23:28.612316 basicbedrock-0.1.0/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3684 2024-04-08 15:52:46.000000 basicbedrock-0.1.0/test/tests.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.242970 basicbedrock-0.1.1/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.1/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-11 00:28:17.242720 basicbedrock-0.1.1/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-11 00:28:17.243025 basicbedrock-0.1.1/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.238760 basicbedrock-0.1.1/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.239658 basicbedrock-0.1.1/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    15825 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/basicbedrock.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.241812 basicbedrock-0.1.1/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3008 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3659 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/ai21.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     6036 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     7095 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4710 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3221 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2864 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.242404 basicbedrock-0.1.1/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-11 00:28:17.000000 basicbedrock-0.1.1/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-11 00:28:17.241953 basicbedrock-0.1.1/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 00:27:04.000000 basicbedrock-0.1.1/test/tests.py
```

### Comparing `basicbedrock-0.1.0/LICENSE` & `basicbedrock-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.0/pyproject.toml` & `basicbedrock-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basicbedrock"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
     { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock/basicbedrock.py` & `basicbedrock-0.1.1/src/basicbedrock/basicbedrock.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,18 +31,24 @@
             warnings.warn('No session provided, attemtping to use "default" profile', category=RuntimeWarning)
             session = boto3.session.Session(profile_name='default')
         self.client = session.client("bedrock-runtime")
         self._default_k = 100
         self._default_p = .5
         self._default_t = .5
         self._default_n = 150
-        self._k = kwargs.get('top_k', self._default_k)
-        self._p = kwargs.get('top_p', self._default_p)
-        self._t = kwargs.get('temp', self._default_t)
-        self._n = kwargs.get('max_tokens', self._default_n)
+        self._default_stop = []
+        # intialize params to default values
+        self._k = self._default_k
+        self._p = self._default_p
+        self._t = self._default_t
+        self._n = self._default_n
+        self._s = self._default_stop
+        # set params according to kwargs
+        if kwargs:
+            self.set_params(kwargs)
 
     def print_available_models(self) -> None:
         """
         Prints all available models line by line
         :return: None
         """
         print(os.linesep.join(self.get_available_models()))
@@ -110,14 +116,34 @@
             model = model_request_mapping.get(model_id)
             _inst = model()
             j = _inst.json()
             if indent:
                 j = json.dumps(json.loads(j), indent=indent)
         print(j)
 
+    def get_boto3_body(self, model_id: str, prompt: str) -> str:
+        """
+        given a model_id and a prompt, this will construct the boto3 'body' parameter using the specified prompt and params,
+        but it will not invoke bedrock or pass it to boto3, it will simply return the boto3 'body' param as a string.
+        Internally, this calls the update_prompt() function, not update_prompt_raw(), which means that it will take into account
+        the expected calling convention of the underlying model by inserting things such as 'Human:' or '<s>[INST]' as appropriate
+        :param model_id: the model to construct a boto3 body for
+        :param prompt: the prompt to pass the model.
+        :return: a string, representing the equivalent boto3 'body' parameter.
+        """
+        if model_id not in self.get_available_models():
+            raise ValueError(f"requested model {model_id} is not an available model")
+        if not isinstance(prompt, str):
+            raise ValueError(f"prompt must be a string, but got {type(prompt)}")
+        schema = model_request_mapping.get(model_id)
+        schema_inst: BaseAbstractRequest = schema()
+        schema_inst.set_prompt(prompt)
+        j = schema_inst.json()
+        return j
+
     def invoke(self, model_id: str, request: typing.Union[str, dict],
                show_request: bool = False) -> BaseAbstractResponse:
         """
         invokes a model_id and returns the response.  Non-streaming only.
         request may by one of: a prompt, a json string represent the request schema, or a dict representing the request schema
         invoking with a request of a string containing valid json data, if it is not a valid json schema for the model
         it will be interpreted as a prompt string and a runtime warning will be raised
@@ -156,15 +182,15 @@
                         category=Warning
                     )
                     sys.stderr.flush()
             except json.decoder.JSONDecodeError:  # its not marshalled json, its a string
                 pass
         if schema_inst is None:
             schema_inst = schema_obj()
-            schema_inst.update_prompt(request)
+            schema_inst.set_prompt(request)
         schema_inst.set_params(self.params)
         body = schema_inst.json()
         full_request = {
             "modelId": model_id,
             "body": body
         }
         if show_request:
@@ -206,50 +232,60 @@
         returns the params dictionary
         :return: params dict in format of {'top_p': float, 'top_k': int, 'temp': float, 'max_tokens': int}
         """
         return {
             "top_p": self._p,
             "top_k": self._k,
             "temp": self._t,
-            "max_tokens": self._n
+            "max_tokens": self._n,
+            "stop_words": self._s
         }
 
     @params.setter
     def params(self, params: dict):
         """
         applys a provided params dict to internal params
         :param params:
         :return:
         """
         if not isinstance(params, dict):
             raise ValueError(f"params must be a dict, not a {type(params)}")
         if "top_p" not in params and \
                 "top_k" not in params and \
                 "max_tokens" not in params and \
-                "temp" not in params:
-            raise ValueError(f"params must contain top_p, top_k, max_tokens or temp")
+                "temp" not in params and \
+                "stop_words" not in params:
+            raise ValueError(f"params must contain top_p, top_k, max_tokens, temp or stop_tokens")
         if "top_p" in params:
-            self.top_p = params["top_p"]
+            top_p = params.get("top_p")
+            self.top_p = top_p
         if "top_k" in params:
-            self.top_k = params["top_k"]
+            top_k = params.get("top_k")
+            self.top_k = top_k
         if "temp" in params:
-            self.temp = params["temp"]
+            temp = params.get("temp")
+            self.temp = temp
         if "max_tokens" in params:
-            self.max_tokens = params["max_tokens"]
+            max_tokens = params.get("max_tokens")
+            self.max_tokens = max_tokens
+        if "stop_words" in params:
+            stop_tokens = params.get("stop_words")
+            self._s = stop_tokens
 
     @params.deleter
     def params(self):
         """
         resets all params to default values
         :return:
         """
         self._p = self._default_p
         self._k = self._default_k
         self._t = self._default_t
         self._n = self._default_n
+        self._s = self._default_stop
 
     @property
     def top_p(self) -> float:
         """
         returns the top_p parameter
         :return:
         """
@@ -356,7 +392,38 @@
     @max_tokens.deleter
     def max_tokens(self):
         """
         resets the max_tokens parameter
         :return:
         """
         self._n = self._default_n
+
+    @property
+    def stop_words(self) -> list:
+        """
+        returns the max_tokens parameter
+        :return:
+        """
+
+        return self._s
+
+    @stop_words.setter
+    def stop_words(self, stop_words: List[str]):
+        """
+        sets the max_tokens parameter
+        :param n_tokens:
+        :return:
+        """
+        if not isinstance(stop_words, list):
+            raise ValueError(f"stop_tokens must be a list, not a {type(stop_words)}")
+        for i, item in enumerate(stop_words):
+            if not isinstance(item, str):
+                raise ValueError(f"stop_tokens must be a list of strings, but element {i} is a {type(item)}")
+        self._s = stop_words
+
+    @stop_words.deleter
+    def stop_words(self):
+        """
+        resets the max_tokens parameter
+        :return:
+        """
+        self._s = self._default_stop
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock/models/__init__.py` & `basicbedrock-0.1.1/src/basicbedrock/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 This package contains all models used in basicbedrock.  It models and abstracts all the response/request schemas used by bedrock.
 """
 import os
 import sys
 
 sys.path.append(os.path.dirname(os.path.realpath(__file__)))
+from .ai21 import *
 from .amazon import *
 from .anthropic import *
 from .baseclasses import BaseAbstractRequest
 from .cohere import *
 from .meta import *
 from .mistral import *
 
 model_request_mapping = {
+    "ai21.j2-ultra-v1": AI21Jurassic2UltraV1Request,
+    "ai21.j2-mid-v1": AI21Jurassic2MidV1Request,
     "amazon.titan-embed-text-v1": AmazonTitanEmbedTextV1Request,
     "amazon.titan-text-lite-v1": AmazonTitanTextLiteV1Request,
     "amazon.titan-text-express-v1": AmazonTitanTextExpressV1Request,
     "anthropic.claude-instant-v1": AnthropicClaudeInstantV1Request,
     "anthropic.claude-v2": AnthropicClaudeV2Request,
     "anthropic.claude-v2:1": AnthropicClaudeV2_1Request,
     "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3Sonnet20240229V1_0Request,
@@ -29,14 +32,16 @@
     "meta.llama2-70b-chat-v1": MetaLlama270bChatV1Request,
     "mistral.mistral-7b-instruct-v0:2": MistralMistral7bInstructV0_2Request,
     "mistral.mixtral-8x7b-instruct-v0:1": MistralMistral8x7bInstructV0_1Request,
     "mistral.mistral-large-2402-v1:0": MistralMistralLarge2402V1_0Request
 }
 
 model_response_mapping = {
+    "ai21.j2-ultra-v1": AI21Jurassic2UltraV1Response,
+    "ai21.j2-mid-v1": AI21Jurassic2MidV1Response,
     "amazon.titan-embed-text-v1": AmazonTitanEmbedTextV1Response,
     "amazon.titan-text-lite-v1": AmazonTitanTextLiteV1Response,
     "amazon.titan-text-express-v1": AmazonTitanTextExpressV1Response,
     "anthropic.claude-instant-v1": AnthropicClaudeInstantV1Response,
     "anthropic.claude-v2": AnthropicClaudeV2Response,
     "anthropic.claude-v2:1": AnthropicClaudeV2_1Response,
     "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3Sonnet20240229V1_0Response,
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock/models/amazon.py` & `basicbedrock-0.1.1/src/basicbedrock/models/amazon.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,37 +10,59 @@
 
 class AmazonTitanTextGenerationConfig(BaseModel):
     """
     Stub class for the configuration blob included as part of requests to Amazon Titan family models.
     the available hyperparameters are kept internally here and include P, temperate and max_tokens
     this model does not support K values.
     """
-    maxTokenCount: int = 1000
+    maxTokenCount: int = 250
     stopSequences: List[Optional[str]] = []
     temperature: float = 0.5
-    topP: float = 1.
+    topP: float = 0.5
 
 
 class AmazonTitanBaseModelRequest(BaseAbstractRequest):
     """
     All current Amazon Titan family models use the same request schema.
     This base class is used by both Amazon Titan Text G1 Express and Titan Text v1 Lite
     This model does not support top_k parameter.
     """
     inputText: str = "{PROMPT}"
     textGenerationConfig: AmazonTitanTextGenerationConfig = AmazonTitanTextGenerationConfig()
 
-    def update_prompt(self, text):
+    def set_prompt(self, text):
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
-        self.update_prompt_raw(input_text)
+        self.set_prompt_raw(input_text)
 
-    def update_prompt_raw(self, text):
+    def set_prompt_raw(self, text):
         self.inputText = text
 
+    def set_stop_words(self, stop_words: List[str]):
+        """
+        https://docs.aws.amazon.com/bedrock/latest/userguide/model-parameters-titan-text.html#model-parameters-titan-request-response
+        Only valid stop words are "|", "User:" or none at all
+        If no valid stop words are passed, the default of [] is used
+        If a valid stop word is present in the list, the first one will be used
+        :param stop_words:
+        :return:
+        """
+        if not stop_words:
+            self.textGenerationConfig.stopSequences = []
+        else:
+            # titan only accepts a single stop word.  and, it only accepts '| and 'User:' as a valid stop word
+            # I want to ensure that if a valid stop word is given, we use the first one.
+            # if no valid stop words are given, we wont use any
+            if '|' not in stop_words and 'User:' not in stop_words:
+                self.textGenerationConfig.stopSequences = []
+            for word in stop_words:
+                if word in ('|', 'User:'):
+                    self.textGenerationConfig.stopSequences = [word]
+
+
     def set_k(self, top_k: int):
         """
         Top K is not supported by Amazon Titan model family.  This method does nothing.
         :param top_k: int
         :return:
         """
         pass
@@ -116,22 +138,25 @@
 class AmazonTitanEmbedTextV1Request(BaseAbstractRequest):
     """
     Request structure for Amazon Titan Embedding V1 API
     This model accepts text and returns a list of floats, representing Amazon Titan embedding vectors.
     """
     inputText: str = "{PROMPT}"
 
-    def update_prompt(self, text):
+    def set_prompt(self, text):
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
-        self.update_prompt_raw(input_text)
+        self.set_prompt_raw(input_text)
 
-    def update_prompt_raw(self, text):
+    def set_prompt_raw(self, text):
         self.inputText = text
 
+    def set_stop_words(self, stop_words: List[str]):
+        pass
+
     def set_k(self, top_k: int):
         """
         Top K is not supported by Amazon Titan Embedding V1 API
         :param top_k:
         :return:
         """
         pass
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock/models/anthropic.py` & `basicbedrock-0.1.1/src/basicbedrock/models/anthropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 """
 File containing all of the definitions and implementations for the Anthropic family of requests and responses.
 """
+import typing
 from typing import List
 
 from pydantic import BaseModel
 
 from baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 
 class AnthropicV1V2BaseModelRequest(BaseAbstractRequest):
     """
     Claude V1 and V2 family models all utilize the same request/response format
     This handles all the logic for them
     this model supports temp, top_k, top_p, stop sequences and max_tokens
     """
     prompt: str = "\n\nHuman: {PROMPT}\n\nAssistant:"
-    max_tokens_to_sample: int = 300
+    max_tokens_to_sample: int = 250
     temperature: float = 0.5
-    top_k: int = 250
-    top_p: float = 1.
+    top_k: int = 125
+    top_p: float = 0.5
     stop_sequences: list = ["\n\nHuman:"]
     anthropic_version: str = "bedrock-2023-05-31"
 
-    def update_prompt(self, text):
+    def set_prompt(self, text):
         prompt = f"\n\nHuman: {text}\n\nAssistant:"
-        self.update_prompt_raw(prompt)
+        self.set_prompt_raw(prompt)
 
-    def update_prompt_raw(self, text):
+    def set_prompt_raw(self, text):
         self.prompt = text
 
+    def set_stop_words(self, stop_sequences: List[str]):
+        """
+        Anthropic Claude V1 and V2 seems to accept any number of stop sequences of any format
+        :param stop_sequences: the stop sequences to use
+        :return:
+        """
+        self.stop_sequences = stop_sequences
+
     def set_p(self, top_p: float):
         self.top_p = top_p
 
     def set_k(self, top_k: int):
         self.top_k = top_k
 
     def set_temp(self, temp: float):
@@ -133,21 +142,30 @@
     """
     max_tokens: int = 300
     top_p: float = 1.
     top_k: int = 25
     temperature: float = 0.5
     messages: List[AntropicClaude3Message] = [AntropicClaude3Message()]
     anthropic_version: str = "bedrock-2023-05-31"
+    stop_sequences: List[str] = []
 
-    def update_prompt(self, text):
+    def set_prompt(self, text):
         self.messages[0].update_prompt(text)
 
-    def update_prompt_raw(self, text):
+    def set_prompt_raw(self, text):
         self.messages[0].update_prompt_raw(text)
 
+    def set_stop_words(self, stop_sequences: List[str]):
+        """
+        Anthropic Claude V3 seems to accept any number of stop sequences of any format
+        :param stop_sequences: the stop sequences to use
+        :return:
+        """
+        self.stop_sequences = stop_sequences
+
     def set_p(self, top_p: float):
         self.top_p = top_p
 
     def set_k(self, top_k: int):
         self.top_k = top_k
 
     def set_temp(self, temp: float):
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock/models/baseclasses.py` & `basicbedrock-0.1.1/src/basicbedrock/models/baseclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 File containing the base classes used for all model requests and responses.
 Contains abstract base classes for the requests and responses, as well as a concrete class for hyperparameters p, k, temp and max_tokens
 """
 import abc
 import json
+import typing
 
 from pydantic import BaseModel
 
 
 class Hyperparams(BaseModel, extra="forbid"):
     """
     Hyperparameters for a model.
@@ -15,46 +16,56 @@
     Not all models support all parameters.
     Any parameters used in here which are not supported by the model are ignored at runtime
     """
     top_p: float = None
     top_k: int = None
     temp: float = None
     max_tokens: int = None
+    stop_words: typing.List[str] = []
 
 
 class BaseAbstractRequest(BaseModel, extra='forbid'):
     """
     Abstract base class for all model requests. All model requests must inherit this class.
     update_prompt and update_promp_raw differ in the fact that some models expect a certain request format to work properly,
     eg, in certain cases boto3 may reject the request if the prompt does not begin with "Human:"\
     update_prompt will format all prompts as expected by the model, whereas update_prompt_raw will input text without formatting.
     The other abstract methods all deal with setting hyperparam values P, K, temp, and max tokens.
     Additionally, two non abstract methods allow the caller to return the request as a dict or json.
     """
 
     @abc.abstractmethod
-    def update_prompt(self, text):
+    def set_prompt(self, text: str):
         """
         Updates the prompt while maintaining its expected internal prompt structure
         Example, if the prompt must begin with 'Human:' this will be maintained
         :param text: the prompt you want to use
         :return:
         """
         raise NotImplementedError("Abstract method update_prompt not implemented")
 
     @abc.abstractmethod
-    def update_prompt_raw(self, text):
+    def set_prompt_raw(self, text: str):
         """
         Updates the prompt without regards to any expected prompt structure.
         this is used for very precisely modifying prompts.
         :param text: the exact prompt you want to use
         :return:
         """
         raise NotImplementedError("Abstract method update_prompt_raw not implemented")
 
+    @abc.abstractmethod
+    def set_stop_words(self, stop_words: typing.List[str]):
+        """
+        Sets the stop words used in the model.
+        If the model does not support stop words, this is ignored
+        :param stop_words: the list of strings
+        :return:
+        """
+
     def get_dict(self):
         j = json.loads(self.json())
         return j
 
     def get_json(self, indent: int = None):
         if not indent:
             return self.json()
@@ -76,14 +87,16 @@
             self.set_temp(hparams.temp)
         if hparams.top_k is not None:
             self.set_k(hparams.top_k)
         if hparams.top_p is not None:
             self.set_p(hparams.top_p)
         if hparams.max_tokens is not None:
             self.set_max_tokens(hparams.max_tokens)
+        if hparams.stop_words is not None:
+            self.set_stop_words(hparams.stop_words)
 
     @abc.abstractmethod
     def set_p(self, top_p: float):
         raise NotImplementedError("Abstract method set_p not implemented")
 
     @abc.abstractmethod
     def set_k(self, top_k: int):
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock/models/cohere.py` & `basicbedrock-0.1.1/src/basicbedrock/models/cohere.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 File containing all of the definitions and implementations for the Cohere family of requests and responses.
 """
+import typing
 from typing import List
 
 from baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 
 class CohereCommandBaseRequest(BaseAbstractRequest):
     """
@@ -12,23 +13,32 @@
     These models support top_p, top_k, max_tokens and temperature.
     """
     prompt: str = "{PROMPT}"
     max_tokens: int = 250
     temperature: float = 0.5
     p: float = 0.5
     k: int = 125
+    stop_sequences: List[str] = []
 
-    def update_prompt(self, text):
+    def set_prompt(self, text):
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
-        self.update_prompt_raw(input_text)
+        self.set_prompt_raw(input_text)
 
-    def update_prompt_raw(self, text):
+    def set_prompt_raw(self, text):
         self.prompt = text
 
+    def set_stop_words(self, stop_words: typing.List[str]):
+        """
+        Cohere seems to accept any number of stop words
+        :param stop_words:
+        :return:
+        """
+        self.stop_sequences = stop_words
+
     def set_p(self, top_p: float):
         self.p = top_p
 
     def set_k(self, top_k: int):
         self.k = top_k
 
     def set_temp(self, temp: float):
@@ -84,23 +94,26 @@
     """
     All cohere command models use the same request format.
     Models support input text only.
     """
     texts: List[str] = ["{PROMPT}"]
     input_type: str = "search_document"
 
-    def update_prompt(self, text):
+    def set_prompt(self, text):
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
         texts = [input_text]
-        self.update_prompt_raw(texts)
+        self.set_prompt_raw(texts)
 
-    def update_prompt_raw(self, texts: list):
+    def set_prompt_raw(self, texts: list):
         self.texts = texts
 
+    def set_stop_words(self, stop_words: typing.List[str]):
+        pass
+
     def set_p(self, top_p: float):
         """
         Cohere Embed V3 does not support top_p
         :param top_p:
         :return:
         """
         pass
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock/models/meta.py` & `basicbedrock-0.1.1/src/basicbedrock/models/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 """
 File containing all of the definitions and implementations for the Meta family of requests and responses.
 Amazon docs currently do not have request schemas for Llama 2 13b and Llama 2 70b, only the chat versions
 """
+import typing
+
 from baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 
 class MetaLlama2ChatV1BaseRequest(BaseAbstractRequest):
     """
     Meta LLama 2 13b chat request format.
     This model supports max_token, temperature and top_p.
     It does not support top_k
     """
     prompt: str = "{PROMPT}"
-    max_gen_len: int = 512
+    max_gen_len: int = 250
     temperature: float = 0.5
     top_p: float = 0.5
 
-    def update_prompt(self, text):
+    def set_prompt(self, text):
         """
         Update the prompt based on the input text.
         inserts text according to expected request conventions.
         :param text:
         :return:
         """
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
-        self.update_prompt_raw(input_text)
+        self.set_prompt_raw(input_text)
 
-    def update_prompt_raw(self, text):
+    def set_prompt_raw(self, text):
         """
         Update the prompt based on the input text without regards to expected input format
         what you insert, is inserted raw without formatting
         :param text:
         :return:
         """
         self.prompt = text
 
+    def set_stop_words(self, stop_words: typing.List[str]):
+        """
+        Meta Llama 2 models dont support stop words
+        :param stop_words:
+        :return:
+        """
+        pass
+
+
     def set_p(self, top_p: float):
         """
         Set the top_p parameter.
         :param top_p:
         :return:
         """
         self.top_p = top_p
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock/models/mistral.py` & `basicbedrock-0.1.1/src/basicbedrock/models/mistral.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 """
 File containing all of the definitions and implementations for the Mistral family of requests and responses.
 """
+import typing
+
 from .baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 
 class MistralBaseRequest(BaseAbstractRequest):
     """
     Base request for Mistral family of models.
     this mnodel supports temperature, top_p, top_k and max_tokens
     """
     prompt: str = "<s>[INST] this is where you place your input text [/INST]"
     max_tokens: int = 250
     temperature: float = 0.5
     top_p: float = 0.5
     top_k: int = 125
+    stop: typing.List[str] = []
 
-    def update_prompt(self, text):
+    def set_prompt(self, text):
         input_text = "<s>[INST] {PROMPT} [/INST]"
         input_text = input_text.format(PROMPT=text)
-        self.update_prompt_raw(input_text)
+        self.set_prompt_raw(input_text)
 
-    def update_prompt_raw(self, text):
+    def set_prompt_raw(self, text):
         self.prompt = text
 
+    def set_stop_words(self, stop_words: typing.List[str]):
+        """
+        Mistral models seem to accept any number of stop words in any format
+        :param stop_words:
+        :return:
+        """
+        self.stop = stop_words
+
     def set_p(self, top_p: float):
         self.top_p = top_p
 
     def set_k(self, top_k: int):
         self.top_k = top_k
 
     def set_temp(self, temp: float):
```

### Comparing `basicbedrock-0.1.0/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.1.1/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/basicbedrock/basicbedrock.py
 src/basicbedrock.egg-info/PKG-INFO
 src/basicbedrock.egg-info/SOURCES.txt
 src/basicbedrock.egg-info/dependency_links.txt
 src/basicbedrock.egg-info/requires.txt
 src/basicbedrock.egg-info/top_level.txt
 src/basicbedrock/models/__init__.py
+src/basicbedrock/models/ai21.py
 src/basicbedrock/models/amazon.py
 src/basicbedrock/models/anthropic.py
 src/basicbedrock/models/baseclasses.py
 src/basicbedrock/models/cohere.py
 src/basicbedrock/models/meta.py
 src/basicbedrock/models/mistral.py
 test/tests.py
```

### Comparing `basicbedrock-0.1.0/test/tests.py` & `basicbedrock-0.1.1/test/tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,29 +31,29 @@
 
 def test_invoke_with_valid_json_blob(bb, verbose=False):
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with valid json blob")
         schema_inst = bb.get_model_request_object(model)
-        schema_inst.update_prompt(prompt)
+        schema_inst.set_prompt(prompt)
         blob = schema_inst.json()
         r = bb.invoke(model, blob, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
         print(f"done testing {model} in invoke with valid json blob")
 
 
 def test_invoke_with_valid_dict(bb, verbose=False):
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with valid dict")
         schema_inst = bb.get_model_request_object(model)
-        schema_inst.update_prompt(prompt)
+        schema_inst.set_prompt(prompt)
         j = schema_inst.json()
         d = json.loads(j)
         r = bb.invoke(model, d, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
         print(f"done testing {model} in invoke with valid dict")
 
@@ -68,38 +68,58 @@
         except ValueError:
             pass  # we expect this, it should fail in this case
         if verbose:
             print(f"could not call model {model} in invoke with dict {d} (Ok)")
         print(f"done testing {model} in invoke with dict")
 
 
+def test_get_boto3_body(bb,sess:boto3.session.Session, verbose=False):
+    client = sess.client("bedrock-runtime")
+    prompt = "tell me about foobar"
+    all_models = bb.get_available_models()
+    for model_id in all_models:
+        print(f"now testing {model_id} invoke boto3 invoke_model() directly using get_boto3_body")
+        body = bb.get_boto3_body(model_id, prompt)
+        full_request = {
+            "modelId": model_id,
+            "body": body
+        }
+        if verbose:
+            print(f"boto3 request: {full_request}")
+        r = client.invoke_model(**full_request)
+        assert (r['ResponseMetadata']['HTTPStatusCode'] == 200)
+        print(f"done testing {model_id} invoke boto3 invoke_model() directly using get_boto3_body")
+
+
 def single_run(bb, verbose=False):
     prompt = "tell me about foobar"
-    bb.invoke("cohere.command-text-v14", prompt)
+    bb.invoke("ai21.j2-mid-v1", prompt)
 
 
-def invoke_set_params(bb, verbose=True):
+def test_set_params(bb, verbose=True):
     params = bb.params
     params["max_tokens"] = 88
     params["top_p"] = 0.88
     params["top_k"] = 88
     params["temp"] = .88
+    params["stop_words"] = ["User:", "foobar"]
     bb.set_params(params)
     prompt = "Hittem hard with dem params doe"
     for model in bb.get_available_models():
         r = bb.invoke(model, prompt, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
 
 
 if __name__ == "__main__":
     verbose = True
     session = boto3.session.Session(profile_name='default')
     bb = BasicBedrock(session=session)
     single_run(bb, verbose)
     test_invoke_with_string(bb, verbose=verbose)
-    invoke_set_params(bb, verbose=verbose)
+    test_get_boto3_body(bb, sess=session, verbose=verbose)
+    test_set_params(bb, verbose=verbose)
     test_invoke_with_invalid_json_blob(bb, verbose=verbose)
     test_invoke_with_valid_json_blob(bb, verbose=verbose)
     test_invoke_with_valid_dict(bb, verbose=verbose)
     test_invoke_with_invalid_dict(bb, verbose=verbose)
     print("All tests successful")
```

