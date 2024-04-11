# Comparing `tmp/brevia-0.0.8.tar.gz` & `tmp/brevia-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brevia-0.0.8.tar", max compression
+gzip compressed data, was "brevia-0.0.9.tar", max compression
```

## Comparing `brevia-0.0.8.tar` & `brevia-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1066 2023-11-28 16:39:55.471257 brevia-0.0.8/LICENSE
--rw-r--r--   0        0        0     8086 2023-11-28 16:39:55.471257 brevia-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/__init__.py
--rw-r--r--   0        0        0       38 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/alembic/README
--rw-r--r--   0        0        0      392 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/alembic/__init__.py
--rw-r--r--   0        0        0     2834 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/alembic/env.py
--rw-r--r--   0        0        0      510 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/alembic/script.py.mako
--rw-r--r--   0        0        0      918 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/alembic/versions/1d927e0cbc61_locked_until_column.py
--rw-r--r--   0        0        0     2408 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/alembic/versions/1eab976dea29_initial_schema.py
--rw-r--r--   0        0        0     1233 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/alembic/versions/be67c72a4e5a_async_jobs_table.py
--rw-r--r--   0        0        0     6704 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/analysis.py
--rw-r--r--   0        0        0     5616 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/async_jobs.py
--rw-r--r--   0        0        0     7544 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/callback.py
--rw-r--r--   0        0        0     6520 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/chat_history.py
--rw-r--r--   0        0        0     2642 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/collections.py
--rw-r--r--   0        0        0     3833 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/commands.py
--rw-r--r--   0        0        0     2274 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/connection.py
--rw-r--r--   0        0        0     2818 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/dependencies.py
--rw-r--r--   0        0        0        0 2023-11-28 16:39:55.471257 brevia-0.0.8/brevia/extensions/__init__.py
--rw-r--r--   0        0        0     3272 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/index.py
--rw-r--r--   0        0        0     1038 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/language.py
--rw-r--r--   0        0        0     4243 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/load_file.py
--rw-r--r--   0        0        0     3064 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/models.py
--rw-r--r--   0        0        0    55577 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/postman/Brevia API.postman_collection.json
--rw-r--r--   0        0        0     1066 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/postman/Brevia API.postman_environment.json
--rw-r--r--   0        0        0      426 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/prompts/qa/default.condense.yaml
--rw-r--r--   0        0        0       85 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/prompts/qa/default.human.yaml
--rw-r--r--   0        0        0     8053 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/query.py
--rw-r--r--   0        0        0        0 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/__init__.py
--rw-r--r--   0        0        0     7063 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/analyze_router.py
--rw-r--r--   0        0        0      752 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/app_routers.py
--rw-r--r--   0        0        0     1180 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/audio_router.py
--rw-r--r--   0        0        0      682 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/chat_history_router.py
--rw-r--r--   0        0        0     2006 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/collections_router.py
--rw-r--r--   0        0        0     3708 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/index_router.py
--rw-r--r--   0        0        0      559 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/jobs_router.py
--rw-r--r--   0        0        0     6337 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/qa_router.py
--rw-r--r--   0        0        0      612 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/routers/status_router.py
--rw-r--r--   0        0        0     3059 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/services.py
--rw-r--r--   0        0        0     1263 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/tokens.py
--rw-r--r--   0        0        0        0 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/utilities/__init__.py
--rw-r--r--   0        0        0     2702 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/utilities/collections_io.py
--rw-r--r--   0        0        0     1116 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/utilities/files_import.py
--rw-r--r--   0        0        0     1704 2023-11-28 16:39:55.475257 brevia-0.0.8/brevia/utilities/run_service.py
--rw-r--r--   0        0        0     1762 2023-11-28 16:39:55.891255 brevia-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     9457 1970-01-01 00:00:00.000000 brevia-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-11-30 15:23:10.306076 brevia-0.0.9/LICENSE
+-rw-r--r--   0        0        0     8086 2023-11-30 15:23:10.306076 brevia-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/__init__.py
+-rw-r--r--   0        0        0       38 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/alembic/README
+-rw-r--r--   0        0        0      392 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/alembic/__init__.py
+-rw-r--r--   0        0        0     2788 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/alembic/env.py
+-rw-r--r--   0        0        0      510 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/alembic/script.py.mako
+-rw-r--r--   0        0        0      918 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/alembic/versions/1d927e0cbc61_locked_until_column.py
+-rw-r--r--   0        0        0     2408 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/alembic/versions/1eab976dea29_initial_schema.py
+-rw-r--r--   0        0        0     1233 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/alembic/versions/be67c72a4e5a_async_jobs_table.py
+-rw-r--r--   0        0        0     6477 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/analysis.py
+-rw-r--r--   0        0        0     5616 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/async_jobs.py
+-rw-r--r--   0        0        0     7544 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/callback.py
+-rw-r--r--   0        0        0     6518 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/chat_history.py
+-rw-r--r--   0        0        0     2642 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/collections.py
+-rw-r--r--   0        0        0     3658 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/commands.py
+-rw-r--r--   0        0        0     2196 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/connection.py
+-rw-r--r--   0        0        0     2836 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/dependencies.py
+-rw-r--r--   0        0        0        0 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/extensions/__init__.py
+-rw-r--r--   0        0        0     3308 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/index.py
+-rw-r--r--   0        0        0     1050 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/language.py
+-rw-r--r--   0        0        0     4243 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/load_file.py
+-rw-r--r--   0        0        0     3552 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/models.py
+-rw-r--r--   0        0        0    55577 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/postman/Brevia API.postman_collection.json
+-rw-r--r--   0        0        0     1066 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/postman/Brevia API.postman_environment.json
+-rw-r--r--   0        0        0      426 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/prompts/qa/default.condense.yaml
+-rw-r--r--   0        0        0       85 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/prompts/qa/default.human.yaml
+-rw-r--r--   0        0        0     7741 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/query.py
+-rw-r--r--   0        0        0        0 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/__init__.py
+-rw-r--r--   0        0        0     7069 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/analyze_router.py
+-rw-r--r--   0        0        0      752 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/app_routers.py
+-rw-r--r--   0        0        0     1198 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/audio_router.py
+-rw-r--r--   0        0        0      682 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/chat_history_router.py
+-rw-r--r--   0        0        0     2006 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/collections_router.py
+-rw-r--r--   0        0        0     3708 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/index_router.py
+-rw-r--r--   0        0        0      559 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/jobs_router.py
+-rw-r--r--   0        0        0     6343 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/qa_router.py
+-rw-r--r--   0        0        0      612 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/routers/status_router.py
+-rw-r--r--   0        0        0     3059 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/services.py
+-rw-r--r--   0        0        0     2673 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/settings.py
+-rw-r--r--   0        0        0     1299 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/tokens.py
+-rw-r--r--   0        0        0        0 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/utilities/__init__.py
+-rw-r--r--   0        0        0     2702 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/utilities/collections_io.py
+-rw-r--r--   0        0        0     1116 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/utilities/files_import.py
+-rw-r--r--   0        0        0     1704 2023-11-30 15:23:10.306076 brevia-0.0.9/brevia/utilities/run_service.py
+-rw-r--r--   0        0        0     1794 2023-11-30 15:23:10.710074 brevia-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9509 1970-01-01 00:00:00.000000 brevia-0.0.9/PKG-INFO
```

### Comparing `brevia-0.0.8/LICENSE` & `brevia-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/README.md` & `brevia-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/alembic/env.py` & `brevia-0.0.9/brevia/alembic/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from logging.config import fileConfig
-from dotenv import load_dotenv
 from sqlalchemy import engine_from_config
 from sqlalchemy import pool
 from alembic import context
 from sqlalchemy_utils import database_exists, create_database
 from brevia.connection import connection_string
 
-load_dotenv()
-
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
 
 # we need to double escape "%" into "%%"
 # because alembic uses configparser (that requires an additional escape of %)
 # see https://github.com/sqlalchemy/alembic/issues/700
```

### Comparing `brevia-0.0.8/brevia/alembic/versions/1d927e0cbc61_locked_until_column.py` & `brevia-0.0.9/brevia/alembic/versions/1d927e0cbc61_locked_until_column.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/alembic/versions/1eab976dea29_initial_schema.py` & `brevia-0.0.9/brevia/alembic/versions/1eab976dea29_initial_schema.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/alembic/versions/be67c72a4e5a_async_jobs_table.py` & `brevia-0.0.9/brevia/alembic/versions/be67c72a4e5a_async_jobs_table.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/analysis.py` & `brevia-0.0.9/brevia/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Functions to perform summarization & document analysis"""
-from os import environ
 from langchain.docstore.document import Document
 from langchain.chains.summarize import load_summarize_chain
 from langchain.text_splitter import TokenTextSplitter
 from langchain.chat_models.base import BaseChatModel
 from langchain.prompts.loading import load_prompt_from_config
 from brevia.callback import LoggingCallbackHandler
 from brevia.models import load_chatmodel
+from brevia.settings import get_settings
 
 
 def load_stuff_prompts(prompts: dict | None) -> dict:
     """Load custom prompts for the 'stuff' summarization chain.
     Summarization chain is the simplest one and have only one prompt
 
     Args:
@@ -94,23 +94,18 @@
     This function returns a language model for use in the summarization process.
     The model's configuration is defined by environment variables.
 
     Returns:
         BaseChatModel: A language model suitable for text summarization.
 
     """
-    logging_handler = LoggingCallbackHandler()
+    model = get_settings().summarize_llm.copy()
+    model['callbacks'] = [LoggingCallbackHandler()]
 
-    return load_chatmodel({
-        '_type': 'openai-chat',
-        'model_name': environ.get('SUMM_COMPLETIONS_MODEL'),
-        'temperature': float(environ.get('SUMM_TEMPERATURE', 0)),
-        'max_tokens': int(environ.get('SUMM_MAX_TOKENS', 2000)),
-        'callbacks': [logging_handler],
-    })
+    return load_chatmodel(model)
 
 
 def summarize(
     text: str,
     chain_type: str | None = None,
     initial_prompt: dict | None = None,
     iteration_prompt: dict | None = None
@@ -137,38 +132,38 @@
     """
 
     summarize_chain_map = {
         'stuff': load_stuff_prompts,
         'map_reduce': load_map_prompts,
         'refine': load_refine_prompts
     }
-
-    chain_type = chain_type or environ.get('SUMM_DEFAULT_CHAIN', 'stuff')
+    settings = get_settings()
+    chain_type = chain_type or settings.summ_default_chain
     if chain_type not in summarize_chain_map:
         raise ValueError(
             f"Got unsupported chain type: {chain_type}. "
             f"Should be one of {list(summarize_chain_map.keys())}"
         )
 
     logging_handler = LoggingCallbackHandler()
     kwargs = {
         'llm': get_summarize_llm(),
         'chain_type': chain_type,
-        'verbose': environ.get('VERBOSE_MODE', False),
+        'verbose': settings.verbose_mode,
         'callbacks': [logging_handler],
     }
 
     # load chain_type specific prompts:
     prompts_args = summarize_chain_map[chain_type]({
         'initial_prompt': initial_prompt,
         'iteration_prompt': iteration_prompt
     })
 
     chain = load_summarize_chain(**kwargs, **prompts_args)
     text_splitter = TokenTextSplitter(
-        chunk_size=int(environ.get("SUMM_TOKEN_SPLITTER", 4000)),
-        chunk_overlap=int(environ.get("SUMM_TOKEN_OVERLAP", 500))
+        chunk_size=settings.summ_token_splitter,
+        chunk_overlap=settings.summ_token_overlap
     )
     texts = text_splitter.split_text(text)
     docs = [Document(page_content=t) for t in texts]
 
     return chain.run(**{'input_documents': docs})
```

### Comparing `brevia-0.0.8/brevia/async_jobs.py` & `brevia-0.0.9/brevia/async_jobs.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/callback.py` & `brevia-0.0.9/brevia/callback.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/chat_history.py` & `brevia-0.0.9/brevia/chat_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Chat history table & utilities"""
 from typing import List
 import uuid
 import logging
 from datetime import datetime
-from os import environ
 from langchain.vectorstores.pgvector import BaseModel
 from langchain.vectorstores._pgvector_data_models import CollectionStore
 import sqlalchemy
 from sqlalchemy.dialects.postgresql import JSON, UUID
 from sqlalchemy.orm import Mapped, Query, Session
 from sqlalchemy.sql.expression import BinaryExpression
 from brevia.connection import db_connection
 from brevia.models import load_embeddings
+from brevia.settings import get_settings
 
 
 class ChatHistoryStore(BaseModel):
     # pylint: disable=too-few-public-methods
     """ Chat History table """
     __tablename__ = "chat_history"
 
@@ -39,15 +39,15 @@
 
 
 def history(chat_history: list, session: str = None):
     """ Load chat history from input or from DB """
     if len(chat_history) > 0:
         return [(x["query"], x["answer"]) for x in chat_history]
 
-    if not is_valid_uuid(session) or bool(environ.get('QA_NO_CHAT_HISTORY')):
+    if not is_valid_uuid(session) or get_settings().qa_no_chat_history:
         return []
 
     return history_from_db(session)
 
 
 def is_related(chat_history: list, question: str):
     """
@@ -59,15 +59,15 @@
     embeddings = load_embeddings()
     q_e = embeddings.embed_query(question)
     h_e = embeddings.embed_query(
         ''.join([sentence for tuple in chat_history for sentence in tuple])
     )
     sim = dot_product(q_e, h_e)
     logging.getLogger(__name__).info("similarity: %s", sim)
-    threshold = float(environ.get('QA_FOLLOWUP_SIM_THRESHOLD', False))
+    threshold = get_settings().qa_followup_sim_threshold
     return sim >= threshold
 
 
 def dot_product(v1_list, v2_list):
     """
     Calculate the scalar product between two vectors (similarity).
     """
```

### Comparing `brevia-0.0.8/brevia/collections.py` & `brevia-0.0.9/brevia/collections.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/commands.py` & `brevia-0.0.9/brevia/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 """Utility commands for applications"""
 import json
 import sys
 from os import getcwd, path
 from logging import config
 import click
-from dotenv import load_dotenv
 from brevia.alembic import current, upgrade, downgrade
 from brevia.utilities import files_import, run_service, collections_io
 from brevia.tokens import create_token
 
 
 @click.command()
 @click.option("-v", "--verbose", is_flag=True, default=False, help="Verbose mode")
 def db_current_cmd(verbose):
     """Display current database revision"""
-    load_dotenv()
     current(verbose)
 
 
 @click.command()
 @click.option("-r", "--revision", default="head", help="Revision target")
 def db_upgrade_cmd(revision):
     """Upgrade to a later database revision"""
-    load_dotenv()
     upgrade(revision)
 
 
 @click.command()
 @click.option("-r", "--revision", required=True, help="Revision target")
 def db_downgrade_cmd(revision):
     """Revert to a previous database revision"""
-    load_dotenv()
     downgrade(revision)
 
 
 @click.command()
 @click.option("-f", "--file-path", required=True, help="File or folder path")
 @click.option("-c", "--collection", required=True, help="Collection name")
 @click.option("-o", "--options", required=False, help="Loader options in JSON format")
 def import_file(file_path: str, collection: str, options: str = ''):
     """Add file or folder content to collection"""
-    load_dotenv()
     # pass loader options via JSON string
     kwargs = {} if not options else json.loads(options)
     num = files_import.index_file_folder(
         file_path=file_path,
         collection=collection,
         **kwargs
     )
@@ -70,15 +65,14 @@
     "-f",
     "--file-path",
     default=f'{getcwd()}/test_service.yml',
     help="yaml file path"
 )
 def run_test_service(num: int = 1, file_path: str = f'{getcwd()}/test_service.yml'):
     """Service test"""
-    load_dotenv()
     # allow module import from current working directory
     sys.path.append(getcwd())
     # initialize logging from optional log.ini
     log_ini_path = f'{getcwd()}/log.ini'
     if path.exists(log_ini_path):
         config.fileConfig(log_ini_path)
 
@@ -91,15 +85,14 @@
     "-f",
     "--folder-path",
     required=True,
     help="Folder output path"
 )
 def export_collection(folder_path: str, collection: str):
     """Export a collection to CSV postgres files."""
-    load_dotenv()
     collections_io.export_collection_data(
         folder_path=folder_path,
         collection=collection
     )
 
 
 @click.command()
@@ -108,22 +101,20 @@
     "-f",
     "--folder-path",
     required=True,
     help="Folder input path"
 )
 def import_collection(folder_path: str, collection: str):
     """Import a collection from a CSV postgres files."""
-    load_dotenv()
     collections_io.import_collection_data(
         folder_path=folder_path,
         collection=collection
     )
 
 
 @click.command()
 @click.option("-u", "--user", default="brevia", help="Token user name")
 @click.option("-d", "--duration", default=60, help="Token duration in minutes")
 def create_access_token(user: str, duration: int):
     """Create an access token """
-    load_dotenv()
     token = create_token(user=user, duration=duration)
     print(token)
```

### Comparing `brevia-0.0.8/brevia/dependencies.py` & `brevia-0.0.9/brevia/dependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """FastAPI endpoints dependencies"""
-from os import environ
 import shutil
 from pathlib import Path
 import tempfile
 from jose import JWTError
 from langchain.vectorstores._pgvector_data_models import CollectionStore
 from fastapi import HTTPException, status, Header, Depends, UploadFile
 from fastapi.security import OAuth2PasswordBearer
 from brevia import collections, tokens
+from brevia.settings import get_settings
 
 oauth2_scheme = OAuth2PasswordBearer(tokenUrl='token')  # use token authentication
 
 
 def get_dependencies(json_content_type: bool = True) -> list[Depends]:
     """Get endpoint dependencies"""
     deps = []
     # add authorization header check only if access tokens are defined
-    if environ.get('TOKENS_SECRET'):
+    if get_settings().tokens_secret:
         deps.append(Depends(token_auth))
 
     if json_content_type:
         deps.append(Depends(application_json))
 
     return deps
```

### Comparing `brevia-0.0.8/brevia/index.py` & `brevia-0.0.9/brevia/index.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Index document with embeddings in vector database."""
-import os
+from os import path
 from langchain.docstore.document import Document
 from langchain.text_splitter import NLTKTextSplitter
 from langchain.vectorstores.pgvector import PGVector
 from langchain.vectorstores._pgvector_data_models import EmbeddingStore
 from sqlalchemy.orm import Session
 from brevia import connection, load_file
 from brevia.models import load_embeddings
+from brevia.settings import get_settings
 
 
 def init_index():
     """Init index data"""
     try:
         import nltk  # pylint: disable=import-outside-toplevel
         nltk.download('punkt')
@@ -30,24 +31,24 @@
     page_from: int = None,  # from page, used in PDF
     page_to: int = None,  # to page, used in PDF
 ) -> int:
     """
     Load document from PDF file, add document to collection index
     and return number of splitted text chunks
     """
-    if not os.path.isfile(file_path):
+    if not path.isfile(file_path):
         raise FileNotFoundError(file_path)
 
     text = load_file.read_pdf_file(
         file_path=file_path,
         page_from=page_from,
         page_to=page_to,
     )
     if metadata is None:
-        metadata = {'source': os.path.basename(file_path)}
+        metadata = {'source': path.basename(file_path)}
 
     return add_document(
         document=Document(
             page_content=text,
             metadata=metadata,
         ),
         collection_name=collection_name,
@@ -57,18 +58,19 @@
 
 def add_document(
     document: Document,
     collection_name: str,
     document_id: str = None,
 ) -> int:
     """ Add document to index and return number of splitted text chunks"""
+    settings = get_settings()
     text_splitter = NLTKTextSplitter(
         separator="\n",
-        chunk_size=int(os.environ.get('TEXT_CHUNK_SIZE', 2000)),
-        chunk_overlap=int(os.environ.get('TEXT_CHUNK_OVERLAP', 200))
+        chunk_size=settings.text_chunk_size,
+        chunk_overlap=settings.text_chunk_overlap
     )
     texts = text_splitter.split_documents([document])
 
     PGVector.from_documents(
         embedding=load_embeddings(),
         documents=texts,
         collection_name=collection_name,
```

### Comparing `brevia-0.0.8/brevia/language.py` & `brevia-0.0.9/brevia/language.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Language detection utilities"""
-from os import environ
 import spacy
 from spacy.language import Language
 import langcodes
+from brevia.settings import get_settings
 
 
 class Detector():
     """Language detection class"""
     nlp: Language | None = None
 
     def __init__(self):
         """Init internal nlp"""
-        if not bool(environ.get('FEATURE_QA_LANG_DETECT')):
+        if not get_settings().feature_qa_lang_detect:
             return
 
         try:
             import spacy_fastlang  # noqa: F401 pylint: disable=import-outside-toplevel
 
             self.nlp = spacy.load('en_core_web_sm')
             self.nlp.add_pipe('language_detector')
```

### Comparing `brevia-0.0.8/brevia/load_file.py` & `brevia-0.0.9/brevia/load_file.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/models.py` & `brevia-0.0.9/brevia/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Utilities to create langchain LLM and Chat Model instances."""
 from abc import ABC, abstractmethod
-from os import environ
-from typing import Dict, List, Any
+from typing import Any
 from langchain.llms.loading import load_llm_from_config
 from langchain.llms.base import BaseLLM
 from langchain.llms.fake import FakeListLLM
 from langchain.chat_models.base import BaseChatModel
-from langchain.chat_models.fake import FakeListChatModel
-from langchain.chat_models import ChatOpenAI
-from langchain.embeddings.openai import OpenAIEmbeddings
-from langchain.embeddings.fake import FakeEmbeddings
+from langchain.chat_models import (
+    ChatOpenAI,
+    ChatAnthropic,
+    ChatCohere,
+    FakeListChatModel
+)
+from langchain.embeddings import OpenAIEmbeddings, CohereEmbeddings, FakeEmbeddings
 from langchain.embeddings.base import Embeddings
 from openai import Audio
+from brevia.settings import get_settings
 
 
 class FakeBreviaLLM(FakeListLLM):
     """Fake LLM for testing purposes."""
-    def get_token_ids(self, text: str) -> List[int]:
+    def get_token_ids(self, text: str) -> list[int]:
         return [10] * 10
 
 
 LOREM_IPSUM = """Lorem ipsum dolor sit amet, consectetur adipisici elit,
 sed eiusmod tempor incidunt ut labore et dolore magna aliqua."""
 
 
@@ -28,23 +31,25 @@
     """Load langchain LLM, use Fake LLM in test mode"""
     if test_models_in_use():
         return FakeBreviaLLM(responses=[LOREM_IPSUM] * 10)
 
     return load_llm_from_config(config=config)
 
 
-CHAT_MODEL_TYPES: Dict[str, BaseChatModel] = {
+CHAT_MODEL_TYPES: dict[str, BaseChatModel] = {
     'openai-chat': ChatOpenAI,
+    'cohere-chat': ChatCohere,
+    'anthropic-chat': ChatAnthropic,
     'fake-list-chat-model': FakeListChatModel,
 }
 
 
 class FakeBreviaChatModel(FakeListChatModel):
     """Fake LLM for testing purposes."""
-    def get_token_ids(self, text: str) -> List[int]:
+    def get_token_ids(self, text: str) -> list[int]:
         return [10] * 10
 
 
 def load_chatmodel(config: dict) -> BaseChatModel:
     """Load Chat Model from Config Dict."""
     if test_models_in_use():
         return FakeBreviaChatModel(responses=[LOREM_IPSUM] * 10)
@@ -85,18 +90,32 @@
     """Load Audio transcriber (only openAI supported for now)."""
     if test_models_in_use():
         return FakeAudio()
 
     return AudioOpenAI()
 
 
+EMBEDDING_TYPES: dict[str, BaseChatModel] = {
+    'openai-embeddings': OpenAIEmbeddings,
+    'cohere-embeddings': CohereEmbeddings,
+    'fake-embeddings': FakeEmbeddings,
+}
+
+
 def load_embeddings() -> Embeddings:
-    """ Load Embeddings engine: only OpenAI or Fake for now """
+    """ Load Embeddings engine """
+    settings = get_settings()
     if test_models_in_use():
-        return FakeEmbeddings(size=1536)
+        return FakeEmbeddings(size=settings.embeddings_size)
+
+    config = settings.embeddings.copy()
+    config_type = config.pop('_type', None)
+    if config_type not in EMBEDDING_TYPES:
+        raise ValueError(f'Loading "{config_type}" Embeddings not supported')
 
-    return OpenAIEmbeddings()
+    emb_cls = EMBEDDING_TYPES[config_type]
+    return emb_cls(**config)
 
 
 def test_models_in_use() -> bool:
     """Check if test models are in use (via `USE_TEST_MODELS` env var)"""
-    return bool(environ.get('USE_TEST_MODELS', False))
+    return get_settings().use_test_models
```

### Comparing `brevia-0.0.8/brevia/postman/Brevia API.postman_collection.json` & `brevia-0.0.9/brevia/postman/Brevia API.postman_collection.json`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/postman/Brevia API.postman_environment.json` & `brevia-0.0.9/brevia/postman/Brevia API.postman_environment.json`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/query.py` & `brevia-0.0.9/brevia/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Question-answering and search functions against a vector database."""
-from os import environ, path
+from os import path
 from langchain.docstore.document import Document
 from langchain.vectorstores.pgvector import PGVector, DistanceStrategy
 from langchain.vectorstores._pgvector_data_models import CollectionStore
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.chains.base import Chain
 from langchain.chains import ConversationalRetrievalChain
 from langchain.chains.question_answering import load_qa_chain
@@ -16,14 +16,15 @@
     HumanMessagePromptTemplate,
 )
 from langchain.prompts.loading import load_prompt_from_config
 from brevia.connection import connection_string
 from brevia.collections import single_collection_by_name
 from brevia.callback import AsyncLoggingCallbackHandler
 from brevia.models import load_chatmodel, load_embeddings
+from brevia.settings import get_settings
 
 # system = load_prompt(f'{prompts_path}/qa/default.system.yaml')
 # jinja2 template from file was disabled by langchain so, for now
 # we load from here
 SYSTEM_TEMPLATE = """
                 As an AI assistant your task is to provide valuable
                 information and support to our users. Answer the question
@@ -89,15 +90,15 @@
     distance_strategy_name: str = 'cosine',
 ) -> list[tuple[Document, float]]:
     """ Perform a similarity search on vector index """
     collection_store = single_collection_by_name(collection)
     if not collection_store:
         raise ValueError(f'Collection not found: {collection}')
     if docs_num is None:
-        default_num = environ.get('SEARCH_DOCS_NUM', 4)
+        default_num = get_settings().search_docs_num
         docs_num = int(collection_store.cmetadata.get('docs_num', default_num))
     strategy = DISTANCE_MAP.get(distance_strategy_name, DistanceStrategy.COSINE)
     docsearch = PGVector(
         connection_string=connection_string(),
         embedding_function=load_embeddings(),
         collection_name=collection,
         distance_strategy=strategy,
@@ -131,16 +132,17 @@
             (default empty list)
 
         can implement "vectordbkwargs" into quest_dict:
             {
                 "search_distance": 0.9
             }
     """
+    settings = get_settings()
     if docs_num is None:
-        default_num = environ.get('SEARCH_DOCS_NUM', 4)
+        default_num = settings.search_docs_num
         docs_num = int(collection.cmetadata.get('docs_num', default_num))
     if answer_callbacks is None:
         answer_callbacks = []
     if conversation_callbacks is None:
         conversation_callbacks = []
 
     strategy = DISTANCE_MAP.get(distance_strategy_name, DistanceStrategy.COSINE)
@@ -148,47 +150,42 @@
         connection_string=connection_string(),
         embedding_function=load_embeddings(),
         collection_name=collection.name,
         distance_strategy=strategy,
     )
 
     prompts = collection.cmetadata.get('prompts')
-    model_name = collection.cmetadata.get('model_name', environ.get('QA_MODEL'))
-    temperature = collection.cmetadata.get('temperature', environ.get('QA_TEMPERATURE'))
-    verbose = environ.get('VERBOSE_MODE', False)
+    qa_llm_conf = collection.cmetadata.get(
+        'qa_completion_llm',
+        settings.qa_completion_llm.copy()
+    )
+    fup_llm_conf = collection.cmetadata.get(
+        'qa_followup_llm',
+        settings.qa_followup_llm.copy()
+    )
+
+    verbose = settings.verbose_mode
 
     # LLM to rewrite follow-up question
-    fup_llm = load_chatmodel({
-        '_type': 'openai-chat',
-        'model_name': environ.get('QA_FOLLOWUP_MODEL', 'gpt-3.5-turbo'),
-        'temperature': float(temperature),
-        'max_tokens': int(environ.get('QA_FOLLOWUP_MAX_TOKENS', 200)),
-        'verbose': verbose,
-    })
+    fup_llm = load_chatmodel(fup_llm_conf)
 
     logging_handler = AsyncLoggingCallbackHandler()
     # Create chain for follow-up question using chat history (if present)
     question_generator = LLMChain(
         llm=fup_llm,
         prompt=load_condense_prompt(prompts),
         verbose=verbose,
         callbacks=[logging_handler],
     )
 
     # Model to use in final prompt
     answer_callbacks.append(logging_handler)
-    chatllm = load_chatmodel({
-        '_type': 'openai-chat',
-        'model_name': model_name,
-        'temperature': float(temperature),
-        'max_tokens': int(environ.get('QA_MAX_TOKENS', 800)),
-        'callbacks': answer_callbacks,
-        'streaming': streaming,
-        'verbose': verbose,
-    })
+    qa_llm_conf['callbacks'] = answer_callbacks
+    qa_llm_conf['streaming'] = streaming
+    chatllm = load_chatmodel(qa_llm_conf)
 
     # this chain use "stuff" to elaborate context
     doc_chain = load_qa_chain(
         llm=chatllm,
         prompt=load_qa_prompt(prompts),
         chain_type="stuff",
         verbose=verbose,
```

### Comparing `brevia-0.0.8/brevia/routers/analyze_router.py` & `brevia-0.0.9/brevia/routers/analyze_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     if not summarize.text:
         raise HTTPException(
             status.HTTP_400_BAD_REQUEST,
             'Empty text field',
         )
 
     service = SummarizeTextService()
-    return service.run(summarize.dict())
+    return service.run(summarize.model_dump())
 
 
 @router.post(
     '/upload_summarize',
     dependencies=get_dependencies(json_content_type=False)
 )
 def upload_summarize(
```

### Comparing `brevia-0.0.8/brevia/routers/app_routers.py` & `brevia-0.0.9/brevia/routers/app_routers.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/routers/audio_router.py` & `brevia-0.0.9/brevia/routers/audio_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """API endpoints definitions to handle audio input"""
 import logging
-from os import environ
 from typing import Annotated
 from fastapi import APIRouter, UploadFile, Form
 from brevia.models import load_audiotranscriber
 from brevia.dependencies import (
     get_dependencies,
     save_upload_file_tmp,
 )
+from brevia.settings import get_settings
 
 router = APIRouter()
 
 
 @router.post(
     '/transcribe',
     dependencies=get_dependencies(json_content_type=False)
@@ -27,13 +27,13 @@
     tmp_file_path = save_upload_file_tmp(file)
 
     with open(tmp_file_path, 'rb') as audio_file:
         audio = load_audiotranscriber()
         result = audio.transcribe(
                 file=audio_file,
                 model='whisper-1',
-                api_key=environ.get('OPENAI_API_KEY'),
+                api_key=get_settings().openai_api_key,
                 params={'language': language},
         )
         log.info('Audio transcription completed')
         log.info(result)
         return result
```

### Comparing `brevia-0.0.8/brevia/routers/chat_history_router.py` & `brevia-0.0.9/brevia/routers/chat_history_router.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/routers/collections_router.py` & `brevia-0.0.9/brevia/routers/collections_router.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/routers/index_router.py` & `brevia-0.0.9/brevia/routers/index_router.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/routers/jobs_router.py` & `brevia-0.0.9/brevia/routers/jobs_router.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/routers/qa_router.py` & `brevia-0.0.9/brevia/routers/qa_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         Specify distance_strategy:
             EUCLIDEAN = EmbeddingStore.embedding.l2_distance (default)
             COSINE = EmbeddingStore.embedding.cosine_distance
             MAX_INNER_PRODUCT = EmbeddingStore.embedding.max_inner_product
     """
     collection = check_collection_name(search.collection)
 
-    params = {k: v for k, v in search.dict().items() if v is not None}
+    params = {k: v for k, v in search.model_dump().items() if v is not None}
     if 'docs_num' not in params and 'docs_num' in collection.cmetadata:
         params['docs_num'] = collection.cmetadata['docs_num']
     result = query.search_vector_qa(**params)
 
     return extract_content_score(result)
```

### Comparing `brevia-0.0.8/brevia/routers/status_router.py` & `brevia-0.0.9/brevia/routers/status_router.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/services.py` & `brevia-0.0.9/brevia/services.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/tokens.py` & `brevia-0.0.9/brevia/tokens.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """JWT Utility methods"""
-from os import environ
 from datetime import datetime, timedelta
 from jose import jwt, JWTError
+from brevia.settings import get_settings
 
 ALGORITHM = 'HS256'
 
 
 def create_token(user: str, duration: int) -> str:
     """Create an access token """
     # expire time of the token
     expire = datetime.utcnow() + timedelta(minutes=duration)
     to_encode = {
         'user': user,
         'exp': expire,
     }
-    secret = environ.get('TOKENS_SECRET')
+    secret = get_settings().tokens_secret
 
     return jwt.encode(to_encode, secret, algorithm=ALGORITHM)
 
 
 def verify_token(token: str):
     """
         Try to decode the token, it will
         raise a JWTError if the token is not correct
     """
-    secret = environ.get('TOKENS_SECRET')
+    settings = get_settings()
+    secret = settings.tokens_secret
     payload = jwt.decode(token, secret, algorithms=[ALGORITHM])
     # basic check: presence of `user` key, must be a non empty string
     if 'user' not in payload:
         raise JWTError('Bad payload format')
     user = payload['user']
     if not isinstance(user, str) or len(user.strip()) == 0:
         raise JWTError('Bad payload format')
     # further check: user must one of `TOKENS_USERS` env var (if set)
-    valid_users = environ.get('TOKENS_USERS')
+    valid_users = settings.tokens_users
     if not valid_users:
         return
     if user not in valid_users.split(','):
         raise JWTError('Bad payload format')
```

### Comparing `brevia-0.0.8/brevia/utilities/collections_io.py` & `brevia-0.0.9/brevia/utilities/collections_io.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/utilities/files_import.py` & `brevia-0.0.9/brevia/utilities/files_import.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/brevia/utilities/run_service.py` & `brevia-0.0.9/brevia/utilities/run_service.py`

 * *Files identical despite different names*

### Comparing `brevia-0.0.8/pyproject.toml` & `brevia-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "brevia"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = [
   "Niki Corradetti <niki.corradetti@atlasconsulting.it>",
   "Stefano Rosanelli <stefano.rosanelli@atlasconsulting.it>"
 ]
 readme = "README.md"
 homepage = "https://github.com/brevia-ai/brevia"
 repository = "https://github.com/brevia-ai/brevia"
 
   [tool.poetry.dependencies]
   python = "^3.10"
   bs4 = "^0.0.1"
   lxml = "^4.9.2"
   langchain = "0.0.338"
-  fastapi = "^0.95.2"
+  fastapi = "^0.104.1"
   nltk = "^3.8.1"
   openai = "^0.27.7"
   pgvector = "^0.1.8"
   psycopg2-binary = "^2.9.6"
   pypdf = "^3.9.0"
   python-dotenv = "^1.0.0"
   python-multipart = "^0.0.6"
@@ -27,14 +27,15 @@
   spacy-fastlang = "^1.0.1"
   langcodes = "^3.3.0"
   language-data = "^1.1"
   pycryptodome = "^3.18.0"
   alembic = "^1.11.1"
   python-jose = "^3.3.0"
   sqlalchemy-utils = "^0.41.1"
+  pydantic-settings = "^2.1.0"
 
     [tool.poetry.dependencies.uvicorn]
     extras = [ "standard" ]
     version = "^0.22.0"
 
   [tool.poetry.scripts]
   create_token = "brevia.commands:create_access_token"
```

### Comparing `brevia-0.0.8/PKG-INFO` & `brevia-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: brevia
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Home-page: https://github.com/brevia-ai/brevia
 Author: Niki Corradetti
 Author-email: niki.corradetti@atlasconsulting.it
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.11.1,<2.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
+Requires-Dist: fastapi (>=0.104.1,<0.105.0)
 Requires-Dist: langchain (==0.0.338)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pgvector (>=0.1.8,<0.2.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
+Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: pypdf (>=3.9.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: spacy-fastlang (>=1.0.1,<2.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
```

