# Comparing `tmp/text_tagging_model-0.1.1.tar.gz` & `tmp/text_tagging_model-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_tagging_model-0.1.1.tar", max compression
+gzip compressed data, was "text_tagging_model-0.1.2a0.tar", max compression
```

## Comparing `text_tagging_model-0.1.1.tar` & `text_tagging_model-0.1.2a0.tar`

### file list

```diff
@@ -1,16 +1,30 @@
--rw-r--r--   0        0        0       41 2024-04-05 18:27:57.393842 text_tagging_model-0.1.1/README.md
--rw-r--r--   0        0        0     1471 2024-04-10 13:19:34.984053 text_tagging_model-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 13:02:16.948922 text_tagging_model-0.1.1/text_tagging_model/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-10 13:02:16.949132 text_tagging_model-0.1.1/text_tagging_model/logger_config.py
--rw-r--r--   0        0        0        0 2024-04-10 13:02:16.949177 text_tagging_model-0.1.1/text_tagging_model/models/__init__.py
--rw-r--r--   0        0        0     1230 2024-04-10 13:02:16.949377 text_tagging_model-0.1.1/text_tagging_model/models/metrics.py
--rw-r--r--   0        0        0        0 2024-04-10 13:02:16.949423 text_tagging_model-0.1.1/text_tagging_model/models/rake_extractor/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-10 13:02:16.949625 text_tagging_model-0.1.1/text_tagging_model/models/rake_extractor/keyphrases_extractor.py
--rw-r--r--   0        0        0     3475 2024-04-10 13:02:16.949782 text_tagging_model-0.1.1/text_tagging_model/models/rake_extractor/keyword_extractor.py
--rw-r--r--   0        0        0      216 2024-04-10 13:02:16.949937 text_tagging_model-0.1.1/text_tagging_model/processing/__init__.py
--rw-r--r--   0        0        0      125 2024-04-10 13:02:16.950076 text_tagging_model-0.1.1/text_tagging_model/processing/analyzer/__init__.py
--rw-r--r--   0        0        0     2305 2024-04-10 13:02:16.950214 text_tagging_model-0.1.1/text_tagging_model/processing/analyzer/word_vector_ranker.py
--rw-r--r--   0        0        0      109 2024-04-10 13:02:16.950344 text_tagging_model-0.1.1/text_tagging_model/processing/normalizers/__init__.py
--rw-r--r--   0        0        0     1456 2024-04-10 13:02:16.950497 text_tagging_model-0.1.1/text_tagging_model/processing/normalizers/text_normalizer.py
--rw-r--r--   0        0        0       58 2024-04-10 13:02:16.950631 text_tagging_model-0.1.1/text_tagging_model/processing/utils.py
--rw-r--r--   0        0        0      926 1970-01-01 00:00:00.000000 text_tagging_model-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-05 18:27:57.393842 text_tagging_model-0.1.2a0/README.md
+-rw-r--r--   0        0        0     1540 2024-04-10 22:37:17.705733 text_tagging_model-0.1.2a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 13:26:29.785403 text_tagging_model-0.1.2a0/text_tagging_model/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-10 17:38:45.908803 text_tagging_model-0.1.2a0/text_tagging_model/logger_config.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:59:49.958211 text_tagging_model-0.1.2a0/text_tagging_model/models/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-10 21:18:16.240769 text_tagging_model-0.1.2a0/text_tagging_model/models/bart_based_model/__init__.py
+-rw-r--r--   0        0        0     3665 2024-04-10 22:32:28.676356 text_tagging_model-0.1.2a0/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
+-rw-r--r--   0        0        0     1230 2024-04-10 13:26:29.785889 text_tagging_model-0.1.2a0/text_tagging_model/models/metrics.py
+-rw-r--r--   0        0        0       84 2024-04-10 19:51:48.269012 text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-10 17:03:50.201269 text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
+-rw-r--r--   0        0        0     3741 2024-04-10 21:13:41.651750 text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/tags_extractor.py
+-rw-r--r--   0        0        0      216 2024-04-10 15:00:17.918296 text_tagging_model-0.1.2a0/text_tagging_model/processing/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:49:15.254929 text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-10 20:39:51.551412 text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/base_embedder.py
+-rw-r--r--   0        0        0      509 2024-04-10 20:00:44.503406 text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/fasttext_embedder.py
+-rw-r--r--   0        0        0      674 2024-04-10 22:32:28.678868 text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/hg_embedder.py
+-rw-r--r--   0        0        0      365 2024-04-10 17:07:38.801435 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-10 16:36:32.623920 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/base_normalizer.py
+-rw-r--r--   0        0        0      996 2024-04-10 20:00:44.506705 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/nouns_keeper.py
+-rw-r--r--   0        0        0      624 2024-04-10 20:06:17.954874 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/pipe.py
+-rw-r--r--   0        0        0      456 2024-04-10 20:00:44.508075 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/punctuation_deleter.py
+-rw-r--r--   0        0        0      746 2024-04-10 20:00:44.508861 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/stopwords_deleter.py
+-rw-r--r--   0        0        0     1456 2024-04-10 13:26:29.787845 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/text_normalizer.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:47:50.375775 text_tagging_model-0.1.2a0/text_tagging_model/processing/ranker/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-10 20:39:31.891187 text_tagging_model-0.1.2a0/text_tagging_model/processing/ranker/base_ranker.py
+-rw-r--r--   0        0        0      746 2024-04-10 20:09:31.231012 text_tagging_model-0.1.2a0/text_tagging_model/processing/ranker/max_distance_ranker.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:50:54.437113 text_tagging_model-0.1.2a0/text_tagging_model/processing/summarizator/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-10 22:33:37.704033 text_tagging_model-0.1.2a0/text_tagging_model/processing/summarizator/bart_summarization.py
+-rw-r--r--   0        0        0       58 2024-04-10 13:26:29.787998 text_tagging_model-0.1.2a0/text_tagging_model/processing/utils.py
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 text_tagging_model-0.1.2a0/PKG-INFO
```

### Comparing `text_tagging_model-0.1.1/pyproject.toml` & `text_tagging_model-0.1.2a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 [tool.poetry]
 name = "text-tagging-model"
-version = "0.1.1"
+version = "0.1.2a0"
 description = "Here we collected some online and offline models for text tagging."
 authors = [
     "Pavel Kochkin <kochkin27@gmail.com>",
     "Shamil Nurkaev <nurkaievs1204@gmail.com>",
     "Denis <denison03@mail.ru>",
     "Stephan Olizko <stepa.olizko@yandex.ru>"
 ]
 readme = "README.md"
 packages = [{include = "text_tagging_model"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rouge = "^1.0.1"
-numpy = "^1.26.4"
+numpy = "~1.25.2"
 scikit-learn = "^1.4.1.post1"
 pymorphy2 = "^0.9.1"
 nltk = "^3.8.1"
 rake-nltk = "^1.0.6"
 coloredlogs = "^15.0.1"
-pandas = "^2.2.1"
+pandas = "^2.0.3"
 tqdm = "^4.66.2"
 fasttext-wheel = "^0.9.2"
+transformers = "^4.39.3"
+sentencepiece = "^0.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
 flake8 = "^6.0.0"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
 ipykernel = "^6.29.4"
 isort = "^5.13.2"
 pre-commit = "^3.7.0"
 black = "^24.3.0"
 coverage = "^7.4.4"
+torch = "^2.2.2"
 
 
 [tool.pytest.ini_options]
 pythonpath = [
   ".", "text_tagging_model",
 ]
 testpaths = ["./tests/"]
```

### Comparing `text_tagging_model-0.1.1/text_tagging_model/logger_config.py` & `text_tagging_model-0.1.2a0/text_tagging_model/logger_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,9 +36,9 @@
 
         # Add handler to logger
         local_logger.addHandler(handler)
 
         return local_logger
 
 
-logger = LoggerFactory().get_logger(level=logging.WARNING)
+logger = LoggerFactory().get_logger(level=logging.INFO)
 # sys.modules["logger"] = logger
```

### Comparing `text_tagging_model-0.1.1/text_tagging_model/models/metrics.py` & `text_tagging_model-0.1.2a0/text_tagging_model/models/metrics.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.1/text_tagging_model/models/rake_extractor/keyphrases_extractor.py` & `text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/keyphrases_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.1/text_tagging_model/models/rake_extractor/keyword_extractor.py` & `text_tagging_model-0.1.2a0/text_tagging_model/models/bart_based_model/tag_sum_extractor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from collections import Counter
 from typing import List
 
 import numpy as np
 from tqdm import tqdm
 
-from text_tagging_model.logger_config import logger
-from text_tagging_model.models.rake_extractor.keyphrases_extractor import RakeKeyphrasesExtractor
-from text_tagging_model.processing.analyzer.word_vector_ranker import WordVectorRanker
-from text_tagging_model.processing.normalizers.text_normalizer import TextNormalizer
+from text_tagging_model.processing.embedder.hg_embedder import HGEmbedder
+from text_tagging_model.processing.normalizers import NounsKeeper, PunctDeleter, StopwordsDeleter
+from text_tagging_model.processing.normalizers.pipe import NormalizersPipe
+from text_tagging_model.processing.ranker.max_distance_ranker import MaxDistanceRanker
+from text_tagging_model.processing.summarizator.bart_summarization import MBartSummarizator
 
 
-class KeywordExtractor:
+class TagSumExtractor:
     """
     The class is used to extract keywords from the text.
 
     Attributes
     ----------
     language : str
         language that will be used. available: 'russian', 'english'
@@ -23,26 +25,40 @@
 
     Methods
     -------
     extract(text, top_n, min_keyword_cnt, distance_metric)
         Returns list with extracted keywords
     """
 
-    def __init__(self, language: str = "russian", model_name: str = "cc.ru.300.bin"):
-        self.language = language
-        self.extractor = RakeKeyphrasesExtractor(language=language)
-        self.normalizer = TextNormalizer(language=language)
-        self.ranker = WordVectorRanker(language=language, model_name=model_name)
+    def __init__(
+        self,
+        summarizator_model: str = "IlyaGusev/mbart_ru_sum_gazeta",
+        embedder_model: str = "cointegrated/rubert-tiny2",
+        language: str = "russian",
+        min_cnt_keyword: int = 2,
+        device: str = "cpu",
+    ) -> None:
+        self.summarizator = MBartSummarizator(summarizator_model, device=device)
+        self.normalizer = NormalizersPipe(
+            [
+                PunctDeleter(),
+                StopwordsDeleter(language),
+                NounsKeeper(language),
+            ],
+            final_split=True,
+        )
+
+        embedder = HGEmbedder(embedder_model)
+        self.ranker = MaxDistanceRanker(embedder)
+        self.min_cnt_keyword = min_cnt_keyword
 
     def extract_for_corpus(
         self,
         texts: List[str],
         top_n: int,
-        min_keyword_cnt: int,
-        distance_metric: str = "cosine",
     ) -> np.ndarray:
         """Returns extracted keywords for corpus of texts
 
         Args:
             texts (List[str]): list with texts
             top_n (int): number of words to extract
             min_keyword_cnt (int): min number of words in the extracted phrases
@@ -52,25 +68,23 @@
 
         Returns:
             np.ndarray: array with arrays extracted keywords
         """
         extracted_keywords = list()
 
         for text in tqdm(texts):
-            keywords = self.extract(text, top_n, min_keyword_cnt, distance_metric)
+            keywords = self.extract(text, top_n)
             extracted_keywords.append(keywords)
 
         return extracted_keywords
 
     def extract(
         self,
         text: str,
         top_n: int,
-        min_keyword_cnt: int,
-        distance_metric: str = "cosine",
     ) -> np.ndarray:
         """Returns extracted keywords from the text
 
         Args:
             text (str): text to extract
             top_n (int): number of words to extract
             min_keyword_cnt (int): min number of words in the extracted phrases
@@ -78,22 +92,20 @@
             available ['cityblock', 'cosine', 'euclidean', 'l1', 'l2', 'manhattan'].
             Defaults to "cosine".
 
         Returns:
             np.ndarray: array with extracted keywords
         """
 
-        logger.info("Keywords extraction...")
-        keyphrases_with_scores = self.extractor.extract(text)
-        keyphrases = [text for _, text in keyphrases_with_scores]
-
-        logger.info("Keywords normalization and filtering by count...")
-        normalized_words = self.normalizer.normalize(keyphrases)
-
+        keyphrase = self.summarizator.get_summary(text.lower())
+        normalized_keyphrase = list(map(self.normalizer.normalize, keyphrase))
         most_co_occurring_words = np.array(
-            [word for word, cnt in normalized_words.most_common(top_n) if cnt >= min_keyword_cnt]
+            [
+                word
+                for word, cnt in Counter(normalized_keyphrase).most_common(top_n)
+                if cnt >= self.min_cnt_keyword
+            ]
         )
 
-        logger.info("Keywords analysing to get tags...")
-        keywords = self.ranker.get_top_n_keywords(most_co_occurring_words, top_n, distance_metric)
+        keywords = self.ranker.get_top_n_keywords(most_co_occurring_words, top_n)
 
         return keywords
```

### Comparing `text_tagging_model-0.1.1/text_tagging_model/processing/normalizers/text_normalizer.py` & `text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.1/PKG-INFO` & `text_tagging_model-0.1.2a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: text-tagging-model
-Version: 0.1.1
+Version: 0.1.2a0
 Summary: Here we collected some online and offline models for text tagging.
 Author: Pavel Kochkin
 Author-email: kochkin27@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: fasttext-wheel (>=0.9.2,<0.10.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: numpy (>=1.25.2,<1.26.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pymorphy2 (>=0.9.1,<0.10.0)
 Requires-Dist: rake-nltk (>=1.0.6,<2.0.0)
 Requires-Dist: rouge (>=1.0.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
+Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: transformers (>=4.39.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # text-tagging-model
 Text tagging model.
```

