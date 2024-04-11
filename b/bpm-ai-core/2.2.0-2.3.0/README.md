# Comparing `tmp/bpm_ai_core-2.2.0.tar.gz` & `tmp/bpm_ai_core-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai_core-2.2.0.tar", max compression
+gzip compressed data, was "bpm_ai_core-2.3.0.tar", max compression
```

## Comparing `bpm_ai_core-2.2.0.tar` & `bpm_ai_core-2.3.0.tar`

### file list

```diff
@@ -1,68 +1,62 @@
--rw-r--r--   0        0        0       13 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/classification/__init__.py
--rw-r--r--   0        0        0     1187 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/classification/zero_shot_classifier.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/__init__.py
--rw-r--r--   0        0        0      862 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/__init__.py
--rw-r--r--   0        0        0      306 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/_constants.py
--rw-r--r--   0        0        0     6130 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
--rw-r--r--   0        0        0      226 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/tools/__init__.py
--rw-r--r--   0        0        0     1480 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/tools/base_tool.py
--rw-r--r--   0        0        0     1976 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/tools/messages_api_converters.py
--rw-r--r--   0        0        0     9833 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/tools/prompt_constructors.py
--rw-r--r--   0        0        0     1509 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/tools/tool.py
--rw-r--r--   0        0        0    17771 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/tools/tool_user.py
--rw-r--r--   0        0        0     2629 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/common/__init__.py
--rw-r--r--   0        0        0     6036 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/common/blob.py
--rw-r--r--   0        0        0     2445 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/common/llm.py
--rw-r--r--   0        0        0     2710 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/common/message.py
--rw-r--r--   0        0        0     2781 2024-04-02 14:31:06.952583 bpm_ai_core-2.2.0/bpm_ai_core/llm/common/tool.py
--rw-r--r--   0        0        0     1455 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/llm/openai_chat/__init__.py
--rw-r--r--   0        0        0      438 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/llm/openai_chat/_constants.py
--rw-r--r--   0        0        0     7710 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/llm/openai_chat/openai_chat.py
--rw-r--r--   0        0        0     2626 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/llm/openai_chat/util.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/ocr/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/ocr/amazon_textract.py
--rw-r--r--   0        0        0     2698 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/ocr/azure_doc_intelligence.py
--rw-r--r--   0        0        0     1220 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/ocr/ocr.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/pos/__init__.py
--rw-r--r--   0        0        0      590 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/pos/pos_tagger.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/prompt/__init__.py
--rw-r--r--   0        0        0      372 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/prompt/filters.py
--rw-r--r--   0        0        0     6259 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/question_answering/__init__.py
--rw-r--r--   0        0        0     2085 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
--rw-r--r--   0        0        0     3018 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
--rw-r--r--   0        0        0     1096 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/question_answering/question_answering.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/speech_recognition/__init__.py
--rw-r--r--   0        0        0      827 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/speech_recognition/asr.py
--rw-r--r--   0        0        0     1428 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/speech_recognition/openai_whisper.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/testing/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/testing/fake_llm.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/token_classification/__init__.py
--rw-r--r--   0        0        0      909 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/tracing/__init__.py
--rw-r--r--   0        0        0     2434 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/tracing/decorators.py
--rw-r--r--   0        0        0     1597 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/tracing/delegate.py
--rw-r--r--   0        0        0     4370 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/tracing/langfuse.py
--rw-r--r--   0        0        0     2267 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/tracing/logging.py
--rw-r--r--   0        0        0     1097 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/tracing/tracer.py
--rw-r--r--   0        0        0      876 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/tracing/tracing.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/translation/__init__.py
--rw-r--r--   0        0        0     1302 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/translation/amazon_translate.py
--rw-r--r--   0        0        0     1572 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/translation/azure_translation.py
--rw-r--r--   0        0        0      475 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/translation/nmt.py
--rw-r--r--   0        0        0        0 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/audio.py
--rw-r--r--   0        0        0     1836 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/file.py
--rw-r--r--   0        0        0     5233 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/image.py
--rw-r--r--   0        0        0     1670 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/json_schema.py
--rw-r--r--   0        0        0    21191 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/linguistics.py
--rw-r--r--   0        0        0     1130 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/markdown.py
--rw-r--r--   0        0        0     5280 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/remote_object.py
--rw-r--r--   0        0        0     2596 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/storage.py
--rw-r--r--   0        0        0      675 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/bpm_ai_core/util/xml_convert.py
--rw-r--r--   0        0        0     1014 2024-04-02 14:31:06.956583 bpm_ai_core-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/classification/__init__.py
+-rw-r--r--   0        0        0     1187 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/classification/zero_shot_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/_constants.py
+-rw-r--r--   0        0        0     7213 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py
+-rw-r--r--   0        0        0      226 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/output_schema.prompt
+-rw-r--r--   0        0        0     2872 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/__init__.py
+-rw-r--r--   0        0        0     6036 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/blob.py
+-rw-r--r--   0        0        0     2445 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/llm.py
+-rw-r--r--   0        0        0     2710 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/message.py
+-rw-r--r--   0        0        0     2781 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/common/tool.py
+-rw-r--r--   0        0        0     1455 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/_constants.py
+-rw-r--r--   0        0        0     7715 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/openai_chat.py
+-rw-r--r--   0        0        0     2626 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/util.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/ocr/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/ocr/amazon_textract.py
+-rw-r--r--   0        0        0     2698 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/ocr/azure_doc_intelligence.py
+-rw-r--r--   0        0        0     1220 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/ocr/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/pos/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/pos/pos_tagger.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/prompt/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/prompt/filters.py
+-rw-r--r--   0        0        0     6259 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/question_answering/__init__.py
+-rw-r--r--   0        0        0     2085 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py
+-rw-r--r--   0        0        0     3018 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py
+-rw-r--r--   0        0        0     1096 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/question_answering/question_answering.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/asr.py
+-rw-r--r--   0        0        0     1428 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/openai_whisper.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/testing/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/testing/fake_llm.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/token_classification/__init__.py
+-rw-r--r--   0        0        0      909 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/decorators.py
+-rw-r--r--   0        0        0     1597 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/delegate.py
+-rw-r--r--   0        0        0     4370 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/langfuse.py
+-rw-r--r--   0        0        0     2267 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/logging.py
+-rw-r--r--   0        0        0     1097 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/tracer.py
+-rw-r--r--   0        0        0      876 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/tracing/tracing.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/translation/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/translation/amazon_translate.py
+-rw-r--r--   0        0        0     1572 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/translation/azure_translation.py
+-rw-r--r--   0        0        0      475 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/translation/nmt.py
+-rw-r--r--   0        0        0        0 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/__init__.py
+-rw-r--r--   0        0        0     1154 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/audio.py
+-rw-r--r--   0        0        0     1836 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/file.py
+-rw-r--r--   0        0        0     5233 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/image.py
+-rw-r--r--   0        0        0     1670 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/json_schema.py
+-rw-r--r--   0        0        0    21191 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/linguistics.py
+-rw-r--r--   0        0        0     1130 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/markdown.py
+-rw-r--r--   0        0        0     5280 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/remote_object.py
+-rw-r--r--   0        0        0     2596 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/storage.py
+-rw-r--r--   0        0        0      675 2024-04-10 15:12:38.094810 bpm_ai_core-2.3.0/bpm_ai_core/util/xml_convert.py
+-rw-r--r--   0        0        0     1014 2024-04-10 15:12:38.098810 bpm_ai_core-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 bpm_ai_core-2.3.0/PKG-INFO
```

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/classification/zero_shot_classifier.py` & `bpm_ai_core-2.3.0/bpm_ai_core/classification/zero_shot_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/__init__.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/anthropic_chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import json
 import logging
 from typing import Dict, Any, Optional, List
 
+from typing_extensions import deprecated
+
 from bpm_ai_core.llm.anthropic_chat import get_anthropic_client
 from bpm_ai_core.llm.anthropic_chat._constants import DEFAULT_MODEL, DEFAULT_TEMPERATURE, \
     DEFAULT_MAX_RETRIES
-from bpm_ai_core.llm.anthropic_chat.tools.tool import AnthropicTool
-from bpm_ai_core.llm.anthropic_chat.tools.tool_user import ToolUser
-from bpm_ai_core.llm.anthropic_chat.util import messages_to_anthropic_dicts
+from bpm_ai_core.llm.anthropic_chat.util import messages_to_anthropic_dicts, json_schema_to_anthropic_tool
 from bpm_ai_core.llm.common.llm import LLM
 from bpm_ai_core.llm.common.message import ChatMessage, ToolCallMessage, AssistantMessage, SystemMessage
 from bpm_ai_core.llm.common.tool import Tool
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.tracing.tracing import Tracing
 from bpm_ai_core.util.json_schema import expand_simplified_json_schema
 
 logger = logging.getLogger(__name__)
 
 try:
     from anthropic import AsyncAnthropic, RateLimitError, InternalServerError, APIConnectionError
-    from anthropic.types import Message
+    from anthropic.types import Message, TextBlock
+    from anthropic.types.beta.tools import ToolUseBlock, ToolsBetaMessage
 
     has_anthropic = True
 except ImportError:
     has_anthropic = False
 
 
 class ChatAnthropic(LLM):
@@ -73,19 +74,22 @@
         messages: List[ChatMessage],
         output_schema: Optional[Dict[str, Any]] = None,
         tools: Optional[List[Tool]] = None,
         stop: list[str] = None,
         current_try: int = None
     ) -> AssistantMessage:
         if output_schema:
-            result_dict = await self._run_output_schema_completion(messages, output_schema, current_try)
-            return AssistantMessage(content=result_dict)
+            tools = [self._output_schema_to_tool(output_schema)]
+            message = await self._run_tool_completion(messages, tools, current_try)
+            if message.has_tool_calls():
+                return AssistantMessage(content=message.tool_calls[0].payload)
+            else:
+                return AssistantMessage(content=None)
         elif tools:
-            result_dict = await self._run_tool_completion(messages, tools)
-            return self._tool_calls_to_tool_message(result_dict, tools)
+            return await self._run_tool_completion(messages, tools, current_try)
         else:
             completion = await self._run_completion(messages, stop, current_try)
             return AssistantMessage(content=completion.content[0].text.strip())
 
     async def _run_completion(self, messages: List[ChatMessage], stop: list[str] = None, current_try: int = None) -> Message:
         Tracing.tracers().start_llm_trace(self, messages, current_try, None)
         completion = await self.client.messages.create(
@@ -95,25 +99,56 @@
             system=messages.pop(0).content if (messages and messages[0].role == "system") else "",
             messages=messages_to_anthropic_dicts(messages),
             stop_sequences=stop
         )
         Tracing.tracers().end_llm_trace(completion.content[0].text)
         return completion
 
-    async def _run_tool_completion(self, messages: list[ChatMessage], tools: list[Tool] = None) -> dict:
-        tool_user = ToolUser(tools=[
-            AnthropicTool(name=tool.name, description=tool.description, args_schema=tool.args_schema)
-            for tool in tools
-        ])
-        return await tool_user.use_tools(
+    async def _run_tool_completion(self, messages: list[ChatMessage], tools: list[Tool] = None, current_try: int = None) -> AssistantMessage:
+        anthropic_tools = [json_schema_to_anthropic_tool(f.name, f.description, f.args_schema) for f in tools] if tools else []
+        Tracing.tracers().start_llm_trace(self, messages, current_try, anthropic_tools)
+        completion = await self.client.beta.tools.messages.create(
+            max_tokens=4096,
+            model=self.model,
+            temperature=self.temperature,
+            system=messages.pop(0).content if (messages and messages[0].role == "system") else "",
             messages=messages_to_anthropic_dicts(messages),
-            execution_mode='manual',
-            verbose=0
+            tools=anthropic_tools
         )
+        Tracing.tracers().end_llm_trace(completion.content[0].text)
+        return self._tool_calls_to_tool_message(completion, tools)
 
+    @staticmethod
+    def _tool_calls_to_tool_message(message: ToolsBetaMessage, tools: List[Tool]) -> AssistantMessage:
+        texts = [c.text for c in message.content if isinstance(c, TextBlock)]
+        tool_uses = [c for c in message.content if isinstance(c, ToolUseBlock)]
+        return AssistantMessage(
+            name=", ".join([t.name for t in tool_uses]),
+            content="\n".join(texts),
+            tool_calls=[
+                ToolCallMessage(
+                    id=t.id,
+                    name=t.name,
+                    payload=t.input,
+                    tool=next((item for item in tools if item.name == t.name), None)
+                )
+                for t in tool_uses
+            ]
+        )
+
+    @staticmethod
+    def _output_schema_to_tool(output_schema: dict):
+        output_schema = output_schema.copy()
+        return Tool.create(
+            name=output_schema.pop("name", None) or "record_result",
+            description=output_schema.pop("description", None) or "Record your result into well-structured JSON.",
+            args_schema=output_schema
+        )
+
+    @deprecated("Using a tool for now but still need to evaluate which is better")
     async def _run_output_schema_completion(self, messages: list[ChatMessage], output_schema: dict[str, Any], current_try: int = None) -> dict:
         output_schema = expand_simplified_json_schema(output_schema)
         output_prompt = Prompt.from_file(
             "output_schema",
             output_schema=json.dumps(output_schema, indent=2)
         ).format()[0].content
         if messages[0].role == "system":
@@ -127,30 +162,14 @@
         completion = await self._run_completion(messages, stop=["</result>"], current_try=current_try)
         try:
             json_object = json.loads(completion.content[0].text.strip())
         except ValueError:
             json_object = None
         return json_object
 
-    @staticmethod
-    def _tool_calls_to_tool_message(result_dict: dict, tools: List[Tool]) -> AssistantMessage:
-        return AssistantMessage(
-            name=", ".join([t['tool_name'] for t in result_dict['tool_inputs']]),
-            content=result_dict['content'],
-            tool_calls=[
-                ToolCallMessage(
-                    id=t['tool_name'],
-                    name=t['tool_name'],
-                    payload=t['tool_arguments'],
-                    tool=next((item for item in tools if item.name == t['tool_name']), None)
-                )
-                for t in result_dict['tool_inputs']
-            ]
-        )
-
     def supports_images(self) -> bool:
         return True
 
     def supports_video(self) -> bool:
         return False
 
     def supports_audio(self) -> bool:
```

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/anthropic_chat/util.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/anthropic_chat/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import List
+from typing import List, Any
 
 from PIL.Image import Image
 
 from bpm_ai_core.llm.common.message import ChatMessage, ToolResultMessage, AssistantMessage
 from bpm_ai_core.util.image import base64_encode_image
 
 logger = logging.getLogger(__name__)
@@ -41,36 +41,32 @@
         **({"content": content} if content else {}),
         **({"name": message.name} if message.name else {})
     }
 
 
 def tool_calls_message_to_anthropic_dict(message: AssistantMessage) -> dict:
     return {
-        "role": "tool_inputs",
-        "content": message.content,
-        "tool_inputs": [
-            {
-                "tool_name": call.name,
-                "tool_arguments": call.payload_dict()
-            }
-            for call in message.tool_calls
-        ]
+        "role": "assistant",
+        "content": ([{"type": "text", "text": message.content}] if message.content else [])
+                 + [{"type": "tool_use", "id": call.id, "name": call.name, "input": call.payload}
+                    for call in message.tool_calls]
     }
 
 
-def tool_result_message_to_anthropic_dict(message: ToolResultMessage) -> dict:
+def tool_result_message_to_anthropic_dict(message: ToolResultMessage, is_error: bool = False) -> dict:
     return {
-        "role": "tool_outputs",
-        "tool_outputs": [
-            {
-                "tool_name": message.id,
-                "tool_result": message.content
-            }
-        ],
-        "tool_error": None
+      "role": "user",
+      "content": [
+        {
+          "type": "tool_result",
+          "tool_use_id": message.id,
+          "content": message.content,
+          **({"is_error": True} if is_error else {})
+        }
+      ]
     }
 
 
 def image_to_anthropic_image_dict(image: Image) -> dict:
     return {
         "type": "image",
         "source": {
@@ -81,8 +77,16 @@
     }
 
 
 def str_to_anthropic_text_dict(text: str) -> dict:
     return {
         "type": "text",
         "text": text
+    }
+
+
+def json_schema_to_anthropic_tool(name: str, desc: str, schema: dict[str, Any]) -> dict:
+    return {
+        "name": name,
+        "description": desc,
+        "input_schema": schema
     }
```

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/common/blob.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/common/blob.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/common/llm.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/common/llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/common/message.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/common/message.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/common/tool.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/common/tool.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/openai_chat/__init__.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/openai_chat/openai_chat.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/openai_chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         try:
             json_object = json.loads(message.tool_calls[0].function.arguments)
         except ValueError as e:
             json_object = None
         return json_object
 
     def supports_images(self) -> bool:
-        return "vision" in self.model
+        return self.model == "gpt-4-turbo"
 
     def supports_video(self) -> bool:
         return False
 
     def supports_audio(self) -> bool:
         return False
```

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/llm/openai_chat/util.py` & `bpm_ai_core-2.3.0/bpm_ai_core/llm/openai_chat/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/ocr/amazon_textract.py` & `bpm_ai_core-2.3.0/bpm_ai_core/ocr/amazon_textract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/ocr/azure_doc_intelligence.py` & `bpm_ai_core-2.3.0/bpm_ai_core/ocr/azure_doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/ocr/ocr.py` & `bpm_ai_core-2.3.0/bpm_ai_core/ocr/ocr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/pos/pos_tagger.py` & `bpm_ai_core-2.3.0/bpm_ai_core/pos/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/prompt/prompt.py` & `bpm_ai_core-2.3.0/bpm_ai_core/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py` & `bpm_ai_core-2.3.0/bpm_ai_core/question_answering/amazon_textract_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py` & `bpm_ai_core-2.3.0/bpm_ai_core/question_answering/azure_doc_intelligence_docvqa.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/question_answering/question_answering.py` & `bpm_ai_core-2.3.0/bpm_ai_core/question_answering/question_answering.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/speech_recognition/asr.py` & `bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/asr.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/speech_recognition/openai_whisper.py` & `bpm_ai_core-2.3.0/bpm_ai_core/speech_recognition/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/testing/fake_llm.py` & `bpm_ai_core-2.3.0/bpm_ai_core/testing/fake_llm.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py` & `bpm_ai_core-2.3.0/bpm_ai_core/token_classification/zero_shot_token_classifier.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/tracing/decorators.py` & `bpm_ai_core-2.3.0/bpm_ai_core/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/tracing/delegate.py` & `bpm_ai_core-2.3.0/bpm_ai_core/tracing/delegate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/tracing/langfuse.py` & `bpm_ai_core-2.3.0/bpm_ai_core/tracing/langfuse.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/tracing/logging.py` & `bpm_ai_core-2.3.0/bpm_ai_core/tracing/logging.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/tracing/tracer.py` & `bpm_ai_core-2.3.0/bpm_ai_core/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/tracing/tracing.py` & `bpm_ai_core-2.3.0/bpm_ai_core/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/translation/amazon_translate.py` & `bpm_ai_core-2.3.0/bpm_ai_core/translation/amazon_translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/translation/azure_translation.py` & `bpm_ai_core-2.3.0/bpm_ai_core/translation/azure_translation.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/audio.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/audio.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/file.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/file.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/image.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/image.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/json_schema.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/json_schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/linguistics.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/linguistics.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/markdown.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/markdown.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/remote_object.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/remote_object.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/storage.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/storage.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/bpm_ai_core/util/xml_convert.py` & `bpm_ai_core-2.3.0/bpm_ai_core/util/xml_convert.py`

 * *Files identical despite different names*

### Comparing `bpm_ai_core-2.2.0/pyproject.toml` & `bpm_ai_core-2.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai-core"
-version = "2.2.0"
+version = "2.3.0"
 description = "Core AI abstractions and helpers."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
 
@@ -23,15 +23,15 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.2"
 pytest-asyncio = "^0.23.5"
 pytest-dotenv = "^0.5.2"
 
 [tool.poetry.group.dev.dependencies]
 openai = "^1.11.0"
-anthropic = "^0.18.1"
+anthropic = "^0.23.1"
 mistralai = "^0.1.3"
 langfuse = "^2.7.6"
 pyro5 = "^5.15"
 amazon-textract-prettyprinter = "^0.1.9"
 aiobotocore = "^2.12.1"
 azure-storage-blob = "^12.19.1"
 azure-ai-translation-text = "^1.0.0b1"
```

### Comparing `bpm_ai_core-2.2.0/PKG-INFO` & `bpm_ai_core-2.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai-core
-Version: 2.2.0
+Version: 2.3.0
 Summary: Core AI abstractions and helpers.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

