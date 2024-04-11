# Comparing `tmp/bpm_ai_inference-0.2.3.tar.gz` & `tmp/bpm_ai_inference-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_inference-0.2.3.tar", max compression
+gzip compressed data, was "bpm_ai_inference-0.2.4.tar", max compression
```

## Comparing `bpm_ai_inference-0.2.3.tar` & `bpm_ai_inference-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0    35128 2024-04-03 15:16:12.105317 bpm_ai_inference-0.2.3/LICENSE
--rw-r--r--   0        0        0       18 2024-04-03 15:16:12.105317 bpm_ai_inference-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.105317 bpm_ai_inference-0.2.3/bpm_ai_inference/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/classification/__init__.py
--rw-r--r--   0        0        0     2177 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/classification/transformers_classifier.py
--rw-r--r--   0        0        0     1396 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/daemon.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/llm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/ocr/__init__.py
--rw-r--r--   0        0        0     3213 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/pos/__init__.py
--rw-r--r--   0        0        0     1848 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/pos/spacy_pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/pix2struct_vqa.py
--rw-r--r--   0        0        0     2013 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/transformers_docvqa.py
--rw-r--r--   0        0        0     1742 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/transformers_qa.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/speech_recognition/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/speech_recognition/faster_whisper.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/token_classification/__init__.py
--rw-r--r--   0        0        0     3115 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/token_classification/transformers_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/__init__.py
--rw-r--r--   0        0        0        2 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/__init__.py
--rw-r--r--   0        0        0    18637 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
--rw-r--r--   0        0        0     2423 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/opus_mt.py
--rw-r--r--   0        0        0     1784 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/util.py
--rw-r--r--   0        0        0        0 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/util/__init__.py
--rw-r--r--   0        0        0      828 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/bpm_ai_inference/util/language.py
--rw-r--r--   0        0        0     1401 2024-04-03 15:16:12.109317 bpm_ai_inference-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/LICENSE
+-rw-r--r--   0        0        0       18 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/classification/__init__.py
+-rw-r--r--   0        0        0     2475 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/classification/transformers_classifier.py
+-rw-r--r--   0        0        0     1396 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/daemon.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/ocr/__init__.py
+-rw-r--r--   0        0        0     3213 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/pos/__init__.py
+-rw-r--r--   0        0        0     1848 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/pos/spacy_pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/question_answering/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/question_answering/pix2struct_vqa.py
+-rw-r--r--   0        0        0     2013 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/question_answering/transformers_docvqa.py
+-rw-r--r--   0        0        0     1882 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/question_answering/transformers_qa.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/speech_recognition/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/speech_recognition/faster_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/token_classification/__init__.py
+-rw-r--r--   0        0        0     1338 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/token_classification/gliner_token_classifier.py
+-rw-r--r--   0        0        0     3115 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/token_classification/transformers_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/translation/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/translation/easy_nmt/__init__.py
+-rw-r--r--   0        0        0    18637 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/translation/easy_nmt/easy_nmt.py
+-rw-r--r--   0        0        0     2423 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/translation/easy_nmt/opus_mt.py
+-rw-r--r--   0        0        0     1784 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/translation/easy_nmt/util.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/util/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/util/language.py
+-rw-r--r--   0        0        0     6718 2024-04-11 13:53:38.187802 bpm_ai_inference-0.2.4/bpm_ai_inference/util/optimum.py
+-rw-r--r--   0        0        0     1471 2024-04-11 13:53:38.191802 bpm_ai_inference-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 bpm_ai_inference-0.2.4/PKG-INFO
```

### Comparing `bpm_ai_inference-0.2.3/LICENSE` & `bpm_ai_inference-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/classification/transformers_classifier.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/classification/transformers_classifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,65 @@
-import asyncio
 import logging
 
 from bpm_ai_core.classification.zero_shot_classifier import ZeroShotClassifier, ClassificationResult
 from typing_extensions import override
 
+from bpm_ai_inference.util.optimum import get_optimized_model
+
 try:
-    from transformers import pipeline, AutoTokenizer
+    from transformers import pipeline, AutoTokenizer, AutoModelForSequenceClassification
+    from optimum.onnxruntime import ORTModelForSequenceClassification, ORTOptimizer, ORTQuantizer
+
     has_transformers = True
 except ImportError:
     has_transformers = False
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_MODEL_EN = "MoritzLaurer/deberta-v3-large-zeroshot-v1.1-all-33"
-DEFAULT_MODEL_MULTI = "MoritzLaurer/mDeBERTa-v3-base-mnli-xnli"
+DEFAULT_MODEL_EN = "MoritzLaurer/deberta-v3-large-zeroshot-v2.0"
+DEFAULT_MODEL_MULTI = "MoritzLaurer/bge-m3-zeroshot-v2.0"
 
 
 class TransformersClassifier(ZeroShotClassifier):
     """
     Local zero-shot classification model based on Huggingface transformers library.
 
-    To use, you should have the ``transformers`` python package installed.
+    To use, you should have the ``transformers`` and ``optimum`` python packages installed.
     """
 
     def __init__(self, model: str = DEFAULT_MODEL_EN):
         if not has_transformers:
-            raise ImportError('transformers is not installed')
-        self.model = model
+            raise ImportError('transformers or optimum not installed')
+
+        model, self.tokenizer = get_optimized_model(model, "zero-shot-classification")
+
+        self.zeroshot_classifier = pipeline(
+            "zero-shot-classification",
+            model=model,
+            tokenizer=self.tokenizer
+        )
 
     @override
     async def _do_classify(
             self,
             text: str,
             classes: list[str],
             hypothesis_template: str | None = None
     ) -> ClassificationResult:
-        zeroshot_classifier = pipeline("zero-shot-classification", model=self.model)
-
-        tokenizer = AutoTokenizer.from_pretrained(self.model)
-        input_tokens = len(tokenizer.encode(text))
-        max_tokens = tokenizer.model_max_length
+        input_tokens = len(self.tokenizer.encode(text))
+        max_tokens = self.tokenizer.model_max_length
         logger.debug(f"Input tokens: {input_tokens}")
         if input_tokens > max_tokens:
             logger.warning(
                 f"Input tokens exceed max model context size: {input_tokens} > {max_tokens}. Input will be truncated."
             )
 
-        prediction = zeroshot_classifier(
+        prediction = self.zeroshot_classifier(
             text,
-            classes,
+            candidate_labels=classes,
             hypothesis_template=hypothesis_template or "This example is about {}",
             multi_label=False
         )
         # Zip the labels and scores together and find the label with the max score
         labels_scores = list(zip(prediction['labels'], prediction['scores']))
         max_label, max_score = max(labels_scores, key=lambda x: x[1])
```

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/daemon.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/daemon.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/ocr/tesseract.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/pos/spacy_pos_tagger.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/pos/spacy_pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/pix2struct_vqa.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/question_answering/pix2struct_vqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/transformers_docvqa.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/question_answering/transformers_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/question_answering/transformers_qa.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/question_answering/transformers_qa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,58 @@
-import asyncio
 import logging
 
 from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.question_answering.question_answering import QuestionAnswering, QAResult
 from typing_extensions import override
 
+from bpm_ai_inference.util.optimum import get_optimized_model
+
 try:
     from transformers import pipeline, AutoTokenizer
     has_transformers = True
 except ImportError:
     has_transformers = False
 
 logger = logging.getLogger(__name__)
 
 
 class TransformersExtractiveQA(QuestionAnswering):
     """
     Local extractive question answering model based on Huggingface transformers library.
 
-    To use, you should have the ``transformers`` python package installed.
+    To use, you should have the ``transformers`` and ``optimum`` python packages installed.
     """
 
     def __init__(self, model: str = "deepset/deberta-v3-large-squad2"):
         if not has_transformers:
             raise ImportError('transformers is not installed')
-        self.model = model
+
+        model, self.tokenizer = get_optimized_model(model, "question-answering")
+
+        self.qa_model = pipeline(
+            "question-answering",
+            model=model,
+            tokenizer=self.tokenizer
+        )
 
     @override
     async def _do_answer(
             self,
             context_str_or_blob: str | Blob,
             question: str
     ) -> QAResult:
         if not isinstance(context_str_or_blob, str):
             raise Exception('TransformersExtractiveQA only supports string input')
         else:
             context = context_str_or_blob
 
-        qa_model = pipeline("question-answering", model=self.model)
-
-        tokenizer = AutoTokenizer.from_pretrained(self.model)
-        tokens = tokenizer.encode(context + question)
+        tokens = self.tokenizer.encode(context + question)
         logger.debug(f"Input tokens: {len(tokens)}")
 
-        prediction = qa_model(
+        prediction = self.qa_model(
             question=question,
             context=context
         )
         logger.debug(f"prediction: {prediction}")
 
         return QAResult(
             answer=prediction['answer'],
```

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/speech_recognition/faster_whisper.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/speech_recognition/faster_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/token_classification/transformers_token_classifier.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/token_classification/transformers_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/easy_nmt.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/translation/easy_nmt/easy_nmt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/opus_mt.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/translation/easy_nmt/opus_mt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/translation/easy_nmt/util.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/translation/easy_nmt/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/bpm_ai_inference/util/language.py` & `bpm_ai_inference-0.2.4/bpm_ai_inference/util/language.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_inference-0.2.3/pyproject.toml` & `bpm_ai_inference-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 [tool.poetry]
 name = "bpm-ai-inference"
-version = "0.2.3"
+version = "0.2.4"
 description = "Inference and server for local AI implementations of bpm-ai-core abstractions."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai-inference"
 homepage = "https://www.holisticon.de/"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
-bpm-ai-core = "2.2.0"
+python = ">=3.11,<3.12"
+bpm-ai-core = "^2.2.0"
 faster-whisper = "^0.10.0"
 lingua-language-detector = "^2.0.2"
-langcodes = { version = "^3.3.0", extras = ["data"]}
 pytesseract = "^0.3.10"
 transformers = "^4.37.2"
 sacremoses = "^0.1.1"
 sentencepiece = "^0.2.0"
 nltk = "^3.8.0"
 pyro5 = "^5.15"
+optimum = {extras = ["onnxruntime"], version = "^1.18.0"}
+gliner = "^0.1.6"
+scipy = "1.10.1"
+py-cpuinfo = "^9.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 torch = [
     { version = "=2.2.2", source="pypi", markers = "sys_platform == 'darwin'" },
     { version = "=2.2.2+cpu", source = "torch-cpu", markers = "sys_platform != 'darwin'" },
 ]
 spacy = [
     { version = "=3.7.4", markers = "sys_platform != 'darwin'" },
     { version = "=3.7.4", extras = ["apple"], markers = "sys_platform == 'darwin' and platform_machine == 'arm64'" },
 ]
 
 
-[[tool.poetry.source]]
-name = "torch-cpu"
-url = "https://download.pytorch.org/whl/cpu"
-priority = "explicit"
-
-
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.5"
 pytest-dotenv = "^0.5.2"
 
 
+[[tool.poetry.source]]
+name = "torch-cpu"
+url = "https://download.pytorch.org/whl/cpu"
+priority = "explicit"
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bpm_ai_inference-0.2.3/PKG-INFO` & `bpm_ai_inference-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: bpm-ai-inference
-Version: 0.2.3
+Version: 0.2.4
 Summary: Inference and server for local AI implementations of bpm-ai-core abstractions.
 Home-page: https://www.holisticon.de/
 License: GPL-3.0-or-later
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: bpm-ai-core (==2.2.0)
+Requires-Dist: bpm-ai-core (>=2.2.0,<3.0.0)
 Requires-Dist: faster-whisper (>=0.10.0,<0.11.0)
-Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0)
+Requires-Dist: gliner (>=0.1.6,<0.2.0)
 Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
 Requires-Dist: nltk (>=3.8.0,<4.0.0)
+Requires-Dist: optimum[onnxruntime] (>=1.18.0,<2.0.0)
+Requires-Dist: py-cpuinfo (>=9.0.0,<10.0.0)
 Requires-Dist: pyro5 (>=5.15,<6.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: sacremoses (>=0.1.1,<0.2.0)
+Requires-Dist: scipy (==1.10.1)
 Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
 Requires-Dist: transformers (>=4.37.2,<5.0.0)
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai-inference
 Description-Content-Type: text/markdown
 
 # bpm-ai-inference
```

