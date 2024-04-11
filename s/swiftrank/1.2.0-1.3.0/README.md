# Comparing `tmp/swiftrank-1.2.0.tar.gz` & `tmp/swiftrank-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftrank-1.2.0.tar", max compression
+gzip compressed data, was "swiftrank-1.3.0.tar", max compression
```

## Comparing `swiftrank-1.2.0.tar` & `swiftrank-1.3.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0    11556 2024-03-19 11:38:33.490689 swiftrank-1.2.0/LICENSE
--rw-r--r--   0        0        0      708 2024-03-19 19:18:38.667427 swiftrank-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    24905 2024-03-19 19:37:32.921018 swiftrank-1.2.0/readme.md
--rw-r--r--   0        0        0       77 2024-03-19 11:38:33.492690 swiftrank-1.2.0/swiftrank/__init__.py
--rw-r--r--   0        0        0     3766 2024-03-19 19:33:27.645029 swiftrank-1.2.0/swiftrank/cli/__init__.py
--rw-r--r--   0        0        0     1967 2024-01-22 18:26:22.022055 swiftrank-1.2.0/swiftrank/cli/utils.py
--rw-r--r--   0        0        0     7745 2024-03-19 19:34:39.368538 swiftrank-1.2.0/swiftrank/ranker.py
--rw-r--r--   0        0        0     1712 2024-03-19 19:07:47.416396 swiftrank-1.2.0/swiftrank/settings.py
--rw-r--r--   0        0        0    25595 1970-01-01 00:00:00.000000 swiftrank-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11556 2024-03-19 11:38:33.490689 swiftrank-1.3.0/LICENSE
+-rw-r--r--   0        0        0      868 2024-04-11 17:05:54.313904 swiftrank-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    25776 2024-04-11 17:03:14.641654 swiftrank-1.3.0/readme.md
+-rw-r--r--   0        0        0       77 2024-04-10 10:49:05.804973 swiftrank-1.3.0/swiftrank/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 10:49:35.101477 swiftrank-1.3.0/swiftrank/interface/__init__.py
+-rw-r--r--   0        0        0     4160 2024-04-11 17:36:01.893072 swiftrank-1.3.0/swiftrank/interface/api.py
+-rw-r--r--   0        0        0     4316 2024-04-11 12:55:57.952263 swiftrank-1.3.0/swiftrank/interface/cli.py
+-rw-r--r--   0        0        0     2484 2024-04-11 08:06:09.354512 swiftrank-1.3.0/swiftrank/interface/utils.py
+-rw-r--r--   0        0        0     7962 2024-04-11 17:38:50.849728 swiftrank-1.3.0/swiftrank/ranker.py
+-rw-r--r--   0        0        0     1712 2024-03-19 19:07:47.416396 swiftrank-1.3.0/swiftrank/settings.py
+-rw-r--r--   0        0        0    26530 1970-01-01 00:00:00.000000 swiftrank-1.3.0/PKG-INFO
```

### Comparing `swiftrank-1.2.0/LICENSE` & `swiftrank-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftrank-1.2.0/pyproject.toml` & `swiftrank-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "swiftrank"
-version = "1.2.0"
+version = "1.3.0"
 description = "Compact, ultra-fast SoTA reranker enhancing retrieval pipelines and terminal applications."
 authors = ["Harsh Verma <synacktra.work@gmail.com>"]
 license = "Apache Software License (Apache 2.0)"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
@@ -13,15 +13,22 @@
 numpy = ">=1.24.4"
 requests = "2.31.0"
 rich = "13.7.0"
 tqdm = "4.66.1"
 cyclopts = "2.1.2"
 pyyaml = "6.0.1"
 orjson = "3.9.10"
+pydantic = "2.6.4"
+fastapi = "0.110.1"
+uvicorn = "0.29.0"
 
 [tool.poetry.scripts]
-swiftrank = "swiftrank.cli:app.meta"
-srank = "swiftrank.cli:app.meta"
+swiftrank = "swiftrank.interface.cli:app.meta"
+srank = "swiftrank.interface.cli:app.meta"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "8.1.1"
+requests = "2.31.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `swiftrank-1.2.0/readme.md` & `swiftrank-1.3.0/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-> Important: Previously It was using [PrithivirajDamodaran](https://github.com/PrithivirajDamodaran) hosted models(I had no idea that the models were being downloaded was stored on paid cloud and now he is very upset about it). Swiftrank will use models from [Huggingface](https://huggingface.co/prithivida/flashrank) in new update. Thanks for understanding.
+> Swiftrank is now using flashrank int8 models from [Huggingface repository](https://huggingface.co/prithivida/flashrank)
 
 <div align="center">
   <img src="https://i.imgur.com/MYThQ5c.gif" alt="SwiftRank GIF">
 </div>
 
 ---
 
@@ -36,14 +36,17 @@
 - Implements a structured pipeline for the reranking process. `Ranker` and `Tokenizer` instances are passed to create the pipeline.
 - Supports complex dictionary/class objects handling.
 - Includes a customizable threshold parameter to filter contexts, ensuring only those with a value equal to or exceeding the threshold are selected.
 
 ⌨️ **Terminal Integration**:
 - Pipe your output into `swiftrank` cli tool and get reranked output
 
+🌐 **API Integration**:
+- Deploy `swiftrank` as an API service for seamless integration into your workflow.
+
 ---
 
 ### 🚀 Installation 
 
 ```sh
 pip install swiftrank
 ```
@@ -53,14 +56,15 @@
 ```
 Usage: swiftrank COMMAND
 
 Rerank contexts provided on stdin.
 
 ╭─ Commands ─────────────────────────────────────────────────────╮
 │ process    STDIN processor. [ json | jsonl | yaml ]            │
+│ serve      Startup a swiftrank server                          │
 │ --help,-h  Display this message and exit.                      │
 │ --version  Display application version.                        │
 ╰────────────────────────────────────────────────────────────────╯
 ╭─ Parameters ───────────────────────────────────────────────────╮
 │ *  --query      -q  query for reranking evaluation. [required] │
 │    --threshold  -t  filter contexts using threshold.           │
 │    --first      -f  get most relevant context.                 │
@@ -176,14 +180,35 @@
   ```sh
   cat files/contextlines.yaml | swiftrank -q "Monogatari Series: Season 2" process -c '.name' -f  
   ```
   ```
   Monogatari Series: Second Season
   ```
 
+#### Startup a FastAPI server instance
+
+```
+Usage: swiftrank serve [OPTIONS]
+
+Startup a swiftrank server
+
+╭─ Parameters ──────────────────────────────╮
+│ --host  Host name [default: 0.0.0.0]      │
+│ --port  Port number. [default: 12345]     │
+╰───────────────────────────────────────────╯
+```
+
+```sh
+swiftrank serve
+```
+```
+[GET] /models - List Models
+[POST] /rerank - Rerank Endpoint
+```
+
 ### Library Usage 🤗
 
 - Build a `ReRankPipeline` instance
   - From `Ranker` and `Tokenizer` instance
     ```py
     from swiftrank import Ranker, Tokenizer, ReRankPipeline
 
@@ -233,18 +258,18 @@
   (0.47455463, 'vLLM is a fast and easy-to-use library for LLM inference and serving. vLLM is fast with: State-of-the-art serving throughput Efficient management of attention key and value memory with PagedAttention Continuous batching of incoming requests Optimized CUDA kernels')
   (0.43783104, 'LLM inference efficiency will be one of the most crucial topics for both industry and academia, simply because the more efficient you are, the more $$$ you will save. vllm project is a must-read for this direction, and now they have just released the paper')
   (0.043041725, 'Ever want to make your LLM inference go brrrrr but got stuck at implementing speculative decoding and finding the suitable draft model? No more pain! Thrilled to unveil Medusa, a simple framework that removes the annoying draft model while getting 2x speedup.')
   ```
 
 - Want to filter contexts? Utilize `threshold` parameter.
   ```py
-  for mapping in reranker.invoke(
+  for ctx in reranker.invoke(
       query="Tricks to accelerate LLM inference", contexts=contexts, threshold=0.8
   ):
-      print(mapping)
+      print(ctx)
   ```
   ```
   Introduce *lookahead decoding*: - a parallel decoding algo to accelerate LLM inference - w/o the need for a draft model or a data store - linearly decreases # decoding steps relative to log(FLOPs) used per decoding step.
   There are many ways to increase LLM inference throughput (tokens/second) and decrease memory footprint, sometimes at the same time. Here are a few methods I’ve found effective when working with Llama 2. These methods are all well-integrated with Hugging Face. This list is far from exhaustive; some of these techniques can be used in combination with each other and there are plenty of others to try. - Bettertransformer (Optimum Library): Simply call `model.to_bettertransformer()` on your Hugging Face model for a modest improvement in tokens per second.  - Fp4 Mixed-Precision (Bitsandbytes): Requires minimal configuration and dramatically reduces the model's memory footprint.  - AutoGPTQ: Time-consuming but leads to a much smaller model and faster inference. The quantization is a one-time cost that pays off in the long run.
   ```
 
 - Have dictionary or class instance as contexts? Utilize `key` parameter.
@@ -293,8 +318,22 @@
     page_content='LLM inference efficiency will be one of the most crucial topics for both industry and academia, simply because the more efficient you are, the more $$$ you will save. vllm project is a must-read for this direction, and now they have just released the paper'
     page_content='Ever want to make your LLM inference go brrrrr but got stuck at implementing speculative decoding and finding the suitable draft model? No more pain! Thrilled to unveil Medusa, a simple framework that removes the annoying draft model while getting 2x speedup.'
     ```
 ---
 
 #### Acknowledgment of Original Repository
 
-This project is derived from [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank), which is licensed under the Apache License 2.0. We extend our gratitude to the original authors and contributors for their work. The original repository provided a foundational framework for the development of our project, and we have built upon it with additional features and improvements.
+This project is derived from [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank), which is licensed under the Apache License 2.0. We extend our gratitude to the original authors and contributors for their work. The original repository provided a foundational framework for the development of our project, and we have built upon it with additional features and improvements.
+
+#### Citation
+
+```bibtex
+@software{Damodaran_FlashRank_Lightest_and_2023,
+author = {Damodaran, Prithiviraj},
+doi = {10.5281/zenodo.10426927},
+month = dec,
+title = {{FlashRank, Lightest and Fastest 2nd Stage Reranker for search pipelines.}},
+url = {https://github.com/PrithivirajDamodaran/FlashRank},
+version = {1.0.0},
+year = {2023}
+}
+```
```

### Comparing `swiftrank-1.2.0/swiftrank/cli/__init__.py` & `swiftrank-1.3.0/swiftrank/interface/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Annotated
 
-from cyclopts import App, Parameter
+from cyclopts import App, Parameter, validators
 
 try:
 	from signal import signal, SIGPIPE, SIG_DFL
 	signal(SIGPIPE, SIG_DFL)
 except ImportError:
 	pass
 
@@ -19,87 +19,103 @@
         help="schema for pre-processing input.", show_default=False)] = '.',
     ctx: Annotated[str, Parameter(name=('-c', '--ctx'),
         help="schema for extracting context.", show_default=False)] = '.',
     post: Annotated[str, Parameter(name=('-p', '--post'),
         help="schema for extracting field after reranking.", show_default=False
     )] = None
 ):  
-    from .utils import object_parser, print_and_exit
+    from .utils import cli_object_parser, print_and_exit
     def preprocessor(_input: str):
         if _input.startswith(('{', '[')):
             from orjson import loads, JSONDecodeError
             try:
-                return object_parser(loads(_input), pre)
+                return cli_object_parser(loads(_input), pre)
             except JSONDecodeError:
-                from io import StringIO
-                with StringIO(_input) as handler:
-                    return list(map(loads, handler))
+                try:
+                    from io import StringIO
+                    with StringIO(_input) as handler:
+                        return list(map(loads, handler))
+                except (JSONDecodeError, Exception):
+                    print_and_exit("Input data format not valid.", code=1)
             except Exception:
-                print_and_exit("Malformed JSON object not parseable.", code=1)
+                print_and_exit("Input data format not valid.", code=1)
         
         import yaml    
         try:
-            return object_parser(yaml.safe_load(_input), pre)
+            return cli_object_parser(yaml.safe_load(_input), pre)
         except yaml.MarkedYAMLError:
             return list(yaml.safe_load_all(_input))
         except yaml.YAMLError:
             print_and_exit("Input data format not valid.", code=1)
     
     return {'preprocessor': preprocessor, 'ctx_schema': ctx, 'post_schema': post}
 
 
 @app.meta.default
 def __entry__(
     *tokens: Annotated[str, Parameter(show=False, allow_leading_hyphen=True)], 
     query: Annotated[str, Parameter(
         name=("-q", "--query"), help="query for reranking evaluation.")],
     threshold: Annotated[float, Parameter(
-        name=("-t", "--threshold"), help="filter contexts using threshold.")] = None,
+        name=("-t", "--threshold"), help="filter contexts using threshold.", validator=validators.Number(gte=0.0, lte=1.0))] = None,
     first: Annotated[bool, Parameter(
         name=("-f", "--first"), help="get most relevant context.", negative="", show_default=False)] = False,
 ):
-    from .utils import read_stdin, object_parser, print_and_exit
+    from .utils import read_stdin, cli_object_parser, print_and_exit
     
     processing_params: dict = {}
     if tokens:
         processing_params = app(tokens=tokens)
         _input = read_stdin()
         if not _input:
             return
         contexts = processing_params['preprocessor'](_input)
-            
     else:
         contexts = read_stdin(readlines=True)
 
     ctx_schema = processing_params.get('ctx_schema', '.')
+    post_schema = processing_params.get('post_schema') or ctx_schema
+
     if not isinstance(contexts, list):
-        print_and_exit(object_parser(contexts, ctx_schema))
+        print_and_exit(cli_object_parser(contexts, post_schema))
 
-    if not all(contexts):
-        print_and_exit("No contexts found on stdin", code=1)
-    if len(contexts) == 1:
-        print_and_exit(contexts[0])
+    if not contexts:
+        print_and_exit("Nothing to rerank!", code=1)
 
     from .. import settings
     from ..ranker import ReRankPipeline
 
     pipeline = ReRankPipeline.from_model_id(settings.DEFAULT_MODEL)
     try:
         reranked = pipeline.invoke(
             query=query, 
             contexts=contexts, 
             threshold=threshold, 
-            key=lambda x: object_parser(x, ctx_schema)
+            key=lambda x: cli_object_parser(x, ctx_schema)
         )
+
+        if reranked and first:
+            print_and_exit(
+                cli_object_parser(reranked[0], post_schema)
+            )
+            
+        for context in reranked:
+            print(cli_object_parser(context, post_schema))
+
     except TypeError:
         print_and_exit(
-            'Context processing must result into string. Hint: `--ctx` flag might help.', code=1
+            'Context processing must result into string.', code=1
         )
 
-    post_schema = processing_params.get('post_schema') or ctx_schema
-    if reranked and first:
-        print_and_exit(
-            object_parser(reranked[0], post_schema)
-        )
-        
-    for context in reranked:
-        print(object_parser(context, post_schema))
+@app.meta.command(name="serve", help="Startup a swiftrank server")
+def serve(
+    *, 
+    host: Annotated[str, Parameter(
+        name=('--host'), help="Host name")] = '0.0.0.0',
+    port: Annotated[int, Parameter(
+        name=('--port',), help="Port number.")] = 12345
+):
+    from .api import _serve
+    _serve(host=host, port=port)
+
+if __name__ == "__main__":
+    app.meta()
```

### Comparing `swiftrank-1.2.0/swiftrank/ranker.py` & `swiftrank-1.3.0/swiftrank/ranker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from pathlib import Path
 from collections import OrderedDict
 from typing import (
-    overload, Any, Optional, Iterable, Callable, TypeVar
+    overload, cast, Any, Optional, Iterable, Callable, TypeVar
 )
 
 import numpy as np
 import onnxruntime as ort
 from tokenizers import AddedToken, Tokenizer as TokenizerLoader
 
 from . import settings
@@ -62,17 +62,17 @@
 
     def __load(self):
         """Load tokenizer"""
         config = self.__file_handler("config.json")
         tokenizer_config = self.__file_handler("tokenizer_config.json")
         tokens_map = self.__file_handler("special_tokens_map.json")
 
-        tokenizer: TokenizerLoader = TokenizerLoader.from_file(str(
+        tokenizer = cast(TokenizerLoader, TokenizerLoader.from_file(str(
             self.__file_handler("tokenizer.json", read_json=False)
-        ))
+        )))
         tokenizer.enable_truncation(max_length=min(tokenizer_config["model_max_length"], self.max_length))
         tokenizer.enable_padding(pad_id=config["pad_token_id"], pad_token=tokenizer_config["pad_token"])
 
         for token in tokens_map.values():
             if isinstance(token, str):
                 tokenizer.add_special_tokens([token])
             elif isinstance(token, dict):
@@ -84,26 +84,36 @@
 
         return tokenizer
     
     
 class ReRankPipeline:
     """
     Pipeline for reranking task.
-    :param ranker: `Ranker` class instance
-    :param tokenizer: `Tokenizer` class instance
 
-    >>> from flashrank import ReRankPipeline
-    >>> pipeline = ReRankPipeline(ranker=ranker, tokenizer=tokenizer)
-    >>> pipeline.invoke(
-    ...     query="<query>", contexts=["<context1>", "<context2>", ...]    
-    ... )
+    Example:
+    ```python
+    from swiftrank import ReRankPipeline
+    pipeline = ReRankPipeline(ranker=ranker, tokenizer=tokenizer)
+    pipeline.invoke(
+        query="<query>", contexts=["<context1>", "<context2>", ...]    
+    )
+    ```
     """
-    def __init__(self, ranker: Ranker, tokenizer: Tokenizer) -> None:
-        self.ranker = ranker.instance
-        self.tokenizer = tokenizer.instance
+    def __init__(
+        self, 
+        ranker: Optional[Ranker] = None, 
+        tokenizer: Optional[Tokenizer] = None
+    ) -> None:
+        """
+        Initialize a rerank pipeline
+        @param ranker: `Ranker` class instance
+        @param tokenizer: `Tokenizer` class instance
+        """
+        self.ranker = (ranker or Ranker()).instance
+        self.tokenizer = (tokenizer or Tokenizer()).instance
 
     @classmethod
     def from_model_id(cls, __id: str, tk_max_length: int = 512):
         """
         Create Reranker from model ID
         @param __id: Model ID
         @param tk_max_length: Max length for tokenizer
@@ -119,29 +129,29 @@
 
     @overload
     def invoke_with_score(
         self, query: str, contexts: Iterable[str], threshold: Optional[float] = None
     ) -> list[tuple[float, str]]:
         """
         Rerank contexts based on query.
-        :param query: The query to use for reranking evaluation.
-        :param contexts: The contexts to rerank.
-        :param threshold: Get contexts that are equal or higher than threshold value.
+        @param query: The query to use for reranking evaluation.
+        @param contexts: The contexts to rerank.
+        @param threshold: Get contexts that are equal or higher than threshold value.
         """
     
     @overload
     def invoke_with_score(
         self, query: str, contexts: Iterable[_T], threshold: Optional[float] = None, *, key: Callable[[_T], str]
     ) -> list[tuple[float, _T]]:
         """
         Rerank contexts based on query.
-        :param query: The query to use for reranking evaluation.
-        :param contexts: The contexts object.
-        :param threshold: Get contexts that are equal or higher than threshold value.
-        :param key: callback to use for getting fields from contexts object.
+        @param query: The query to use for reranking evaluation.
+        @param contexts: The contexts object.
+        @param threshold: Get contexts that are equal or higher than threshold value.
+        @param key: callback to use for getting fields from contexts object.
         """
 
     def invoke_with_score(
         self, 
         query: str, 
         contexts: Iterable, 
         threshold: Optional[float] = None, 
@@ -163,38 +173,38 @@
 
         output = self.ranker.run(None, onnx_input)[0]
         scores = list(1 / (1 + np.exp(
             -(output[:, 1] if output.shape[1] > 1 else output.flatten()))))
         combined = sorted(zip(scores, contexts), key=lambda x: x[0], reverse=True)
 
         if threshold is None:
-            return [(sc, ctx) for sc, ctx in combined]
-        return [(sc, ctx) for sc, ctx in combined if sc >= threshold]
+            return [(float(sc), ctx) for sc, ctx in combined]
+        return [(float(sc), ctx) for sc, ctx in combined if sc >= threshold]
 
     @overload
     def invoke(
         self, query: str, contexts: Iterable[str], threshold: Optional[float] = None
     ) -> list[str]:
         """
         Rerank contexts based on query.
-        :param query: The query to use for reranking evaluation.
-        :param contexts: The contexts to rerank.
-        :param threshold: Get contexts that are equal or higher than threshold value.
+        @param query: The query to use for reranking evaluation.
+        @param contexts: The contexts to rerank.
+        @param threshold: Get contexts that are equal or higher than threshold value.
         """
     
     @overload
     def invoke(
         self, query: str, contexts: Iterable[_T], threshold: Optional[float] = None, *, key: Callable[[_T], str]
     ) -> list[_T]:
         """
         Rerank contexts based on query.
-        :param query: The query to use for reranking evaluation.
-        :param contexts: The contexts object.
-        :param threshold: Get contexts that are equal or higher than threshold value.
-        :param key: callback to use for getting fields from contexts object.
+        @param query: The query to use for reranking evaluation.
+        @param contexts: The contexts object.
+        @param threshold: Get contexts that are equal or higher than threshold value.
+        @param key: callback to use for getting fields from contexts object.
         """
 
     def invoke(
         self, 
         query: str, 
         contexts: Iterable, 
         threshold: Optional[float] = None,
```

### Comparing `swiftrank-1.2.0/swiftrank/settings.py` & `swiftrank-1.3.0/swiftrank/settings.py`

 * *Files identical despite different names*

### Comparing `swiftrank-1.2.0/PKG-INFO` & `swiftrank-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: swiftrank
-Version: 1.2.0
+Version: 1.3.0
 Summary: Compact, ultra-fast SoTA reranker enhancing retrieval pipelines and terminal applications.
 License: Apache Software License (Apache 2.0)
 Author: Harsh Verma
 Author-email: synacktra.work@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cyclopts (==2.1.2)
+Requires-Dist: fastapi (==0.110.1)
 Requires-Dist: numpy (>=1.24.4)
 Requires-Dist: onnxruntime (==1.16.3)
 Requires-Dist: orjson (==3.9.10)
+Requires-Dist: pydantic (==2.6.4)
 Requires-Dist: pyyaml (==6.0.1)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.7.0)
 Requires-Dist: tokenizers (>=0.15.0,<0.16.0)
 Requires-Dist: tqdm (==4.66.1)
+Requires-Dist: uvicorn (==0.29.0)
 Description-Content-Type: text/markdown
 
-> Important: Previously It was using [PrithivirajDamodaran](https://github.com/PrithivirajDamodaran) hosted models(I had no idea that the models were being downloaded was stored on paid cloud and now he is very upset about it). Swiftrank will use models from [Huggingface](https://huggingface.co/prithivida/flashrank) in new update. Thanks for understanding.
+> Swiftrank is now using flashrank int8 models from [Huggingface repository](https://huggingface.co/prithivida/flashrank)
 
 <div align="center">
   <img src="https://i.imgur.com/MYThQ5c.gif" alt="SwiftRank GIF">
 </div>
 
 ---
 
@@ -62,14 +65,17 @@
 - Implements a structured pipeline for the reranking process. `Ranker` and `Tokenizer` instances are passed to create the pipeline.
 - Supports complex dictionary/class objects handling.
 - Includes a customizable threshold parameter to filter contexts, ensuring only those with a value equal to or exceeding the threshold are selected.
 
 ⌨️ **Terminal Integration**:
 - Pipe your output into `swiftrank` cli tool and get reranked output
 
+🌐 **API Integration**:
+- Deploy `swiftrank` as an API service for seamless integration into your workflow.
+
 ---
 
 ### 🚀 Installation 
 
 ```sh
 pip install swiftrank
 ```
@@ -79,14 +85,15 @@
 ```
 Usage: swiftrank COMMAND
 
 Rerank contexts provided on stdin.
 
 ╭─ Commands ─────────────────────────────────────────────────────╮
 │ process    STDIN processor. [ json | jsonl | yaml ]            │
+│ serve      Startup a swiftrank server                          │
 │ --help,-h  Display this message and exit.                      │
 │ --version  Display application version.                        │
 ╰────────────────────────────────────────────────────────────────╯
 ╭─ Parameters ───────────────────────────────────────────────────╮
 │ *  --query      -q  query for reranking evaluation. [required] │
 │    --threshold  -t  filter contexts using threshold.           │
 │    --first      -f  get most relevant context.                 │
@@ -202,14 +209,35 @@
   ```sh
   cat files/contextlines.yaml | swiftrank -q "Monogatari Series: Season 2" process -c '.name' -f  
   ```
   ```
   Monogatari Series: Second Season
   ```
 
+#### Startup a FastAPI server instance
+
+```
+Usage: swiftrank serve [OPTIONS]
+
+Startup a swiftrank server
+
+╭─ Parameters ──────────────────────────────╮
+│ --host  Host name [default: 0.0.0.0]      │
+│ --port  Port number. [default: 12345]     │
+╰───────────────────────────────────────────╯
+```
+
+```sh
+swiftrank serve
+```
+```
+[GET] /models - List Models
+[POST] /rerank - Rerank Endpoint
+```
+
 ### Library Usage 🤗
 
 - Build a `ReRankPipeline` instance
   - From `Ranker` and `Tokenizer` instance
     ```py
     from swiftrank import Ranker, Tokenizer, ReRankPipeline
 
@@ -259,18 +287,18 @@
   (0.47455463, 'vLLM is a fast and easy-to-use library for LLM inference and serving. vLLM is fast with: State-of-the-art serving throughput Efficient management of attention key and value memory with PagedAttention Continuous batching of incoming requests Optimized CUDA kernels')
   (0.43783104, 'LLM inference efficiency will be one of the most crucial topics for both industry and academia, simply because the more efficient you are, the more $$$ you will save. vllm project is a must-read for this direction, and now they have just released the paper')
   (0.043041725, 'Ever want to make your LLM inference go brrrrr but got stuck at implementing speculative decoding and finding the suitable draft model? No more pain! Thrilled to unveil Medusa, a simple framework that removes the annoying draft model while getting 2x speedup.')
   ```
 
 - Want to filter contexts? Utilize `threshold` parameter.
   ```py
-  for mapping in reranker.invoke(
+  for ctx in reranker.invoke(
       query="Tricks to accelerate LLM inference", contexts=contexts, threshold=0.8
   ):
-      print(mapping)
+      print(ctx)
   ```
   ```
   Introduce *lookahead decoding*: - a parallel decoding algo to accelerate LLM inference - w/o the need for a draft model or a data store - linearly decreases # decoding steps relative to log(FLOPs) used per decoding step.
   There are many ways to increase LLM inference throughput (tokens/second) and decrease memory footprint, sometimes at the same time. Here are a few methods I’ve found effective when working with Llama 2. These methods are all well-integrated with Hugging Face. This list is far from exhaustive; some of these techniques can be used in combination with each other and there are plenty of others to try. - Bettertransformer (Optimum Library): Simply call `model.to_bettertransformer()` on your Hugging Face model for a modest improvement in tokens per second.  - Fp4 Mixed-Precision (Bitsandbytes): Requires minimal configuration and dramatically reduces the model's memory footprint.  - AutoGPTQ: Time-consuming but leads to a much smaller model and faster inference. The quantization is a one-time cost that pays off in the long run.
   ```
 
 - Have dictionary or class instance as contexts? Utilize `key` parameter.
@@ -320,7 +348,21 @@
     page_content='Ever want to make your LLM inference go brrrrr but got stuck at implementing speculative decoding and finding the suitable draft model? No more pain! Thrilled to unveil Medusa, a simple framework that removes the annoying draft model while getting 2x speedup.'
     ```
 ---
 
 #### Acknowledgment of Original Repository
 
 This project is derived from [FlashRank](https://github.com/PrithivirajDamodaran/FlashRank), which is licensed under the Apache License 2.0. We extend our gratitude to the original authors and contributors for their work. The original repository provided a foundational framework for the development of our project, and we have built upon it with additional features and improvements.
+
+#### Citation
+
+```bibtex
+@software{Damodaran_FlashRank_Lightest_and_2023,
+author = {Damodaran, Prithiviraj},
+doi = {10.5281/zenodo.10426927},
+month = dec,
+title = {{FlashRank, Lightest and Fastest 2nd Stage Reranker for search pipelines.}},
+url = {https://github.com/PrithivirajDamodaran/FlashRank},
+version = {1.0.0},
+year = {2023}
+}
+```
```

