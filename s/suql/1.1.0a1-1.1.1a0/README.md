# Comparing `tmp/suql-1.1.0a1.tar.gz` & `tmp/suql-1.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.0a1.tar", last modified: Mon Apr  8 19:12:49 2024, max compression
+gzip compressed data, was "suql-1.1.1a0.tar", last modified: Thu Apr 11 05:10:46 2024, max compression
```

## Comparing `suql-1.1.0a1.tar` & `suql-1.1.1a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-08 19:12:49.175326 suql-1.1.0a1/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.0a1/LICENSE
--rw-r--r--   0 oval      (1000) users      (100)     5324 2024-04-08 19:12:49.175326 suql-1.1.0a1/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4306 2024-04-08 18:37:27.000000 suql-1.1.0a1/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-08 19:12:49.175326 suql-1.1.0a1/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1560 2024-04-08 19:12:37.000000 suql-1.1.0a1/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-08 19:12:49.175326 suql-1.1.0a1/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-08 19:12:49.175326 suql-1.1.0a1/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.0a1/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16980 2024-04-07 05:13:01.000000 suql-1.1.0a1/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8646 2024-04-06 00:50:57.000000 suql-1.1.0a1/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)    12093 2024-04-06 00:13:31.000000 suql-1.1.0a1/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-08 19:12:49.175326 suql-1.1.0a1/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.0a1/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-08 19:12:49.175326 suql-1.1.0a1/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.0a1/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    61719 2024-04-08 18:29:19.000000 suql-1.1.0a1/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.0a1/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-08 19:12:49.175326 suql-1.1.0a1/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     5324 2024-04-08 19:12:49.000000 suql-1.1.0a1/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-08 19:12:49.000000 suql-1.1.0a1/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-08 19:12:49.000000 suql-1.1.0a1/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      217 2024-04-08 19:12:49.000000 suql-1.1.0a1/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-08 19:12:49.000000 suql-1.1.0a1/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.182489 suql-1.1.1a0/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.1a0/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4912 2024-04-11 05:10:46.182489 suql-1.1.1a0/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4306 2024-04-08 18:37:27.000000 suql-1.1.1a0/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-11 05:10:46.182489 suql-1.1.1a0/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1535 2024-04-10 21:17:54.000000 suql-1.1.1a0/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.166489 suql-1.1.1a0/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.174489 suql-1.1.1a0/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.1a0/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    16980 2024-04-07 05:13:01.000000 suql-1.1.1a0/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8646 2024-04-06 00:50:57.000000 suql-1.1.1a0/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     4095 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9870 2024-04-10 21:17:41.000000 suql-1.1.1a0/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.182489 suql-1.1.1a0/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.1a0/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.182489 suql-1.1.1a0/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.1a0/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    62450 2024-04-11 05:09:58.000000 suql-1.1.1a0/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.1a0/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-11 05:10:46.174489 suql-1.1.1a0/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     4912 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      200 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-11 05:10:46.000000 suql-1.1.1a0/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.0a1/LICENSE` & `suql-1.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/PKG-INFO` & `suql-1.1.1a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,22 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.0a1
+Version: 1.1.1a0
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.3.2
-Requires-Dist: Jinja2==3.1.2
-Requires-Dist: Flask==2.3.2
-Requires-Dist: Flask-Cors==4.0.0
-Requires-Dist: Flask-RESTful==0.3.10
-Requires-Dist: transformers==4.38.2
-Requires-Dist: torch==2.0.1
-Requires-Dist: requests==2.31.0
-Requires-Dist: spacy==3.7.4
-Requires-Dist: tiktoken==0.4.0
-Requires-Dist: psycopg2-binary==2.9.7
-Requires-Dist: pglast==5.3
-Requires-Dist: FlagEmbedding==1.2.5
 
 <p align="center">
     <h1 align="center">
         <b>SUQL (Structured and Unstructured Query Language)</b>
         <br>
         <a href="https://arxiv.org/abs/2311.09818">
             <img src="https://img.shields.io/badge/cs.CL-2311.09818-b31b1b" alt="arXiv">
```

#### html2text {}

```diff
@@ -1,21 +1,15 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.0a1 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.1a0 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: openai==1.3.2 Requires-Dist: Jinja2==3.1.2 Requires-Dist:
-Flask==2.3.2 Requires-Dist: Flask-Cors==4.0.0 Requires-Dist: Flask-
-RESTful==0.3.10 Requires-Dist: transformers==4.38.2 Requires-Dist: torch==2.0.1
-Requires-Dist: requests==2.31.0 Requires-Dist: spacy==3.7.4 Requires-Dist:
-tiktoken==0.4.0 Requires-Dist: psycopg2-binary==2.9.7 Requires-Dist:
-pglast==5.3 Requires-Dist: FlagEmbedding==1.2.5
            ************ SSUUQQLL ((SSttrruuccttuurreedd aanndd UUnnssttrruuccttuurreedd QQuueerryy LLaanngguuaaggee))
                   _[[_aa_rr_XX_ii_vv_]]_[[_GG_ii_tt_hh_uu_bb_ _SS_tt_aa_rr_ss_]]_[[_PP_yy_PP_II_ _vv_ee_rr_ss_ii_oo_nn_]] ************
      Conversational Search over Structured and Unstructured Data with LLMs
                 Online demo: _h_t_t_p_s_:_/_/_y_e_l_p_b_o_t_._g_e_n_i_e_._s_t_a_n_f_o_r_d_._e_d_u
 # What is SUQL SUQL stands for Structured and Unstructured Query Language. It
 augments SQL with several important free text primitives for a precise,
 succinct, and expressive representation. It can be used to build chatbots for
```

### Comparing `suql-1.1.0a1/README.md` & `suql-1.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/setup.py` & `suql-1.1.1a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.0a1"
+version = "1.1.1a0"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
@@ -14,22 +14,21 @@
 # Define your dependencies
 install_requires = [
     'openai==1.3.2',
     'Jinja2==3.1.2',
     'Flask==2.3.2',
     'Flask-Cors==4.0.0',
     'Flask-RESTful==0.3.10',
-    'transformers==4.38.2',
-    'torch==2.0.1',
     'requests==2.31.0',
     'spacy==3.7.4',
     'tiktoken==0.4.0',
     'psycopg2-binary==2.9.7',
     'pglast==5.3',
     'FlagEmbedding==1.2.5',
+    'litellm==1.34.34'
 ]
 
 # Additional package information
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `suql-1.1.0a1/src/suql/agent.py` & `suql-1.1.1a0/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/faiss_embedding.py` & `suql-1.1.1a0/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/free_text_fcns_server.py` & `suql-1.1.1a0/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/postgresql_connection.py` & `suql-1.1.1a0/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.1a0/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/prompts/opening_hours.prompt` & `suql-1.1.1a0/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/prompts/parser_suql.prompt` & `suql-1.1.1a0/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.1a0/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.1a0/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.1a0/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import concurrent.futures
 import json
 import random
 import string
 import time
 import traceback
+import logging
 from collections import defaultdict
 from copy import deepcopy
 from typing import List, Union
 
 import pglast
 import requests
 from pglast import parse_sql
@@ -225,14 +226,15 @@
             )
 
             # based on results and column_info, insert a temporary table
             column_create_stmt = ",\n".join(
                 list(map(lambda x: f'"{x[0]}" {x[1]}', column_info))
             )
             create_stmt = f"CREATE TABLE {tmp_table_name} (\n{column_create_stmt}\n); GRANT SELECT ON {tmp_table_name} TO {self.select_username};"
+            logging.info("created table {}".format(tmp_table_name))
             execute_sql(
                 create_stmt,
                 user=self.create_username,
                 password=self.create_userpswd,
                 commit_in_lieu_fetch=True,
                 no_print=True,
             )
@@ -479,17 +481,17 @@
             else:
                 found_stmt.append(
                     "Verified answer({}, '{}') {} {} in table = {} based on document: {}".format(
                         field[1], query, operator, value, field[0], doc[1][i]
                     )
                 )
     if all_found:
-        print("\n".join(found_stmt))
+        logging.info("\n".join(found_stmt))
     elif found_stmt:
-        print("partially verified: " + "\n".join(found_stmt))
+        logging.info("partially verified: " + "\n".join(found_stmt))
 
     return all_found
 
 
 def _parallel_filtering(fcn, source: list, limit, enforce_ordering=False):
     true_count = 0
     true_items = set()
@@ -672,15 +674,15 @@
     else:
         id_res = []
         for each_res in parsed_result:
             if _verify_single_res(each_res, field_query_list, llm_model_name):
                 id_res.append(each_res[0])
 
     end_time = time.time()
-    print("retrieve + verification time {}s".format(end_time - start_time))
+    logging.info("retrieve + verification time {}s".format(end_time - start_time))
 
     if single_table:
         res = list(filter(lambda x: x[id_index] in id_res, existing_results))
     else:
         res = [
             i[1:]
             for i in list(filter(lambda x: x[id_index] in id_res, existing_results))
@@ -901,35 +903,35 @@
                 to_execute_node.whereClause = None
                 _, column_infos = execute_sql_with_column_info(
                     RawStream()(to_execute_node),
                     user=self.select_username,
                     password=self.select_userpswd,
                 )
         except psyconpg2Error:
-            print(
+            logging.info(
                 "above error happens during ENUM classification attempts. Marking this predicate as returning answer."
             )
             res = True
 
         if not res:
-            print("determined the above predicate returns no result")
+            logging.info("determined the above predicate returns no result")
             # try to classify into one of the known values
             # first, we need to find out what is the value here - some heuristics here to find out
             column_name, value_res = _get_a_expr_field_value(node)
 
             if isinstance(value_res, String):
                 value_res_clear = value_res.sval
             elif isinstance(value_res, Integer):
                 value_res_clear = value_res.ival
             elif isinstance(value_res, Float):
                 value_res_clear = value_res.fval
             else:
                 raise ValueError()
 
-            print(
+            logging.info(
                 "determined column name: {}; value: {}".format(
                     column_name, value_res_clear
                 )
             )
 
             # first check if this is already in the cache
             # TODO: for best performance move this before the execution above
@@ -1519,14 +1521,15 @@
 def suql_execute(
     suql,
     table_w_ids,
     fts_fields=[],
     llm_model_name="gpt-3.5-turbo-0125",
     max_verify=20,
     loggings="",
+    log_filename=None,
     disable_try_catch=False,
     embedding_server_address="http://127.0.0.1:8501",
     select_username="select_user",
     select_userpswd="select_user",
     create_username="creator_role",
     create_userpswd="creator_role",
 ):
@@ -1548,14 +1551,16 @@
         Defaults to `gpt-3.5-turbo-0125`.
         
     `max_verify` (str): For each LIMIT x clause, `max_verify * x` results will be retrieved together from
         the embedding model for LLM to verify. Defaults to 20.
         
     `loggings` (str, optional): Prefix for error case loggings. Errors are written to a "_suql_error_log.txt"
         file by default.
+
+    `log_filename` (str, optional): Logging file name for the SUQL compiler. If not provided, logging is disabled.
         
     `disable_try_catch` (bool, optional): whether to disable try-catch (errors would directly propagate to caller).
     
     `embedding_server_address` (str, optional): the embedding server address. Defaults to 'http://127.0.0.1:8501'.
     
     `select_username` (str, optional): user name with select privilege in db. Defaults to "select_user".
     
@@ -1584,14 +1589,26 @@
     since for queries that search by name, e.g.:
     ```
     suql_execute("SELECT * FROM restaurants WHERE name = 'mcdonalds'", fts_fields=[("restaurants", "name")])
     ```
     Ideally, this query should match against all `Mcdonald's`, as opposed to just 'mcdonalds'.
     FTS helps with such cases.
     """
+    if log_filename:
+        logging.basicConfig(level=logging.INFO,
+                            format='%(asctime)s - %(levelname)s - %(message)s',
+                            datefmt='%Y-%m-%d %H:%M:%S',
+                            handlers=[
+                                logging.FileHandler(log_filename),
+                                logging.StreamHandler()
+                            ])
+
+    else:
+        logging.basicConfig(level=logging.CRITICAL + 1)
+
     results, column_names, cache = _suql_execute_single(
         suql,
         table_w_ids,
         fts_fields,
         llm_model_name,
         max_verify,
         embedding_server_address,
```

### Comparing `suql-1.1.0a1/src/suql/utils.py` & `suql-1.1.1a0/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.0a1/src/suql.egg-info/PKG-INFO` & `suql-1.1.1a0/src/suql.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,22 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.0a1
+Version: 1.1.1a0
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.3.2
-Requires-Dist: Jinja2==3.1.2
-Requires-Dist: Flask==2.3.2
-Requires-Dist: Flask-Cors==4.0.0
-Requires-Dist: Flask-RESTful==0.3.10
-Requires-Dist: transformers==4.38.2
-Requires-Dist: torch==2.0.1
-Requires-Dist: requests==2.31.0
-Requires-Dist: spacy==3.7.4
-Requires-Dist: tiktoken==0.4.0
-Requires-Dist: psycopg2-binary==2.9.7
-Requires-Dist: pglast==5.3
-Requires-Dist: FlagEmbedding==1.2.5
 
 <p align="center">
     <h1 align="center">
         <b>SUQL (Structured and Unstructured Query Language)</b>
         <br>
         <a href="https://arxiv.org/abs/2311.09818">
             <img src="https://img.shields.io/badge/cs.CL-2311.09818-b31b1b" alt="arXiv">
```

#### html2text {}

```diff
@@ -1,21 +1,15 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.0a1 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.1a0 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: openai==1.3.2 Requires-Dist: Jinja2==3.1.2 Requires-Dist:
-Flask==2.3.2 Requires-Dist: Flask-Cors==4.0.0 Requires-Dist: Flask-
-RESTful==0.3.10 Requires-Dist: transformers==4.38.2 Requires-Dist: torch==2.0.1
-Requires-Dist: requests==2.31.0 Requires-Dist: spacy==3.7.4 Requires-Dist:
-tiktoken==0.4.0 Requires-Dist: psycopg2-binary==2.9.7 Requires-Dist:
-pglast==5.3 Requires-Dist: FlagEmbedding==1.2.5
            ************ SSUUQQLL ((SSttrruuccttuurreedd aanndd UUnnssttrruuccttuurreedd QQuueerryy LLaanngguuaaggee))
                   _[[_aa_rr_XX_ii_vv_]]_[[_GG_ii_tt_hh_uu_bb_ _SS_tt_aa_rr_ss_]]_[[_PP_yy_PP_II_ _vv_ee_rr_ss_ii_oo_nn_]] ************
      Conversational Search over Structured and Unstructured Data with LLMs
                 Online demo: _h_t_t_p_s_:_/_/_y_e_l_p_b_o_t_._g_e_n_i_e_._s_t_a_n_f_o_r_d_._e_d_u
 # What is SUQL SUQL stands for Structured and Unstructured Query Language. It
 augments SQL with several important free text primitives for a precise,
 succinct, and expressive representation. It can be used to build chatbots for
```

### Comparing `suql-1.1.0a1/src/suql.egg-info/SOURCES.txt` & `suql-1.1.1a0/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

