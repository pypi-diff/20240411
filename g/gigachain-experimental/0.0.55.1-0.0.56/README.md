# Comparing `tmp/gigachain_experimental-0.0.55.1.tar.gz` & `tmp/gigachain_experimental-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_experimental-0.0.55.1.tar", max compression
+gzip compressed data, was "gigachain_experimental-0.0.56.tar", max compression
```

## Comparing `gigachain_experimental-0.0.55.1.tar` & `gigachain_experimental-0.0.56.tar`

### file list

```diff
@@ -1,150 +1,159 @@
--rw-r--r--   0        0        0     1067 2024-03-14 13:23:46.793403 gigachain_experimental-0.0.55.1/LICENSE
--rw-r--r--   0        0        0      731 2023-10-06 15:21:09.714881 gigachain_experimental-0.0.55.1/README.md
--rw-r--r--   0        0        0      271 2024-03-14 13:23:46.793978 gigachain_experimental-0.0.55.1/langchain_experimental/__init__.py
--rw-r--r--   0        0        0      643 2024-03-28 09:36:51.652536 gigachain_experimental-0.0.55.1/langchain_experimental/agents/__init__.py
--rw-r--r--   0        0        0      653 2024-03-14 13:23:46.794474 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       19 2024-03-14 13:23:46.794818 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0     2407 2024-03-14 13:23:46.795018 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/csv/base.py
--rw-r--r--   0        0        0       22 2024-03-14 13:23:46.795255 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0    11290 2024-03-28 09:36:51.653497 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/base.py
--rw-r--r--   0        0        0     1113 2024-03-14 13:23:46.795892 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/prompt.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:46.796139 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0     2224 2024-03-14 13:23:46.796434 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/base.py
--rw-r--r--   0        0        0      513 2024-03-14 13:23:46.796678 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/prompt.py
--rw-r--r--   0        0        0       20 2024-03-14 13:23:46.797026 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0     2761 2024-03-14 13:23:46.797378 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/spark/base.py
--rw-r--r--   0        0        0      295 2024-03-14 13:23:46.797631 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/spark/prompt.py
--rw-r--r--   0        0        0       23 2024-03-14 13:23:46.797989 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0     3143 2024-03-14 13:23:46.798282 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/base.py
--rw-r--r--   0        0        0     1070 2024-03-14 13:23:46.798536 gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py
--rw-r--r--   0        0        0      866 2024-03-28 09:36:51.653973 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.140059 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5443 2024-03-14 13:23:46.799095 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1164 2024-03-14 13:23:46.799560 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1909 2024-03-14 13:23:46.799976 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     5000 2024-03-14 13:23:46.800435 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     7963 2024-03-14 13:23:46.800907 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-09-14 13:23:58.140895 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     8687 2024-03-14 13:23:46.801553 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1668 2024-03-28 09:36:51.654888 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      967 2024-03-28 09:36:51.655786 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1283 2024-03-28 09:36:51.656463 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.141519 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-14 13:23:46.803494 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
--rw-r--r--   0        0        0     1742 2024-03-28 09:36:51.657200 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
--rw-r--r--   0        0        0     4598 2024-03-14 13:23:46.804390 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
--rw-r--r--   0        0        0     7859 2024-03-14 13:23:46.804893 gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
--rw-r--r--   0        0        0      674 2024-03-28 09:36:51.657715 gigachain_experimental-0.0.55.1/langchain_experimental/chat_models/__init__.py
--rw-r--r--   0        0        0     6063 2024-03-28 09:36:51.658161 gigachain_experimental-0.0.55.1/langchain_experimental/chat_models/llm_wrapper.py
--rw-r--r--   0        0        0     2190 2024-03-28 09:36:51.658590 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/__init__.py
--rw-r--r--   0        0        0     6659 2024-03-14 13:23:46.807228 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py
--rw-r--r--   0        0        0     7411 2024-03-14 13:23:46.807736 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation.py
--rw-r--r--   0        0        0     2390 2024-03-14 13:23:46.808072 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py
--rw-r--r--   0        0        0     1614 2024-03-14 13:23:46.808388 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_config.py
--rw-r--r--   0        0        0      192 2023-09-14 13:23:58.142645 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_enums.py
--rw-r--r--   0        0        0     1054 2024-03-14 13:23:46.808784 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py
--rw-r--r--   0        0        0     6834 2024-03-14 13:23:46.809097 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/pii.py
--rw-r--r--   0        0        0     3142 2024-03-14 13:23:46.809305 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/prompt_safety.py
--rw-r--r--   0        0        0     8134 2024-03-14 13:23:46.809624 gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/toxicity.py
--rw-r--r--   0        0        0      103 2023-10-03 14:29:06.367456 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/README.md
--rw-r--r--   0        0        0      750 2024-03-28 09:36:51.658918 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/__init__.py
--rw-r--r--   0        0        0    11087 2024-03-14 13:23:46.809990 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/base.py
--rw-r--r--   0        0        0      246 2023-09-14 13:23:58.143626 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/constants.py
--rw-r--r--   0        0        0     9183 2024-03-14 13:23:46.810525 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.143845 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.144036 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2548 2024-03-14 13:23:46.811061 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      853 2024-03-14 13:23:46.811497 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     2905 2024-03-14 13:23:46.811993 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     5468 2024-03-14 13:23:46.812441 gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      631 2024-03-28 09:36:51.659356 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-14 13:23:46.813062 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/base.py
--rw-r--r--   0        0        0     4793 2024-03-14 13:23:46.813631 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/deanonymizer_mapping.py
--rw-r--r--   0        0        0     6801 2024-03-14 13:23:46.814004 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py
--rw-r--r--   0        0        0     2861 2024-03-14 13:23:46.814331 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/faker_presidio_mapping.py
--rw-r--r--   0        0        0    17162 2024-03-14 13:23:46.814652 gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/presidio.py
--rw-r--r--   0        0        0      368 2024-03-28 09:36:51.659603 gigachain_experimental-0.0.55.1/langchain_experimental/fallacy_removal/__init__.py
--rw-r--r--   0        0        0      263 2024-03-28 09:36:51.660007 gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10252 2024-03-28 09:36:51.660456 gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    13413 2024-03-28 09:36:51.661467 gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      308 2024-03-28 09:36:51.661909 gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/__init__.py
--rw-r--r--   0        0        0    10723 2024-03-28 09:36:51.662387 gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/diffbot.py
--rw-r--r--   0        0        0    12290 2024-03-28 09:36:51.662690 gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/llm.py
--rw-r--r--   0        0        0       94 2024-03-28 09:36:51.663096 gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/__init__.py
--rw-r--r--   0        0        0     4454 2024-03-14 13:23:46.816866 gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/base.py
--rw-r--r--   0        0        0     5708 2024-03-14 13:23:46.817282 gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/bash.py
--rw-r--r--   0        0        0     2038 2024-03-14 13:23:46.817632 gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/prompt.py
--rw-r--r--   0        0        0      164 2024-03-28 09:36:51.663490 gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0     5791 2024-03-14 13:23:46.818120 gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/base.py
--rw-r--r--   0        0        0     1087 2023-10-06 15:21:09.721677 gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/prompt.py
--rw-r--r--   0        0        0      453 2024-03-28 09:36:51.663878 gigachain_experimental-0.0.55.1/langchain_experimental/llms/__init__.py
--rw-r--r--   0        0        0     8768 2024-03-28 09:36:51.664630 gigachain_experimental-0.0.55.1/langchain_experimental/llms/anthropic_functions.py
--rw-r--r--   0        0        0     2228 2024-03-14 13:23:46.820107 gigachain_experimental-0.0.55.1/langchain_experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     4344 2024-03-14 13:23:46.820880 gigachain_experimental-0.0.55.1/langchain_experimental/llms/llamaapi.py
--rw-r--r--   0        0        0     2843 2024-03-14 13:23:46.821460 gigachain_experimental-0.0.55.1/langchain_experimental/llms/lmformatenforcer_decoder.py
--rw-r--r--   0        0        0     4932 2024-03-14 13:23:46.821957 gigachain_experimental-0.0.55.1/langchain_experimental/llms/ollama_functions.py
--rw-r--r--   0        0        0     2342 2024-03-14 13:23:46.822538 gigachain_experimental-0.0.55.1/langchain_experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      346 2024-03-28 09:36:51.665067 gigachain_experimental-0.0.55.1/langchain_experimental/open_clip/__init__.py
--rw-r--r--   0        0        0     3383 2024-03-14 13:23:46.823943 gigachain_experimental-0.0.55.1/langchain_experimental/open_clip/open_clip.py
--rw-r--r--   0        0        0      120 2024-03-14 13:23:46.824923 gigachain_experimental-0.0.55.1/langchain_experimental/openai_assistant/__init__.py
--rw-r--r--   0        0        0      185 2024-03-14 13:23:46.825679 gigachain_experimental-0.0.55.1/langchain_experimental/openai_assistant/base.py
--rw-r--r--   0        0        0      330 2024-03-28 09:36:51.665470 gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    13320 2024-03-14 13:23:46.826384 gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/base.py
--rw-r--r--   0        0        0     3537 2023-09-14 13:23:58.147176 gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     5767 2023-09-14 13:23:58.147272 gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      488 2024-03-28 09:36:51.665891 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     3570 2023-09-14 13:23:58.147536 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.147634 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1463 2024-03-14 13:23:46.826994 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1269 2023-09-14 13:23:58.147861 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.147962 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1567 2023-09-14 13:23:58.148116 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     2314 2024-03-14 13:23:46.827423 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1439 2024-03-14 13:23:46.827784 gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0      369 2024-03-28 09:36:51.666293 gigachain_experimental-0.0.55.1/langchain_experimental/prompt_injection_identifier/__init__.py
--rw-r--r--   0        0        0     3369 2024-03-28 09:36:51.666703 gigachain_experimental-0.0.55.1/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py
--rw-r--r--   0        0        0      174 2024-03-28 09:36:51.667078 gigachain_experimental-0.0.55.1/langchain_experimental/prompts/__init__.py
--rw-r--r--   0        0        0     1942 2024-03-14 13:23:46.828890 gigachain_experimental-0.0.55.1/langchain_experimental/prompts/load.py
--rw-r--r--   0        0        0        0 2023-09-14 13:23:58.148908 gigachain_experimental-0.0.55.1/langchain_experimental/py.typed
--rw-r--r--   0        0        0     1285 2023-09-14 13:23:58.149124 gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      548 2023-09-14 13:23:58.149226 gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      520 2023-09-14 13:23:58.149317 gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/main.py
--rw-r--r--   0        0        0      518 2024-03-28 09:36:51.667459 gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/__init__.py
--rw-r--r--   0        0        0     7967 2024-03-28 09:36:51.667839 gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/amazon_personalize.py
--rw-r--r--   0        0        0     6964 2024-03-14 13:23:46.829648 gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/amazon_personalize_chain.py
--rw-r--r--   0        0        0      200 2024-03-28 09:36:51.668184 gigachain_experimental-0.0.55.1/langchain_experimental/retrievers/__init__.py
--rw-r--r--   0        0        0     1248 2024-03-14 13:23:46.830070 gigachain_experimental-0.0.55.1/langchain_experimental/retrievers/vector_sql_database.py
--rw-r--r--   0        0        0     1447 2024-03-28 09:36:51.668550 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/__init__.py
--rw-r--r--   0        0        0    23241 2024-03-14 13:23:46.830706 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/base.py
--rw-r--r--   0        0        0     1989 2024-03-14 13:23:46.831066 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/metrics.py
--rw-r--r--   0        0        0     2126 2024-03-14 13:23:46.831366 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/model_repository.py
--rw-r--r--   0        0        0    16279 2024-03-14 13:23:46.831741 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/pick_best_chain.py
--rw-r--r--   0        0        0      556 2024-03-14 13:23:46.832050 gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/vw_logger.py
--rw-r--r--   0        0        0      946 2024-03-28 09:36:51.668927 gigachain_experimental-0.0.55.1/langchain_experimental/smart_llm/__init__.py
--rw-r--r--   0        0        0    14423 2024-03-14 13:23:46.832807 gigachain_experimental-0.0.55.1/langchain_experimental/smart_llm/base.py
--rw-r--r--   0        0        0      202 2024-03-28 09:36:51.669275 gigachain_experimental-0.0.55.1/langchain_experimental/sql/__init__.py
--rw-r--r--   0        0        0    13112 2024-03-14 13:23:46.833225 gigachain_experimental-0.0.55.1/langchain_experimental/sql/base.py
--rw-r--r--   0        0        0     4658 2023-09-25 11:47:07.505993 gigachain_experimental-0.0.55.1/langchain_experimental/sql/prompt.py
--rw-r--r--   0        0        0     9846 2024-03-14 13:23:46.833581 gigachain_experimental-0.0.55.1/langchain_experimental/sql/vector_sql.py
--rw-r--r--   0        0        0     1576 2024-03-28 09:36:51.669999 gigachain_experimental-0.0.55.1/langchain_experimental/synthetic_data/__init__.py
--rw-r--r--   0        0        0      459 2023-09-25 11:47:07.506582 gigachain_experimental-0.0.55.1/langchain_experimental/synthetic_data/prompts.py
--rw-r--r--   0        0        0       75 2024-03-28 09:36:51.670326 gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/__init__.py
--rw-r--r--   0        0        0     5341 2024-03-14 13:23:46.834246 gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/base.py
--rw-r--r--   0        0        0     2523 2024-03-28 09:36:51.670695 gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/openai.py
--rw-r--r--   0        0        0      412 2023-10-02 10:00:42.632968 gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/prompts.py
--rw-r--r--   0        0        0     9717 2024-03-28 09:36:51.671475 gigachain_experimental-0.0.55.1/langchain_experimental/text_splitter.py
--rw-r--r--   0        0        0      180 2024-03-28 09:36:51.671871 gigachain_experimental-0.0.55.1/langchain_experimental/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 13:23:46.835906 gigachain_experimental-0.0.55.1/langchain_experimental/tools/python/__init__.py
--rw-r--r--   0        0        0     4763 2024-03-14 13:23:46.836127 gigachain_experimental-0.0.55.1/langchain_experimental/tools/python/tool.py
--rw-r--r--   0        0        0      425 2024-03-28 09:36:51.672261 gigachain_experimental-0.0.55.1/langchain_experimental/tot/__init__.py
--rw-r--r--   0        0        0     4853 2024-03-14 13:23:46.836804 gigachain_experimental-0.0.55.1/langchain_experimental/tot/base.py
--rw-r--r--   0        0        0     1405 2023-09-14 13:23:58.150719 gigachain_experimental-0.0.55.1/langchain_experimental/tot/checker.py
--rw-r--r--   0        0        0     1666 2023-09-14 13:23:58.150815 gigachain_experimental-0.0.55.1/langchain_experimental/tot/controller.py
--rw-r--r--   0        0        0     1467 2024-03-14 13:23:46.837178 gigachain_experimental-0.0.55.1/langchain_experimental/tot/memory.py
--rw-r--r--   0        0        0     4797 2024-03-28 09:36:51.672937 gigachain_experimental-0.0.55.1/langchain_experimental/tot/prompts.py
--rw-r--r--   0        0        0      504 2024-03-14 13:23:46.837821 gigachain_experimental-0.0.55.1/langchain_experimental/tot/thought.py
--rw-r--r--   0        0        0     3118 2024-03-14 13:23:46.838108 gigachain_experimental-0.0.55.1/langchain_experimental/tot/thought_generation.py
--rw-r--r--   0        0        0      148 2024-03-28 09:36:51.673359 gigachain_experimental-0.0.55.1/langchain_experimental/utilities/__init__.py
--rw-r--r--   0        0        0     2154 2024-03-14 13:23:46.838528 gigachain_experimental-0.0.55.1/langchain_experimental/utilities/python.py
--rw-r--r--   0        0        0     3926 2024-04-03 12:54:10.693476 gigachain_experimental-0.0.55.1/pyproject.toml
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 gigachain_experimental-0.0.55.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-12-18 12:05:46.761829 gigachain_experimental-0.0.56/LICENSE
+-rw-r--r--   0        0        0      731 2023-10-06 14:43:01.321479 gigachain_experimental-0.0.56/README.md
+-rw-r--r--   0        0        0      271 2023-10-19 12:57:52.560036 gigachain_experimental-0.0.56/langchain_experimental/__init__.py
+-rw-r--r--   0        0        0      643 2024-03-28 12:44:20.382264 gigachain_experimental-0.0.56/langchain_experimental/agents/__init__.py
+-rw-r--r--   0        0        0      653 2023-11-10 13:07:49.949600 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       19 2023-10-30 16:05:53.796780 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0     2407 2024-02-22 08:54:03.015149 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/csv/base.py
+-rw-r--r--   0        0        0       22 2023-10-19 12:57:52.561598 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0    11290 2024-03-28 12:44:20.383718 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/pandas/base.py
+-rw-r--r--   0        0        0     1113 2023-10-19 12:57:52.562307 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/pandas/prompt.py
+-rw-r--r--   0        0        0        0 2023-10-19 12:57:52.562706 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0     2224 2024-01-18 15:16:40.505131 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/python/base.py
+-rw-r--r--   0        0        0      513 2023-10-19 12:57:52.563558 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/python/prompt.py
+-rw-r--r--   0        0        0       20 2023-10-19 12:57:52.564007 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0     2761 2024-01-18 15:16:40.506986 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/spark/base.py
+-rw-r--r--   0        0        0      295 2023-10-19 12:57:52.565847 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/spark/prompt.py
+-rw-r--r--   0        0        0       23 2023-10-19 12:57:52.566362 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0     3143 2024-01-18 15:16:40.507943 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/xorbits/base.py
+-rw-r--r--   0        0        0     1070 2023-10-19 12:57:52.567043 gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py
+-rw-r--r--   0        0        0      866 2024-03-28 12:44:20.384386 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.490847 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5443 2024-03-28 12:44:20.386884 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1164 2024-02-22 08:54:03.020154 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1909 2024-03-28 12:44:20.391604 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     5000 2024-02-22 08:54:03.022979 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     7963 2024-03-28 12:44:20.393342 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-08-21 13:51:28.493975 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     8687 2024-02-22 08:54:03.024294 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1668 2024-03-28 12:44:20.393983 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      967 2024-03-28 12:44:20.394699 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1283 2024-03-28 12:44:20.395266 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.495536 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
+-rw-r--r--   0        0        0     1133 2024-03-28 12:44:20.397027 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
+-rw-r--r--   0        0        0     1742 2024-03-28 12:44:20.397664 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
+-rw-r--r--   0        0        0     4598 2024-03-28 12:44:20.399096 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
+-rw-r--r--   0        0        0     7859 2024-03-28 12:44:20.400788 gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
+-rw-r--r--   0        0        0      674 2024-03-28 12:44:20.401473 gigachain_experimental-0.0.56/langchain_experimental/chat_models/__init__.py
+-rw-r--r--   0        0        0     6063 2024-03-28 12:44:20.402985 gigachain_experimental-0.0.56/langchain_experimental/chat_models/llm_wrapper.py
+-rw-r--r--   0        0        0     2190 2024-03-28 12:44:20.403904 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/__init__.py
+-rw-r--r--   0        0        0     6664 2024-04-10 08:38:06.859348 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py
+-rw-r--r--   0        0        0     7411 2024-03-28 12:44:20.406460 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation.py
+-rw-r--r--   0        0        0     2390 2024-03-28 12:44:20.407747 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py
+-rw-r--r--   0        0        0     1614 2024-03-28 12:44:20.409023 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation_config.py
+-rw-r--r--   0        0        0      192 2023-09-04 05:57:22.495380 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation_enums.py
+-rw-r--r--   0        0        0     1054 2024-03-28 12:44:20.409588 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py
+-rw-r--r--   0        0        0     6834 2024-03-28 12:44:20.410890 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/pii.py
+-rw-r--r--   0        0        0     3142 2024-03-28 12:44:20.411826 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/prompt_safety.py
+-rw-r--r--   0        0        0     8134 2024-03-28 12:44:20.413206 gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/toxicity.py
+-rw-r--r--   0        0        0      103 2023-10-03 07:51:15.765558 gigachain_experimental-0.0.56/langchain_experimental/cpal/README.md
+-rw-r--r--   0        0        0      750 2024-03-28 12:44:20.413845 gigachain_experimental-0.0.56/langchain_experimental/cpal/__init__.py
+-rw-r--r--   0        0        0    11087 2024-03-28 12:44:20.415084 gigachain_experimental-0.0.56/langchain_experimental/cpal/base.py
+-rw-r--r--   0        0        0      246 2023-08-21 13:51:28.498799 gigachain_experimental-0.0.56/langchain_experimental/cpal/constants.py
+-rw-r--r--   0        0        0     9183 2024-03-28 12:44:20.416997 gigachain_experimental-0.0.56/langchain_experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499460 gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.499832 gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2548 2023-10-19 12:57:52.577909 gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      853 2023-10-19 12:57:52.579560 gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     2905 2023-10-19 12:57:52.581896 gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     5468 2023-10-19 12:57:52.583797 gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      631 2024-03-28 12:44:20.417734 gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/__init__.py
+-rw-r--r--   0        0        0     1811 2024-03-28 12:44:20.419349 gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/base.py
+-rw-r--r--   0        0        0     4793 2024-03-28 12:44:20.420547 gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/deanonymizer_mapping.py
+-rw-r--r--   0        0        0     6801 2024-03-28 12:44:20.421773 gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py
+-rw-r--r--   0        0        0     2861 2024-03-28 12:44:20.422573 gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/faker_presidio_mapping.py
+-rw-r--r--   0        0        0    17162 2024-03-28 12:44:20.423295 gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/presidio.py
+-rw-r--r--   0        0        0      368 2024-03-28 12:44:20.423942 gigachain_experimental-0.0.56/langchain_experimental/fallacy_removal/__init__.py
+-rw-r--r--   0        0        0      263 2024-03-28 12:44:20.424513 gigachain_experimental-0.0.56/langchain_experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10252 2024-03-28 12:44:20.425251 gigachain_experimental-0.0.56/langchain_experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    13413 2024-03-28 12:44:20.425996 gigachain_experimental-0.0.56/langchain_experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      308 2024-03-28 12:44:20.426581 gigachain_experimental-0.0.56/langchain_experimental/graph_transformers/__init__.py
+-rw-r--r--   0        0        0    10723 2024-03-28 12:44:20.427932 gigachain_experimental-0.0.56/langchain_experimental/graph_transformers/diffbot.py
+-rw-r--r--   0        0        0    12871 2024-04-10 08:38:06.859994 gigachain_experimental-0.0.56/langchain_experimental/graph_transformers/llm.py
+-rw-r--r--   0        0        0       94 2024-03-28 12:44:20.429416 gigachain_experimental-0.0.56/langchain_experimental/llm_bash/__init__.py
+-rw-r--r--   0        0        0     4454 2024-01-18 15:16:40.536504 gigachain_experimental-0.0.56/langchain_experimental/llm_bash/base.py
+-rw-r--r--   0        0        0     5708 2024-03-28 12:44:20.431110 gigachain_experimental-0.0.56/langchain_experimental/llm_bash/bash.py
+-rw-r--r--   0        0        0     2038 2024-03-28 12:44:20.431773 gigachain_experimental-0.0.56/langchain_experimental/llm_bash/prompt.py
+-rw-r--r--   0        0        0      164 2024-03-28 12:44:20.432361 gigachain_experimental-0.0.56/langchain_experimental/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0     5791 2024-03-28 12:44:20.433601 gigachain_experimental-0.0.56/langchain_experimental/llm_symbolic_math/base.py
+-rw-r--r--   0        0        0     1087 2023-10-06 14:43:01.344104 gigachain_experimental-0.0.56/langchain_experimental/llm_symbolic_math/prompt.py
+-rw-r--r--   0        0        0      453 2024-03-28 12:44:20.434660 gigachain_experimental-0.0.56/langchain_experimental/llms/__init__.py
+-rw-r--r--   0        0        0     8768 2024-03-28 12:44:20.436322 gigachain_experimental-0.0.56/langchain_experimental/llms/anthropic_functions.py
+-rw-r--r--   0        0        0     2228 2024-03-28 12:44:20.438106 gigachain_experimental-0.0.56/langchain_experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     4344 2024-03-28 12:44:20.439958 gigachain_experimental-0.0.56/langchain_experimental/llms/llamaapi.py
+-rw-r--r--   0        0        0     2843 2024-03-28 12:44:20.440627 gigachain_experimental-0.0.56/langchain_experimental/llms/lmformatenforcer_decoder.py
+-rw-r--r--   0        0        0     4932 2024-03-28 12:44:20.441319 gigachain_experimental-0.0.56/langchain_experimental/llms/ollama_functions.py
+-rw-r--r--   0        0        0     2342 2024-03-28 12:44:20.441799 gigachain_experimental-0.0.56/langchain_experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      346 2024-03-28 12:44:20.442410 gigachain_experimental-0.0.56/langchain_experimental/open_clip/__init__.py
+-rw-r--r--   0        0        0     3383 2024-03-28 12:44:20.442806 gigachain_experimental-0.0.56/langchain_experimental/open_clip/open_clip.py
+-rw-r--r--   0        0        0      120 2023-11-10 13:07:49.953805 gigachain_experimental-0.0.56/langchain_experimental/openai_assistant/__init__.py
+-rw-r--r--   0        0        0      185 2023-11-15 10:30:09.322265 gigachain_experimental-0.0.56/langchain_experimental/openai_assistant/base.py
+-rw-r--r--   0        0        0      330 2024-03-28 12:44:20.443329 gigachain_experimental-0.0.56/langchain_experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    13320 2024-03-28 12:44:20.444258 gigachain_experimental-0.0.56/langchain_experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     3537 2023-08-21 13:51:28.506235 gigachain_experimental-0.0.56/langchain_experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     5767 2023-08-21 13:51:28.506905 gigachain_experimental-0.0.56/langchain_experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      488 2024-03-28 12:44:20.444965 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     3570 2023-08-21 13:51:28.507952 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.508275 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1463 2024-01-18 15:16:40.555727 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1269 2023-08-21 13:51:28.508950 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-08-21 13:51:28.509270 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1567 2023-08-21 13:51:28.509627 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     2314 2024-01-18 15:16:40.558911 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1439 2024-03-28 12:44:20.445521 gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0      369 2024-03-28 12:44:20.446237 gigachain_experimental-0.0.56/langchain_experimental/prompt_injection_identifier/__init__.py
+-rw-r--r--   0        0        0     3369 2024-03-28 12:44:20.447465 gigachain_experimental-0.0.56/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py
+-rw-r--r--   0        0        0      174 2024-03-28 12:44:20.448585 gigachain_experimental-0.0.56/langchain_experimental/prompts/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-10 08:38:06.860353 gigachain_experimental-0.0.56/langchain_experimental/prompts/load.py
+-rw-r--r--   0        0        0        0 2023-08-22 08:04:55.368181 gigachain_experimental-0.0.56/langchain_experimental/py.typed
+-rw-r--r--   0        0        0     1285 2023-08-24 07:36:02.836411 gigachain_experimental-0.0.56/langchain_experimental/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      548 2023-08-24 07:36:02.836900 gigachain_experimental-0.0.56/langchain_experimental/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      520 2023-08-24 07:36:02.837404 gigachain_experimental-0.0.56/langchain_experimental/pydantic_v1/main.py
+-rw-r--r--   0        0        0      518 2024-03-28 12:44:20.449970 gigachain_experimental-0.0.56/langchain_experimental/recommenders/__init__.py
+-rw-r--r--   0        0        0     7967 2024-03-28 12:44:20.450624 gigachain_experimental-0.0.56/langchain_experimental/recommenders/amazon_personalize.py
+-rw-r--r--   0        0        0     6964 2024-03-28 12:44:20.451327 gigachain_experimental-0.0.56/langchain_experimental/recommenders/amazon_personalize_chain.py
+-rw-r--r--   0        0        0      200 2024-03-28 12:44:20.452015 gigachain_experimental-0.0.56/langchain_experimental/retrievers/__init__.py
+-rw-r--r--   0        0        0     1248 2024-03-28 12:44:20.453407 gigachain_experimental-0.0.56/langchain_experimental/retrievers/vector_sql_database.py
+-rw-r--r--   0        0        0     1447 2024-03-28 12:44:20.454189 gigachain_experimental-0.0.56/langchain_experimental/rl_chain/__init__.py
+-rw-r--r--   0        0        0    23241 2024-03-28 12:44:20.455891 gigachain_experimental-0.0.56/langchain_experimental/rl_chain/base.py
+-rw-r--r--   0        0        0     1989 2024-03-28 12:44:20.456634 gigachain_experimental-0.0.56/langchain_experimental/rl_chain/metrics.py
+-rw-r--r--   0        0        0     2126 2024-03-28 12:44:20.457637 gigachain_experimental-0.0.56/langchain_experimental/rl_chain/model_repository.py
+-rw-r--r--   0        0        0    16279 2024-03-28 12:44:20.459002 gigachain_experimental-0.0.56/langchain_experimental/rl_chain/pick_best_chain.py
+-rw-r--r--   0        0        0      556 2024-03-28 12:44:20.459800 gigachain_experimental-0.0.56/langchain_experimental/rl_chain/vw_logger.py
+-rw-r--r--   0        0        0      946 2024-03-28 12:44:20.460545 gigachain_experimental-0.0.56/langchain_experimental/smart_llm/__init__.py
+-rw-r--r--   0        0        0    14423 2024-03-28 12:44:20.462679 gigachain_experimental-0.0.56/langchain_experimental/smart_llm/base.py
+-rw-r--r--   0        0        0      202 2024-03-28 12:44:20.463580 gigachain_experimental-0.0.56/langchain_experimental/sql/__init__.py
+-rw-r--r--   0        0        0    13247 2024-04-10 08:38:06.861007 gigachain_experimental-0.0.56/langchain_experimental/sql/base.py
+-rw-r--r--   0        0        0     4658 2023-09-25 07:40:35.486005 gigachain_experimental-0.0.56/langchain_experimental/sql/prompt.py
+-rw-r--r--   0        0        0     9846 2024-03-28 12:44:20.464697 gigachain_experimental-0.0.56/langchain_experimental/sql/vector_sql.py
+-rw-r--r--   0        0        0     1576 2024-03-28 12:44:20.465321 gigachain_experimental-0.0.56/langchain_experimental/synthetic_data/__init__.py
+-rw-r--r--   0        0        0      459 2023-09-25 07:40:35.486981 gigachain_experimental-0.0.56/langchain_experimental/synthetic_data/prompts.py
+-rw-r--r--   0        0        0       75 2024-03-28 12:44:20.465865 gigachain_experimental-0.0.56/langchain_experimental/tabular_synthetic_data/__init__.py
+-rw-r--r--   0        0        0     5341 2024-03-28 12:44:20.466662 gigachain_experimental-0.0.56/langchain_experimental/tabular_synthetic_data/base.py
+-rw-r--r--   0        0        0     2523 2024-03-28 12:44:20.467247 gigachain_experimental-0.0.56/langchain_experimental/tabular_synthetic_data/openai.py
+-rw-r--r--   0        0        0      412 2023-10-03 07:51:15.769901 gigachain_experimental-0.0.56/langchain_experimental/tabular_synthetic_data/prompts.py
+-rw-r--r--   0        0        0     9717 2024-03-28 12:44:20.468288 gigachain_experimental-0.0.56/langchain_experimental/text_splitter.py
+-rw-r--r--   0        0        0      180 2024-03-28 12:44:20.469622 gigachain_experimental-0.0.56/langchain_experimental/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-19 12:57:52.604149 gigachain_experimental-0.0.56/langchain_experimental/tools/python/__init__.py
+-rw-r--r--   0        0        0     4763 2024-03-28 12:44:20.471048 gigachain_experimental-0.0.56/langchain_experimental/tools/python/tool.py
+-rw-r--r--   0        0        0      425 2024-03-28 12:44:20.471866 gigachain_experimental-0.0.56/langchain_experimental/tot/__init__.py
+-rw-r--r--   0        0        0     4853 2024-03-28 12:44:20.473425 gigachain_experimental-0.0.56/langchain_experimental/tot/base.py
+-rw-r--r--   0        0        0     1405 2023-08-21 13:51:28.514934 gigachain_experimental-0.0.56/langchain_experimental/tot/checker.py
+-rw-r--r--   0        0        0     1666 2023-08-21 13:51:28.515184 gigachain_experimental-0.0.56/langchain_experimental/tot/controller.py
+-rw-r--r--   0        0        0     1467 2024-03-28 12:44:20.474461 gigachain_experimental-0.0.56/langchain_experimental/tot/memory.py
+-rw-r--r--   0        0        0     4797 2024-03-28 12:44:20.475292 gigachain_experimental-0.0.56/langchain_experimental/tot/prompts.py
+-rw-r--r--   0        0        0      504 2024-03-28 12:44:20.475874 gigachain_experimental-0.0.56/langchain_experimental/tot/thought.py
+-rw-r--r--   0        0        0     3118 2024-03-28 12:44:20.476518 gigachain_experimental-0.0.56/langchain_experimental/tot/thought_generation.py
+-rw-r--r--   0        0        0      148 2024-03-28 12:44:20.477224 gigachain_experimental-0.0.56/langchain_experimental/utilities/__init__.py
+-rw-r--r--   0        0        0     2154 2023-10-19 12:57:52.605471 gigachain_experimental-0.0.56/langchain_experimental/utilities/python.py
+-rw-r--r--   0        0        0      114 2024-04-10 08:38:06.861195 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/__init__.py
+-rw-r--r--   0        0        0     5034 2024-04-10 08:38:06.861410 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/base.py
+-rw-r--r--   0        0        0     4880 2024-04-10 08:38:06.861624 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/models.py
+-rw-r--r--   0        0        0     4369 2024-04-10 08:38:06.861878 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/prompts.py
+-rw-r--r--   0        0        0     3191 2024-04-10 08:38:06.862082 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/services/audio_service.py
+-rw-r--r--   0        0        0    11296 2024-04-10 08:38:06.862336 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/services/caption_service.py
+-rw-r--r--   0        0        0     4927 2024-04-10 08:38:06.862556 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/services/combine_service.py
+-rw-r--r--   0        0        0     3773 2024-04-10 08:38:06.862736 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/services/image_service.py
+-rw-r--r--   0        0        0      459 2024-04-10 08:38:06.862899 gigachain_experimental-0.0.56/langchain_experimental/video_captioning/services/srt_service.py
+-rw-r--r--   0        0        0     3951 2024-04-10 14:24:00.611813 gigachain_experimental-0.0.56/pyproject.toml
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 gigachain_experimental-0.0.56/PKG-INFO
```

### Comparing `gigachain_experimental-0.0.55.1/LICENSE` & `gigachain_experimental-0.0.56/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/README.md` & `gigachain_experimental-0.0.56/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/csv/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/csv/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/pandas/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/pandas/prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/pandas/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/python/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/python/prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/python/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/spark/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/spark/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/xorbits/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/agents/agent_toolkits/xorbits/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/agent.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/agent.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/memory.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/output_parser.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_creation.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_execution.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py` & `gigachain_experimental-0.0.56/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/chat_models/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/chat_models/llm_wrapper.py` & `gigachain_experimental-0.0.56/langchain_experimental/chat_models/llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/amazon_comprehend_moderation.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 "Could not import boto3 python package. "
                 "Please install it with `pip install boto3`."
             )
         except Exception as e:
             raise ValueError(
                 "Could not load credentials to authenticate with AWS client. "
                 "Please check that credentials in the specified "
-                "profile name are valid."
+                f"profile name are valid. {e}"
             ) from e
 
     @property
     def output_keys(self) -> List[str]:
         """
         Returns a list of output keys.
```

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation_callbacks.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_config.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation_config.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/base_moderation_exceptions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/pii.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/pii.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/prompt_safety.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/prompt_safety.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/comprehend_moderation/toxicity.py` & `gigachain_experimental-0.0.56/langchain_experimental/comprehend_moderation/toxicity.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/cpal/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/cpal/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/models.py` & `gigachain_experimental-0.0.56/langchain_experimental/cpal/models.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/causal.py` & `gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/intervention.py` & `gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/narrative.py` & `gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/cpal/templates/univariate/query.py` & `gigachain_experimental-0.0.56/langchain_experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/deanonymizer_mapping.py` & `gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/deanonymizer_mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py` & `gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/deanonymizer_matching_strategies.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/faker_presidio_mapping.py` & `gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/faker_presidio_mapping.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/data_anonymizer/presidio.py` & `gigachain_experimental-0.0.56/langchain_experimental/data_anonymizer/presidio.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/generative_agent.py` & `gigachain_experimental-0.0.56/langchain_experimental/generative_agents/generative_agent.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/generative_agents/memory.py` & `gigachain_experimental-0.0.56/langchain_experimental/generative_agents/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/diffbot.py` & `gigachain_experimental-0.0.56/langchain_experimental/graph_transformers/diffbot.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/graph_transformers/llm.py` & `gigachain_experimental-0.0.56/langchain_experimental/graph_transformers/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Any, List, Optional, Sequence
+from typing import Any, List, Optional, Sequence, Type, cast
 
 from langchain_community.graphs.graph_document import GraphDocument, Node, Relationship
 from langchain_core.documents import Document
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.pydantic_v1 import BaseModel, Field
 
@@ -89,17 +89,22 @@
             "'BECAME_PROFESSOR', use more general and timeless relationship types like "
             "'PROFESSOR'. However, do not sacrifice any accuracy for generality"
         )
         additional_info = rel_info if is_rel else node_info
         return Field(..., description=description + additional_info, **field_kwargs)
 
 
+class _Graph(BaseModel):
+    nodes: Optional[List]
+    relationships: Optional[List]
+
+
 def create_simple_model(
     node_labels: Optional[List[str]] = None, rel_types: Optional[List[str]] = None
-) -> Any:
+) -> Type[_Graph]:
     """
     Simple model allows to limit node and/or relationship types.
     Doesn't have any node or relationship properties.
     """
 
     class SimpleNode(BaseModel):
         """Represents a node in a graph with associated properties."""
@@ -108,21 +113,31 @@
         type: str = optional_enum_field(
             node_labels, description="The type or label of the node."
         )
 
     class SimpleRelationship(BaseModel):
         """Represents a directed relationship between two nodes in a graph."""
 
-        source: SimpleNode = Field(description="The source node of the relationship.")
-        target: SimpleNode = Field(description="The target node of the relationship.")
+        source_node_id: str = Field(
+            description="Name or human-readable unique identifier of source node"
+        )
+        source_node_type: str = optional_enum_field(
+            node_labels, description="The type or label of the source node."
+        )
+        target_node_id: str = Field(
+            description="Name or human-readable unique identifier of target node"
+        )
+        target_node_type: str = optional_enum_field(
+            node_labels, description="The type or label of the target node."
+        )
         type: str = optional_enum_field(
             rel_types, description="The type of the relationship.", is_rel=True
         )
 
-    class DynamicGraph(BaseModel):
+    class DynamicGraph(_Graph):
         """Represents a graph document consisting of nodes and relationships."""
 
         nodes: Optional[List[SimpleNode]] = Field(description="List of nodes")
         relationships: Optional[List[SimpleRelationship]] = Field(
             description="List of relationships"
         )
 
@@ -132,16 +147,16 @@
 def map_to_base_node(node: Any) -> Node:
     """Map the SimpleNode to the base Node."""
     return Node(id=node.id.title(), type=node.type.capitalize())
 
 
 def map_to_base_relationship(rel: Any) -> Relationship:
     """Map the SimpleRelationship to the base Relationship."""
-    source = map_to_base_node(rel.source)
-    target = map_to_base_node(rel.target)
+    source = Node(id=rel.source_node_id.title(), type=rel.source_node_type.capitalize())
+    target = Node(id=rel.target_node_id.title(), type=rel.target_node_type.capitalize())
     return Relationship(
         source=source, target=target, type=rel.type.replace(" ", "_").upper()
     )
 
 
 class LLMGraphTransformer:
     """Transform documents into graph-based documents using a LLM.
@@ -180,15 +195,15 @@
     """
 
     def __init__(
         self,
         llm: BaseLanguageModel,
         allowed_nodes: List[str] = [],
         allowed_relationships: List[str] = [],
-        prompt: Optional[ChatPromptTemplate] = default_prompt,
+        prompt: ChatPromptTemplate = default_prompt,
         strict_mode: bool = True,
     ) -> None:
         if not hasattr(llm, "with_structured_output"):
             raise ValueError(
                 "The specified LLM does not support the 'with_structured_output'. "
                 "Please ensure you are using an LLM that supports this feature."
             )
@@ -203,15 +218,15 @@
 
     def process_response(self, document: Document) -> GraphDocument:
         """
         Processes a single document, transforming it into a graph document using
         an LLM based on the model's schema and constraints.
         """
         text = document.page_content
-        raw_schema = self.chain.invoke({"input": text})
+        raw_schema = cast(_Graph, self.chain.invoke({"input": text}))
         nodes = (
             [map_to_base_node(node) for node in raw_schema.nodes]
             if raw_schema.nodes
             else []
         )
         relationships = (
             [map_to_base_relationship(rel) for rel in raw_schema.relationships]
@@ -254,15 +269,15 @@
 
     async def aprocess_response(self, document: Document) -> GraphDocument:
         """
         Asynchronously processes a single document, transforming it into a
         graph document.
         """
         text = document.page_content
-        raw_schema = await self.chain.ainvoke({"input": text})
+        raw_schema = cast(_Graph, await self.chain.ainvoke({"input": text}))
 
         nodes = (
             [map_to_base_node(node) for node in raw_schema.nodes]
             if raw_schema.nodes
             else []
         )
         relationships = (
```

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/llm_bash/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/bash.py` & `gigachain_experimental-0.0.56/langchain_experimental/llm_bash/bash.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llm_bash/prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/llm_bash/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/llm_symbolic_math/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llm_symbolic_math/prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/llm_symbolic_math/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llms/anthropic_functions.py` & `gigachain_experimental-0.0.56/langchain_experimental/llms/anthropic_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llms/jsonformer_decoder.py` & `gigachain_experimental-0.0.56/langchain_experimental/llms/jsonformer_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llms/llamaapi.py` & `gigachain_experimental-0.0.56/langchain_experimental/llms/llamaapi.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llms/lmformatenforcer_decoder.py` & `gigachain_experimental-0.0.56/langchain_experimental/llms/lmformatenforcer_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llms/ollama_functions.py` & `gigachain_experimental-0.0.56/langchain_experimental/llms/ollama_functions.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/llms/rellm_decoder.py` & `gigachain_experimental-0.0.56/langchain_experimental/llms/rellm_decoder.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/open_clip/open_clip.py` & `gigachain_experimental-0.0.56/langchain_experimental/open_clip/open_clip.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/pal_chain/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/colored_object_prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/pal_chain/colored_object_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/pal_chain/math_prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/pal_chain/math_prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/agent_executor.py` & `gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/agent_executor.py` & `gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/executors/agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/executors/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/executors/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/planners/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/planners/chat_planner.py` & `gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/planners/chat_planner.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/plan_and_execute/schema.py` & `gigachain_experimental-0.0.56/langchain_experimental/plan_and_execute/schema.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py` & `gigachain_experimental-0.0.56/langchain_experimental/prompt_injection_identifier/hugging_face_identifier.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/dataclasses.py` & `gigachain_experimental-0.0.56/langchain_experimental/pydantic_v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/pydantic_v1/main.py` & `gigachain_experimental-0.0.56/langchain_experimental/pydantic_v1/main.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/recommenders/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/amazon_personalize.py` & `gigachain_experimental-0.0.56/langchain_experimental/recommenders/amazon_personalize.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/recommenders/amazon_personalize_chain.py` & `gigachain_experimental-0.0.56/langchain_experimental/recommenders/amazon_personalize_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/retrievers/vector_sql_database.py` & `gigachain_experimental-0.0.56/langchain_experimental/retrievers/vector_sql_database.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/rl_chain/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/rl_chain/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/metrics.py` & `gigachain_experimental-0.0.56/langchain_experimental/rl_chain/metrics.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/model_repository.py` & `gigachain_experimental-0.0.56/langchain_experimental/rl_chain/model_repository.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/pick_best_chain.py` & `gigachain_experimental-0.0.56/langchain_experimental/rl_chain/pick_best_chain.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/rl_chain/vw_logger.py` & `gigachain_experimental-0.0.56/langchain_experimental/rl_chain/vw_logger.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/smart_llm/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/smart_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/smart_llm/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/smart_llm/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/sql/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/sql/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from langchain_community.utilities.sql_database import SQLDatabase
 from langchain_core.language_models import BaseLanguageModel
 
 from langchain_experimental.pydantic_v1 import Extra, Field, root_validator
 
 INTERMEDIATE_STEPS_KEY = "intermediate_steps"
 SQL_QUERY = "SQLQuery:"
+SQL_RESULT = "SQLResult:"
 
 
 class SQLDatabaseChain(Chain):
     """Chain for interacting with SQL Database.
 
     Example:
         .. code-block:: python
@@ -139,14 +140,16 @@
                 _run_manager.on_text(sql_cmd, color="green", verbose=self.verbose)
                 intermediate_steps.append(
                     sql_cmd
                 )  # output: sql generation (no checker)
                 intermediate_steps.append({"sql_cmd": sql_cmd})  # input: sql exec
                 if SQL_QUERY in sql_cmd:
                     sql_cmd = sql_cmd.split(SQL_QUERY)[1].strip()
+                if SQL_RESULT in sql_cmd:
+                    sql_cmd = sql_cmd.split(SQL_RESULT)[0].strip()
                 result = self.database.run(sql_cmd)
                 intermediate_steps.append(str(result))  # output: sql exec
             else:
                 query_checker_prompt = self.query_checker_prompt or PromptTemplate(
                     template=QUERY_CHECKER, input_variables=["query", "dialect"]
                 )
                 query_checker_chain = LLMChain(
```

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/sql/prompt.py` & `gigachain_experimental-0.0.56/langchain_experimental/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/sql/vector_sql.py` & `gigachain_experimental-0.0.56/langchain_experimental/sql/vector_sql.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/synthetic_data/__init__.py` & `gigachain_experimental-0.0.56/langchain_experimental/synthetic_data/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/tabular_synthetic_data/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tabular_synthetic_data/openai.py` & `gigachain_experimental-0.0.56/langchain_experimental/tabular_synthetic_data/openai.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/text_splitter.py` & `gigachain_experimental-0.0.56/langchain_experimental/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tools/python/tool.py` & `gigachain_experimental-0.0.56/langchain_experimental/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tot/base.py` & `gigachain_experimental-0.0.56/langchain_experimental/tot/base.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tot/checker.py` & `gigachain_experimental-0.0.56/langchain_experimental/tot/checker.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tot/controller.py` & `gigachain_experimental-0.0.56/langchain_experimental/tot/controller.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tot/memory.py` & `gigachain_experimental-0.0.56/langchain_experimental/tot/memory.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tot/prompts.py` & `gigachain_experimental-0.0.56/langchain_experimental/tot/prompts.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/tot/thought_generation.py` & `gigachain_experimental-0.0.56/langchain_experimental/tot/thought_generation.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/langchain_experimental/utilities/python.py` & `gigachain_experimental-0.0.56/langchain_experimental/utilities/python.py`

 * *Files identical despite different names*

### Comparing `gigachain_experimental-0.0.55.1/pyproject.toml` & `gigachain_experimental-0.0.56/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "gigachain-experimental"
-version = "0.0.55.1"
+version = "0.0.56"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigachain"
 packages = [
     {include = "langchain_experimental"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gigachain-core = "^0.1.33"
-gigachain = "^0.1.13"
+gigachain-core = "^0.1.37"
+gigachain = "^0.1.14"
+gigachain_openai = "^0.1.1"
 presidio-anonymizer = {version = "^2.2.352", optional = true}
 presidio-analyzer = {version = "^2.2.352", optional = true}
 faker = {version = "^19.3.1", optional = true}
 vowpal-wabbit-next = {version = "0.6.0", optional = true}
 sentence-transformers = {version = "^2", optional = true}
 jinja2 = {version = "^3", optional = true}
 pandas = { version = "^2.0.1", optional = true }
@@ -60,15 +61,14 @@
 pytest = "^7.3.0"
 pytest-asyncio = "^0.20.3"
 gigachain = {path = "../langchain", develop = true}
 gigachain-core = {path = "../core", develop = true}
 gigachain-community = {path = "../community", develop = true}
 gigachat = "^0.1.22"
 
-
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 gigachain = {path = "../langchain", develop = true}
 gigachain-core = {path = "../core", develop = true}
 gigachain-community = {path = "../community", develop = true}
```

### Comparing `gigachain_experimental-0.0.55.1/PKG-INFO` & `gigachain_experimental-0.0.56/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gigachain-experimental
-Version: 0.0.55.1
+Version: 0.0.56
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/ai-forever/gigachain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: extended-testing
 Requires-Dist: faker (>=19.3.1,<20.0.0) ; extra == "extended-testing"
-Requires-Dist: gigachain (>=0.1.13,<0.2.0)
-Requires-Dist: gigachain-core (>=0.1.33,<0.2.0)
+Requires-Dist: gigachain (>=0.1.14,<0.2.0)
+Requires-Dist: gigachain-core (>=0.1.37,<0.2.0)
+Requires-Dist: gigachain_openai (>=0.1.1,<0.2.0)
 Requires-Dist: jinja2 (>=3,<4) ; extra == "extended-testing"
 Requires-Dist: pandas (>=2.0.1,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: presidio-analyzer (>=2.2.352,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: presidio-anonymizer (>=2.2.352,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: sentence-transformers (>=2,<3) ; extra == "extended-testing"
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "extended-testing"
 Requires-Dist: vowpal-wabbit-next (==0.6.0) ; extra == "extended-testing"
```

