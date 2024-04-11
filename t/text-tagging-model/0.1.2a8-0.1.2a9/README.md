# Comparing `tmp/text_tagging_model-0.1.2a8.tar.gz` & `tmp/text_tagging_model-0.1.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_tagging_model-0.1.2a8.tar", max compression
+gzip compressed data, was "text_tagging_model-0.1.2a9.tar", max compression
```

## Comparing `text_tagging_model-0.1.2a8.tar` & `text_tagging_model-0.1.2a9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       41 2024-04-05 18:27:57.393842 text_tagging_model-0.1.2a8/README.md
--rw-r--r--   0        0        0     1540 2024-04-11 00:09:25.689821 text_tagging_model-0.1.2a8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 13:26:29.785403 text_tagging_model-0.1.2a8/text_tagging_model/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-10 17:38:45.908803 text_tagging_model-0.1.2a8/text_tagging_model/logger_config.py
--rw-r--r--   0        0        0        0 2024-04-10 14:59:49.958211 text_tagging_model-0.1.2a8/text_tagging_model/models/__init__.py
--rw-r--r--   0        0        0       89 2024-04-10 21:18:16.240769 text_tagging_model-0.1.2a8/text_tagging_model/models/bart_based_model/__init__.py
--rw-r--r--   0        0        0     3620 2024-04-11 00:04:27.462313 text_tagging_model-0.1.2a8/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
--rw-r--r--   0        0        0     1230 2024-04-10 13:26:29.785889 text_tagging_model-0.1.2a8/text_tagging_model/models/metrics.py
--rw-r--r--   0        0        0       84 2024-04-10 19:51:48.269012 text_tagging_model-0.1.2a8/text_tagging_model/models/rake_based_model/__init__.py
--rw-r--r--   0        0        0     1526 2024-04-10 17:03:50.201269 text_tagging_model-0.1.2a8/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
--rw-r--r--   0        0        0     3745 2024-04-10 23:59:27.661434 text_tagging_model-0.1.2a8/text_tagging_model/models/rake_based_model/tags_extractor.py
--rw-r--r--   0        0        0      216 2024-04-10 15:00:17.918296 text_tagging_model-0.1.2a8/text_tagging_model/processing/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 15:49:15.254929 text_tagging_model-0.1.2a8/text_tagging_model/processing/embedder/__init__.py
--rw-r--r--   0        0        0      376 2024-04-10 20:39:51.551412 text_tagging_model-0.1.2a8/text_tagging_model/processing/embedder/base_embedder.py
--rw-r--r--   0        0        0      509 2024-04-10 20:00:44.503406 text_tagging_model-0.1.2a8/text_tagging_model/processing/embedder/fasttext_embedder.py
--rw-r--r--   0        0        0      822 2024-04-11 00:09:17.764085 text_tagging_model-0.1.2a8/text_tagging_model/processing/embedder/hg_embedder.py
--rw-r--r--   0        0        0      365 2024-04-10 17:07:38.801435 text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/__init__.py
--rw-r--r--   0        0        0      166 2024-04-10 16:36:32.623920 text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/base_normalizer.py
--rw-r--r--   0        0        0      996 2024-04-10 20:00:44.506705 text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/nouns_keeper.py
--rw-r--r--   0        0        0      624 2024-04-10 20:06:17.954874 text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/pipe.py
--rw-r--r--   0        0        0      456 2024-04-10 20:00:44.508075 text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/punctuation_deleter.py
--rw-r--r--   0        0        0      746 2024-04-10 20:00:44.508861 text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/stopwords_deleter.py
--rw-r--r--   0        0        0        0 2024-04-10 15:47:50.375775 text_tagging_model-0.1.2a8/text_tagging_model/processing/ranker/__init__.py
--rw-r--r--   0        0        0      843 2024-04-11 00:02:41.411968 text_tagging_model-0.1.2a8/text_tagging_model/processing/ranker/base_ranker.py
--rw-r--r--   0        0        0      781 2024-04-11 00:01:12.682816 text_tagging_model-0.1.2a8/text_tagging_model/processing/ranker/max_distance_ranker.py
--rw-r--r--   0        0        0        0 2024-04-10 20:50:54.437113 text_tagging_model-0.1.2a8/text_tagging_model/processing/summarizator/__init__.py
--rw-r--r--   0        0        0     1126 2024-04-10 22:49:41.812642 text_tagging_model-0.1.2a8/text_tagging_model/processing/summarizator/bart_summarization.py
--rw-r--r--   0        0        0       58 2024-04-10 13:26:29.787998 text_tagging_model-0.1.2a8/text_tagging_model/processing/utils.py
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 text_tagging_model-0.1.2a8/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-05 18:27:57.393842 text_tagging_model-0.1.2a9/README.md
+-rw-r--r--   0        0        0     1540 2024-04-11 10:07:05.228849 text_tagging_model-0.1.2a9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 13:26:29.785403 text_tagging_model-0.1.2a9/text_tagging_model/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-10 17:38:45.908803 text_tagging_model-0.1.2a9/text_tagging_model/logger_config.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:59:49.958211 text_tagging_model-0.1.2a9/text_tagging_model/models/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-10 21:18:16.240769 text_tagging_model-0.1.2a9/text_tagging_model/models/bart_based_model/__init__.py
+-rw-r--r--   0        0        0     3622 2024-04-11 10:06:53.010074 text_tagging_model-0.1.2a9/text_tagging_model/models/bart_based_model/tag_sum_extractor.py
+-rw-r--r--   0        0        0     1230 2024-04-10 13:26:29.785889 text_tagging_model-0.1.2a9/text_tagging_model/models/metrics.py
+-rw-r--r--   0        0        0       84 2024-04-10 19:51:48.269012 text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/__init__.py
+-rw-r--r--   0        0        0     1526 2024-04-10 17:03:50.201269 text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/keyphrases_extractor.py
+-rw-r--r--   0        0        0     3741 2024-04-11 00:11:22.852114 text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/tags_extractor.py
+-rw-r--r--   0        0        0      216 2024-04-10 15:00:17.918296 text_tagging_model-0.1.2a9/text_tagging_model/processing/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:49:15.254929 text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-10 20:39:51.551412 text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/base_embedder.py
+-rw-r--r--   0        0        0      509 2024-04-10 20:00:44.503406 text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/fasttext_embedder.py
+-rw-r--r--   0        0        0      822 2024-04-11 00:09:17.764085 text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/hg_embedder.py
+-rw-r--r--   0        0        0      365 2024-04-10 17:07:38.801435 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-10 16:36:32.623920 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/base_normalizer.py
+-rw-r--r--   0        0        0      996 2024-04-10 20:00:44.506705 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/nouns_keeper.py
+-rw-r--r--   0        0        0      624 2024-04-10 20:06:17.954874 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/pipe.py
+-rw-r--r--   0        0        0      456 2024-04-10 20:00:44.508075 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/punctuation_deleter.py
+-rw-r--r--   0        0        0      746 2024-04-10 20:00:44.508861 text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/stopwords_deleter.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:47:50.375775 text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-11 00:02:41.411968 text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/base_ranker.py
+-rw-r--r--   0        0        0      781 2024-04-11 00:01:12.682816 text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/max_distance_ranker.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:50:54.437113 text_tagging_model-0.1.2a9/text_tagging_model/processing/summarizator/__init__.py
+-rw-r--r--   0        0        0     1126 2024-04-10 22:49:41.812642 text_tagging_model-0.1.2a9/text_tagging_model/processing/summarizator/bart_summarization.py
+-rw-r--r--   0        0        0       58 2024-04-10 13:26:29.787998 text_tagging_model-0.1.2a9/text_tagging_model/processing/utils.py
+-rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 text_tagging_model-0.1.2a9/PKG-INFO
```

### Comparing `text_tagging_model-0.1.2a8/pyproject.toml` & `text_tagging_model-0.1.2a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text-tagging-model"
-version = "0.1.2a8"
+version = "0.1.2a9"
 description = "Here we collected some online and offline models for text tagging."
 authors = [
     "Pavel Kochkin <kochkin27@gmail.com>",
     "Shamil Nurkaev <nurkaievs1204@gmail.com>",
     "Denis <denison03@mail.ru>",
     "Stephan Olizko <stepa.olizko@yandex.ru>"
 ]
```

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/logger_config.py` & `text_tagging_model-0.1.2a9/text_tagging_model/logger_config.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/models/bart_based_model/tag_sum_extractor.py` & `text_tagging_model-0.1.2a9/text_tagging_model/models/bart_based_model/tag_sum_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,13 +97,13 @@
         """
 
         keyphrase = self.summarizator.get_summary(text.lower())
         normalized_keyphrase = self.normalizer.normalize(keyphrase)
         most_co_occurring_words = [
             word
             for word, cnt in Counter(normalized_keyphrase).most_common(2 * top_n)
-            if cnt >= self.min_cnt_keyword
+            # if cnt >= self.min_cnt_keyword
         ]
 
         keywords = self.ranker.get_top_n_keywords(np.array(most_co_occurring_words), top_n)
 
         return keywords
```

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/models/metrics.py` & `text_tagging_model-0.1.2a9/text_tagging_model/models/metrics.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/models/rake_based_model/keyphrases_extractor.py` & `text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/keyphrases_extractor.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/models/rake_based_model/tags_extractor.py` & `text_tagging_model-0.1.2a9/text_tagging_model/models/rake_based_model/tags_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
         normalized_keyphrases = list(map(self.normalizer.normalize, keyphrases))
         normalized_words = list(chain(*normalized_keyphrases))
 
         most_co_occurring_words = np.array(
             [
                 word
-                for word, cnt in Counter(normalized_words).most_common(2 * top_n)
+                for word, cnt in Counter(normalized_words).most_common(top_n)
                 if cnt >= self.min_cnt_keyword
             ]
         )
 
         keywords = self.ranker.get_top_n_keywords(most_co_occurring_words, top_n)
 
         return keywords
```

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/processing/embedder/hg_embedder.py` & `text_tagging_model-0.1.2a9/text_tagging_model/processing/embedder/hg_embedder.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/nouns_keeper.py` & `text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/nouns_keeper.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/pipe.py` & `text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/pipe.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/processing/normalizers/stopwords_deleter.py` & `text_tagging_model-0.1.2a9/text_tagging_model/processing/normalizers/stopwords_deleter.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/processing/ranker/base_ranker.py` & `text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/base_ranker.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/processing/ranker/max_distance_ranker.py` & `text_tagging_model-0.1.2a9/text_tagging_model/processing/ranker/max_distance_ranker.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/text_tagging_model/processing/summarizator/bart_summarization.py` & `text_tagging_model-0.1.2a9/text_tagging_model/processing/summarizator/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `text_tagging_model-0.1.2a8/PKG-INFO` & `text_tagging_model-0.1.2a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-tagging-model
-Version: 0.1.2a8
+Version: 0.1.2a9
 Summary: Here we collected some online and offline models for text tagging.
 Author: Pavel Kochkin
 Author-email: kochkin27@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

