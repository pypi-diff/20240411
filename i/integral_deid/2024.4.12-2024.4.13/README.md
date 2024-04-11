# Comparing `tmp/integral_deid-2024.4.12.tar.gz` & `tmp/integral_deid-2024.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integral_deid-2024.4.12.tar", max compression
+gzip compressed data, was "integral_deid-2024.4.13.tar", max compression
```

## Comparing `integral_deid-2024.4.12.tar` & `integral_deid-2024.4.13.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     7126 2024-04-05 16:49:03.600397 integral_deid-2024.4.12/integral_deid/__init__.py
--rw-r--r--   0        0        0     2441 2024-03-27 18:41:58.720831 integral_deid-2024.4.12/integral_deid/argmax_process.py
--rw-r--r--   0        0        0      665 2024-03-27 18:41:58.721027 integral_deid-2024.4.12/integral_deid/check_consistent_length.py
--rw-r--r--   0        0        0     3178 2024-03-27 18:41:58.721206 integral_deid-2024.4.12/integral_deid/clean_regex.py
--rw-r--r--   0        0        0    14684 2024-03-27 18:41:58.721410 integral_deid-2024.4.12/integral_deid/clinical_regex.py
--rw-r--r--   0        0        0     3264 2024-04-05 16:49:03.600759 integral_deid-2024.4.12/integral_deid/clinical_spacy_tokenizer.py
--rw-r--r--   0        0        0     2017 2024-03-27 18:41:58.721936 integral_deid-2024.4.12/integral_deid/conditional_random_field_sub.py
--rw-r--r--   0        0        0     2385 2024-03-27 18:41:58.722088 integral_deid-2024.4.12/integral_deid/core_nlp_tokenizer.py
--rw-r--r--   0        0        0     1128 2024-03-27 18:41:58.722299 integral_deid-2024.4.12/integral_deid/crf_argmax_process.py
--rw-r--r--   0        0        0     3374 2024-03-27 18:41:58.722533 integral_deid-2024.4.12/integral_deid/crf_bert_model_for_token_classification.py
--rw-r--r--   0        0        0     3954 2024-03-27 18:41:58.722750 integral_deid-2024.4.12/integral_deid/crf_process.py
--rw-r--r--   0        0        0      659 2024-03-27 18:41:58.722929 integral_deid-2024.4.12/integral_deid/crf_token_classifier_output.py
--rw-r--r--   0        0        0     5886 2024-03-27 18:41:58.723170 integral_deid-2024.4.12/integral_deid/crf_utils.py
--rw-r--r--   0        0        0     4066 2024-03-27 18:41:58.723347 integral_deid-2024.4.12/integral_deid/data_training_arguments.py
--rw-r--r--   0        0        0     6834 2024-03-27 18:41:58.723573 integral_deid-2024.4.12/integral_deid/dataset.py
--rw-r--r--   0        0        0     8995 2024-03-27 18:41:58.723814 integral_deid-2024.4.12/integral_deid/dataset_creator.py
--rw-r--r--   0        0        0    10063 2024-03-27 18:41:58.724005 integral_deid-2024.4.12/integral_deid/dataset_tokenizer.py
--rw-r--r--   0        0        0     3827 2024-03-27 18:41:58.724178 integral_deid-2024.4.12/integral_deid/date_regex.py
--rw-r--r--   0        0        0     1055 2024-03-27 18:41:58.724416 integral_deid-2024.4.12/integral_deid/evaluation_arguments.py
--rw-r--r--   0        0        0     4071 2024-03-27 18:41:58.724705 integral_deid-2024.4.12/integral_deid/label_mapper.py
--rw-r--r--   0        0        0     2255 2024-03-27 18:41:58.724927 integral_deid-2024.4.12/integral_deid/logits_process.py
--rw-r--r--   0        0        0      326 2024-03-27 18:41:58.725115 integral_deid-2024.4.12/integral_deid/mismatch_error.py
--rw-r--r--   0        0        0     1527 2024-03-27 18:41:58.725304 integral_deid-2024.4.12/integral_deid/model_arguments.py
--rw-r--r--   0        0        0     3568 2024-03-27 18:41:58.725546 integral_deid-2024.4.12/integral_deid/model_picker.py
--rw-r--r--   0        0        0     3637 2024-03-27 18:41:58.725725 integral_deid-2024.4.12/integral_deid/ner_dataset.py
--rw-r--r--   0        0        0     2937 2024-03-27 18:41:58.725893 integral_deid-2024.4.12/integral_deid/ner_labels.py
--rw-r--r--   0        0        0     1072 2024-03-27 18:41:58.726064 integral_deid-2024.4.12/integral_deid/ner_predict_token_labels.py
--rw-r--r--   0        0        0     7780 2024-03-27 18:41:58.726318 integral_deid-2024.4.12/integral_deid/ner_token_labels.py
--rw-r--r--   0        0        0     8420 2024-03-27 18:41:58.726521 integral_deid-2024.4.12/integral_deid/note_level_aggregator.py
--rw-r--r--   0        0        0     1053 2024-03-27 18:41:58.726707 integral_deid-2024.4.12/integral_deid/note_sentencizer.py
--rw-r--r--   0        0        0     2649 2024-03-27 18:41:58.726935 integral_deid-2024.4.12/integral_deid/post_process_picker.py
--rw-r--r--   0        0        0     2370 2024-03-27 18:41:58.727189 integral_deid-2024.4.12/integral_deid/preprocessing_loader.py
--rw-r--r--   0        0        0    24393 2024-03-27 18:41:58.727527 integral_deid-2024.4.12/integral_deid/sentence_dataset.py
--rw-r--r--   0        0        0    25713 2024-04-08 17:17:05.742627 integral_deid-2024.4.12/integral_deid/sequence_tagging.py
--rw-r--r--   0        0        0     1258 2024-03-27 18:41:58.728155 integral_deid-2024.4.12/integral_deid/spacy_sentencizer.py
--rw-r--r--   0        0        0     1864 2024-03-27 18:41:58.728303 integral_deid-2024.4.12/integral_deid/spacy_tokenizer.py
--rw-r--r--   0        0        0     9040 2024-04-05 21:19:42.937516 integral_deid-2024.4.12/integral_deid/text_deid.py
--rw-r--r--   0        0        0     1079 2024-03-27 18:41:58.728699 integral_deid-2024.4.12/integral_deid/text_deid_utils.py
--rw-r--r--   0        0        0     2442 2024-03-27 18:41:58.728911 integral_deid-2024.4.12/integral_deid/threshold_process_max.py
--rw-r--r--   0        0        0     2356 2024-03-27 18:41:58.729134 integral_deid-2024.4.12/integral_deid/threshold_process_sum.py
--rw-r--r--   0        0        0      760 2024-04-11 15:20:41.814857 integral_deid-2024.4.12/pyproject.toml
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 integral_deid-2024.4.12/PKG-INFO
+-rw-r--r--   0        0        0     7126 2024-04-05 16:49:03.600397 integral_deid-2024.4.13/integral_deid/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-11 16:09:06.913504 integral_deid-2024.4.13/integral_deid/argmax_process.py
+-rw-r--r--   0        0        0      665 2024-03-27 18:41:58.721027 integral_deid-2024.4.13/integral_deid/check_consistent_length.py
+-rw-r--r--   0        0        0     3178 2024-03-27 18:41:58.721206 integral_deid-2024.4.13/integral_deid/clean_regex.py
+-rw-r--r--   0        0        0    14684 2024-03-27 18:41:58.721410 integral_deid-2024.4.13/integral_deid/clinical_regex.py
+-rw-r--r--   0        0        0     3274 2024-04-11 16:09:06.917170 integral_deid-2024.4.13/integral_deid/clinical_spacy_tokenizer.py
+-rw-r--r--   0        0        0     2017 2024-03-27 18:41:58.721936 integral_deid-2024.4.13/integral_deid/conditional_random_field_sub.py
+-rw-r--r--   0        0        0     2385 2024-03-27 18:41:58.722088 integral_deid-2024.4.13/integral_deid/core_nlp_tokenizer.py
+-rw-r--r--   0        0        0     1130 2024-04-11 16:09:06.921313 integral_deid-2024.4.13/integral_deid/crf_argmax_process.py
+-rw-r--r--   0        0        0     3378 2024-04-11 16:09:06.923955 integral_deid-2024.4.13/integral_deid/crf_bert_model_for_token_classification.py
+-rw-r--r--   0        0        0     3956 2024-04-11 16:09:06.926157 integral_deid-2024.4.13/integral_deid/crf_process.py
+-rw-r--r--   0        0        0      659 2024-03-27 18:41:58.722929 integral_deid-2024.4.13/integral_deid/crf_token_classifier_output.py
+-rw-r--r--   0        0        0     5886 2024-03-27 18:41:58.723170 integral_deid-2024.4.13/integral_deid/crf_utils.py
+-rw-r--r--   0        0        0     4066 2024-03-27 18:41:58.723347 integral_deid-2024.4.13/integral_deid/data_training_arguments.py
+-rw-r--r--   0        0        0     6840 2024-04-11 16:09:06.928227 integral_deid-2024.4.13/integral_deid/dataset.py
+-rw-r--r--   0        0        0     9001 2024-04-11 16:09:06.930502 integral_deid-2024.4.13/integral_deid/dataset_creator.py
+-rw-r--r--   0        0        0    10063 2024-03-27 18:41:58.724005 integral_deid-2024.4.13/integral_deid/dataset_tokenizer.py
+-rw-r--r--   0        0        0     3827 2024-03-27 18:41:58.724178 integral_deid-2024.4.13/integral_deid/date_regex.py
+-rw-r--r--   0        0        0     1055 2024-03-27 18:41:58.724416 integral_deid-2024.4.13/integral_deid/evaluation_arguments.py
+-rw-r--r--   0        0        0     4073 2024-04-11 16:09:06.933240 integral_deid-2024.4.13/integral_deid/label_mapper.py
+-rw-r--r--   0        0        0     2255 2024-03-27 18:41:58.724927 integral_deid-2024.4.13/integral_deid/logits_process.py
+-rw-r--r--   0        0        0      326 2024-03-27 18:41:58.725115 integral_deid-2024.4.13/integral_deid/mismatch_error.py
+-rw-r--r--   0        0        0     1527 2024-03-27 18:41:58.725304 integral_deid-2024.4.13/integral_deid/model_arguments.py
+-rw-r--r--   0        0        0     3572 2024-04-11 16:09:06.935112 integral_deid-2024.4.13/integral_deid/model_picker.py
+-rw-r--r--   0        0        0     3637 2024-03-27 18:41:58.725725 integral_deid-2024.4.13/integral_deid/ner_dataset.py
+-rw-r--r--   0        0        0     2937 2024-03-27 18:41:58.725893 integral_deid-2024.4.13/integral_deid/ner_labels.py
+-rw-r--r--   0        0        0     1072 2024-03-27 18:41:58.726064 integral_deid-2024.4.13/integral_deid/ner_predict_token_labels.py
+-rw-r--r--   0        0        0     7782 2024-04-11 16:09:06.949311 integral_deid-2024.4.13/integral_deid/ner_token_labels.py
+-rw-r--r--   0        0        0     8420 2024-03-27 18:41:58.726521 integral_deid-2024.4.13/integral_deid/note_level_aggregator.py
+-rw-r--r--   0        0        0     1053 2024-03-27 18:41:58.726707 integral_deid-2024.4.13/integral_deid/note_sentencizer.py
+-rw-r--r--   0        0        0     2659 2024-04-11 16:09:06.951048 integral_deid-2024.4.13/integral_deid/post_process_picker.py
+-rw-r--r--   0        0        0     2380 2024-04-11 16:09:06.952852 integral_deid-2024.4.13/integral_deid/preprocessing_loader.py
+-rw-r--r--   0        0        0    24393 2024-03-27 18:41:58.727527 integral_deid-2024.4.13/integral_deid/sentence_dataset.py
+-rw-r--r--   0        0        0    25731 2024-04-11 16:09:06.955005 integral_deid-2024.4.13/integral_deid/sequence_tagging.py
+-rw-r--r--   0        0        0     1258 2024-03-27 18:41:58.728155 integral_deid-2024.4.13/integral_deid/spacy_sentencizer.py
+-rw-r--r--   0        0        0     1864 2024-03-27 18:41:58.728303 integral_deid-2024.4.13/integral_deid/spacy_tokenizer.py
+-rw-r--r--   0        0        0     9042 2024-04-11 16:09:06.957370 integral_deid-2024.4.13/integral_deid/text_deid.py
+-rw-r--r--   0        0        0     1079 2024-03-27 18:41:58.728699 integral_deid-2024.4.13/integral_deid/text_deid_utils.py
+-rw-r--r--   0        0        0     2444 2024-04-11 16:09:06.959161 integral_deid-2024.4.13/integral_deid/threshold_process_max.py
+-rw-r--r--   0        0        0     2358 2024-04-11 16:09:06.961033 integral_deid-2024.4.13/integral_deid/threshold_process_sum.py
+-rw-r--r--   0        0        0      760 2024-04-11 16:09:25.434538 integral_deid-2024.4.13/pyproject.toml
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 integral_deid-2024.4.13/PKG-INFO
```

### Comparing `integral_deid-2024.4.12/integral_deid/__init__.py` & `integral_deid-2024.4.13/integral_deid/__init__.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/argmax_process.py` & `integral_deid-2024.4.13/integral_deid/logits_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-import numpy as np
 from typing import Sequence, NoReturn, Tuple
 
-from robust_deid.check_consistent_length import check_consistent_length
 
-
-class ArgmaxProcess(object):
+class LogitsProcess(object):
     """
     Process the output of the model forward pass. The forward pass will return the predictions
     (e.g the logits), labels if present. We process the output and return the processed
     values based on the application. This script we return the final prediction as the
     argmax of the logits.
     """
 
@@ -19,33 +16,31 @@
         Args:
             label_list (Sequence[str]): The list of NER labels
         """
         self._label_list = label_list
 
     def decode(
         self, predictions: Sequence[Sequence[Sequence[float]]], labels: Sequence[Sequence[int]]
-    ) -> Tuple[Sequence[Sequence[str]], Sequence[Sequence[str]]]:
+    ) -> Tuple[Sequence[Sequence[Sequence[float]]], Sequence[Sequence[str]]]:
         """
         Decode the predictions and labels so that the evaluation function and prediction
         functions can use them accordingly. The predictions and labels are numbers (ids)
         of the labels, these will be converted back to the NER tags (B-AGE, I-DATE etc) using
         the label_list. In this function we just take the argmax of the logits (scores) of the predictions
         Also remove the predictions and labels on the subword and context tokens
         Args:
             predictions (Sequence[Sequence[Sequence[float]]]): The logits (scores for each tag) returned by the model
-            labels (Sequence[Sequence[str]]): Gold standard labels
+            labels (Sequence[Sequence[int]]): Gold standard labels
         Returns:
             true_predictions (Sequence[Sequence[str]]): The predicted NER tags
             true_labels (Sequence[Sequence[str]]): The gold standard NER tags
         """
-        predictions = np.argmax(predictions, axis=2)
         # Remove ignored index (special tokens)
         true_predictions = [
-            [self._label_list[p] for (p, l) in zip(prediction, label) if l != -100]
+            [[float(value) for value in p] for (p, l) in zip(prediction, label) if l != -100]
             for prediction, label in zip(predictions, labels)
         ]
         true_labels = [
             [self._label_list[l] for (p, l) in zip(prediction, label) if l != -100]
             for prediction, label in zip(predictions, labels)
         ]
-        check_consistent_length(true_predictions, true_labels)
         return true_predictions, true_labels
```

### Comparing `integral_deid-2024.4.12/integral_deid/check_consistent_length.py` & `integral_deid-2024.4.13/integral_deid/check_consistent_length.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/clean_regex.py` & `integral_deid-2024.4.13/integral_deid/clean_regex.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/clinical_regex.py` & `integral_deid-2024.4.13/integral_deid/clinical_regex.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/clinical_spacy_tokenizer.py` & `integral_deid-2024.4.13/integral_deid/clinical_spacy_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 import spacy
 from spacy.symbols import ORTH
-from robust_deid.spacy_tokenizer import SpacyTokenizer
-from robust_deid.date_regex import DateRegex
-from robust_deid.clean_regex import CleanRegex
-from robust_deid.clinical_regex import ClinicalRegex
+from integral_deid.spacy_tokenizer import SpacyTokenizer
+from integral_deid.date_regex import DateRegex
+from integral_deid.clean_regex import CleanRegex
+from integral_deid.clinical_regex import ClinicalRegex
 
 
 def read_abbreviations():
-    from robust_deid import abbreviations
+    from integral_deid import abbreviations
 
     return abbreviations
 
 
 class ClinicalSpacyTokenizer(SpacyTokenizer):
     """
     This class is used to read text and return the tokens
```

### Comparing `integral_deid-2024.4.12/integral_deid/conditional_random_field_sub.py` & `integral_deid-2024.4.13/integral_deid/conditional_random_field_sub.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/core_nlp_tokenizer.py` & `integral_deid-2024.4.13/integral_deid/core_nlp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/crf_argmax_process.py` & `integral_deid-2024.4.13/integral_deid/crf_argmax_process.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Sequence, NoReturn, List
 
-from robust_deid.crf_process import CRFProcess
+from integral_deid.crf_process import CRFProcess
 
 
 class CRFArgmaxProcess(CRFProcess):
     def __init__(self, label_list: Sequence[str], top_k: int = None) -> NoReturn:
         """
         Initialize a label list where the position corresponds to a particular label. For example
         position 0 will correspond to B-DATE etc. top k will return the top k CRF sequences
```

### Comparing `integral_deid-2024.4.12/integral_deid/crf_bert_model_for_token_classification.py` & `integral_deid-2024.4.13/integral_deid/crf_bert_model_for_token_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from transformers import (
     BertConfig,
     BertForTokenClassification,
 )
 
-from robust_deid.conditional_random_field_sub import ConditionalRandomFieldSub
-from robust_deid.crf_token_classifier_output import CRFTokenClassifierOutput
+from integral_deid.conditional_random_field_sub import ConditionalRandomFieldSub
+from integral_deid.crf_token_classifier_output import CRFTokenClassifierOutput
 
 
 class CRFBertModelForTokenClassification(BertForTokenClassification):
     def __init__(self, config: BertConfig, crf_constraints):
         super().__init__(config)
         self.crf = ConditionalRandomFieldSub(num_labels=config.num_labels, constraints=crf_constraints)
```

### Comparing `integral_deid-2024.4.12/integral_deid/crf_process.py` & `integral_deid-2024.4.13/integral_deid/crf_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Sequence, NoReturn
 
 import torch
 
-from robust_deid.check_consistent_length import check_consistent_length
+from integral_deid.check_consistent_length import check_consistent_length
 
 
 class CRFProcess(object):
     def __init__(self, label_list: Sequence[str], top_k: int) -> NoReturn:
         """
         Initialize a label list where the position corresponds to a particular label. For example
         position 0 will correspond to B-DATE etc. top k will return the top k CRF sequences
```

### Comparing `integral_deid-2024.4.12/integral_deid/crf_token_classifier_output.py` & `integral_deid-2024.4.13/integral_deid/crf_token_classifier_output.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/crf_utils.py` & `integral_deid-2024.4.13/integral_deid/crf_utils.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/data_training_arguments.py` & `integral_deid-2024.4.13/integral_deid/data_training_arguments.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/dataset.py` & `integral_deid-2024.4.13/integral_deid/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import re
 from typing import Iterable, Dict, Sequence, Union, Mapping, Optional, List
 
-from robust_deid.ner_token_labels import NERTokenLabels
-from robust_deid.ner_predict_token_labels import NERPredictTokenLabels
-from robust_deid.mismatch_error import MismatchError
+from integral_deid.ner_token_labels import NERTokenLabels
+from integral_deid.ner_predict_token_labels import NERPredictTokenLabels
+from integral_deid.mismatch_error import MismatchError
 
 random.seed(41)
 
 
 class Dataset(object):
     """
     Build a NER token classification dataset. Each token should have a corresponding label
```

### Comparing `integral_deid-2024.4.12/integral_deid/dataset_creator.py` & `integral_deid-2024.4.13/integral_deid/dataset_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import random
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from typing import Dict, Iterable, List, NoReturn, Union
 
-from robust_deid.dataset import Dataset
-from robust_deid.sentence_dataset import SentenceDataset
-from robust_deid.preprocessing_loader import PreprocessingLoader
+from integral_deid.dataset import Dataset
+from integral_deid.sentence_dataset import SentenceDataset
+from integral_deid.preprocessing_loader import PreprocessingLoader
 
 random.seed(41)
 
 
 class DatasetCreator(object):
     """
     Build a NER token classification dataset
```

### Comparing `integral_deid-2024.4.12/integral_deid/dataset_tokenizer.py` & `integral_deid-2024.4.13/integral_deid/dataset_tokenizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/date_regex.py` & `integral_deid-2024.4.13/integral_deid/date_regex.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/evaluation_arguments.py` & `integral_deid-2024.4.13/integral_deid/evaluation_arguments.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/label_mapper.py` & `integral_deid-2024.4.13/integral_deid/label_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, List, Mapping, NoReturn, Sequence, Union
-from robust_deid.ner_labels import NERLabels
+from integral_deid.ner_labels import NERLabels
 
 
 class LabelMapper(object):
     """
     This class is used to map one set of NER labels to another set of NER labels
     For example we might want to map all NER labels to Binary HIPAA labels.
     E.g:
```

### Comparing `integral_deid-2024.4.12/integral_deid/logits_process.py` & `integral_deid-2024.4.13/integral_deid/argmax_process.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import numpy as np
 from typing import Sequence, NoReturn, Tuple
 
+from integral_deid.check_consistent_length import check_consistent_length
 
-class LogitsProcess(object):
+
+class ArgmaxProcess(object):
     """
     Process the output of the model forward pass. The forward pass will return the predictions
     (e.g the logits), labels if present. We process the output and return the processed
     values based on the application. This script we return the final prediction as the
     argmax of the logits.
     """
 
@@ -16,31 +19,33 @@
         Args:
             label_list (Sequence[str]): The list of NER labels
         """
         self._label_list = label_list
 
     def decode(
         self, predictions: Sequence[Sequence[Sequence[float]]], labels: Sequence[Sequence[int]]
-    ) -> Tuple[Sequence[Sequence[Sequence[float]]], Sequence[Sequence[str]]]:
+    ) -> Tuple[Sequence[Sequence[str]], Sequence[Sequence[str]]]:
         """
         Decode the predictions and labels so that the evaluation function and prediction
         functions can use them accordingly. The predictions and labels are numbers (ids)
         of the labels, these will be converted back to the NER tags (B-AGE, I-DATE etc) using
         the label_list. In this function we just take the argmax of the logits (scores) of the predictions
         Also remove the predictions and labels on the subword and context tokens
         Args:
             predictions (Sequence[Sequence[Sequence[float]]]): The logits (scores for each tag) returned by the model
-            labels (Sequence[Sequence[int]]): Gold standard labels
+            labels (Sequence[Sequence[str]]): Gold standard labels
         Returns:
             true_predictions (Sequence[Sequence[str]]): The predicted NER tags
             true_labels (Sequence[Sequence[str]]): The gold standard NER tags
         """
+        predictions = np.argmax(predictions, axis=2)
         # Remove ignored index (special tokens)
         true_predictions = [
-            [[float(value) for value in p] for (p, l) in zip(prediction, label) if l != -100]
+            [self._label_list[p] for (p, l) in zip(prediction, label) if l != -100]
             for prediction, label in zip(predictions, labels)
         ]
         true_labels = [
             [self._label_list[l] for (p, l) in zip(prediction, label) if l != -100]
             for prediction, label in zip(predictions, labels)
         ]
+        check_consistent_length(true_predictions, true_labels)
         return true_predictions, true_labels
```

### Comparing `integral_deid-2024.4.12/integral_deid/model_arguments.py` & `integral_deid-2024.4.13/integral_deid/model_arguments.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/model_picker.py` & `integral_deid-2024.4.13/integral_deid/model_picker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Use the functions below to get the desired model for training.
 from typing import Dict, NoReturn
 
 from transformers import AutoConfig, AutoModelForTokenClassification
 
-from robust_deid.crf_utils import allowed_transitions
-from robust_deid.crf_bert_model_for_token_classification import CRFBertModelForTokenClassification
+from integral_deid.crf_utils import allowed_transitions
+from integral_deid.crf_bert_model_for_token_classification import CRFBertModelForTokenClassification
 
 
 class ModelPicker(object):
     """
     This class is used to pick the model we are using to train.
     The class provides functions that returns the desired model objects
     i.e get the desired model for training etc
```

### Comparing `integral_deid-2024.4.12/integral_deid/ner_dataset.py` & `integral_deid-2024.4.13/integral_deid/ner_dataset.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/ner_labels.py` & `integral_deid-2024.4.13/integral_deid/ner_labels.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/ner_predict_token_labels.py` & `integral_deid-2024.4.13/integral_deid/ner_predict_token_labels.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/ner_token_labels.py` & `integral_deid-2024.4.13/integral_deid/ner_token_labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Mapping, Union
-from robust_deid.mismatch_error import MismatchError
+from integral_deid.mismatch_error import MismatchError
 
 
 class NERTokenLabels(object):
     """
     This class is used to align tokens with the spans
     Each token is assigned one of the following labels
     'B-LABEL', 'I-LABEL', 'O'. For example the text
```

### Comparing `integral_deid-2024.4.12/integral_deid/note_level_aggregator.py` & `integral_deid-2024.4.13/integral_deid/note_level_aggregator.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/note_sentencizer.py` & `integral_deid-2024.4.13/integral_deid/note_sentencizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/post_process_picker.py` & `integral_deid-2024.4.13/integral_deid/post_process_picker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from robust_deid.argmax_process import ArgmaxProcess
-from robust_deid.crf_argmax_process import CRFArgmaxProcess
-from robust_deid.logits_process import LogitsProcess
-from robust_deid.threshold_process_max import ThresholdProcessMax
-from robust_deid.threshold_process_sum import ThresholdProcessSum
+from integral_deid.argmax_process import ArgmaxProcess
+from integral_deid.crf_argmax_process import CRFArgmaxProcess
+from integral_deid.logits_process import LogitsProcess
+from integral_deid.threshold_process_max import ThresholdProcessMax
+from integral_deid.threshold_process_sum import ThresholdProcessSum
 
 
 class PostProcessPicker(object):
     """
     This class is used to pick the post process layer that processed the model
     logits. The class provides functions that returns the desired post processor objects
     For example we can pick the argamx of the logits, where we just choose the highest scoring
```

### Comparing `integral_deid-2024.4.12/integral_deid/preprocessing_loader.py` & `integral_deid-2024.4.13/integral_deid/preprocessing_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
-from robust_deid.spacy_sentencizer import SpacySentencizer
-from robust_deid.note_sentencizer import NoteSentencizer
-from robust_deid.clinical_spacy_tokenizer import ClinicalSpacyTokenizer
-from robust_deid.spacy_tokenizer import SpacyTokenizer
-from robust_deid.core_nlp_tokenizer import CoreNLPTokenizer
+from integral_deid.spacy_sentencizer import SpacySentencizer
+from integral_deid.note_sentencizer import NoteSentencizer
+from integral_deid.clinical_spacy_tokenizer import ClinicalSpacyTokenizer
+from integral_deid.spacy_tokenizer import SpacyTokenizer
+from integral_deid.core_nlp_tokenizer import CoreNLPTokenizer
 
 
 class PreprocessingLoader(object):
     @staticmethod
     def get_sentencizer(sentencizer: str) -> Union[SpacySentencizer, NoteSentencizer]:
         """
         Get the desired the sentencizer
```

### Comparing `integral_deid-2024.4.12/integral_deid/sentence_dataset.py` & `integral_deid-2024.4.13/integral_deid/sentence_dataset.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/sequence_tagging.py` & `integral_deid-2024.4.13/integral_deid/sequence_tagging.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 device = torch.device("cpu")
 
 
 # Will error if the minimal version of Transformers is not installed. Remove at your own risks.
 # check_min_version("4.13.0.dev0")
 
 # require_version("datasets>=1.8.0", "To fix: pip install -r examples/pytorch/token-classification/requirements.txt")
-from robust_deid.post_process_picker import PostProcessPicker
-from robust_deid.dataset_tokenizer import DatasetTokenizer
-from robust_deid.label_mapper import LabelMapper
-from robust_deid.ner_labels import NERLabels
-from robust_deid.model_arguments import ModelArguments
-from robust_deid.data_training_arguments import DataTrainingArguments
-from robust_deid.evaluation_arguments import EvaluationArguments
-from robust_deid.model_picker import ModelPicker
-from robust_deid.note_level_aggregator import NoteLevelAggregator
+from integral_deid.post_process_picker import PostProcessPicker
+from integral_deid.dataset_tokenizer import DatasetTokenizer
+from integral_deid.label_mapper import LabelMapper
+from integral_deid.ner_labels import NERLabels
+from integral_deid.model_arguments import ModelArguments
+from integral_deid.data_training_arguments import DataTrainingArguments
+from integral_deid.evaluation_arguments import EvaluationArguments
+from integral_deid.model_picker import ModelPicker
+from integral_deid.note_level_aggregator import NoteLevelAggregator
 
 
 class SequenceTagger(object):
     def __init__(
         self,
         task_name,
         notation,
```

### Comparing `integral_deid-2024.4.12/integral_deid/spacy_sentencizer.py` & `integral_deid-2024.4.13/integral_deid/spacy_sentencizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/spacy_tokenizer.py` & `integral_deid-2024.4.13/integral_deid/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/text_deid.py` & `integral_deid-2024.4.13/integral_deid/text_deid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import re
 from argparse import ArgumentParser
 from typing import Sequence, List, Tuple, Mapping, Union, Any, Type
 import regex
 from seqeval.scheme import IOB1, IOB2, IOBES, BILOU, Entities
 
-from robust_deid.text_deid_utils import remove, replace_tag_type, replace_informative
+from integral_deid.text_deid_utils import remove, replace_tag_type, replace_informative
 
 
 class TextDeid(object):
     def __init__(self, notation, span_constraint):
         self._span_constraint = span_constraint
         if self._span_constraint == "strict":
             self._scheme = TextDeid.__get_scheme("IO")
```

### Comparing `integral_deid-2024.4.12/integral_deid/text_deid_utils.py` & `integral_deid-2024.4.13/integral_deid/text_deid_utils.py`

 * *Files identical despite different names*

### Comparing `integral_deid-2024.4.12/integral_deid/threshold_process_max.py` & `integral_deid-2024.4.13/integral_deid/threshold_process_sum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Sequence, NoReturn, Tuple
 
 import numpy as np
 from scipy.special import softmax
 
-from robust_deid.check_consistent_length import check_consistent_length
+from integral_deid.check_consistent_length import check_consistent_length
 
 
-class ThresholdProcessMax(object):
+class ThresholdProcessSum(object):
     """ """
 
     def __init__(self, label_list: Sequence[str], threshold: float) -> NoReturn:
         """
         Initialize a label list where the posiion corresponds to a particular label. For example
         position 0 will correspond to B-DATE etc.
         Args:
@@ -24,19 +24,18 @@
 
     def get_masked_array(self, data):
         return np.ma.MaskedArray(data=data, mask=self._mask)
 
     def process_prediction(self, prediction):
         softmax_prob = softmax(prediction)
         masked_softmax_prob = self.get_masked_array(data=softmax_prob)
-        max_value = masked_softmax_prob[masked_softmax_prob >= self._threshold]
-        if type(max_value.sum()) == np.ma.core.MaskedConstant:
-            return self._outside_label_index
-        else:
+        if masked_softmax_prob.sum() >= self._threshold:
             return masked_softmax_prob.argmax()
+        else:
+            return self._outside_label_index
 
     def decode(
         self, predictions: Sequence[Sequence[Sequence[float]]], labels: Sequence[Sequence[int]]
     ) -> Tuple[Sequence[Sequence[str]], Sequence[Sequence[str]]]:
         """
         Args:
             predictions (Sequence[Sequence[Sequence[float]]]): The logits (scores for each tag) returned by the model
```

### Comparing `integral_deid-2024.4.12/integral_deid/threshold_process_sum.py` & `integral_deid-2024.4.13/integral_deid/threshold_process_max.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Sequence, NoReturn, Tuple
 
 import numpy as np
 from scipy.special import softmax
 
-from robust_deid.check_consistent_length import check_consistent_length
+from integral_deid.check_consistent_length import check_consistent_length
 
 
-class ThresholdProcessSum(object):
+class ThresholdProcessMax(object):
     """ """
 
     def __init__(self, label_list: Sequence[str], threshold: float) -> NoReturn:
         """
         Initialize a label list where the posiion corresponds to a particular label. For example
         position 0 will correspond to B-DATE etc.
         Args:
@@ -24,18 +24,19 @@
 
     def get_masked_array(self, data):
         return np.ma.MaskedArray(data=data, mask=self._mask)
 
     def process_prediction(self, prediction):
         softmax_prob = softmax(prediction)
         masked_softmax_prob = self.get_masked_array(data=softmax_prob)
-        if masked_softmax_prob.sum() >= self._threshold:
-            return masked_softmax_prob.argmax()
-        else:
+        max_value = masked_softmax_prob[masked_softmax_prob >= self._threshold]
+        if type(max_value.sum()) == np.ma.core.MaskedConstant:
             return self._outside_label_index
+        else:
+            return masked_softmax_prob.argmax()
 
     def decode(
         self, predictions: Sequence[Sequence[Sequence[float]]], labels: Sequence[Sequence[int]]
     ) -> Tuple[Sequence[Sequence[str]], Sequence[Sequence[str]]]:
         """
         Args:
             predictions (Sequence[Sequence[Sequence[float]]]): The logits (scores for each tag) returned by the model
```

### Comparing `integral_deid-2024.4.12/pyproject.toml` & `integral_deid-2024.4.13/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "integral_deid"
-version = "2024.04.12"
+version = "2024.04.13"
 description = "PHI taggging and redaction"
 authors = ["Kevin DeSimone <kevin@useintegral.com>", "Dominick Villano <dominick@useintegral.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 transformers = "4.39.1"
 spacy = "3.7.4"
```

### Comparing `integral_deid-2024.4.12/PKG-INFO` & `integral_deid-2024.4.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integral_deid
-Version: 2024.4.12
+Version: 2024.4.13
 Summary: PHI taggging and redaction
 Author: Kevin DeSimone
 Author-email: kevin@useintegral.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

