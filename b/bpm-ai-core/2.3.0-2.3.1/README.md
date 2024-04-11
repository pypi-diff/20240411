# Comparing `tmp/bpm_ai_core-2.3.0.tar.gz` & `tmp/bpm_ai_core-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_core-2.3.0.tar", max compression
+gzip compressed data, was "bpm_ai_core-2.3.1.tar", max compression
```

## Comparing `bpm_ai_core-2.3.0.tar` & `bpm_ai_core-2.3.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0       13 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/classification/__init__.py
--rw-r--r--   0        0        0     1187 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/classification/zero_shot_classifier.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/__init__.py
--rw-r--r--   0        0        0      862 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/__init__.py
--rw-r--r--   0        0        0      306 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/_constants.py
--rw-r--r--   0        0        0     7213 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
--rw-r--r--   0        0        0      226 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
--rw-r--r--   0        0        0     2872 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/__init__.py
--rw-r--r--   0        0        0     6036 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/blob.py
--rw-r--r--   0        0        0     2445 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/llm.py
--rw-r--r--   0        0        0     2710 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/message.py
--rw-r--r--   0        0        0     2781 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/tool.py
--rw-r--r--   0        0        0     1455 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/__init__.py
--rw-r--r--   0        0        0      430 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/_constants.py
--rw-r--r--   0        0        0     7715 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/openai_chat.py
--rw-r--r--   0        0        0     2626 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/ocr/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/ocr/amazon_textract.py
--rw-r--r--   0        0        0     2698 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/ocr/azure_doc_intelligence.py
--rw-r--r--   0        0        0     1220 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/ocr/ocr.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/pos/__init__.py
--rw-r--r--   0        0        0      590 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/pos/pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/prompt/__init__.py
--rw-r--r--   0        0        0      372 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/prompt/filters.py
--rw-r--r--   0        0        0     6259 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/question_answering/__init__.py
--rw-r--r--   0        0        0     2085 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
--rw-r--r--   0        0        0     3018 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
--rw-r--r--   0        0        0     1096 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/question_answering/question_answering.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/__init__.py
--rw-r--r--   0        0        0      827 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/asr.py
--rw-r--r--   0        0        0     1428 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/openai_whisper.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/testing/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/testing/fake_llm.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/token_classification/__init__.py
--rw-r--r--   0        0        0      909 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/__init__.py
--rw-r--r--   0        0        0     2434 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/decorators.py
--rw-r--r--   0        0        0     1597 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/delegate.py
--rw-r--r--   0        0        0     4370 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/langfuse.py
--rw-r--r--   0        0        0     2267 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/logging.py
--rw-r--r--   0        0        0     1097 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/tracer.py
--rw-r--r--   0        0        0      876 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/tracing.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/translation/__init__.py
--rw-r--r--   0        0        0     1302 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/translation/amazon_translate.py
--rw-r--r--   0        0        0     1572 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/translation/azure_translation.py
--rw-r--r--   0        0        0      475 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/translation/nmt.py
--rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/audio.py
--rw-r--r--   0        0        0     1836 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/file.py
--rw-r--r--   0        0        0     5233 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/image.py
--rw-r--r--   0        0        0     1670 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/json_schema.py
--rw-r--r--   0        0        0    21191 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/linguistics.py
--rw-r--r--   0        0        0     1130 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/markdown.py
--rw-r--r--   0        0        0     5280 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/remote_object.py
--rw-r--r--   0        0        0     2596 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/storage.py
--rw-r--r--   0        0        0      675 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/xml_convert.py
--rw-r--r--   0        0        0     1014 2024-04-10 15:12:38.098810 bpm_ai_core-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/classification/__init__.py
+-rw-r--r--   0        0        0     1187 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/classification/zero_shot_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/anthropic_chat/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/anthropic_chat/_constants.py
+-rw-r--r--   0        0        0     7217 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
+-rw-r--r--   0        0        0      226 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
+-rw-r--r--   0        0        0     3100 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/anthropic_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/common/__init__.py
+-rw-r--r--   0        0        0     6036 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/common/blob.py
+-rw-r--r--   0        0        0     2445 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/common/llm.py
+-rw-r--r--   0        0        0     2710 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/common/message.py
+-rw-r--r--   0        0        0     2781 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/common/tool.py
+-rw-r--r--   0        0        0     1455 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/openai_chat/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/openai_chat/_constants.py
+-rw-r--r--   0        0        0     7749 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/openai_chat/openai_chat.py
+-rw-r--r--   0        0        0     2854 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/llm/openai_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/ocr/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/ocr/amazon_textract.py
+-rw-r--r--   0        0        0     2698 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/ocr/azure_doc_intelligence.py
+-rw-r--r--   0        0        0     1220 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/ocr/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/pos/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/pos/pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/prompt/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/prompt/filters.py
+-rw-r--r--   0        0        0     6259 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/question_answering/__init__.py
+-rw-r--r--   0        0        0     2085 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/question_answering/amazon_textract_docvqa.py
+-rw-r--r--   0        0        0     3018 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
+-rw-r--r--   0        0        0     1096 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/question_answering/question_answering.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/speech_recognition/asr.py
+-rw-r--r--   0        0        0     1428 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/speech_recognition/openai_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/testing/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/testing/fake_llm.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/token_classification/__init__.py
+-rw-r--r--   0        0        0      909 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/token_classification/zero_shot_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/tracing/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/tracing/decorators.py
+-rw-r--r--   0        0        0     1597 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/tracing/delegate.py
+-rw-r--r--   0        0        0     4370 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/tracing/langfuse.py
+-rw-r--r--   0        0        0     2267 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/tracing/logging.py
+-rw-r--r--   0        0        0     1097 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/tracing/tracer.py
+-rw-r--r--   0        0        0      876 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/tracing/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/translation/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-11 13:51:07.586444 bpm_ai_core-2.3.1/bpm_ai_core/translation/amazon_translate.py
+-rw-r--r--   0        0        0     1572 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/translation/azure_translation.py
+-rw-r--r--   0        0        0      475 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/translation/nmt.py
+-rw-r--r--   0        0        0        0 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/audio.py
+-rw-r--r--   0        0        0     1836 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/file.py
+-rw-r--r--   0        0        0     5233 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/image.py
+-rw-r--r--   0        0        0     1670 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/json_schema.py
+-rw-r--r--   0        0        0    21191 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/linguistics.py
+-rw-r--r--   0        0        0     1130 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/markdown.py
+-rw-r--r--   0        0        0     5280 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/remote_object.py
+-rw-r--r--   0        0        0     2596 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/storage.py
+-rw-r--r--   0        0        0      675 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/bpm_ai_core/util/xml_convert.py
+-rw-r--r--   0        0        0     1014 2024-04-11 13:51:07.590444 bpm_ai_core-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.3.1/PKG-INFO
```

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/classification/zero_shot_classifier.py` & `bpm_ai_core-2.3.1/bpm_ai_core/classification/zero_shot_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/__init__.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/anthropic_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,32 +93,32 @@
     async def _run_completion(self, messages: List[ChatMessage], stop: list[str] = None, current_try: int = None) -> Message:
         Tracing.tracers().start_llm_trace(self, messages, current_try, None)
         completion = await self.client.messages.create(
             max_tokens=4096,
             model=self.model,
             temperature=self.temperature,
             system=messages.pop(0).content if (messages and messages[0].role == "system") else "",
-            messages=messages_to_anthropic_dicts(messages),
+            messages=await messages_to_anthropic_dicts(messages),
             stop_sequences=stop
         )
         Tracing.tracers().end_llm_trace(completion.content[0].text)
         return completion
 
     async def _run_tool_completion(self, messages: list[ChatMessage], tools: list[Tool] = None, current_try: int = None) -> AssistantMessage:
         anthropic_tools = [json_schema_to_anthropic_tool(f.name, f.description, f.args_schema) for f in tools] if tools else []
         Tracing.tracers().start_llm_trace(self, messages, current_try, anthropic_tools)
         completion = await self.client.beta.tools.messages.create(
             max_tokens=4096,
             model=self.model,
             temperature=self.temperature,
             system=messages.pop(0).content if (messages and messages[0].role == "system") else "",
-            messages=messages_to_anthropic_dicts(messages),
+            messages=await messages_to_anthropic_dicts(messages),
             tools=anthropic_tools
         )
-        Tracing.tracers().end_llm_trace(completion.content[0].text)
+        Tracing.tracers().end_llm_trace(completion.content)
         return self._tool_calls_to_tool_message(completion, tools)
 
     @staticmethod
     def _tool_calls_to_tool_message(message: ToolsBetaMessage, tools: List[Tool]) -> AssistantMessage:
         texts = [c.text for c in message.content if isinstance(c, TextBlock)]
         tool_uses = [c for c in message.content if isinstance(c, ToolUseBlock)]
         return AssistantMessage(
```

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/util.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/anthropic_chat/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import logging
 from typing import List, Any
 
 from PIL.Image import Image
 
+from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.llm.common.message import ChatMessage, ToolResultMessage, AssistantMessage
-from bpm_ai_core.util.image import base64_encode_image
+from bpm_ai_core.util.image import base64_encode_image, blob_as_images
 
 logger = logging.getLogger(__name__)
 
 
-def messages_to_anthropic_dicts(messages: List[ChatMessage]):
-    return [message_to_anthropic_dict(m) for m in messages]
+async def messages_to_anthropic_dicts(messages: List[ChatMessage]):
+    return [await message_to_anthropic_dict(m) for m in messages]
 
 
-def message_to_anthropic_dict(message: ChatMessage) -> dict:
+async def message_to_anthropic_dict(message: ChatMessage) -> dict:
     if isinstance(message, AssistantMessage) and message.has_tool_calls():
         return tool_calls_message_to_anthropic_dict(message)
     elif isinstance(message, ToolResultMessage):
         return tool_result_message_to_anthropic_dict(message)
     elif isinstance(message.content, str):
         content = message.content
     elif isinstance(message.content, list):
         content = []
         for e in message.content:
             if isinstance(e, str):
                 content.append(str_to_anthropic_text_dict(e))
-            elif isinstance(e, Image):
-                content.append(image_to_anthropic_image_dict(e))
+            elif isinstance(e, Blob) and (e.is_image() or e.is_pdf()):
+                images = await blob_as_images(e, accept_formats=["jpg", "png"])
+                for image in images:
+                    content.append(image_to_anthropic_image_dict(image))
             else:
                 raise ValueError(
-                    "Elements in ChatMessage.content must be of type str or PIL.Image."
+                    "Elements in ChatMessage.content must be str or image Blob"
                 )
     else:
         content = None
         logger.warning(
             "ChatMessage.content must be of type str or List[Union[str, PIL.Image]] if used for chat completions."
         )
     return {
```

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/common/blob.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/common/blob.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/common/llm.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/common/llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/common/message.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/common/message.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/common/tool.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/common/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/__init__.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/openai_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/openai_chat.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/openai_chat/openai_chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,16 +152,16 @@
         stop: list[str] = None,
         current_try: int = None
     ) -> ChatCompletion:
         args = {
             "model": self.model,
             "temperature": self.temperature,
             **({"seed": self.seed} if self.seed else {}),
-            "messages": messages_to_openai_dicts(messages),
-            "stop": stop or [],
+            "messages": await messages_to_openai_dicts(messages),
+            **({"stop": stop} if stop else {}),
             **({
                    "tool_choice": {
                        "type": "function",
                        "function": {"name": tools[0]["function"]["name"]}
                    } if (len(tools) == 1) else ("auto" if tools else "none"),
                    "tools": tools
                } if tools else {})
@@ -171,16 +171,16 @@
         Tracing.tracers().end_llm_trace(completion.choices[0].message)
         return completion
 
     @staticmethod
     def _output_schema_to_tool(output_schema: dict):
         output_schema = output_schema.copy()
         return Tool.create(
-            name=output_schema.pop("name") or "store_result",
-            description=output_schema.pop("description") or "Stores your result",
+            name=output_schema.pop("name", None) or "store_result",
+            description=output_schema.pop("description", None) or "Stores your result",
             args_schema=output_schema
         )
 
     @staticmethod
     def _openai_tool_calls_to_tool_message(message: OpenAIChatCompletionMessage, tools: List[Tool]) -> AssistantMessage:
         return AssistantMessage(
             name=", ".join([t.function.name for t in message.tool_calls]),
```

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/util.py` & `bpm_ai_core-2.3.1/bpm_ai_core/llm/openai_chat/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import List, Dict, Any
 
 from PIL.Image import Image
 
+from bpm_ai_core.llm.common.blob import Blob
 from bpm_ai_core.llm.common.message import ChatMessage, ToolResultMessage, AssistantMessage
-from bpm_ai_core.util.image import base64_encode_image
+from bpm_ai_core.util.image import base64_encode_image, blob_as_images
 
 logger = logging.getLogger(__name__)
 
 
 def get_openai_tool_call_dict(message: AssistantMessage):
     return {
         "tool_calls": [
@@ -21,19 +22,19 @@
                 }
             }
             for t in message.tool_calls
         ]
     }
 
 
-def messages_to_openai_dicts(messages: List[ChatMessage]):
-    return [message_to_openai_dict(m) for m in messages]
+async def messages_to_openai_dicts(messages: List[ChatMessage]):
+    return [await message_to_openai_dict(m) for m in messages]
 
 
-def message_to_openai_dict(message: ChatMessage) -> dict:
+async def message_to_openai_dict(message: ChatMessage) -> dict:
     if isinstance(message, AssistantMessage) and message.has_tool_calls():
         extra_dict = {
             **get_openai_tool_call_dict(message)
         }
     elif isinstance(message, ToolResultMessage):
         extra_dict = {
             "tool_call_id": message.id
@@ -44,19 +45,21 @@
     if isinstance(message.content, str):
         content = message.content
     elif isinstance(message.content, list):
         content = []
         for e in message.content:
             if isinstance(e, str):
                 content.append(str_to_openai_text_dict(e))
-            elif isinstance(e, Image):
-                content.append(image_to_openai_image_dict(e))
+            elif isinstance(e, Blob) and (e.is_image() or e.is_pdf()):
+                images = await blob_as_images(e, accept_formats=["jpg", "png"])
+                for image in images:
+                    content.append(image_to_openai_image_dict(image))
             else:
                 raise ValueError(
-                    "Elements in ChatMessage.content must be of type str or PIL.Image."
+                    "Elements in ChatMessage.content must be str or image Blob"
                 )
     else:
         content = None
         logger.warning(
             "ChatMessage.content must be of type str or List[Union[str, PIL.Image]] if used for chat completions."
         )
     return {
```

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/ocr/amazon_textract.py` & `bpm_ai_core-2.3.1/bpm_ai_core/ocr/amazon_textract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/ocr/azure_doc_intelligence.py` & `bpm_ai_core-2.3.1/bpm_ai_core/ocr/azure_doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/ocr/ocr.py` & `bpm_ai_core-2.3.1/bpm_ai_core/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/pos/pos_tagger.py` & `bpm_ai_core-2.3.1/bpm_ai_core/pos/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/prompt/prompt.py` & `bpm_ai_core-2.3.1/bpm_ai_core/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py` & `bpm_ai_core-2.3.1/bpm_ai_core/question_answering/amazon_textract_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py` & `bpm_ai_core-2.3.1/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/question_answering/question_answering.py` & `bpm_ai_core-2.3.1/bpm_ai_core/question_answering/question_answering.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/asr.py` & `bpm_ai_core-2.3.1/bpm_ai_core/speech_recognition/asr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/openai_whisper.py` & `bpm_ai_core-2.3.1/bpm_ai_core/speech_recognition/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/testing/fake_llm.py` & `bpm_ai_core-2.3.1/bpm_ai_core/testing/fake_llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py` & `bpm_ai_core-2.3.1/bpm_ai_core/token_classification/zero_shot_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/tracing/decorators.py` & `bpm_ai_core-2.3.1/bpm_ai_core/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/tracing/delegate.py` & `bpm_ai_core-2.3.1/bpm_ai_core/tracing/delegate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/tracing/langfuse.py` & `bpm_ai_core-2.3.1/bpm_ai_core/tracing/langfuse.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/tracing/logging.py` & `bpm_ai_core-2.3.1/bpm_ai_core/tracing/logging.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/tracing/tracer.py` & `bpm_ai_core-2.3.1/bpm_ai_core/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/tracing/tracing.py` & `bpm_ai_core-2.3.1/bpm_ai_core/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/translation/amazon_translate.py` & `bpm_ai_core-2.3.1/bpm_ai_core/translation/amazon_translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/translation/azure_translation.py` & `bpm_ai_core-2.3.1/bpm_ai_core/translation/azure_translation.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/audio.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/audio.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/file.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/file.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/image.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/image.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/json_schema.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/json_schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/linguistics.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/linguistics.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/markdown.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/markdown.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/remote_object.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/remote_object.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/storage.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/storage.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/bpm_ai_core/util/xml_convert.py` & `bpm_ai_core-2.3.1/bpm_ai_core/util/xml_convert.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.3.0/pyproject.toml` & `bpm_ai_core-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-core"
-version = "2.3.0"
+version = "2.3.1"
 description = "Core AI abstractions and helpers."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `bpm_ai_core-2.3.0/PKG-INFO` & `bpm_ai_core-2.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-core
-Version: 2.3.0
+Version: 2.3.1
 Summary: Core AI abstractions and helpers.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

