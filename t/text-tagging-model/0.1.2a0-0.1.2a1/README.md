# Comparing `tmp/text_tagging_model-0.1.2a0.tar.gz` & `tmp/text_tagging_model-0.1.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_tagging_model-0.1.2a0.tar", max compression
+gzip compressed data, was "text_tagging_model-0.1.2a1.tar", max compression
```

## Comparing `text_tagging_model-0.1.2a0.tar` & `text_tagging_model-0.1.2a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       41 2024-04-05 18:27:57.393842 text_tagging_model-0.1.2a0/README.md
--rw-r--r--   0        0        0     1540 2024-04-10 22:37:17.705733 text_tagging_model-0.1.2a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 13:26:29.785403 text_tagging_model-0.1.2a0/text_tagging_model/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-10 17:38:45.908803 text_tagging_model-0.1.2a0/text_tagging_model/logger_config.py
--rw-r--r--   0        0        0        0 2024-04-10 14:59:49.958211 text_tagging_model-0.1.2a0/text_tagging_model/models/__init__.py
--rw-r--r--   0        0        0       89 2024-04-10 21:18:16.240769 text_tagging_model-0.1.2a0/text_tagging_model/models/bart_based_model/__init__.py
--rw-r--r--   0        0        0     3665 2024-04-10 22:32:28.676356 text_tagging_model-0.1.2a0/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
--rw-r--r--   0        0        0     1230 2024-04-10 13:26:29.785889 text_tagging_model-0.1.2a0/text_tagging_model/models/metrics.py
--rw-r--r--   0        0        0       84 2024-04-10 19:51:48.269012 text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-10 17:03:50.201269 text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
--rw-r--r--   0        0        0     3741 2024-04-10 21:13:41.651750 text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/tags_extractor.py
--rw-r--r--   0        0        0      216 2024-04-10 15:00:17.918296 text_tagging_model-0.1.2a0/text_tagging_model/processing/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 15:49:15.254929 text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/__init__.py
--rw-r--r--   0        0        0      376 2024-04-10 20:39:51.551412 text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/base_embedder.py
--rw-r--r--   0        0        0      509 2024-04-10 20:00:44.503406 text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/fasttext_embedder.py
--rw-r--r--   0        0        0      674 2024-04-10 22:32:28.678868 text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/hg_embedder.py
--rw-r--r--   0        0        0      365 2024-04-10 17:07:38.801435 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/__init__.py
--rw-r--r--   0        0        0      166 2024-04-10 16:36:32.623920 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/base_normalizer.py
--rw-r--r--   0        0        0      996 2024-04-10 20:00:44.506705 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/nouns_keeper.py
--rw-r--r--   0        0        0      624 2024-04-10 20:06:17.954874 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/pipe.py
--rw-r--r--   0        0        0      456 2024-04-10 20:00:44.508075 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/punctuation_deleter.py
--rw-r--r--   0        0        0      746 2024-04-10 20:00:44.508861 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/stopwords_deleter.py
--rw-r--r--   0        0        0     1456 2024-04-10 13:26:29.787845 text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/text_normalizer.py
--rw-r--r--   0        0        0        0 2024-04-10 15:47:50.375775 text_tagging_model-0.1.2a0/text_tagging_model/processing/ranker/__init__.py
--rw-r--r--   0        0        0      843 2024-04-10 20:39:31.891187 text_tagging_model-0.1.2a0/text_tagging_model/processing/ranker/base_ranker.py
--rw-r--r--   0        0        0      746 2024-04-10 20:09:31.231012 text_tagging_model-0.1.2a0/text_tagging_model/processing/ranker/max_distance_ranker.py
--rw-r--r--   0        0        0        0 2024-04-10 20:50:54.437113 text_tagging_model-0.1.2a0/text_tagging_model/processing/summarizator/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-10 22:33:37.704033 text_tagging_model-0.1.2a0/text_tagging_model/processing/summarizator/bart_summarization.py
--rw-r--r--   0        0        0       58 2024-04-10 13:26:29.787998 text_tagging_model-0.1.2a0/text_tagging_model/processing/utils.py
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 text_tagging_model-0.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-05 18:27:57.393842 text_tagging_model-0.1.2a1/README.md
+-rw-r--r--   0        0        0     1540 2024-04-10 22:45:47.381118 text_tagging_model-0.1.2a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 13:26:29.785403 text_tagging_model-0.1.2a1/text_tagging_model/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-10 17:38:45.908803 text_tagging_model-0.1.2a1/text_tagging_model/logger_config.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:59:49.958211 text_tagging_model-0.1.2a1/text_tagging_model/models/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-10 21:18:16.240769 text_tagging_model-0.1.2a1/text_tagging_model/models/bart_based_model/__init__.py
+-rw-r--r--   0        0        0     3665 2024-04-10 22:32:28.676356 text_tagging_model-0.1.2a1/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
+-rw-r--r--   0        0        0     1230 2024-04-10 13:26:29.785889 text_tagging_model-0.1.2a1/text_tagging_model/models/metrics.py
+-rw-r--r--   0        0        0       84 2024-04-10 19:51:48.269012 text_tagging_model-0.1.2a1/text_tagging_model/models/rake_based_model/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-10 17:03:50.201269 text_tagging_model-0.1.2a1/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
+-rw-r--r--   0        0        0     3741 2024-04-10 21:13:41.651750 text_tagging_model-0.1.2a1/text_tagging_model/models/rake_based_model/tags_extractor.py
+-rw-r--r--   0        0        0      216 2024-04-10 15:00:17.918296 text_tagging_model-0.1.2a1/text_tagging_model/processing/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:49:15.254929 text_tagging_model-0.1.2a1/text_tagging_model/processing/embedder/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-10 20:39:51.551412 text_tagging_model-0.1.2a1/text_tagging_model/processing/embedder/base_embedder.py
+-rw-r--r--   0        0        0      509 2024-04-10 20:00:44.503406 text_tagging_model-0.1.2a1/text_tagging_model/processing/embedder/fasttext_embedder.py
+-rw-r--r--   0        0        0      674 2024-04-10 22:32:28.678868 text_tagging_model-0.1.2a1/text_tagging_model/processing/embedder/hg_embedder.py
+-rw-r--r--   0        0        0      365 2024-04-10 17:07:38.801435 text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-10 16:36:32.623920 text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/base_normalizer.py
+-rw-r--r--   0        0        0      996 2024-04-10 20:00:44.506705 text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/nouns_keeper.py
+-rw-r--r--   0        0        0      624 2024-04-10 20:06:17.954874 text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/pipe.py
+-rw-r--r--   0        0        0      456 2024-04-10 20:00:44.508075 text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/punctuation_deleter.py
+-rw-r--r--   0        0        0      746 2024-04-10 20:00:44.508861 text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/stopwords_deleter.py
+-rw-r--r--   0        0        0     1456 2024-04-10 13:26:29.787845 text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/text_normalizer.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:47:50.375775 text_tagging_model-0.1.2a1/text_tagging_model/processing/ranker/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-10 20:39:31.891187 text_tagging_model-0.1.2a1/text_tagging_model/processing/ranker/base_ranker.py
+-rw-r--r--   0        0        0      746 2024-04-10 20:09:31.231012 text_tagging_model-0.1.2a1/text_tagging_model/processing/ranker/max_distance_ranker.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:50:54.437113 text_tagging_model-0.1.2a1/text_tagging_model/processing/summarizator/__init__.py
+-rw-r--r--   0        0        0     1126 2024-04-10 22:44:50.235590 text_tagging_model-0.1.2a1/text_tagging_model/processing/summarizator/bart_summarization.py
+-rw-r--r--   0        0        0       58 2024-04-10 13:26:29.787998 text_tagging_model-0.1.2a1/text_tagging_model/processing/utils.py
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 text_tagging_model-0.1.2a1/PKG-INFO
```

### Comparing `text_tagging_model-0.1.2a0/pyproject.toml` & `text_tagging_model-0.1.2a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text-tagging-model"
-version = "0.1.2a0"
+version = "0.1.2a1"
 description = "Here we collected some online and offline models for text tagging."
 authors = [
     "Pavel Kochkin <kochkin27@gmail.com>",
     "Shamil Nurkaev <nurkaievs1204@gmail.com>",
     "Denis <denison03@mail.ru>",
     "Stephan Olizko <stepa.olizko@yandex.ru>"
 ]
```

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/logger_config.py` & `text_tagging_model-0.1.2a1/text_tagging_model/logger_config.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/models/bart_based_model/tag_sum_extractor.py` & `text_tagging_model-0.1.2a1/text_tagging_model/models/bart_based_model/tag_sum_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/models/metrics.py` & `text_tagging_model-0.1.2a1/text_tagging_model/models/metrics.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/keyphrases_extractor.py` & `text_tagging_model-0.1.2a1/text_tagging_model/models/rake_based_model/keyphrases_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/models/rake_based_model/tags_extractor.py` & `text_tagging_model-0.1.2a1/text_tagging_model/models/rake_based_model/tags_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/processing/embedder/hg_embedder.py` & `text_tagging_model-0.1.2a1/text_tagging_model/processing/embedder/hg_embedder.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/nouns_keeper.py` & `text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/nouns_keeper.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/pipe.py` & `text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/pipe.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/stopwords_deleter.py` & `text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/stopwords_deleter.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/processing/normalizers/text_normalizer.py` & `text_tagging_model-0.1.2a1/text_tagging_model/processing/normalizers/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/processing/ranker/base_ranker.py` & `text_tagging_model-0.1.2a1/text_tagging_model/processing/ranker/base_ranker.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/processing/ranker/max_distance_ranker.py` & `text_tagging_model-0.1.2a1/text_tagging_model/processing/ranker/max_distance_ranker.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a0/text_tagging_model/processing/summarizator/bart_summarization.py` & `text_tagging_model-0.1.2a1/text_tagging_model/processing/summarizator/bart_summarization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from transformers import AutoModel, AutoTokenizer
+from transformers import MBartForConditionalGeneration, MBartTokenizer
 
 
 class MBartSummarizator:
     def __init__(
         self,
         model_name: str = "IlyaGusev/mbart_ru_sum_gazeta",
         device: str = "cpu",
     ) -> None:
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name)
-        self.model = AutoModel.from_pretrained(model_name).to(device)
+        self.tokenizer = MBartTokenizer.from_pretrained(model_name)
+        self.model = MBartForConditionalGeneration.from_pretrained(model_name).to(device)
         self.device = device
 
     def get_summary(self, text: str) -> str:
         input_ids = self.tokenizer(
             [text],
             add_special_tokens=True,
             max_length=512,
```

### Comparing `text_tagging_model-0.1.2a0/PKG-INFO` & `text_tagging_model-0.1.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-tagging-model
-Version: 0.1.2a0
+Version: 0.1.2a1
 Summary: Here we collected some online and offline models for text tagging.
 Author: Pavel Kochkin
 Author-email: kochkin27@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```
