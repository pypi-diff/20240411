# Comparing `tmp/aibridge_test-0.2.8.tar.gz` & `tmp/aibridge_test-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.2.8.tar", last modified: Mon Apr  8 07:59:08 2024, max compression
+gzip compressed data, was "aibridge_test-0.2.9.tar", last modified: Thu Apr 11 11:23:16 2024, max compression
```

## Comparing `aibridge_test-0.2.8.tar` & `aibridge_test-0.2.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.884324 aibridge_test-0.2.8/
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.594322 aibridge_test-0.2.8/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.8/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.668323 aibridge_test-0.2.8/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     8944 2024-04-02 05:11:26.000000 aibridge_test-0.2.8/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    13216 2024-04-08 07:03:19.000000 aibridge_test-0.2.8/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0    11900 2024-04-05 09:25:51.000000 aibridge_test-0.2.8/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14053 2024-04-04 11:46:45.000000 aibridge_test-0.2.8/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.8/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11525 2024-04-04 09:42:06.000000 aibridge_test-0.2.8/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.8/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.8/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.8/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.694322 aibridge_test-0.2.8/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     7561 2024-04-08 06:59:23.000000 aibridge_test-0.2.8/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.2.8/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.727323 aibridge_test-0.2.8/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.744325 aibridge_test-0.2.8/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.8/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.760326 aibridge_test-0.2.8/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.8/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.8/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.777324 aibridge_test-0.2.8/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.798323 aibridge_test-0.2.8/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.8/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/LICENSE
--rw-rw-rw-   0        0        0    21534 2024-04-08 07:59:08.881330 aibridge_test-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 07:59:08.879331 aibridge_test-0.2.8/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21534 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-08 07:59:08.000000 aibridge_test-0.2.8/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 07:59:08.885325 aibridge_test-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2863 2024-04-08 07:57:56.000000 aibridge_test-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:16.654936 aibridge_test-0.2.9/
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.277304 aibridge_test-0.2.9/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.2.9/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.550299 aibridge_test-0.2.9/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     9311 2024-04-11 09:50:53.000000 aibridge_test-0.2.9/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    13501 2024-04-11 09:51:01.000000 aibridge_test-0.2.9/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    12216 2024-04-11 09:51:03.000000 aibridge_test-0.2.9/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14353 2024-04-11 09:47:06.000000 aibridge_test-0.2.9/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.2.9/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11817 2024-04-11 09:46:41.000000 aibridge_test-0.2.9/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.2.9/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.2.9/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.2.9/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.581300 aibridge_test-0.2.9/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7561 2024-04-08 06:59:23.000000 aibridge_test-0.2.9/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.2.9/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.706308 aibridge_test-0.2.9/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.726300 aibridge_test-0.2.9/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.2.9/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:15.884299 aibridge_test-0.2.9/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.2.9/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.2.9/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:16.220302 aibridge_test-0.2.9/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:16.354298 aibridge_test-0.2.9/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.2.9/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-04-11 11:23:16.644868 aibridge_test-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 11:23:16.642872 aibridge_test-0.2.9/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-04-11 11:23:14.000000 aibridge_test-0.2.9/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-04-11 11:23:15.000000 aibridge_test-0.2.9/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 11:23:14.000000 aibridge_test-0.2.9/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-04-11 11:23:14.000000 aibridge_test-0.2.9/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 11:23:14.000000 aibridge_test-0.2.9/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 11:23:16.654936 aibridge_test-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-04-11 11:12:45.000000 aibridge_test-0.2.9/setup.py
```

### Comparing `aibridge_test-0.2.8/AIBridge/__init__.py` & `aibridge_test-0.2.9/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.2.9/AIBridge/ai_services/ai21labs_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,25 +151,31 @@
                     format_structure = json.loads(format_structure)
             if not prompts:
                 raise Ai21Exception("No prompts provided")
             api_key = api_key if api_key else parse_api_key("ai21_api")
             ai21.api_key = api_key
             model_output = []
             token_used = 0
+            input_tokens = 0
+            output_tokens = 0
             context_string = self.get_prompt_context(context)
             for index, prompt in enumerate(prompts):
                 prompt = context_string + "\n" + prompt
                 response = ai21.Completion.execute(
                     model=model,
                     prompt=prompt,
                     numResults=variation_count,
                     maxTokens=max_tokens,
                     temperature=temperature,
                 )
-                token_used = token_used + len(response["prompt"]["tokens"])
+                input_tokens = input_tokens + len(response["prompt"]["tokens"])
+                output_tokens = output_tokens + len(
+                    response["completions"][0]["data"]["tokens"]
+                )
+                token_used = input_tokens + output_tokens
                 for res in response["completions"]:
                     content = res["data"]["text"]
                     token_used = token_used + len(res["data"]["tokens"])
                     if output_format:
                         _formatter = output_format[index]
                         try:
                             if _formatter == "csv":
@@ -202,14 +208,16 @@
                     if index >= len(model_output):
                         model_output.append({"data": [content]})
                     else:
                         model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
+                    "input_tokens": input_tokens,
+                    "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "ai21_api",
                 }
             }
             return message_value
         except AIBridgeException as e:
```

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.2.9/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.2.9/AIBridge/ai_services/anthropic_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,16 @@
                     format_structure = json.loads(format_structure)
             if not prompts:
                 raise AnthropicsException("No prompts provided")
             api_key = api_key if api_key else parse_api_key("anthropic")
             message_data = self.get_prompt_context(context)
             model_output = []
             token_used = 0
+            input_tokens = 0
+            output_tokens = 0
             _formatter = "string"
             func_call = False
             for index, prompt in enumerate(prompts):
                 if output_format:
                     _formatter = output_format[index]
                 message_data.append({"role": "user", "content": prompt})
                 if _formatter not in ["json", "csv", "xml"]:
@@ -253,17 +255,18 @@
                     )
                     message_data.append(
                         {
                             "role": response.role,
                             "content": response.content[0].text,
                         }
                     )
-                print(response)
                 tokens = response.usage.input_tokens + response.usage.output_tokens
                 token_used = token_used + tokens
+                input_tokens = input_tokens + response.usage.input_tokens
+                output_tokens = output_tokens + response.usage.output_tokens
                 for index, res in enumerate(response.content):
                     content = res.text
                     if func_call:
                         json_content = IntoJson.xml_to_json(content)
                         content = json_content["function_calls"][0]["invoke"][
                             "parameters"
                         ]
@@ -309,14 +312,16 @@
                     if index >= len(model_output):
                         model_output.append({"data": [content]})
                     else:
                         model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
+                    "input_tokens": input_tokens,
+                    "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "anthropic",
                 }
             }
             return message_value
         except AIBridgeException as e:
```

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.2.9/AIBridge/ai_services/cohere_llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -200,15 +200,17 @@
                     format_structure = json.loads(format_structure)
             if not prompts:
                 raise CohereException("No prompts provided")
             api_key = api_key if api_key else parse_api_key("cohere_api")
             model_output = []
             message_data = []
             context = self.get_prompt_context(context)
-            token_used = max_tokens
+            token_used = 0
+            input_tokens = 0
+            output_tokens = 0
             _formatter = "string"
             for index, prompt in enumerate(prompts):
                 if output_format:
                     _formatter = output_format[index]
                 if _formatter not in ["json", "csv", "xml"]:
                     response = self.execute_text_prompt(
                         api_key,
@@ -245,14 +247,16 @@
                         context=message_data,
                     )
                     content = response.tool_calls[0].parameters
                 tokens = (
                     response.meta["billed_units"]["input_tokens"]
                     + response.meta["billed_units"]["output_tokens"]
                 )
+                input_tokens += response.meta["billed_units"]["input_tokens"]
+                output_tokens += response.meta["billed_units"]["output_tokens"]
                 token_used = token_used + tokens
                 if output_format:
                     if isinstance(content, dict):
                         content = json.dumps(content)
                     try:
                         if _formatter == "csv":
                             content = FromJson.json_to_csv(json.loads(content))
@@ -282,14 +286,16 @@
                 if index >= len(model_output):
                     model_output.append({"data": [content]})
                 else:
                     model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
+                    "input_tokens": input_tokens,
+                    "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "cohere",
                 }
             }
             return message_value
         except AIBridgeException as e:
```

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.2.9/AIBridge/ai_services/geminin_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,16 @@
                     format_structure = json.loads(format_structure)
             if not prompts:
                 raise GeminiException("No prompts provided")
             api_key = api_key if api_key else parse_api_key("gemini_ai")
             message_data = self.get_prompt_context(context) if context else []
             model_output = []
             token_used = 0
+            input_tokens=0
+            output_tokens=0
             _formatter = "string"
             for index, prompt in enumerate(prompts):
                 if output_format:
                     _formatter = output_format[index]
                 message_data.append({"role": "user", "parts": [prompt]})
                 print(message_data)
                 # message_data.append(prompt)
@@ -289,22 +291,24 @@
                         "role": "model",
                         "parts": [content],
                     }
                 )
                 tokens = exe_model.count_tokens(str(message_data)).total_tokens
                 print(tokens, type(tokens))
                 token_used = token_used + tokens
+                input_tokens += exe_model.count_tokens(prompt)
                 for res in response.candidates:
                     if response.candidates[0].content.parts[0].text:
                         content = response.candidates[0].content.parts[0].text
                     else:
                         content = response.candidates[0].content.parts[0].function_call
                         content = json.dumps(type(content).to_dict(content))
                         content = json.loads(content)
                         content = content["args"]
+                    output_tokens += exe_model.count_tokens(str(content))
                     if output_format:
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(content)
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(content)
                         except AIBridgeException as e:
@@ -333,14 +337,16 @@
                     if index >= len(model_output):
                         model_output.append({"data": [content]})
                     else:
                         model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
+                    "input_tokens": input_tokens,
+                    "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": int(time.time()),
                     "ai_service": "gemini_ai",
                 }
             }
             return message_value
         except AIBridgeException as e:
```

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.2.9/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.2.9/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.2.9/AIBridge/ai_services/openai_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,16 @@
             if not prompts:
                 raise OpenAIException("No prompts provided")
             api_key = api_key if api_key else parse_api_key("open_ai")
             message_data = self.get_prompt_context(context)
             print(message_data)
             model_output = []
             token_used = 0
+            input_tokens = 0
+            output_tokens = 0
             _formatter = "string"
             for index, prompt in enumerate(prompts):
                 if output_format:
                     _formatter = output_format[index]
                 message_data.append({"role": "user", "content": prompt})
                 if _formatter not in ["json", "csv", "xml"]:
                     response = self.execute_text_prompt(
@@ -226,14 +228,16 @@
                         "content": (
                             response.choices[0].message.content
                             if response.choices[0].message.content
                             else response.choices[0].message.function_call.arguments
                         ),
                     }
                 )
+                input_tokens = response.usage.prompt_tokens
+                output_tokens = response.usage.completion_tokens
                 tokens = response.usage.total_tokens
                 token_used = token_used + tokens
                 for res in response.choices:
                     content = (
                         res.message.content
                         if res.message.content
                         else res.message.function_call.arguments
@@ -270,14 +274,16 @@
                     if index >= len(model_output):
                         model_output.append({"data": [content]})
                     else:
                         model_output[index]["data"].append(content)
             message_value = {
                 "items": {
                     "response": model_output,
+                    "input_tokens": input_tokens,
+                    "output_tokens": output_tokens,
                     "token_used": token_used,
                     "created_at": time.time(),
                     "ai_service": "open_ai",
                 }
             }
             return message_value
         except AIBridgeException as e:
```

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.2.9/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.2.9/AIBridge/ai_services/palm_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.2.9/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.2.9/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/constant/common.py` & `aibridge_test-0.2.9/AIBridge/constant/common.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/constant/constant.py` & `aibridge_test-0.2.9/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/database/db_layer.py` & `aibridge_test-0.2.9/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/database/no_sql_service.py` & `aibridge_test-0.2.9/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/database/session.py` & `aibridge_test-0.2.9/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/database/sql_service.py` & `aibridge_test-0.2.9/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/exceptions.py` & `aibridge_test-0.2.9/AIBridge/exceptions.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/output_validation/convertors.py` & `aibridge_test-0.2.9/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/output_validation/validations.py` & `aibridge_test-0.2.9/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.2.9/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.2.9/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.2.9/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.2.9/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.2.9/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.2.9/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/AIBridge/setconfig.py` & `aibridge_test-0.2.9/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/LICENSE` & `aibridge_test-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/PKG-INFO` & `aibridge_test-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.8
+Version: 0.2.9
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.2.8/README.md` & `aibridge_test-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.2.9/aibridge_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.2.8
+Version: 0.2.9
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.2.8/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.2.9/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.2.8/setup.py` & `aibridge_test-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```

