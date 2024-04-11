# Comparing `tmp/llm_optimized_inference-0.1.2-py3-none-any.whl.zip` & `tmp/llm_optimized_inference-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,37 +1,38 @@
-Zip file size: 64182 bytes, number of entries: 35
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-09 00:35 llm/__init__.py
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-09 00:35 llm/optimized/__init__.py
--rw-rw-r--  2.0 unx      703 b- defN 24-Apr-09 00:35 llm/optimized/inference/__init__.py
--rw-rw-r--  2.0 unx      204 b- defN 24-Apr-09 00:35 llm/optimized/inference/_version.py
--rw-rw-r--  2.0 unx    28124 b- defN 24-Apr-09 00:35 llm/optimized/inference/api_server.py
--rw-rw-r--  2.0 unx     3203 b- defN 24-Apr-09 00:35 llm/optimized/inference/configs.py
--rw-rw-r--  2.0 unx     5210 b- defN 24-Apr-09 00:35 llm/optimized/inference/constants.py
--rw-rw-r--  2.0 unx     3255 b- defN 24-Apr-09 00:35 llm/optimized/inference/conversation.py
--rw-rw-r--  2.0 unx     5802 b- defN 24-Apr-09 00:35 llm/optimized/inference/fm_score.py
--rw-rw-r--  2.0 unx      664 b- defN 24-Apr-09 00:35 llm/optimized/inference/logging_config.py
--rw-rw-r--  2.0 unx     9028 b- defN 24-Apr-09 00:35 llm/optimized/inference/managed_inference.py
--rw-rw-r--  2.0 unx     1369 b- defN 24-Apr-09 00:35 llm/optimized/inference/model_config_factory.py
--rw-rw-r--  2.0 unx     6935 b- defN 24-Apr-09 00:35 llm/optimized/inference/model_utils.py
--rw-rw-r--  2.0 unx     1575 b- defN 24-Apr-09 00:35 llm/optimized/inference/prompt_formatter.py
--rw-rw-r--  2.0 unx    12420 b- defN 24-Apr-09 00:35 llm/optimized/inference/replica_manager.py
--rw-rw-r--  2.0 unx    18786 b- defN 24-Apr-09 00:35 llm/optimized/inference/score.py
--rw-rw-r--  2.0 unx     4731 b- defN 24-Apr-09 00:35 llm/optimized/inference/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-09 00:35 llm/optimized/inference/api_server_setup/__init__.py
--rw-rw-r--  2.0 unx     1878 b- defN 24-Apr-09 00:35 llm/optimized/inference/api_server_setup/protocol.py
--rw-rw-r--  2.0 unx      131 b- defN 24-Apr-09 00:35 llm/optimized/inference/custom_model_configurations/__init__.py
--rw-rw-r--  2.0 unx     2725 b- defN 24-Apr-09 00:35 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
--rw-rw-r--  2.0 unx     8520 b- defN 24-Apr-09 00:35 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
--rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-09 00:35 llm/optimized/inference/custom_model_configurations/schema_output.py
--rw-rw-r--  2.0 unx      259 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/__init__.py
--rw-rw-r--  2.0 unx    38577 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/_hf_predictors.py
--rw-rw-r--  2.0 unx     4583 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/engine.py
--rw-rw-r--  2.0 unx     8617 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/hf_engine.py
--rw-rw-r--  2.0 unx    10755 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/mii_engine.py
--rw-rw-r--  2.0 unx     7971 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/mii_engine_v2.py
--rw-rw-r--  2.0 unx    13820 b- defN 24-Apr-09 00:35 llm/optimized/inference/engine/vllm_engine.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3056 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3489 b- defN 24-Apr-09 00:38 llm_optimized_inference-0.1.2.dist-info/RECORD
-35 files, 208031 bytes uncompressed, 58380 bytes compressed:  71.9%
+Zip file size: 66135 bytes, number of entries: 36
+-rw-rw-r--  2.0 unx      249 b- defN 24-Apr-10 23:44 llm/__init__.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-Apr-10 23:44 llm/optimized/__init__.py
+-rw-rw-r--  2.0 unx      703 b- defN 24-Apr-10 23:44 llm/optimized/inference/__init__.py
+-rw-rw-r--  2.0 unx      204 b- defN 24-Apr-10 23:44 llm/optimized/inference/_version.py
+-rw-rw-r--  2.0 unx    28124 b- defN 24-Apr-10 23:44 llm/optimized/inference/api_server.py
+-rw-rw-r--  2.0 unx     3203 b- defN 24-Apr-10 23:44 llm/optimized/inference/configs.py
+-rw-rw-r--  2.0 unx     5210 b- defN 24-Apr-10 23:44 llm/optimized/inference/constants.py
+-rw-rw-r--  2.0 unx     3255 b- defN 24-Apr-10 23:44 llm/optimized/inference/conversation.py
+-rw-rw-r--  2.0 unx     5802 b- defN 24-Apr-10 23:44 llm/optimized/inference/fm_score.py
+-rw-rw-r--  2.0 unx      664 b- defN 24-Apr-10 23:44 llm/optimized/inference/logging_config.py
+-rw-rw-r--  2.0 unx     9028 b- defN 24-Apr-10 23:44 llm/optimized/inference/managed_inference.py
+-rw-rw-r--  2.0 unx     1369 b- defN 24-Apr-10 23:44 llm/optimized/inference/model_config_factory.py
+-rw-rw-r--  2.0 unx     6935 b- defN 24-Apr-10 23:44 llm/optimized/inference/model_utils.py
+-rw-rw-r--  2.0 unx     1575 b- defN 24-Apr-10 23:44 llm/optimized/inference/prompt_formatter.py
+-rw-rw-r--  2.0 unx    12420 b- defN 24-Apr-10 23:44 llm/optimized/inference/replica_manager.py
+-rw-rw-r--  2.0 unx    18786 b- defN 24-Apr-10 23:44 llm/optimized/inference/score.py
+-rw-rw-r--  2.0 unx     4731 b- defN 24-Apr-10 23:44 llm/optimized/inference/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-10 23:44 llm/optimized/inference/api_server_setup/__init__.py
+-rw-rw-r--  2.0 unx     9502 b- defN 24-Apr-10 23:44 llm/optimized/inference/api_server_setup/openapi.json
+-rw-rw-r--  2.0 unx     1878 b- defN 24-Apr-10 23:44 llm/optimized/inference/api_server_setup/protocol.py
+-rw-rw-r--  2.0 unx      131 b- defN 24-Apr-10 23:44 llm/optimized/inference/custom_model_configurations/__init__.py
+-rw-rw-r--  2.0 unx     2725 b- defN 24-Apr-10 23:44 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
+-rw-rw-r--  2.0 unx     8520 b- defN 24-Apr-10 23:44 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-10 23:44 llm/optimized/inference/custom_model_configurations/schema_output.py
+-rw-rw-r--  2.0 unx      259 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/__init__.py
+-rw-rw-r--  2.0 unx    38577 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/_hf_predictors.py
+-rw-rw-r--  2.0 unx     4583 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/engine.py
+-rw-rw-r--  2.0 unx     8617 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/hf_engine.py
+-rw-rw-r--  2.0 unx    10755 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/mii_engine.py
+-rw-rw-r--  2.0 unx     7971 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/mii_engine_v2.py
+-rw-rw-r--  2.0 unx    13820 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/vllm_engine.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3113 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3599 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/RECORD
+36 files, 217700 bytes uncompressed, 60151 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -48,14 +48,17 @@
 
 Filename: llm/optimized/inference/utils.py
 Comment: 
 
 Filename: llm/optimized/inference/api_server_setup/__init__.py
 Comment: 
 
+Filename: llm/optimized/inference/api_server_setup/openapi.json
+Comment: 
+
 Filename: llm/optimized/inference/api_server_setup/protocol.py
 Comment: 
 
 Filename: llm/optimized/inference/custom_model_configurations/__init__.py
 Comment: 
 
 Filename: llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
@@ -84,23 +87,23 @@
 
 Filename: llm/optimized/inference/engine/mii_engine_v2.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/vllm_engine.py
 Comment: 
 
-Filename: llm_optimized_inference-0.1.2.dist-info/LICENSE
+Filename: llm_optimized_inference-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: llm_optimized_inference-0.1.2.dist-info/METADATA
+Filename: llm_optimized_inference-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: llm_optimized_inference-0.1.2.dist-info/WHEEL
+Filename: llm_optimized_inference-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: llm_optimized_inference-0.1.2.dist-info/top_level.txt
+Filename: llm_optimized_inference-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_optimized_inference-0.1.2.dist-info/RECORD
+Filename: llm_optimized_inference-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llm/optimized/inference/_version.py

```diff
@@ -1,5 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
```

## Comparing `llm_optimized_inference-0.1.2.dist-info/METADATA` & `llm_optimized_inference-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: llm-optimized-inference
-Version: 0.1.2
+Version: 0.1.3
 Home-page: 
 Author: Microsoft
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deepspeed ==0.13.2
 Requires-Dist: deepspeed-mii ==0.2.2
-Requires-Dist: vllm ==0.4.0
+Requires-Dist: vllm ==0.4.0.post1
 Requires-Dist: deepspeed-kernels ==0.0.1.dev1698255861
 Requires-Dist: diffusers ==0.26.2
 Requires-Dist: pandas ~=2.1.4
 Requires-Dist: transformers ~=4.39.1
 Requires-Dist: aiolimiter ~=1.1.0
 Requires-Dist: azure-ai-contentsafety ==1.0.0b1
 Requires-Dist: azure-ai-ml ==1.12.1
```

## Comparing `llm_optimized_inference-0.1.2.dist-info/RECORD` & `llm_optimized_inference-0.1.3.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 llm/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/inference/__init__.py,sha256=rGZODP-qE2NOlUgdbmxhfuS3svmx9gM-kU97d9-jb50,703
-llm/optimized/inference/_version.py,sha256=EgFEHvhE7YI4YfTzWfpYE3qjZ-EAK6k428vwZW69OA0,204
+llm/optimized/inference/_version.py,sha256=nyTOHBjjPDYAxYwXKh0e_MQds1g4eK__bGQIqfBzN7U,204
 llm/optimized/inference/api_server.py,sha256=JokKFHQWG6yQKdC_aYhiGX_THF3XI31CdK_Xy47DLYU,28124
 llm/optimized/inference/configs.py,sha256=d5NKbQlfYVkUQ4SL03KVBQekdOG4VrcD0xGxVeHESeQ,3203
 llm/optimized/inference/constants.py,sha256=3JodVG32H9cRiBmyQ2WwFaa41Eh15zNM4T3eyZQFH7k,5210
 llm/optimized/inference/conversation.py,sha256=cBrHv1sI1hrOQB57sSZKAarplKRgqQWqmYxT-wkZHLM,3255
 llm/optimized/inference/fm_score.py,sha256=7z7ZbLMXUXH6gp1-G_l3rOus9r9vSpIm5-wOj5X17aQ,5802
 llm/optimized/inference/logging_config.py,sha256=egtAiGCNVNoU8E_JPhp2aGJVIJ_QkTwLhkNjpVKjICI,664
 llm/optimized/inference/managed_inference.py,sha256=O_HlOPNl24Uoy68gFKrSM_gOG-rg4P_lishBQFAXyC8,9028
 llm/optimized/inference/model_config_factory.py,sha256=EpHH8QyUaE5DC6A5O5nKbie_kMEpfeqmufbOn0U6jFI,1369
 llm/optimized/inference/model_utils.py,sha256=WRo4cmiMlK5tGUd7UDXRJzdXjQi5Lb0uECPijbVPdaQ,6935
 llm/optimized/inference/prompt_formatter.py,sha256=xxM4MbvvPL6jQcLB37uKA9-wCHXTZUL9l5GiUu3r964,1575
 llm/optimized/inference/replica_manager.py,sha256=AUQn9IWFgdsHEQpHDqQVMjnGdZFdzr55IQnVmXFHefA,12420
 llm/optimized/inference/score.py,sha256=RWEaCZ4Akig88ErqshDD8KFCF-YDwMJvsRJjeBWR-WM,18786
 llm/optimized/inference/utils.py,sha256=STENfqDoR8otc2Ig8MN-nERR-y6O6Nl3gpIOZ8A8fbo,4731
 llm/optimized/inference/api_server_setup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+llm/optimized/inference/api_server_setup/openapi.json,sha256=SMtuKvJK58zuxDig48iZ2GMggHxvCpBx5KgYXVAWtoA,9502
 llm/optimized/inference/api_server_setup/protocol.py,sha256=0WmY2-1iQrCsDXXanqIwM7klNBU3skm6tZMxOMPTrWk,1878
 llm/optimized/inference/custom_model_configurations/__init__.py,sha256=D0zlB3WPH212MfcHh1Wz6TRe6Igcg-0Wh0hHA8Kl_l0,131
 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py,sha256=pX9BNG70Rts3TY5p_Smuq4x8ZDG0DG1-6kLfY90Jht0,2725
 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py,sha256=umom7rGh5HBt43iQYWIKJa_gqJqSxfn35Ezu4D7O0-I,8520
 llm/optimized/inference/custom_model_configurations/schema_output.py,sha256=JIpThLkAPoO7MlhaJVSxP2RYVwYzIpw3R3k-nraLq9k,1047
 llm/optimized/inference/engine/__init__.py,sha256=8GqGW53dbRlGShwO11h5HQH4KjnUzoW0t0cChUUFDPY,259
 llm/optimized/inference/engine/_hf_predictors.py,sha256=AwQTIpmOHb7h31H2DF2Jx-9b03lcB5DOrgSbXGpamIk,38577
 llm/optimized/inference/engine/engine.py,sha256=xbpEVJBjovFyACw6WF8uqnmyodRWqb52oaR3s3pr8Sc,4583
 llm/optimized/inference/engine/hf_engine.py,sha256=4rRldNod-pMDJ_-3q0RDWEkigCTr6I62HyJspb01lAs,8617
 llm/optimized/inference/engine/mii_engine.py,sha256=oL426rosTUkhnn7P2K37sEyNLRAvIfNj616jyhDDBjk,10755
 llm/optimized/inference/engine/mii_engine_v2.py,sha256=rI4tjRyj-dCZBDAiN0YNPKMBtkD3MXxcbucuSlHg6lI,7971
 llm/optimized/inference/engine/vllm_engine.py,sha256=fssm9SzWYcxBp4KxxhKORhe4BdsulxXUozNfz5BTRyw,13820
-llm_optimized_inference-0.1.2.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-llm_optimized_inference-0.1.2.dist-info/METADATA,sha256=Im0lHOtg7E5lxinEqyFd16vsBRLb1IlZQRDxFnhJ-SU,3056
-llm_optimized_inference-0.1.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-llm_optimized_inference-0.1.2.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
-llm_optimized_inference-0.1.2.dist-info/RECORD,,
+llm_optimized_inference-0.1.3.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+llm_optimized_inference-0.1.3.dist-info/METADATA,sha256=6H6ShACnFiHk-Du8NG04ZuALNWeKavohRldaKVXziMg,3113
+llm_optimized_inference-0.1.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+llm_optimized_inference-0.1.3.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
+llm_optimized_inference-0.1.3.dist-info/RECORD,,
```

