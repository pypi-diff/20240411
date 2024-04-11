# Comparing `tmp/pymemgpt_nightly-0.3.8.dev20240410103932.tar.gz` & `tmp/pymemgpt_nightly-0.3.9.dev20240411025350.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemgpt_nightly-0.3.8.dev20240410103932.tar", max compression
+gzip compressed data, was "pymemgpt_nightly-0.3.9.dev20240411025350.tar", max compression
```

## Comparing `pymemgpt_nightly-0.3.8.dev20240410103932.tar` & `pymemgpt_nightly-0.3.9.dev20240411025350.tar`

### file list

```diff
@@ -1,167 +1,171 @@
--rw-r--r--   0        0        0    10760 2024-04-10 10:39:21.314123 pymemgpt_nightly-0.3.8.dev20240410103932/LICENSE
--rw-r--r--   0        0        0     8441 2024-04-10 10:39:21.314123 pymemgpt_nightly-0.3.8.dev20240410103932/README.md
--rw-r--r--   0        0        0      108 2024-04-10 10:39:32.094160 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/__init__.py
--rw-r--r--   0        0        0       29 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/__main__.py
--rw-r--r--   0        0        0    55439 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent.py
--rw-r--r--   0        0        0    10728 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent_store/chroma.py
--rw-r--r--   0        0        0    25552 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent_store/db.py
--rw-r--r--   0        0        0     5288 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent_store/lancedb.py
--rw-r--r--   0        0        0     6390 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent_store/storage.py
--rw-r--r--   0        0        0      169 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/README.md
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/__init__.py
--rw-r--r--   0        0        0     7088 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/examples/agent_autoreply.py
--rw-r--r--   0        0        0     6813 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/examples/agent_docs.py
--rw-r--r--   0        0        0     7929 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/examples/agent_groupchat.py
--rw-r--r--   0        0        0     7375 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
--rw-r--r--   0        0        0     9346 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/interface.py
--rw-r--r--   0        0        0    20931 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/memgpt_agent.py
--rw-r--r--   0        0        0     3644 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/benchmark/benchmark.py
--rw-r--r--   0        0        0      536 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/benchmark/constants.py
--rw-r--r--   0        0        0    34724 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/cli/cli.py
--rw-r--r--   0        0        0    40445 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/cli/cli_config.py
--rw-r--r--   0        0        0    10453 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/cli/cli_load.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/client/__init__.py
--rw-r--r--   0        0        0     3239 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/client/admin.py
--rw-r--r--   0        0        0    26894 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/client/client.py
--rw-r--r--   0        0        0    18729 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/config.py
--rw-r--r--   0        0        0      390 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/configs/memgpt_hosted.json
--rw-r--r--   0        0        0      373 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/configs/openai.json
--rw-r--r--   0        0        0     5364 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/constants.py
--rw-r--r--   0        0        0     4904 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/credentials.py
--rw-r--r--   0        0        0     9529 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/data_sources/connectors.py
--rw-r--r--   0        0        0    23711 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/data_types.py
--rw-r--r--   0        0        0     7601 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/embeddings.py
--rw-r--r--   0        0        0      820 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/errors.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/__init__.py
--rw-r--r--   0        0        0     7343 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/function_sets/base.py
--rw-r--r--   0        0        0     4629 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/function_sets/extras.py
--rw-r--r--   0        0        0     7403 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/functions.py
--rw-r--r--   0        0        0     5433 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/schema_generator.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/humans/__init__.py
--rw-r--r--   0        0        0       17 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/humans/examples/basic.txt
--rw-r--r--   0        0        0      305 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/humans/examples/cs_phd.txt
--rw-r--r--   0        0        0    12994 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/interface.py
--rw-r--r--   0        0        0    21252 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/llm_api_tools.py
--rw-r--r--   0        0        0      175 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/README.md
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/__init__.py
--rw-r--r--   0        0        0    13519 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/chat_completion_proxy.py
--rw-r--r--   0        0        0      912 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/constants.py
--rw-r--r--   0        0        0     2788 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/function_parser.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/grammars/__init__.py
--rw-r--r--   0        0        0    56322 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/grammars/gbnf_grammar_generator.py
--rw-r--r--   0        0        0      667 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/grammars/json.gbnf
--rw-r--r--   0        0        0     3255 2024-04-10 10:39:21.322122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
--rw-r--r--   0        0        0     3562 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/groq/api.py
--rw-r--r--   0        0        0     7434 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/json_parser.py
--rw-r--r--   0        0        0     2586 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/koboldcpp/api.py
--rw-r--r--   0        0        0      557 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/koboldcpp/settings.py
--rw-r--r--   0        0        0     2492 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llamacpp/api.py
--rw-r--r--   0        0        0      548 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llamacpp/settings.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
--rw-r--r--   0        0        0    19913 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
--rw-r--r--   0        0        0    21281 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
--rw-r--r--   0        0        0    19975 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
--rw-r--r--   0        0        0    10300 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
--rw-r--r--   0        0        0     6144 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
--rw-r--r--   0        0        0      419 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
--rw-r--r--   0        0        0    14956 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
--rw-r--r--   0        0        0     4630 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/lmstudio/api.py
--rw-r--r--   0        0        0      857 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/lmstudio/settings.py
--rw-r--r--   0        0        0     3660 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/ollama/api.py
--rw-r--r--   0        0        0      894 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/ollama/settings.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/settings/__init__.py
--rw-r--r--   0        0        0     1222 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/settings/deterministic_mirostat.py
--rw-r--r--   0        0        0     3058 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/settings/settings.py
--rw-r--r--   0        0        0      719 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/settings/simple.py
--rw-r--r--   0        0        0     4846 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/utils.py
--rw-r--r--   0        0        0     2612 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/vllm/api.py
--rw-r--r--   0        0        0     2658 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/webui/api.py
--rw-r--r--   0        0        0     2354 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/webui/legacy_api.py
--rw-r--r--   0        0        0      579 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/webui/legacy_settings.py
--rw-r--r--   0        0        0      593 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/webui/settings.py
--rw-r--r--   0        0        0     1211 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/log.py
--rw-r--r--   0        0        0    19997 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/main.py
--rw-r--r--   0        0        0    19653 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/memory.py
--rw-r--r--   0        0        0    29420 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/metadata.py
--rw-r--r--   0        0        0    31537 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/migrate.py
--rw-r--r--   0        0        0     2517 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/chat_completion_request.py
--rw-r--r--   0        0        0     1562 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/chat_completion_response.py
--rw-r--r--   0        0        0      356 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/embedding_response.py
--rw-r--r--   0        0        0     7977 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/openai.py
--rw-r--r--   0        0        0     8957 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/pydantic_models.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/openai_backcompat/__init__.py
--rw-r--r--   0        0        0    13692 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/openai_backcompat/openai_object.py
--rw-r--r--   0        0        0     5882 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/persistence_manager.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/__init__.py
--rw-r--r--   0        0        0     1849 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/anna_pa.txt
--rw-r--r--   0        0        0     1196 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/google_search_persona.txt
--rw-r--r--   0        0        0      431 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/memgpt_doc.txt
--rw-r--r--   0        0        0      164 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/memgpt_starter.txt
--rw-r--r--   0        0        0     1236 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/sam.txt
--rw-r--r--   0        0        0     1171 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/sam_pov.txt
--rw-r--r--   0        0        0     1053 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/sam_simple_pov_gpt35.txt
--rw-r--r--   0        0        0     8192 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/sqldb/test.db
--rw-r--r--   0        0        0      248 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/presets/examples/memgpt_chat.yaml
--rw-r--r--   0        0        0      247 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/presets/examples/memgpt_docs.yaml
--rw-r--r--   0        0        0      374 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/presets/examples/memgpt_extras.yaml
--rw-r--r--   0        0        0     7575 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/presets/presets.py
--rw-r--r--   0        0        0     2789 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/presets/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/__init__.py
--rw-r--r--   0        0        0    12907 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/gpt_functions.py
--rw-r--r--   0        0        0     1139 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/gpt_summarize.py
--rw-r--r--   0        0        0     1045 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/gpt_system.py
--rw-r--r--   0        0        0     4758 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_base.txt
--rw-r--r--   0        0        0     5479 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_chat.txt
--rw-r--r--   0        0        0     1057 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_chat_compressed.txt
--rw-r--r--   0        0        0     4819 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_doc.txt
--rw-r--r--   0        0        0     5047 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_gpt35_extralong.txt
--rw-r--r--   0        0        0     2967 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
--rw-r--r--   0        0        0     4663 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_modified_chat.txt
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/__init__.py
--rw-r--r--   0        0        0       92 2024-04-10 10:39:21.326122 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/constants.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/admin/__init__.py
--rw-r--r--   0        0        0     6130 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/admin/users.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/command.py
--rw-r--r--   0        0        0     6138 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/config.py
--rw-r--r--   0        0        0     5114 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/index.py
--rw-r--r--   0        0        0     7640 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/memory.py
--rw-r--r--   0        0        0     8583 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/message.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/auth/__init__.py
--rw-r--r--   0        0        0     1303 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/auth/index.py
--rw-r--r--   0        0        0      775 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/auth_token.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/config/__init__.py
--rw-r--r--   0        0        0     1136 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/config/index.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/humans/__init__.py
--rw-r--r--   0        0        0     1732 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/humans/index.py
--rw-r--r--   0        0        0     5482 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/interface.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/models/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/models/index.py
--rw-r--r--   0        0        0    23956 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/openai_assistants/assistants.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/personas/__init__.py
--rw-r--r--   0        0        0     1795 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/personas/index.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/presets/__init__.py
--rw-r--r--   0        0        0     5014 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/presets/index.py
--rw-r--r--   0        0        0     9580 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/server.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/sources/__init__.py
--rw-r--r--   0        0        0     8218 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/sources/index.py
--rw-r--r--   0        0        0      914 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/static_files.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/tools/__init__.py
--rw-r--r--   0        0        0     2560 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/tools/index.py
--rw-r--r--   0        0        0    63646 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/server.py
--rw-r--r--   0        0        0    43424 2024-04-10 10:39:21.330123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/assets/index-0c5d3001.css
--rw-r--r--   0        0        0   725155 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/assets/index-bf421135.js
--rw-r--r--   0        0        0    28783 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/favicon.ico
--rw-r--r--   0        0        0     1199 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/index.html
--rw-r--r--   0        0        0    85383 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/memgpt_logo_transparent.png
--rw-r--r--   0        0        0     1667 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/__init__.py
--rw-r--r--   0        0        0     4264 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/example_client.py
--rw-r--r--   0        0        0     4124 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/interface.py
--rw-r--r--   0        0        0     2257 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/protocol.py
--rw-r--r--   0        0        0     6122 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/server.py
--rw-r--r--   0        0        0     7281 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/system.py
--rw-r--r--   0        0        0    31128 2024-04-10 10:39:21.334123 pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/utils.py
--rw-r--r--   0        0        0     2285 2024-04-10 10:39:32.094160 pymemgpt_nightly-0.3.8.dev20240410103932/pyproject.toml
--rw-r--r--   0        0        0    11046 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.8.dev20240410103932/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-11 02:53:42.943613 pymemgpt_nightly-0.3.9.dev20240411025350/LICENSE
+-rw-r--r--   0        0        0     8441 2024-04-11 02:53:42.943613 pymemgpt_nightly-0.3.9.dev20240411025350/README.md
+-rw-r--r--   0        0        0      108 2024-04-11 02:53:50.131612 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/__main__.py
+-rw-r--r--   0        0        0    55434 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent.py
+-rw-r--r--   0        0        0    10728 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/chroma.py
+-rw-r--r--   0        0        0    25552 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/db.py
+-rw-r--r--   0        0        0     5288 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/lancedb.py
+-rw-r--r--   0        0        0     6390 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/storage.py
+-rw-r--r--   0        0        0      169 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/__init__.py
+-rw-r--r--   0        0        0     7088 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_autoreply.py
+-rw-r--r--   0        0        0     6813 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_docs.py
+-rw-r--r--   0        0        0     7929 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_groupchat.py
+-rw-r--r--   0        0        0     7375 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/memgpt_coder_autogen.ipynb
+-rw-r--r--   0        0        0     9346 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/interface.py
+-rw-r--r--   0        0        0    20931 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/memgpt_agent.py
+-rw-r--r--   0        0        0     3644 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/benchmark/benchmark.py
+-rw-r--r--   0        0        0      536 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/benchmark/constants.py
+-rw-r--r--   0        0        0    34724 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli.py
+-rw-r--r--   0        0        0    45520 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli_config.py
+-rw-r--r--   0        0        0    10453 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli_load.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/admin.py
+-rw-r--r--   0        0        0    26894 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/client.py
+-rw-r--r--   0        0        0    18729 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/config.py
+-rw-r--r--   0        0        0      390 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/configs/memgpt_hosted.json
+-rw-r--r--   0        0        0      373 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/configs/openai.json
+-rw-r--r--   0        0        0     5606 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/constants.py
+-rw-r--r--   0        0        0     5390 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/credentials.py
+-rw-r--r--   0        0        0     9529 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/data_sources/connectors.py
+-rw-r--r--   0        0        0    28513 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/data_types.py
+-rw-r--r--   0        0        0     7601 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/embeddings.py
+-rw-r--r--   0        0        0      820 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/errors.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/__init__.py
+-rw-r--r--   0        0        0     7343 2024-04-11 02:53:42.951613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/function_sets/base.py
+-rw-r--r--   0        0        0     4775 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/function_sets/extras.py
+-rw-r--r--   0        0        0     7403 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/functions.py
+-rw-r--r--   0        0        0     5433 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/schema_generator.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/humans/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/humans/examples/basic.txt
+-rw-r--r--   0        0        0      305 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/humans/examples/cs_phd.txt
+-rw-r--r--   0        0        0    12994 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/interface.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/__init__.py
+-rw-r--r--   0        0        0     6816 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/azure_openai.py
+-rw-r--r--   0        0        0    19315 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/google_ai.py
+-rw-r--r--   0        0        0    10622 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/llm_api_tools.py
+-rw-r--r--   0        0        0     5972 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/openai.py
+-rw-r--r--   0        0        0      175 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/__init__.py
+-rw-r--r--   0        0        0    13519 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/chat_completion_proxy.py
+-rw-r--r--   0        0        0     1032 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/constants.py
+-rw-r--r--   0        0        0     2788 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/function_parser.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/__init__.py
+-rw-r--r--   0        0        0    56322 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/gbnf_grammar_generator.py
+-rw-r--r--   0        0        0      667 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/json.gbnf
+-rw-r--r--   0        0        0     3255 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf
+-rw-r--r--   0        0        0     3562 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/groq/api.py
+-rw-r--r--   0        0        0     7793 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/json_parser.py
+-rw-r--r--   0        0        0     2586 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/koboldcpp/api.py
+-rw-r--r--   0        0        0      557 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/koboldcpp/settings.py
+-rw-r--r--   0        0        0     2492 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llamacpp/api.py
+-rw-r--r--   0        0        0      548 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llamacpp/settings.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/__init__.py
+-rw-r--r--   0        0        0    19913 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py
+-rw-r--r--   0        0        0    21457 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py
+-rw-r--r--   0        0        0    19975 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py
+-rw-r--r--   0        0        0    10300 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py
+-rw-r--r--   0        0        0     6144 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py
+-rw-r--r--   0        0        0      419 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/wrapper_base.py
+-rw-r--r--   0        0        0    14956 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py
+-rw-r--r--   0        0        0     4630 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/lmstudio/api.py
+-rw-r--r--   0        0        0      857 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/lmstudio/settings.py
+-rw-r--r--   0        0        0     3660 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/ollama/api.py
+-rw-r--r--   0        0        0      894 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/ollama/settings.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/__init__.py
+-rw-r--r--   0        0        0     1222 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/deterministic_mirostat.py
+-rw-r--r--   0        0        0     3058 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/settings.py
+-rw-r--r--   0        0        0      719 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/simple.py
+-rw-r--r--   0        0        0     4846 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/utils.py
+-rw-r--r--   0        0        0     2612 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/vllm/api.py
+-rw-r--r--   0        0        0     2658 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/api.py
+-rw-r--r--   0        0        0     2354 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/legacy_api.py
+-rw-r--r--   0        0        0      579 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/legacy_settings.py
+-rw-r--r--   0        0        0      593 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/settings.py
+-rw-r--r--   0        0        0     1211 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/log.py
+-rw-r--r--   0        0        0    20047 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/main.py
+-rw-r--r--   0        0        0    20376 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/memory.py
+-rw-r--r--   0        0        0    29420 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/metadata.py
+-rw-r--r--   0        0        0    31537 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/migrate.py
+-rw-r--r--   0        0        0     3295 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/chat_completion_request.py
+-rw-r--r--   0        0        0     1562 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/chat_completion_response.py
+-rw-r--r--   0        0        0      356 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/embedding_response.py
+-rw-r--r--   0        0        0     7977 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/openai.py
+-rw-r--r--   0        0        0     8957 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/pydantic_models.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/openai_backcompat/__init__.py
+-rw-r--r--   0        0        0    13692 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/openai_backcompat/openai_object.py
+-rw-r--r--   0        0        0     5882 2024-04-11 02:53:42.955613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/persistence_manager.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/__init__.py
+-rw-r--r--   0        0        0     1849 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/anna_pa.txt
+-rw-r--r--   0        0        0     1196 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/google_search_persona.txt
+-rw-r--r--   0        0        0      431 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/memgpt_doc.txt
+-rw-r--r--   0        0        0      164 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/memgpt_starter.txt
+-rw-r--r--   0        0        0     1236 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam.txt
+-rw-r--r--   0        0        0     1171 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam_pov.txt
+-rw-r--r--   0        0        0     1053 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam_simple_pov_gpt35.txt
+-rw-r--r--   0        0        0     8192 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sqldb/test.db
+-rw-r--r--   0        0        0      248 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/examples/memgpt_chat.yaml
+-rw-r--r--   0        0        0      247 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/examples/memgpt_docs.yaml
+-rw-r--r--   0        0        0      374 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/examples/memgpt_extras.yaml
+-rw-r--r--   0        0        0     7575 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/presets.py
+-rw-r--r--   0        0        0     2789 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/__init__.py
+-rw-r--r--   0        0        0    12907 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_functions.py
+-rw-r--r--   0        0        0     1139 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_summarize.py
+-rw-r--r--   0        0        0     1045 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_system.py
+-rw-r--r--   0        0        0     4758 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_base.txt
+-rw-r--r--   0        0        0     5479 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_chat.txt
+-rw-r--r--   0        0        0     1057 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_chat_compressed.txt
+-rw-r--r--   0        0        0     4819 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_doc.txt
+-rw-r--r--   0        0        0     5047 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_gpt35_extralong.txt
+-rw-r--r--   0        0        0     2967 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_intuitive_knowledge.txt
+-rw-r--r--   0        0        0     4663 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_modified_chat.txt
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/admin/__init__.py
+-rw-r--r--   0        0        0     6130 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/admin/users.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/__init__.py
+-rw-r--r--   0        0        0     1757 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/command.py
+-rw-r--r--   0        0        0     6138 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/config.py
+-rw-r--r--   0        0        0     5114 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/index.py
+-rw-r--r--   0        0        0     7640 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/memory.py
+-rw-r--r--   0        0        0     8583 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/message.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth/index.py
+-rw-r--r--   0        0        0      775 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth_token.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/config/__init__.py
+-rw-r--r--   0        0        0     1136 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/config/index.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/humans/__init__.py
+-rw-r--r--   0        0        0     1732 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/humans/index.py
+-rw-r--r--   0        0        0     5482 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/interface.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/models/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/models/index.py
+-rw-r--r--   0        0        0    23956 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/openai_assistants/assistants.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/personas/__init__.py
+-rw-r--r--   0        0        0     1795 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/personas/index.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/presets/__init__.py
+-rw-r--r--   0        0        0     5014 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/presets/index.py
+-rw-r--r--   0        0        0     9580 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/server.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/sources/__init__.py
+-rw-r--r--   0        0        0     8218 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/sources/index.py
+-rw-r--r--   0        0        0      914 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/static_files.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/tools/__init__.py
+-rw-r--r--   0        0        0     2560 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/tools/index.py
+-rw-r--r--   0        0        0    63646 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/server.py
+-rw-r--r--   0        0        0    43424 2024-04-11 02:53:42.959613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/assets/index-0c5d3001.css
+-rw-r--r--   0        0        0   725155 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/assets/index-bf421135.js
+-rw-r--r--   0        0        0    28783 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/favicon.ico
+-rw-r--r--   0        0        0     1199 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/index.html
+-rw-r--r--   0        0        0    85383 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/memgpt_logo_transparent.png
+-rw-r--r--   0        0        0     1667 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/__init__.py
+-rw-r--r--   0        0        0     4264 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/example_client.py
+-rw-r--r--   0        0        0     4124 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/interface.py
+-rw-r--r--   0        0        0     2257 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/protocol.py
+-rw-r--r--   0        0        0     6122 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/server.py
+-rw-r--r--   0        0        0     7281 2024-04-11 02:53:42.963613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/system.py
+-rw-r--r--   0        0        0    31426 2024-04-11 02:53:42.967613 pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/utils.py
+-rw-r--r--   0        0        0     2285 2024-04-11 02:53:50.131612 pymemgpt_nightly-0.3.9.dev20240411025350/pyproject.toml
+-rw-r--r--   0        0        0    11046 1970-01-01 00:00:00.000000 pymemgpt_nightly-0.3.9.dev20240411025350/PKG-INFO
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/LICENSE` & `pymemgpt_nightly-0.3.9.dev20240411025350/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/README.md` & `pymemgpt_nightly-0.3.9.dev20240411025350/README.md`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from memgpt.agent_store.storage import StorageConnector, TableType
 from memgpt.data_types import AgentState, Message, LLMConfig, EmbeddingConfig, Passage, Preset
 from memgpt.models import chat_completion_response
 from memgpt.interface import AgentInterface
 from memgpt.persistence_manager import LocalStateManager
 from memgpt.system import get_login_event, package_function_response, package_summarize_message, get_initial_boot_messages
 from memgpt.memory import CoreMemory as InContextMemory, summarize_messages, ArchivalMemory, RecallMemory
-from memgpt.llm_api_tools import create, is_context_overflow_error
+from memgpt.llm_api.llm_api_tools import create, is_context_overflow_error
 from memgpt.utils import (
     get_utc_time,
     create_random_username,
     get_tool_call_id,
     get_local_time,
     parse_json,
     united_diff,
@@ -396,15 +396,15 @@
         self.persistence_manager.swap_system_message(new_system_message)
 
         new_messages = [new_system_message] + self._messages[1:]  # swap index 0 (system)
         self._messages = new_messages
 
     def _get_ai_reply(
         self,
-        message_sequence: List[dict],
+        message_sequence: List[Message],
         function_call: str = "auto",
         first_message: bool = False,  # hint
     ) -> chat_completion_response.ChatCompletionResponse:
         """Get response from LLM API"""
         try:
             response = create(
                 agent_state=self.agent_state,
@@ -690,20 +690,20 @@
                     )
 
                 else:
                     raise ValueError(f"Bad type for user_message: {type(user_message)}")
 
                 self.interface.user_message(user_message.text, msg_obj=user_message)
 
-                input_message_sequence = self.messages + [user_message.to_openai_dict()]
+                input_message_sequence = self._messages + [user_message]
             # Alternatively, the requestor can send an empty user message
             else:
-                input_message_sequence = self.messages
+                input_message_sequence = self._messages
 
-            if len(input_message_sequence) > 1 and input_message_sequence[-1]["role"] != "user":
+            if len(input_message_sequence) > 1 and input_message_sequence[-1].role != "user":
                 printd(f"{CLI_WARNING_PREFIX}Attempting to run ChatCompletion without user as the last message in the queue")
 
             # Step 1: send the conversation and available functions to GPT
             if not skip_verify and (first_message or self.messages_total == self.messages_total_init):
                 printd(f"This is the first message. Running extra verifier on AI response.")
                 counter = 0
                 while True:
@@ -854,22 +854,22 @@
 
         # Make sure the cutoff isn't on a 'tool' or 'function'
         if disallow_tool_as_first:
             while self.messages[cutoff]["role"] in ["tool", "function"] and cutoff < len(self.messages):
                 printd(f"Selected cutoff {cutoff} was a 'tool', shifting one...")
                 cutoff += 1
 
-        message_sequence_to_summarize = self.messages[1:cutoff]  # do NOT get rid of the system message
+        message_sequence_to_summarize = self._messages[1:cutoff]  # do NOT get rid of the system message
         if len(message_sequence_to_summarize) <= 1:
             # This prevents a potential infinite loop of summarizing the same message over and over
             raise LLMError(
                 f"Summarize error: tried to run summarize, but couldn't find enough messages to compress [len={len(message_sequence_to_summarize)} <= 1]"
             )
         else:
-            printd(f"Attempting to summarize {len(message_sequence_to_summarize)} messages [1:{cutoff}] of {len(self.messages)}")
+            printd(f"Attempting to summarize {len(message_sequence_to_summarize)} messages [1:{cutoff}] of {len(self._messages)}")
 
         # We can't do summarize logic properly if context_window is undefined
         if self.agent_state.llm_config.context_window is None:
             # Fallback if for some reason context_window is missing, just set to the default
             print(f"{CLI_WARNING_PREFIX}could not find context_window in config, setting to default {LLM_MAX_TOKENS['DEFAULT']}")
             print(f"{self.agent_state}")
             self.agent_state.llm_config.context_window = (
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent_store/chroma.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/chroma.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent_store/db.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/db.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent_store/lancedb.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/agent_store/storage.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/agent_store/storage.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/examples/agent_autoreply.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_autoreply.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/examples/agent_docs.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_docs.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/examples/agent_groupchat.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/agent_groupchat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/examples/memgpt_coder_autogen.ipynb` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/examples/memgpt_coder_autogen.ipynb`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/interface.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/autogen/memgpt_agent.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/autogen/memgpt_agent.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/benchmark/benchmark.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/benchmark/constants.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/benchmark/constants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/cli/cli.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/cli/cli_config.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 from memgpt import utils
 from memgpt.agent_store.storage import StorageConnector, TableType
 from memgpt.config import MemGPTConfig
 from memgpt.constants import LLM_MAX_TOKENS
 from memgpt.constants import MEMGPT_DIR
 from memgpt.credentials import MemGPTCredentials, SUPPORTED_AUTH_TYPES
 from memgpt.data_types import User, LLMConfig, EmbeddingConfig
-from memgpt.llm_api_tools import openai_get_model_list, azure_openai_get_model_list, smart_urljoin
+from memgpt.llm_api.openai import openai_get_model_list
+from memgpt.llm_api.azure_openai import azure_openai_get_model_list
+from memgpt.llm_api.google_ai import google_ai_get_model_list, google_ai_get_model_context_window
 from memgpt.local_llm.constants import DEFAULT_ENDPOINTS, DEFAULT_OLLAMA_MODEL, DEFAULT_WRAPPER_NAME
 from memgpt.local_llm.utils import get_available_wrappers
 from memgpt.server.utils import shorten_key_middle
 from memgpt.data_types import User, LLMConfig, EmbeddingConfig, Source
 from memgpt.metadata import MetadataStore
 from memgpt.server.utils import shorten_key_middle
 from memgpt.models.pydantic_models import HumanModel, PersonaModel, PresetModel
@@ -41,33 +43,39 @@
     )
     # embedding endpoint and version default to non-embedding
     creds["azure_embedding_endpoint"] = os.getenv("AZURE_OPENAI_EMBEDDING_ENDPOINT", creds["azure_endpoint"])
     creds["azure_embedding_version"] = os.getenv("AZURE_OPENAI_EMBEDDING_VERSION", creds["azure_version"])
     return creds
 
 
-def get_openai_credentials():
-    openai_key = os.getenv("OPENAI_API_KEY")
+def get_openai_credentials() -> Optional[str]:
+    openai_key = os.getenv("OPENAI_API_KEY", None)
     return openai_key
 
 
+def get_google_ai_credentials() -> Optional[str]:
+    google_ai_key = os.getenv("GOOGLE_AI_API_KEY", None)
+    return google_ai_key
+
+
 def configure_llm_endpoint(config: MemGPTConfig, credentials: MemGPTCredentials):
     # configure model endpoint
     model_endpoint_type, model_endpoint = None, None
 
     # get default
     default_model_endpoint_type = config.default_llm_config.model_endpoint_type
     if config.default_llm_config.model_endpoint_type is not None and config.default_llm_config.model_endpoint_type not in [
         "openai",
         "azure",
+        "google_ai",
     ]:  # local model
         default_model_endpoint_type = "local"
 
     provider = questionary.select(
-        "Select LLM inference provider:", choices=["openai", "azure", "local"], default=default_model_endpoint_type
+        "Select LLM inference provider:", choices=["openai", "azure", "google_ai", "local"], default=default_model_endpoint_type
     ).ask()
     if provider is None:
         raise KeyboardInterrupt
 
     # set: model_endpoint_type, model_endpoint
     if provider == "openai":
         # check for key
@@ -127,14 +135,59 @@
             if "azure_embedding_deployment" in azure_creds:
                 credentials.azure_embedding_deployment = azure_creds["azure_embedding_deployment"]
             credentials.save()
 
         model_endpoint_type = "azure"
         model_endpoint = azure_creds["azure_endpoint"]
 
+    elif provider == "google_ai":
+
+        # check for key
+        if credentials.google_ai_key is None:
+            # allow key to get pulled from env vars
+            google_ai_key = get_google_ai_credentials()
+            # if we still can't find it, ask for it as input
+            if google_ai_key is None:
+                while google_ai_key is None or len(google_ai_key) == 0:
+                    # Ask for API key as input
+                    google_ai_key = questionary.password(
+                        "Enter your Google AI (Gemini) API key (see https://aistudio.google.com/app/apikey):"
+                    ).ask()
+                    if google_ai_key is None:
+                        raise KeyboardInterrupt
+            credentials.google_ai_key = google_ai_key
+        else:
+            # Give the user an opportunity to overwrite the key
+            google_ai_key = None
+            default_input = shorten_key_middle(credentials.google_ai_key)
+
+            google_ai_key = questionary.password(
+                "Enter your Google AI (Gemini) API key (see https://aistudio.google.com/app/apikey):",
+                default=default_input,
+            ).ask()
+            if google_ai_key is None:
+                raise KeyboardInterrupt
+            # If the user modified it, use the new one
+            if google_ai_key != default_input:
+                credentials.google_ai_key = google_ai_key
+
+        default_input = os.getenv("GOOGLE_AI_SERVICE_ENDPOINT", None)
+        if default_input is None:
+            default_input = "generativelanguage"
+        google_ai_service_endpoint = questionary.text(
+            "Enter your Google AI (Gemini) service endpoint (see https://ai.google.dev/api/rest):",
+            default=default_input,
+        ).ask()
+        credentials.google_ai_service_endpoint = google_ai_service_endpoint
+
+        # write out the credentials
+        credentials.save()
+
+        model_endpoint_type = "google_ai"
+
     else:  # local models
         # backend_options_old = ["webui", "webui-legacy", "llamacpp", "koboldcpp", "ollama", "lmstudio", "lmstudio-legacy", "vllm", "openai"]
         backend_options = builtins.list(DEFAULT_ENDPOINTS.keys())
         # assert backend_options_old == backend_options, (backend_options_old, backend_options)
         default_model_endpoint_type = None
         if config.default_llm_config.model_endpoint_type in backend_options:
             # set from previous config
@@ -219,14 +272,29 @@
 
             # Filter the list for "gpt" models only
             if filter_list:
                 model_options = [obj["id"] for obj in fetched_model_options_response["data"] if obj["id"].startswith(filter_prefix)]
             else:
                 model_options = [obj["id"] for obj in fetched_model_options_response["data"]]
 
+        elif model_endpoint_type == "google_ai":
+            if credentials.google_ai_key is None:
+                raise ValueError("Missing Google AI API key")
+            if credentials.google_ai_service_endpoint is None:
+                raise ValueError("Missing Google AI service endpoint")
+            model_options = google_ai_get_model_list(
+                service_endpoint=credentials.google_ai_service_endpoint, api_key=credentials.google_ai_key
+            )
+            model_options = [str(m["name"]) for m in model_options]
+            model_options = [mo[len("models/") :] if mo.startswith("models/") else mo for mo in model_options]
+
+            # TODO remove manual filtering for gemini-pro
+            model_options = [mo for mo in model_options if str(mo).startswith("gemini") and "-pro" in str(mo)]
+            # model_options = ["gemini-pro"]
+
         else:
             # Attempt to do OpenAI endpoint style model fetching
             # TODO support local auth with api-key header
             if credentials.openllm_auth_type == "bearer_token":
                 api_key = credentials.openllm_key
             else:
                 api_key = None
@@ -290,14 +358,34 @@
             while len(model) == 0:
                 model = questionary.text(
                     "Enter custom model name:",
                 ).ask()
                 if model is None:
                     raise KeyboardInterrupt
 
+    elif model_endpoint_type == "google_ai":
+        try:
+            fetched_model_options = get_model_options(
+                credentials=credentials, model_endpoint_type=model_endpoint_type, model_endpoint=model_endpoint
+            )
+        except Exception as e:
+            # NOTE: if this fails, it means the user's key is probably bad
+            typer.secho(
+                f"Failed to get model list from {model_endpoint} - make sure your API key and endpoints are correct!", fg=typer.colors.RED
+            )
+            raise e
+
+        model = questionary.select(
+            "Select default model:",
+            choices=fetched_model_options,
+            default=fetched_model_options[0],
+        ).ask()
+        if model is None:
+            raise KeyboardInterrupt
+
     else:  # local models
 
         # ask about local auth
         if model_endpoint_type in ["groq"]:  # TODO all llm engines under 'local' that will require api keys
             use_local_auth = True
             local_auth_type = "bearer_token"
             local_auth_key = questionary.password(
@@ -408,30 +496,57 @@
             default=DEFAULT_WRAPPER_NAME,
         ).ask()
         if model_wrapper is None:
             raise KeyboardInterrupt
 
     # set: context_window
     if str(model) not in LLM_MAX_TOKENS:
-        # Ask the user to specify the context length
+
         context_length_options = [
             str(2**12),  # 4096
             str(2**13),  # 8192
             str(2**14),  # 16384
             str(2**15),  # 32768
             str(2**18),  # 262144
             "custom",  # enter yourself
         ]
-        context_window_input = questionary.select(
-            "Select your model's context window (for Mistral 7B models, this is probably 8k / 8192):",
-            choices=context_length_options,
-            default=str(LLM_MAX_TOKENS["DEFAULT"]),
-        ).ask()
-        if context_window_input is None:
-            raise KeyboardInterrupt
+
+        if model_endpoint_type == "google_ai":
+            try:
+                fetched_context_window = str(
+                    google_ai_get_model_context_window(
+                        service_endpoint=credentials.google_ai_service_endpoint, api_key=credentials.google_ai_key, model=model
+                    )
+                )
+                print(f"Got context window {fetched_context_window} for model {model} (from Google API)")
+                context_length_options = [
+                    fetched_context_window,
+                    "custom",
+                ]
+            except:
+                print(f"Failed to get model details for model '{model}' on Google AI API")
+
+            context_window_input = questionary.select(
+                "Select your model's context window (see https://cloud.google.com/vertex-ai/generative-ai/docs/learn/model-versioning#gemini-model-versions):",
+                choices=context_length_options,
+                default=context_length_options[0],
+            ).ask()
+            if context_window_input is None:
+                raise KeyboardInterrupt
+
+        else:
+
+            # Ask the user to specify the context length
+            context_window_input = questionary.select(
+                "Select your model's context window (for Mistral 7B models, this is probably 8k / 8192):",
+                choices=context_length_options,
+                default=str(LLM_MAX_TOKENS["DEFAULT"]),
+            ).ask()
+            if context_window_input is None:
+                raise KeyboardInterrupt
 
         # If custom, ask for input
         if context_window_input == "custom":
             while True:
                 context_window_input = questionary.text("Enter context window (e.g. 8192)").ask()
                 if context_window_input is None:
                     raise KeyboardInterrupt
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/cli/cli_load.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/cli/cli_load.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/client/admin.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/admin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/client/client.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/client/client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/config.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/constants.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,16 @@
         "Do NOT tell the user about this system alert, they should not know that the history is reaching max length.",
         "If there is any important new information or general memories about you or the user that you would like to save, you should save that information immediately by calling function core_memory_append, core_memory_replace, or archival_memory_insert.",
         # "Remember to pass request_heartbeat = true if you would like to send a message immediately after.",
     ]
 )
 # The fraction of tokens we truncate down to
 MESSAGE_SUMMARY_TRUNC_TOKEN_FRAC = 0.75
+# The ackknowledgement message used in the summarize sequence
+MESSAGE_SUMMARY_REQUEST_ACK = "Understood, I will respond with a summary of the message (and only the summary, nothing else) once I receive the conversation history. I'm ready."
 
 # Even when summarizing, we want to keep a handful of recent messages
 # These serve as in-context examples of how to use functions / what user messages look like
 MESSAGE_SUMMARY_TRUNC_KEEP_N_LAST = 3
 
 # Default memory limits
 CORE_MEMORY_PERSONA_CHAR_LIMIT = 2000
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/credentials.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     # credentials for MemGPT
     credentials_path: str = os.path.join(MEMGPT_DIR, "credentials")
 
     # openai config
     openai_auth_type: str = "bearer_token"
     openai_key: Optional[str] = None
 
+    # gemini config
+    google_ai_key: Optional[str] = None
+    google_ai_service_endpoint: Optional[str] = None
+
     # azure config
     azure_auth_type: str = "api_key"
     azure_key: Optional[str] = None
     # base llm / model
     azure_version: Optional[str] = None
     azure_endpoint: Optional[str] = None
     azure_deployment: Optional[str] = None
@@ -66,14 +70,17 @@
                 "azure_key": get_field(config, "azure", "key"),
                 "azure_version": get_field(config, "azure", "version"),
                 "azure_endpoint": get_field(config, "azure", "endpoint"),
                 "azure_deployment": get_field(config, "azure", "deployment"),
                 "azure_embedding_version": get_field(config, "azure", "embedding_version"),
                 "azure_embedding_endpoint": get_field(config, "azure", "embedding_endpoint"),
                 "azure_embedding_deployment": get_field(config, "azure", "embedding_deployment"),
+                # gemini
+                "google_ai_key": get_field(config, "google_ai", "key"),
+                "google_ai_service_endpoint": get_field(config, "google_ai", "service_endpoint"),
                 # open llm
                 "openllm_auth_type": get_field(config, "openllm", "auth_type"),
                 "openllm_key": get_field(config, "openllm", "key"),
                 # path
                 "credentials_path": credentials_path,
             }
             config_dict = {k: v for k, v in config_dict.items() if v is not None}
@@ -98,15 +105,19 @@
         set_field(config, "azure", "version", self.azure_version)
         set_field(config, "azure", "endpoint", self.azure_endpoint)
         set_field(config, "azure", "deployment", self.azure_deployment)
         set_field(config, "azure", "embedding_version", self.azure_embedding_version)
         set_field(config, "azure", "embedding_endpoint", self.azure_embedding_endpoint)
         set_field(config, "azure", "embedding_deployment", self.azure_embedding_deployment)
 
-        # openai config
+        # gemini
+        set_field(config, "google_ai", "key", self.google_ai_key)
+        set_field(config, "google_ai", "service_endpoint", self.google_ai_service_endpoint)
+
+        # openllm config
         set_field(config, "openllm", "auth_type", self.openllm_auth_type)
         set_field(config, "openllm", "key", self.openllm_key)
 
         if not os.path.exists(MEMGPT_DIR):
             os.makedirs(MEMGPT_DIR, exist_ok=True)
         with open(self.credentials_path, "w", encoding="utf-8") as f:
             config.write(f)
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/data_sources/connectors.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/data_sources/connectors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/data_types.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/data_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ This module contains the data types used by MemGPT. Each data type must include a function to create a DB model. """
 
 import uuid
+import json
 from datetime import datetime, timezone
 from typing import Optional, List, Dict, TypeVar
 import numpy as np
 from pydantic import BaseModel, Field, Json
 
 from memgpt.constants import (
     DEFAULT_HUMAN,
@@ -14,14 +15,15 @@
     LLM_MAX_TOKENS,
     MAX_EMBEDDING_DIM,
     TOOL_CALL_ID_MAX_LEN,
 )
 from memgpt.utils import get_utc_time, create_uuid_from_string
 from memgpt.models import chat_completion_response
 from memgpt.utils import get_human_text, get_persona_text, printd, is_utc_datetime
+from memgpt.local_llm.constants import INNER_THOUGHTS_KWARG, INNER_THOUGHTS_KWARG_DESCRIPTION
 
 
 class Record:
     """
     Base class for an agent's memory unit. Each memory unit is represented in the database as a single row.
     Memory units are searched over by functions defined in the memory classes
     """
@@ -78,14 +80,15 @@
         role: str,
         text: str,
         model: Optional[str] = None,  # model used to make function call
         name: Optional[str] = None,  # optional participant name
         created_at: Optional[datetime] = None,
         tool_calls: Optional[List[ToolCall]] = None,  # list of tool calls requested
         tool_call_id: Optional[str] = None,
+        # tool_call_name: Optional[str] = None,  # not technically OpenAI spec, but it can be helpful to have on-hand
         embedding: Optional[np.ndarray] = None,
         embedding_dim: Optional[int] = None,
         embedding_model: Optional[str] = None,
         id: Optional[uuid.UUID] = None,
     ):
         super().__init__(id)
         self.user_id = user_id
@@ -234,15 +237,15 @@
                 role=openai_message_dict["role"],
                 text=openai_message_dict["content"],
                 name=openai_message_dict["name"] if "name" in openai_message_dict else None,
                 tool_calls=tool_calls,
                 tool_call_id=openai_message_dict["tool_call_id"] if "tool_call_id" in openai_message_dict else None,
             )
 
-    def to_openai_dict(self, max_tool_id_length=TOOL_CALL_ID_MAX_LEN):
+    def to_openai_dict(self, max_tool_id_length=TOOL_CALL_ID_MAX_LEN) -> dict:
         """Go from Message class to ChatCompletion message object"""
 
         # TODO change to pydantic casting, eg `return SystemMessageModel(self)`
 
         if self.role == "system":
             assert all([v is not None for v in [self.role]]), vars(self)
             openai_message = {
@@ -281,19 +284,125 @@
         elif self.role == "tool":
             assert all([v is not None for v in [self.role, self.tool_call_id]]), vars(self)
             openai_message = {
                 "content": self.text,
                 "role": self.role,
                 "tool_call_id": self.tool_call_id[:max_tool_id_length] if max_tool_id_length else self.tool_call_id,
             }
+
         else:
             raise ValueError(self.role)
 
         return openai_message
 
+    def to_google_ai_dict(self, put_inner_thoughts_in_kwargs: bool = True) -> dict:
+        """Go from Message class to Google AI REST message object
+
+        type Content: https://ai.google.dev/api/rest/v1/Content / https://ai.google.dev/api/rest/v1beta/Content
+            parts[]: Part
+            role: str ('user' or 'model')
+        """
+        if self.role != "tool" and self.name is not None:
+            raise UserWarning(f"Using Google AI with non-null 'name' field ({self.name}) not yet supported.")
+
+        if self.role == "system":
+            # NOTE: Gemini API doesn't have a 'system' role, use 'user' instead
+            # https://www.reddit.com/r/Bard/comments/1b90i8o/does_gemini_have_a_system_prompt_option_while/
+            google_ai_message = {
+                "role": "user",  # NOTE: no 'system'
+                "parts": [{"text": self.text}],
+            }
+
+        elif self.role == "user":
+            assert all([v is not None for v in [self.text, self.role]]), vars(self)
+            google_ai_message = {
+                "role": "user",
+                "parts": [{"text": self.text}],
+            }
+
+        elif self.role == "assistant":
+            assert self.tool_calls is not None or self.text is not None
+            google_ai_message = {
+                "role": "model",  # NOTE: different
+            }
+
+            # NOTE: Google AI API doesn't allow non-null content + function call
+            # To get around this, just two a two part message, inner thoughts first then
+            parts = []
+            if not put_inner_thoughts_in_kwargs and self.text is not None:
+                # NOTE: ideally we do multi-part for CoT / inner thoughts + function call, but Google AI API doesn't allow it
+                raise NotImplementedError
+                parts.append({"text": self.text})
+
+            if self.tool_calls is not None:
+                # NOTE: implied support for multiple calls
+                for tool_call in self.tool_calls:
+                    function_name = tool_call.function["name"]
+                    function_args = tool_call.function["arguments"]
+                    try:
+                        # NOTE: Google AI wants actual JSON objects, not strings
+                        function_args = json.loads(function_args)
+                    except:
+                        raise UserWarning(f"Failed to parse JSON function args: {function_args}")
+                        function_args = {"args": function_args}
+
+                    if put_inner_thoughts_in_kwargs and self.text is not None:
+                        assert "inner_thoughts" not in function_args, function_args
+                        assert len(self.tool_calls) == 1
+                        function_args[INNER_THOUGHTS_KWARG] = self.text
+
+                    parts.append(
+                        {
+                            "functionCall": {
+                                "name": function_name,
+                                "args": function_args,
+                            }
+                        }
+                    )
+            else:
+                assert self.text is not None
+                parts.append({"text": self.text})
+            google_ai_message["parts"] = parts
+
+        elif self.role == "tool":
+            # NOTE: Significantly different tool calling format, more similar to function calling format
+            assert all([v is not None for v in [self.role, self.tool_call_id]]), vars(self)
+
+            if self.name is None:
+                raise UserWarning(f"Couldn't find function name on tool call, defaulting to tool ID instead.")
+                function_name = self.tool_call_id
+            else:
+                function_name = self.name
+
+            # NOTE: Google AI API wants the function response as JSON only, no string
+            try:
+                function_response = json.loads(self.text)
+            except:
+                function_response = {"function_response": self.text}
+
+            google_ai_message = {
+                "role": "function",
+                "parts": [
+                    {
+                        "functionResponse": {
+                            "name": function_name,
+                            "response": {
+                                "name": function_name,  # NOTE: name twice... why?
+                                "content": function_response,
+                            },
+                        }
+                    }
+                ],
+            }
+
+        else:
+            raise ValueError(self.role)
+
+        return google_ai_message
+
 
 class Document(Record):
     """A document represent a document loaded into MemGPT, which is broken down into passages."""
 
     def __init__(self, user_id: uuid.UUID, text: str, data_source: str, id: Optional[uuid.UUID] = None, metadata: Optional[Dict] = {}):
         if id is None:
             # by default, generate ID as a hash of the text (avoid duplicates)
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/embeddings.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/embeddings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/errors.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/errors.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/function_sets/base.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/function_sets/base.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/function_sets/extras.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/function_sets/extras.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from typing import Optional
 import os
 import json
 import requests
-
+import uuid
 
 from memgpt.constants import (
     JSON_LOADS_STRICT,
     MESSAGE_CHATGPT_FUNCTION_MODEL,
     MESSAGE_CHATGPT_FUNCTION_SYSTEM_MESSAGE,
     MAX_PAUSE_HEARTBEATS,
     JSON_ENSURE_ASCII,
 )
-from memgpt.llm_api_tools import create
+from memgpt.llm_api.llm_api_tools import create
+from memgpt.data_types import Message
 
 
 def message_chatgpt(self, message: str):
     """
     Send a message to a more basic AI, ChatGPT. A useful resource for asking questions. ChatGPT does not retain memory of previous interactions.
 
     Args:
         message (str): Message to send ChatGPT. Phrase your message as a full English sentence.
 
     Returns:
         str: Reply message from ChatGPT
     """
+    dummy_user_id = uuid.uuid4()
+    dummy_agent_id = uuid.uuid4()
     message_sequence = [
-        {"role": "system", "content": MESSAGE_CHATGPT_FUNCTION_SYSTEM_MESSAGE},
-        {"role": "user", "content": str(message)},
+        Message(user_id=dummy_user_id, agent_id=dummy_agent_id, role="system", text=MESSAGE_CHATGPT_FUNCTION_SYSTEM_MESSAGE),
+        Message(user_id=dummy_user_id, agent_id=dummy_agent_id, role="user", text=str(message)),
     ]
     response = create(
         model=MESSAGE_CHATGPT_FUNCTION_MODEL,
         messages=message_sequence,
-        # functions=functions,
-        # function_call=function_call,
     )
 
     reply = response.choices[0].message.content
     return reply
 
 
 def read_from_text_file(self, filename: str, line_start: int, num_lines: Optional[int] = 1):
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/functions.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/functions/schema_generator.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/functions/schema_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/interface.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/llm_api_tools.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/llm_api/google_ai.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,495 +1,463 @@
-import random
-import time
-import requests
-import time
-from typing import Union, Optional
-import urllib
-
-from memgpt.credentials import MemGPTCredentials
-from memgpt.local_llm.chat_completion_proxy import get_chat_completion
-from memgpt.constants import CLI_WARNING_PREFIX
-from memgpt.models.chat_completion_response import ChatCompletionResponse
-from memgpt.models.embedding_response import EmbeddingResponse
-
-from memgpt.data_types import AgentState
-
-MODEL_TO_AZURE_ENGINE = {
-    "gpt-4-1106-preview": "gpt-4",
-    "gpt-4": "gpt-4",
-    "gpt-4-32k": "gpt-4-32k",
-    "gpt-3.5": "gpt-35-turbo",
-    "gpt-3.5-turbo": "gpt-35-turbo",
-    "gpt-3.5-turbo-16k": "gpt-35-turbo-16k",
-}
-
-
-def is_context_overflow_error(exception):
-    from memgpt.utils import printd
-
-    match_string = "maximum context length"
-
-    # Backwards compatibility with openai python package/client v0.28 (pre-v1 client migration)
-    if match_string in str(exception):
-        printd(f"Found '{match_string}' in str(exception)={(str(exception))}")
-        return True
-
-    # Based on python requests + OpenAI REST API (/v1)
-    elif isinstance(exception, requests.exceptions.HTTPError):
-        if exception.response is not None and "application/json" in exception.response.headers.get("Content-Type", ""):
-            try:
-                error_details = exception.response.json()
-                if "error" not in error_details:
-                    printd(f"HTTPError occurred, but couldn't find error field: {error_details}")
-                    return False
-                else:
-                    error_details = error_details["error"]
-
-                # Check for the specific error code
-                if error_details.get("code") == "context_length_exceeded":
-                    printd(f"HTTPError occurred, caught error code {error_details.get('code')}")
-                    return True
-                # Soft-check for "maximum context length" inside of the message
-                elif error_details.get("message") and "maximum context length" in error_details.get("message"):
-                    printd(f"HTTPError occurred, found '{match_string}' in error message contents ({error_details})")
-                    return True
-                else:
-                    printd(f"HTTPError occurred, but unknown error message: {error_details}")
-                    return False
-            except ValueError:
-                # JSON decoding failed
-                printd(f"HTTPError occurred ({exception}), but no JSON error message.")
-
-    # Generic fail
-    else:
-        return False
-
-
-def smart_urljoin(base_url, relative_url):
-    """urljoin is stupid and wants a trailing / at the end of the endpoint address, or it will chop the suffix off"""
-    if not base_url.endswith("/"):
-        base_url += "/"
-    return urllib.parse.urljoin(base_url, relative_url)
-
-
-def clean_azure_endpoint(raw_endpoint_name):
-    """Make sure the endpoint is of format 'https://YOUR_RESOURCE_NAME.openai.azure.com'"""
-    if raw_endpoint_name is None:
-        raise ValueError(raw_endpoint_name)
-    endpoint_address = raw_endpoint_name.strip("/").replace(".openai.azure.com", "")
-    endpoint_address = endpoint_address.replace("http://", "")
-    endpoint_address = endpoint_address.replace("https://", "")
-    return endpoint_address
-
-
-def openai_get_model_list(url: str, api_key: Union[str, None], fix_url: Optional[bool] = False) -> dict:
-    """https://platform.openai.com/docs/api-reference/models/list"""
-    from memgpt.utils import printd
-
-    # In some cases we may want to double-check the URL and do basic correction, eg:
-    # In MemGPT config the address for vLLM is w/o a /v1 suffix for simplicity
-    # However if we're treating the server as an OpenAI proxy we want the /v1 suffix on our model hit
-    if fix_url:
-        if not url.endswith("/v1"):
-            url = smart_urljoin(url, "v1")
-
-    url = smart_urljoin(url, "models")
-
-    headers = {"Content-Type": "application/json"}
-    if api_key is not None:
-        headers["Authorization"] = f"Bearer {api_key}"
-
-    printd(f"Sending request to {url}")
-    try:
-        response = requests.get(url, headers=headers)
-        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
-        response = response.json()  # convert to dict from string
-        printd(f"response = {response}")
-        return response
-    except requests.exceptions.HTTPError as http_err:
-        # Handle HTTP errors (e.g., response 4XX, 5XX)
-        try:
-            response = response.json()
-        except:
-            pass
-        printd(f"Got HTTPError, exception={http_err}, response={response}")
-        raise http_err
-    except requests.exceptions.RequestException as req_err:
-        # Handle other requests-related errors (e.g., connection error)
-        try:
-            response = response.json()
-        except:
-            pass
-        printd(f"Got RequestException, exception={req_err}, response={response}")
-        raise req_err
-    except Exception as e:
-        # Handle other potential errors
-        try:
-            response = response.json()
-        except:
-            pass
-        printd(f"Got unknown Exception, exception={e}, response={response}")
-        raise e
-
-
-def azure_openai_get_model_list(url: str, api_key: Union[str, None], api_version: str) -> dict:
-    """https://learn.microsoft.com/en-us/rest/api/azureopenai/models/list?view=rest-azureopenai-2023-05-15&tabs=HTTP"""
-    from memgpt.utils import printd
-
-    # https://xxx.openai.azure.com/openai/models?api-version=xxx
-    url = smart_urljoin(url, "openai")
-    url = smart_urljoin(url, f"models?api-version={api_version}")
-
-    headers = {"Content-Type": "application/json"}
-    if api_key is not None:
-        headers["api-key"] = f"{api_key}"
-
-    printd(f"Sending request to {url}")
-    try:
-        response = requests.get(url, headers=headers)
-        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
-        response = response.json()  # convert to dict from string
-        printd(f"response = {response}")
-        return response
-    except requests.exceptions.HTTPError as http_err:
-        # Handle HTTP errors (e.g., response 4XX, 5XX)
-        try:
-            response = response.json()
-        except:
-            pass
-        printd(f"Got HTTPError, exception={http_err}, response={response}")
-        raise http_err
-    except requests.exceptions.RequestException as req_err:
-        # Handle other requests-related errors (e.g., connection error)
-        try:
-            response = response.json()
-        except:
-            pass
-        printd(f"Got RequestException, exception={req_err}, response={response}")
-        raise req_err
-    except Exception as e:
-        # Handle other potential errors
-        try:
-            response = response.json()
-        except:
-            pass
-        printd(f"Got unknown Exception, exception={e}, response={response}")
-        raise e
-
-
-def openai_chat_completions_request(url, api_key, data):
-    """https://platform.openai.com/docs/guides/text-generation?lang=curl"""
-    from memgpt.utils import printd
-
-    url = smart_urljoin(url, "chat/completions")
-    headers = {"Content-Type": "application/json", "Authorization": f"Bearer {api_key}"}
-
-    # If functions == None, strip from the payload
-    if "functions" in data and data["functions"] is None:
-        data.pop("functions")
-        data.pop("function_call", None)  # extra safe,  should exist always (default="auto")
-
-    if "tools" in data and data["tools"] is None:
-        data.pop("tools")
-        data.pop("tool_choice", None)  # extra safe,  should exist always (default="auto")
-
-    printd(f"Sending request to {url}")
-    try:
-        # Example code to trigger a rate limit response:
-        # mock_response = requests.Response()
-        # mock_response.status_code = 429
-        # http_error = requests.exceptions.HTTPError("429 Client Error: Too Many Requests")
-        # http_error.response = mock_response
-        # raise http_error
-
-        # Example code to trigger a context overflow response (for an 8k model)
-        # data["messages"][-1]["content"] = " ".join(["repeat after me this is not a fluke"] * 1000)
-
-        response = requests.post(url, headers=headers, json=data)
-        printd(f"response = {response}")
-        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
-        response = response.json()  # convert to dict from string
-        printd(f"response.json = {response}")
-        response = ChatCompletionResponse(**response)  # convert to 'dot-dict' style which is the openai python client default
-        return response
-    except requests.exceptions.HTTPError as http_err:
-        # Handle HTTP errors (e.g., response 4XX, 5XX)
-        printd(f"Got HTTPError, exception={http_err}, payload={data}")
-        raise http_err
-    except requests.exceptions.RequestException as req_err:
-        # Handle other requests-related errors (e.g., connection error)
-        printd(f"Got RequestException, exception={req_err}")
-        raise req_err
-    except Exception as e:
-        # Handle other potential errors
-        printd(f"Got unknown Exception, exception={e}")
-        raise e
-
-
-def openai_embeddings_request(url, api_key, data):
-    """https://platform.openai.com/docs/api-reference/embeddings/create"""
-    from memgpt.utils import printd
-
-    url = smart_urljoin(url, "embeddings")
-    headers = {"Content-Type": "application/json", "Authorization": f"Bearer {api_key}"}
-
-    printd(f"Sending request to {url}")
-    try:
-        response = requests.post(url, headers=headers, json=data)
-        printd(f"response = {response}")
-        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
-        response = response.json()  # convert to dict from string
-        printd(f"response.json = {response}")
-        response = EmbeddingResponse(**response)  # convert to 'dot-dict' style which is the openai python client default
-        return response
-    except requests.exceptions.HTTPError as http_err:
-        # Handle HTTP errors (e.g., response 4XX, 5XX)
-        printd(f"Got HTTPError, exception={http_err}, payload={data}")
-        raise http_err
-    except requests.exceptions.RequestException as req_err:
-        # Handle other requests-related errors (e.g., connection error)
-        printd(f"Got RequestException, exception={req_err}")
-        raise req_err
-    except Exception as e:
-        # Handle other potential errors
-        printd(f"Got unknown Exception, exception={e}")
-        raise e
-
-
-def azure_openai_chat_completions_request(resource_name, deployment_id, api_version, api_key, data):
-    """https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#chat-completions"""
-    from memgpt.utils import printd
-
-    assert resource_name is not None, "Missing required field when calling Azure OpenAI"
-    assert deployment_id is not None, "Missing required field when calling Azure OpenAI"
-    assert api_version is not None, "Missing required field when calling Azure OpenAI"
-    assert api_key is not None, "Missing required field when calling Azure OpenAI"
-
-    resource_name = clean_azure_endpoint(resource_name)
-    url = f"https://{resource_name}.openai.azure.com/openai/deployments/{deployment_id}/chat/completions?api-version={api_version}"
-    headers = {"Content-Type": "application/json", "api-key": f"{api_key}"}
-
-    # If functions == None, strip from the payload
-    if "functions" in data and data["functions"] is None:
-        data.pop("functions")
-        data.pop("function_call", None)  # extra safe,  should exist always (default="auto")
-
-    if "tools" in data and data["tools"] is None:
-        data.pop("tools")
-        data.pop("tool_choice", None)  # extra safe,  should exist always (default="auto")
-
-    printd(f"Sending request to {url}")
-    try:
-        response = requests.post(url, headers=headers, json=data)
-        printd(f"response = {response}")
-        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
-        response = response.json()  # convert to dict from string
-        printd(f"response.json = {response}")
-        # NOTE: azure openai does not include "content" in the response when it is None, so we need to add it
-        if "content" not in response["choices"][0].get("message"):
-            response["choices"][0]["message"]["content"] = None
-        response = ChatCompletionResponse(**response)  # convert to 'dot-dict' style which is the openai python client default
-        return response
-    except requests.exceptions.HTTPError as http_err:
-        # Handle HTTP errors (e.g., response 4XX, 5XX)
-        printd(f"Got HTTPError, exception={http_err}, payload={data}")
-        raise http_err
-    except requests.exceptions.RequestException as req_err:
-        # Handle other requests-related errors (e.g., connection error)
-        printd(f"Got RequestException, exception={req_err}")
-        raise req_err
-    except Exception as e:
-        # Handle other potential errors
-        printd(f"Got unknown Exception, exception={e}")
-        raise e
-
-
-def azure_openai_embeddings_request(resource_name, deployment_id, api_version, api_key, data):
-    """https://learn.microsoft.com/en-us/azure/ai-services/openai/reference#embeddings"""
-    from memgpt.utils import printd
-
-    resource_name = clean_azure_endpoint(resource_name)
-    url = f"https://{resource_name}.openai.azure.com/openai/deployments/{deployment_id}/embeddings?api-version={api_version}"
-    headers = {"Content-Type": "application/json", "api-key": f"{api_key}"}
-
-    printd(f"Sending request to {url}")
-    try:
-        response = requests.post(url, headers=headers, json=data)
-        printd(f"response = {response}")
-        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
-        response = response.json()  # convert to dict from string
-        printd(f"response.json = {response}")
-        response = EmbeddingResponse(**response)  # convert to 'dot-dict' style which is the openai python client default
-        return response
-    except requests.exceptions.HTTPError as http_err:
-        # Handle HTTP errors (e.g., response 4XX, 5XX)
-        printd(f"Got HTTPError, exception={http_err}, payload={data}")
-        raise http_err
-    except requests.exceptions.RequestException as req_err:
-        # Handle other requests-related errors (e.g., connection error)
-        printd(f"Got RequestException, exception={req_err}")
-        raise req_err
-    except Exception as e:
-        # Handle other potential errors
-        printd(f"Got unknown Exception, exception={e}")
-        raise e
-
-
-def retry_with_exponential_backoff(
-    func,
-    initial_delay: float = 1,
-    exponential_base: float = 2,
-    jitter: bool = True,
-    max_retries: int = 20,
-    # List of OpenAI error codes: https://github.com/openai/openai-python/blob/17ac6779958b2b74999c634c4ea4c7b74906027a/src/openai/_client.py#L227-L250
-    # 429 = rate limit
-    error_codes: tuple = (429,),
-):
-    """Retry a function with exponential backoff."""
-
-    def wrapper(*args, **kwargs):
-        from memgpt.utils import printd
-
-        # Initialize variables
-        num_retries = 0
-        delay = initial_delay
-
-        # Loop until a successful response or max_retries is hit or an exception is raised
-        while True:
-            try:
-                return func(*args, **kwargs)
-
-            except requests.exceptions.HTTPError as http_err:
-                # Retry on specified errors
-                if http_err.response.status_code in error_codes:
-                    # Increment retries
-                    num_retries += 1
-
-                    # Check if max retries has been reached
-                    if num_retries > max_retries:
-                        raise Exception(f"Maximum number of retries ({max_retries}) exceeded.")
-
-                    # Increment the delay
-                    delay *= exponential_base * (1 + jitter * random.random())
-
-                    # Sleep for the delay
-                    # printd(f"Got a rate limit error ('{http_err}') on LLM backend request, waiting {int(delay)}s then retrying...")
-                    print(
-                        f"{CLI_WARNING_PREFIX}Got a rate limit error ('{http_err}') on LLM backend request, waiting {int(delay)}s then retrying..."
-                    )
-                    time.sleep(delay)
-                else:
-                    # For other HTTP errors, re-raise the exception
-                    raise
-
-            # Raise exceptions for any errors not specified
-            except Exception as e:
-                raise e
-
-    return wrapper
-
-
-@retry_with_exponential_backoff
-def create(
-    agent_state: AgentState,
-    messages,
-    functions=None,
-    functions_python=None,
-    function_call="auto",
-    # hint
-    first_message=False,
-    # use tool naming?
-    # if false, will use deprecated 'functions' style
-    use_tool_naming=True,
-) -> ChatCompletionResponse:
-    """Return response to chat completion with backoff"""
-    from memgpt.utils import printd
-
-    printd(f"Using model {agent_state.llm_config.model_endpoint_type}, endpoint: {agent_state.llm_config.model_endpoint}")
-
-    # TODO eventually refactor so that credentials are passed through
-    credentials = MemGPTCredentials.load()
-
-    if function_call and not functions:
-        printd("unsetting function_call because functions is None")
-        function_call = None
-
-    # openai
-    if agent_state.llm_config.model_endpoint_type == "openai":
-        # TODO do the same for Azure?
-        if credentials.openai_key is None and agent_state.llm_config.model_endpoint == "https://api.openai.com/v1":
-            # only is a problem if we are *not* using an openai proxy
-            raise ValueError(f"OpenAI key is missing from MemGPT config file")
-        if use_tool_naming:
-            data = dict(
-                model=agent_state.llm_config.model,
-                messages=messages,
-                tools=[{"type": "function", "function": f} for f in functions] if functions else None,
-                tool_choice=function_call,
-                user=str(agent_state.user_id),
-            )
-        else:
-            data = dict(
-                model=agent_state.llm_config.model,
-                messages=messages,
-                functions=functions,
-                function_call=function_call,
-                user=str(agent_state.user_id),
-            )
-        return openai_chat_completions_request(
-            url=agent_state.llm_config.model_endpoint,  # https://api.openai.com/v1 -> https://api.openai.com/v1/chat/completions
-            api_key=credentials.openai_key,
-            data=data,
-        )
-
-    # azure
-    elif agent_state.llm_config.model_endpoint_type == "azure":
-        azure_deployment = (
-            credentials.azure_deployment
-            if credentials.azure_deployment is not None
-            else MODEL_TO_AZURE_ENGINE[agent_state.llm_config.model]
-        )
-        if use_tool_naming:
-            data = dict(
-                # NOTE: don't pass model to Azure calls, that is the deployment_id
-                # model=agent_config.model,
-                messages=messages,
-                tools=[{"type": "function", "function": f} for f in functions] if functions else None,
-                tool_choice=function_call,
-                user=str(agent_state.user_id),
-            )
-        else:
-            data = dict(
-                # NOTE: don't pass model to Azure calls, that is the deployment_id
-                # model=agent_config.model,
-                messages=messages,
-                functions=functions,
-                function_call=function_call,
-                user=str(agent_state.user_id),
-            )
-        return azure_openai_chat_completions_request(
-            resource_name=credentials.azure_endpoint,
-            deployment_id=azure_deployment,
-            api_version=credentials.azure_version,
-            api_key=credentials.azure_key,
-            data=data,
-        )
-
-    # local model
-    else:
-        return get_chat_completion(
-            model=agent_state.llm_config.model,
-            messages=messages,
-            functions=functions,
-            functions_python=functions_python,
-            function_call=function_call,
-            context_window=agent_state.llm_config.context_window,
-            endpoint=agent_state.llm_config.model_endpoint,
-            endpoint_type=agent_state.llm_config.model_endpoint_type,
-            wrapper=agent_state.llm_config.model_wrapper,
-            user=str(agent_state.user_id),
-            # hint
-            first_message=first_message,
-            # auth-related
-            auth_type=credentials.openllm_auth_type,
-            auth_key=credentials.openllm_key,
-        )
+import requests
+import json
+import uuid
+from typing import Union, List, Optional
+
+from memgpt.models.chat_completion_response import ChatCompletionResponse, Choice, Message, ToolCall, FunctionCall, UsageStatistics
+from memgpt.models.chat_completion_request import ChatCompletionRequest, Tool
+from memgpt.models.embedding_response import EmbeddingResponse
+from memgpt.utils import smart_urljoin, get_tool_call_id, get_utc_time
+from memgpt.local_llm.utils import count_tokens
+from memgpt.local_llm.json_parser import clean_json_string_extra_backslash
+from memgpt.constants import NON_USER_MSG_PREFIX, JSON_ENSURE_ASCII
+
+# from memgpt.data_types import ToolCall
+
+
+SUPPORTED_MODELS = [
+    "gemini-pro",
+]
+
+
+def google_ai_get_model_details(service_endpoint: str, api_key: str, model: str, key_in_header: bool = True) -> List[dict]:
+    from memgpt.utils import printd
+
+    # Two ways to pass the key: https://ai.google.dev/tutorials/setup
+    if key_in_header:
+        url = f"https://{service_endpoint}.googleapis.com/v1beta/models/{model}"
+        headers = {"Content-Type": "application/json", "x-goog-api-key": api_key}
+    else:
+        url = f"https://{service_endpoint}.googleapis.com/v1beta/models/{model}?key={api_key}"
+        headers = {"Content-Type": "application/json"}
+
+    try:
+        response = requests.get(url, headers=headers)
+        printd(f"response = {response}")
+        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
+        response = response.json()  # convert to dict from string
+        printd(f"response.json = {response}")
+
+        # Grab the models out
+        return response
+
+    except requests.exceptions.HTTPError as http_err:
+        # Handle HTTP errors (e.g., response 4XX, 5XX)
+        printd(f"Got HTTPError, exception={http_err}")
+        # Print the HTTP status code
+        print(f"HTTP Error: {http_err.response.status_code}")
+        # Print the response content (error message from server)
+        print(f"Message: {http_err.response.text}")
+        raise http_err
+
+    except requests.exceptions.RequestException as req_err:
+        # Handle other requests-related errors (e.g., connection error)
+        printd(f"Got RequestException, exception={req_err}")
+        raise req_err
+
+    except Exception as e:
+        # Handle other potential errors
+        printd(f"Got unknown Exception, exception={e}")
+        raise e
+
+
+def google_ai_get_model_context_window(service_endpoint: str, api_key: str, model: str, key_in_header: bool = True) -> int:
+    model_details = google_ai_get_model_details(
+        service_endpoint=service_endpoint, api_key=api_key, model=model, key_in_header=key_in_header
+    )
+    # TODO should this be:
+    # return model_details["inputTokenLimit"] + model_details["outputTokenLimit"]
+    return int(model_details["inputTokenLimit"])
+
+
+def google_ai_get_model_list(service_endpoint: str, api_key: str, key_in_header: bool = True) -> List[dict]:
+    from memgpt.utils import printd
+
+    # Two ways to pass the key: https://ai.google.dev/tutorials/setup
+    if key_in_header:
+        url = f"https://{service_endpoint}.googleapis.com/v1beta/models"
+        headers = {"Content-Type": "application/json", "x-goog-api-key": api_key}
+    else:
+        url = f"https://{service_endpoint}.googleapis.com/v1beta/models?key={api_key}"
+        headers = {"Content-Type": "application/json"}
+
+    try:
+        response = requests.get(url, headers=headers)
+        printd(f"response = {response}")
+        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
+        response = response.json()  # convert to dict from string
+        printd(f"response.json = {response}")
+
+        # Grab the models out
+        model_list = response["models"]
+        return model_list
+
+    except requests.exceptions.HTTPError as http_err:
+        # Handle HTTP errors (e.g., response 4XX, 5XX)
+        printd(f"Got HTTPError, exception={http_err}")
+        # Print the HTTP status code
+        print(f"HTTP Error: {http_err.response.status_code}")
+        # Print the response content (error message from server)
+        print(f"Message: {http_err.response.text}")
+        raise http_err
+
+    except requests.exceptions.RequestException as req_err:
+        # Handle other requests-related errors (e.g., connection error)
+        printd(f"Got RequestException, exception={req_err}")
+        raise req_err
+
+    except Exception as e:
+        # Handle other potential errors
+        printd(f"Got unknown Exception, exception={e}")
+        raise e
+
+
+def add_dummy_model_messages(messages: List[dict]) -> List[dict]:
+    """Google AI API requires all function call returns are immediately followed by a 'model' role message.
+
+    In MemGPT, the 'model' will often call a function (e.g. send_message) that itself yields to the user,
+    so there is no natural follow-up 'model' role message.
+
+    To satisfy the Google AI API restrictions, we can add a dummy 'yield' message
+    with role == 'model' that is placed in-betweeen and function output
+    (role == 'tool') and user message (role == 'user').
+    """
+    dummy_yield_message = {"role": "model", "parts": [{"text": f"{NON_USER_MSG_PREFIX}Function call returned, waiting for user response."}]}
+    messages_with_padding = []
+    for i, message in enumerate(messages):
+        messages_with_padding.append(message)
+        # Check if the current message role is 'tool' and the next message role is 'user'
+        if message["role"] in ["tool", "function"] and (i + 1 < len(messages) and messages[i + 1]["role"] == "user"):
+            messages_with_padding.append(dummy_yield_message)
+
+    return messages_with_padding
+
+
+# TODO use pydantic model as input
+def to_google_ai(openai_message_dict: dict) -> dict:
+
+    # TODO supports "parts" as part of multimodal support
+    assert not isinstance(openai_message_dict["content"], list), "Multi-part content is message not yet supported"
+    if openai_message_dict["role"] == "user":
+        google_ai_message_dict = {
+            "role": "user",
+            "parts": [{"text": openai_message_dict["content"]}],
+        }
+    elif openai_message_dict["role"] == "assistant":
+        google_ai_message_dict = {
+            "role": "model",  # NOTE: diff
+            "parts": [{"text": openai_message_dict["content"]}],
+        }
+    elif openai_message_dict["role"] == "tool":
+        google_ai_message_dict = {
+            "role": "function",  # NOTE: diff
+            "parts": [{"text": openai_message_dict["content"]}],
+        }
+    else:
+        raise ValueError(f"Unsupported conversion (OpenAI -> Google AI) from role {openai_message_dict['role']}")
+
+
+# TODO convert return type to pydantic
+def convert_tools_to_google_ai_format(tools: List[Tool], inner_thoughts_in_kwargs: Optional[bool] = True) -> List[dict]:
+    """
+    OpenAI style:
+      "tools": [{
+        "type": "function",
+        "function": {
+            "name": "find_movies",
+            "description": "find ....",
+            "parameters": {
+              "type": "object",
+              "properties": {
+                 PARAM: {
+                   "type": PARAM_TYPE,  # eg "string"
+                   "description": PARAM_DESCRIPTION,
+                 },
+                 ...
+              },
+              "required": List[str],
+            }
+        }
+      }
+      ]
+
+    Google AI style:
+      "tools": [{
+        "functionDeclarations": [{
+          "name": "find_movies",
+          "description": "find movie titles currently playing in theaters based on any description, genre, title words, etc.",
+          "parameters": {
+            "type": "OBJECT",
+            "properties": {
+              "location": {
+                "type": "STRING",
+                "description": "The city and state, e.g. San Francisco, CA or a zip code e.g. 95616"
+              },
+              "description": {
+                "type": "STRING",
+                "description": "Any kind of description including category or genre, title words, attributes, etc."
+              }
+            },
+            "required": ["description"]
+          }
+        }, {
+          "name": "find_theaters",
+          ...
+    """
+    function_list = [
+        dict(
+            name=t.function.name,
+            description=t.function.description,
+            parameters=t.function.parameters,  # TODO need to unpack
+        )
+        for t in tools
+    ]
+
+    # Correct casing + add inner thoughts if needed
+    for func in function_list:
+        func["parameters"]["type"] = "OBJECT"
+        for param_name, param_fields in func["parameters"]["properties"].items():
+            param_fields["type"] = param_fields["type"].upper()
+        # Add inner thoughts
+        if inner_thoughts_in_kwargs:
+            from memgpt.local_llm.constants import INNER_THOUGHTS_KWARG, INNER_THOUGHTS_KWARG_DESCRIPTION
+
+            func["parameters"]["properties"][INNER_THOUGHTS_KWARG] = {
+                "type": "STRING",
+                "description": INNER_THOUGHTS_KWARG_DESCRIPTION,
+            }
+            func["parameters"]["required"].append(INNER_THOUGHTS_KWARG)
+
+    return [{"functionDeclarations": function_list}]
+
+
+def convert_google_ai_response_to_chatcompletion(
+    response_json: dict,  # REST response from Google AI API
+    model: str,  # Required since not returned
+    input_messages: Optional[List[dict]] = None,  # Required if the API doesn't return UsageMetadata
+    pull_inner_thoughts_from_args: Optional[bool] = True,
+) -> ChatCompletionResponse:
+    """Google AI API response format is not the same as ChatCompletion, requires unpacking
+
+    Example:
+    {
+      "candidates": [
+        {
+          "content": {
+            "parts": [
+              {
+                "text": " OK. Barbie is showing in two theaters in Mountain View, CA: AMC Mountain View 16 and Regal Edwards 14."
+              }
+            ]
+          }
+        }
+      ],
+      "usageMetadata": {
+        "promptTokenCount": 9,
+        "candidatesTokenCount": 27,
+        "totalTokenCount": 36
+      }
+    }
+    """
+    try:
+        choices = []
+        for candidate in response_json["candidates"]:
+            content = candidate["content"]
+
+            role = content["role"]
+            assert role == "model", f"Unknown role in response: {role}"
+
+            parts = content["parts"]
+            # TODO support parts / multimodal
+            assert len(parts) == 1, f"Multi-part not yet supported:\n{parts}"
+            response_message = parts[0]
+
+            # Convert the actual message style to OpenAI style
+            if "functionCall" in response_message and response_message["functionCall"] is not None:
+                function_call = response_message["functionCall"]
+                assert isinstance(function_call, dict), function_call
+                function_name = function_call["name"]
+                assert isinstance(function_name, str), function_name
+                function_args = function_call["args"]
+                assert isinstance(function_args, dict), function_args
+
+                # NOTE: this also involves stripping the inner monologue out of the function
+                if pull_inner_thoughts_from_args:
+                    from memgpt.local_llm.constants import INNER_THOUGHTS_KWARG, INNER_THOUGHTS_KWARG_DESCRIPTION
+
+                    assert INNER_THOUGHTS_KWARG in function_args, f"Couldn't find inner thoughts in function args:\n{function_call}"
+                    inner_thoughts = function_args.pop(INNER_THOUGHTS_KWARG)
+                    assert inner_thoughts is not None, f"Expected non-null inner thoughts function arg:\n{function_call}"
+                else:
+                    inner_thoughts = None
+
+                # Google AI API doesn't generate tool call IDs
+                openai_response_message = Message(
+                    role="assistant",  # NOTE: "model" -> "assistant"
+                    content=inner_thoughts,
+                    tool_calls=[
+                        ToolCall(
+                            id=get_tool_call_id(),
+                            type="function",
+                            function=FunctionCall(
+                                name=function_name,
+                                arguments=clean_json_string_extra_backslash(json.dumps(function_args)),
+                            ),
+                        )
+                    ],
+                )
+
+            else:
+
+                # Inner thoughts are the content by default
+                inner_thoughts = response_message["text"]
+
+                # Google AI API doesn't generate tool call IDs
+                openai_response_message = Message(
+                    role="assistant",  # NOTE: "model" -> "assistant"
+                    content=inner_thoughts,
+                )
+
+            # Google AI API uses different finish reason strings than OpenAI
+            # OpenAI: 'stop', 'length', 'function_call', 'content_filter', null
+            #   see: https://platform.openai.com/docs/guides/text-generation/chat-completions-api
+            # Google AI API: FINISH_REASON_UNSPECIFIED, STOP, MAX_TOKENS, SAFETY, RECITATION, OTHER
+            #   see: https://ai.google.dev/api/python/google/ai/generativelanguage/Candidate/FinishReason
+            finish_reason = candidate["finishReason"]
+            if finish_reason == "STOP":
+                openai_finish_reason = (
+                    "function_call"
+                    if openai_response_message.tool_calls is not None and len(openai_response_message.tool_calls) > 0
+                    else "stop"
+                )
+            elif finish_reason == "MAX_TOKENS":
+                openai_finish_reason = "length"
+            elif finish_reason == "SAFETY":
+                openai_finish_reason = "content_filter"
+            elif finish_reason == "RECITATION":
+                openai_finish_reason = "content_filter"
+            else:
+                raise ValueError(f"Unrecognized finish reason in Google AI response: {finish_reason}")
+
+            choices.append(
+                Choice(
+                    finish_reason=openai_finish_reason,
+                    index=candidate["index"],
+                    message=openai_response_message,
+                )
+            )
+
+        if len(choices) > 1:
+            raise UserWarning(f"Unexpected number of candidates in response (expected 1, got {len(choices)})")
+
+        # NOTE: some of the Google AI APIs show UsageMetadata in the response, but it seems to not exist?
+        #  "usageMetadata": {
+        #     "promptTokenCount": 9,
+        #     "candidatesTokenCount": 27,
+        #     "totalTokenCount": 36
+        #   }
+        if "usageMetadata" in response_json:
+            usage = UsageStatistics(
+                prompt_tokens=response_json["usageMetadata"]["promptTokenCount"],
+                completion_tokens=response_json["usageMetadata"]["candidatesTokenCount"],
+                total_tokens=response_json["usageMetadata"]["totalTokenCount"],
+            )
+        else:
+            # Count it ourselves
+            assert input_messages is not None, f"Didn't get UsageMetadata from the API response, so input_messages is required"
+            prompt_tokens = count_tokens(
+                json.dumps(input_messages, ensure_ascii=JSON_ENSURE_ASCII)
+            )  # NOTE: this is a very rough approximation
+            completion_tokens = count_tokens(
+                json.dumps(openai_response_message.model_dump(), ensure_ascii=JSON_ENSURE_ASCII)
+            )  # NOTE: this is also approximate
+            total_tokens = prompt_tokens + completion_tokens
+            usage = UsageStatistics(
+                prompt_tokens=prompt_tokens,
+                completion_tokens=completion_tokens,
+                total_tokens=total_tokens,
+            )
+
+        response_id = str(uuid.uuid4())
+        return ChatCompletionResponse(
+            id=response_id,
+            choices=choices,
+            model=model,  # NOTE: Google API doesn't pass back model in the response
+            created=get_utc_time(),
+            usage=usage,
+        )
+    except KeyError as e:
+        raise e
+
+
+# TODO convert 'data' type to pydantic
+def google_ai_chat_completions_request(
+    service_endpoint: str,
+    model: str,
+    api_key: str,
+    data: dict,
+    key_in_header: bool = True,
+    add_postfunc_model_messages: bool = True,
+    # NOTE: Google AI API doesn't support mixing parts 'text' and 'function',
+    # so there's no clean way to put inner thoughts in the same message as a function call
+    inner_thoughts_in_kwargs: bool = True,
+) -> ChatCompletionResponse:
+    """https://ai.google.dev/docs/function_calling
+
+    From https://ai.google.dev/api/rest#service-endpoint:
+    "A service endpoint is a base URL that specifies the network address of an API service.
+    One service might have multiple service endpoints.
+    This service has the following service endpoint and all URIs below are relative to this service endpoint:
+    https://xxx.googleapis.com
+    """
+    from memgpt.utils import printd
+
+    assert service_endpoint is not None, "Missing service_endpoint when calling Google AI"
+    assert api_key is not None, "Missing api_key when calling Google AI"
+    assert model in SUPPORTED_MODELS, f"Model '{model}' not in supported models: {', '.join(SUPPORTED_MODELS)}"
+
+    # Two ways to pass the key: https://ai.google.dev/tutorials/setup
+    if key_in_header:
+        url = f"https://{service_endpoint}.googleapis.com/v1beta/models/{model}:generateContent"
+        headers = {"Content-Type": "application/json", "x-goog-api-key": api_key}
+    else:
+        url = f"https://{service_endpoint}.googleapis.com/v1beta/models/{model}:generateContent?key={api_key}"
+        headers = {"Content-Type": "application/json"}
+
+    # data["contents"][-1]["role"] = "model"
+    if add_postfunc_model_messages:
+        data["contents"] = add_dummy_model_messages(data["contents"])
+
+    printd(f"Sending request to {url}")
+    try:
+        response = requests.post(url, headers=headers, json=data)
+        printd(f"response = {response}")
+        response.raise_for_status()  # Raises HTTPError for 4XX/5XX status
+        response = response.json()  # convert to dict from string
+        printd(f"response.json = {response}")
+
+        # Convert Google AI response to ChatCompletion style
+        return convert_google_ai_response_to_chatcompletion(
+            response_json=response,
+            model=model,
+            input_messages=data["contents"],
+            pull_inner_thoughts_from_args=inner_thoughts_in_kwargs,
+        )
+
+    except requests.exceptions.HTTPError as http_err:
+        # Handle HTTP errors (e.g., response 4XX, 5XX)
+        printd(f"Got HTTPError, exception={http_err}, payload={data}")
+        # Print the HTTP status code
+        print(f"HTTP Error: {http_err.response.status_code}")
+        # Print the response content (error message from server)
+        print(f"Message: {http_err.response.text}")
+        raise http_err
+
+    except requests.exceptions.RequestException as req_err:
+        # Handle other requests-related errors (e.g., connection error)
+        printd(f"Got RequestException, exception={req_err}")
+        raise req_err
+
+    except Exception as e:
+        # Handle other potential errors
+        printd(f"Got unknown Exception, exception={e}")
+        raise e
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/chat_completion_proxy.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/chat_completion_proxy.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/constants.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,7 +19,10 @@
 DEFAULT_OLLAMA_MODEL = "dolphin2.2-mistral:7b-q6_K"
 
 # DEFAULT_WRAPPER = airoboros.Airoboros21InnerMonologueWrapper
 # DEFAULT_WRAPPER_NAME = "airoboros-l2-70b-2.1"
 
 DEFAULT_WRAPPER = ChatMLInnerMonologueWrapper
 DEFAULT_WRAPPER_NAME = "chatml"
+
+INNER_THOUGHTS_KWARG = "inner_thoughts"
+INNER_THOUGHTS_KWARG_DESCRIPTION = "Deep inner monologue private to you only."
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/function_parser.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/function_parser.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/grammars/gbnf_grammar_generator.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/gbnf_grammar_generator.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/grammars/json.gbnf` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/grammars/json_func_calls_with_inner_thoughts.gbnf`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/groq/api.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/groq/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/json_parser.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/json_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import json
 import re
 from memgpt.constants import JSON_LOADS_STRICT
 
 from memgpt.errors import LLMJSONParsingError
 
 
+def clean_json_string_extra_backslash(s):
+    """Clean extra backslashes out from stringified JSON
+
+    NOTE: Google AI Gemini API likes to include these
+    """
+    # Strip slashes that are used to escape single quotes and other backslashes
+    # Use json.loads to parse it correctly
+    while "\\\\" in s:
+        s = s.replace("\\\\", "\\")
+    return s
+
+
 def replace_escaped_underscores(string: str):
     """Handles the case of escaped underscores, e.g.:
 
     {
       "function":"send\_message",
       "params": {
         "inner\_thoughts": "User is asking for information about themselves. Retrieving data from core memory.",
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/koboldcpp/api.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/koboldcpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/koboldcpp/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/koboldcpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llamacpp/api.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llamacpp/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llamacpp/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llamacpp/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/airoboros.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/chatml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 
-from .wrapper_base import LLMChatCompletionWrapper
-from ..json_parser import clean_json
-from ...constants import JSON_ENSURE_ASCII, JSON_LOADS_STRICT
-from ...errors import LLMJSONParsingError
+from memgpt.local_llm.llm_chat_completion_wrappers.wrapper_base import LLMChatCompletionWrapper
+from memgpt.local_llm.json_parser import clean_json
+from memgpt.constants import JSON_ENSURE_ASCII, JSON_LOADS_STRICT
+from memgpt.errors import LLMJSONParsingError
 
 
 PREFIX_HINT = """# Reminders:
 # Important information about yourself and the user is stored in (limited) core memory
 # You can modify core memory with core_memory_replace
 # You can add to core memory with core_memory_append
 # Less important information is stored in (unlimited) archival memory
@@ -71,15 +71,17 @@
         """Go from a JSON schema to a string description for a prompt"""
         # airorobos style
         func_str = ""
         func_str += f"{schema['name']}:"
         func_str += f"\n  description: {schema['description']}"
         func_str += f"\n  params:"
         if add_inner_thoughts:
-            func_str += f"\n    inner_thoughts: Deep inner monologue private to you only."
+            from memgpt.local_llm.constants import INNER_THOUGHTS_KWARG, INNER_THOUGHTS_KWARG_DESCRIPTION
+
+            func_str += f"\n    {INNER_THOUGHTS_KWARG}: {INNER_THOUGHTS_KWARG_DESCRIPTION}"
         for param_k, param_v in schema["parameters"]["properties"].items():
             # TODO we're ignoring type
             func_str += f"\n    {param_k}: {param_v['description']}"
         # TODO we're ignoring schema['parameters']['required']
         return func_str
 
     def _compile_function_block(self, functions) -> str:
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/configurable_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/dolphin.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/simple_summary_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/llm_chat_completion_wrappers/zephyr.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/lmstudio/api.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/lmstudio/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/lmstudio/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/lmstudio/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/ollama/api.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/ollama/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/ollama/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/ollama/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/settings/deterministic_mirostat.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/deterministic_mirostat.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/settings/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/settings/simple.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/settings/simple.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/utils.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/vllm/api.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/vllm/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/webui/api.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/webui/legacy_api.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/legacy_api.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/webui/legacy_settings.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/legacy_settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/local_llm/webui/settings.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/local_llm/webui/settings.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/log.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/log.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/main.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 import traceback
+import requests
 import json
 
 import questionary
 import typer
 
 from rich.console import Console
 from memgpt.constants import FUNC_FAILED_HEARTBEAT_MESSAGE, JSON_ENSURE_ASCII, JSON_LOADS_STRICT, REQ_HEARTBEAT_MESSAGE
@@ -267,15 +268,15 @@
                     try:
                         memgpt_agent.summarize_messages_inplace()
                         typer.secho(
                             f"/summarize succeeded",
                             fg=typer.colors.GREEN,
                             bold=True,
                         )
-                    except errors.LLMError as e:
+                    except (errors.LLMError, requests.exceptions.HTTPError) as e:
                         typer.secho(
                             f"/summarize failed:\n{e}",
                             fg=typer.colors.RED,
                             bold=True,
                         )
                     continue
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/memory.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABC, abstractmethod
 import datetime
 import uuid
 from typing import Optional, List, Tuple, Union
 
-from memgpt.constants import MESSAGE_SUMMARY_WARNING_FRAC
+from memgpt.constants import MESSAGE_SUMMARY_WARNING_FRAC, MESSAGE_SUMMARY_REQUEST_ACK
 from memgpt.utils import get_local_time, printd, count_tokens, validate_date_format, extract_date_from_timestamp
 from memgpt.prompts.gpt_summarize import SYSTEM as SUMMARY_PROMPT_SYSTEM
-from memgpt.llm_api_tools import create
+from memgpt.llm_api.llm_api_tools import create
 from memgpt.data_types import Message, Passage, AgentState
 from memgpt.embeddings import embedding_model, query_embedding, parse_and_chunk_text
 
 # from llama_index import Document
 # from llama_index.node_parser import SimpleNodeParser
 
 
@@ -98,36 +98,46 @@
                 return self.edit_human(new_human)
             else:
                 raise ValueError("Content not found in human (make sure to use exact string)")
         else:
             raise KeyError(f'No memory section named {field} (must be either "persona" or "human")')
 
 
+def _format_summary_history(message_history: List[Message]):
+    # TODO use existing prompt formatters for this (eg ChatML)
+    return "\n".join([f"{m.role}: {m.text}" for m in message_history])
+
+
 def summarize_messages(
     agent_state: AgentState,
-    message_sequence_to_summarize,
+    message_sequence_to_summarize: List[Message],
+    insert_acknowledgement_assistant_message: bool = True,
 ):
     """Summarize a message sequence using GPT"""
     # we need the context_window
     context_window = agent_state.llm_config.context_window
 
     summary_prompt = SUMMARY_PROMPT_SYSTEM
-    summary_input = str(message_sequence_to_summarize)
+    summary_input = _format_summary_history(message_sequence_to_summarize)
     summary_input_tkns = count_tokens(summary_input)
     if summary_input_tkns > MESSAGE_SUMMARY_WARNING_FRAC * context_window:
         trunc_ratio = (MESSAGE_SUMMARY_WARNING_FRAC * context_window / summary_input_tkns) * 0.8  # For good measure...
         cutoff = int(len(message_sequence_to_summarize) * trunc_ratio)
         summary_input = str(
             [summarize_messages(agent_state, message_sequence_to_summarize=message_sequence_to_summarize[:cutoff])]
             + message_sequence_to_summarize[cutoff:]
         )
-    message_sequence = [
-        {"role": "system", "content": summary_prompt},
-        {"role": "user", "content": summary_input},
-    ]
+
+    dummy_user_id = uuid.uuid4()
+    dummy_agent_id = uuid.uuid4()
+    message_sequence = []
+    message_sequence.append(Message(user_id=dummy_user_id, agent_id=dummy_agent_id, role="system", text=summary_prompt))
+    if insert_acknowledgement_assistant_message:
+        message_sequence.append(Message(user_id=dummy_user_id, agent_id=dummy_agent_id, role="assistant", text=MESSAGE_SUMMARY_REQUEST_ACK))
+    message_sequence.append(Message(user_id=dummy_user_id, agent_id=dummy_agent_id, role="user", text=summary_input))
 
     response = create(
         agent_state=agent_state,
         messages=message_sequence,
     )
 
     printd(f"summarize_messages gpt reply: {response.choices[0]}")
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/metadata.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/metadata.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/migrate.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/migrate.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/chat_completion_request.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/chat_completion_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,22 +10,54 @@
 
 class UserMessage(BaseModel):
     content: Union[str, List[str]]
     role: str = "user"
     name: Optional[str] = None
 
 
+class ToolCallFunction(BaseModel):
+    name: str
+    arguments: str
+
+
+class ToolCall(BaseModel):
+    id: str
+    type: Literal["function"] = "function"
+    function: ToolCallFunction
+
+
 class AssistantMessage(BaseModel):
     content: Optional[str] = None
     role: str = "assistant"
     name: Optional[str] = None
-    tool_calls: Optional[List] = None
+    tool_calls: Optional[List[ToolCall]] = None
 
 
-ChatMessage = Union[SystemMessage, UserMessage, AssistantMessage]
+class ToolMessage(BaseModel):
+    content: str
+    role: str = "tool"
+    tool_call_id: str
+
+
+ChatMessage = Union[SystemMessage, UserMessage, AssistantMessage, ToolMessage]
+
+
+def cast_message_to_subtype(m_dict: dict) -> ChatMessage:
+    """Cast a dictionary to one of the individual message types"""
+    role = m_dict.get("role")
+    if role == "system":
+        return SystemMessage(**m_dict)
+    elif role == "user":
+        return UserMessage(**m_dict)
+    elif role == "assistant":
+        return AssistantMessage(**m_dict)
+    elif role == "tool":
+        return ToolMessage(**m_dict)
+    else:
+        raise ValueError("Unknown message role")
 
 
 class ResponseFormat(BaseModel):
     type: str = Field(default="text", pattern="^(text|json_object)$")
 
 
 ## tool_choice ##
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/chat_completion_response.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/openai.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/openai.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/models/pydantic_models.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/models/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/openai_backcompat/openai_object.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/openai_backcompat/openai_object.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/persistence_manager.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/anna_pa.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/anna_pa.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/google_search_persona.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/google_search_persona.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/sam.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/sam_pov.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam_pov.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/sam_simple_pov_gpt35.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sam_simple_pov_gpt35.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/personas/examples/sqldb/test.db` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/personas/examples/sqldb/test.db`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/presets/presets.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/presets.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/presets/utils.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/presets/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/gpt_functions.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_functions.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/gpt_summarize.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_summarize.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/gpt_system.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/gpt_system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_base.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_base.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_chat.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_chat_compressed.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_chat_compressed.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_doc.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_doc.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_gpt35_extralong.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_gpt35_extralong.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_intuitive_knowledge.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_intuitive_knowledge.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/prompts/system/memgpt_modified_chat.txt` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/prompts/system/memgpt_modified_chat.txt`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/admin/users.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/admin/users.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/command.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/command.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/config.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/config.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/memory.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/memory.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/agents/message.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/agents/message.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/auth/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/auth_token.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/auth_token.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/config/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/config/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/humans/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/humans/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/interface.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/models/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/models/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/openai_assistants/assistants.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/openai_assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/personas/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/personas/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/presets/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/presets/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/server.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/sources/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/sources/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/static_files.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/static_files.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/rest_api/tools/index.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/rest_api/tools/index.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/server.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/assets/index-0c5d3001.css` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/assets/index-0c5d3001.css`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/assets/index-bf421135.js` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/assets/index-bf421135.js`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/favicon.ico` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/favicon.ico`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/index.html` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/index.html`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/static_files/memgpt_logo_transparent.png` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/static_files/memgpt_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/utils.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/utils.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/example_client.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/example_client.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/interface.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/interface.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/protocol.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/protocol.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/server/ws_api/server.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/server/ws_api/server.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/system.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/system.py`

 * *Files identical despite different names*

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/memgpt/utils.py` & `pymemgpt_nightly-0.3.9.dev20240411025350/memgpt/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import hashlib
 from typing import List
 import inspect
 from functools import wraps
 from typing import get_type_hints, Union, _GenericAlias
 
 
-from urllib.parse import urlparse
+from urllib.parse import urlparse, urljoin
 from contextlib import contextmanager
 import difflib
 import demjson3 as demjson
 import pytz
 import tiktoken
 
 import memgpt
@@ -465,14 +465,21 @@
     "walrus",
     "xylophone",
     "yak",
     "zebra",
 ]
 
 
+def smart_urljoin(base_url: str, relative_url: str) -> str:
+    """urljoin is stupid and wants a trailing / at the end of the endpoint address, or it will chop the suffix off"""
+    if not base_url.endswith("/"):
+        base_url += "/"
+    return urljoin(base_url, relative_url)
+
+
 def is_utc_datetime(dt: datetime) -> bool:
     return dt.tzinfo is not None and dt.tzinfo.utcoffset(dt) == timedelta(0)
 
 
 def get_tool_call_id() -> str:
     return str(uuid.uuid4())[:TOOL_CALL_ID_MAX_LEN]
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/pyproject.toml` & `pymemgpt_nightly-0.3.9.dev20240411025350/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymemgpt-nightly"
-version = "0.3.8.dev20240410103932"
+version = "0.3.9.dev20240411025350"
 packages = [
     {include = "memgpt"}
 ]
 description = "Teaching LLMs memory management for unbounded context"
 authors = [
     "MemGPT Team <hi@memgpt.ai>",
 ]
```

### Comparing `pymemgpt_nightly-0.3.8.dev20240410103932/PKG-INFO` & `pymemgpt_nightly-0.3.9.dev20240411025350/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemgpt-nightly
-Version: 0.3.8.dev20240410103932
+Version: 0.3.9.dev20240411025350
 Summary: Teaching LLMs memory management for unbounded context
 License: Apache License
 Author: MemGPT Team
 Author-email: hi@memgpt.ai
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.8.dev20240410103932
+Metadata-Version: 2.1 Name: pymemgpt-nightly Version: 0.3.9.dev20240411025350
 Summary: Teaching LLMs memory management for unbounded context License: Apache
 License Author: MemGPT Team Author-email: hi@memgpt.ai Requires-Python:
 >=3.10,<3.13 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Provides-Extra: autogen Provides-Extra:
 dev Provides-Extra: local Provides-Extra: postgres Provides-Extra: server
```

