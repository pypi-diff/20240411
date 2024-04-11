# Comparing `tmp/langchain-0.1.8.tar.gz` & `tmp/langchain-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-0.1.8.tar", max compression
+gzip compressed data, was "langchain-0.1.9.tar", max compression
```

## Comparing `langchain-0.1.8.tar` & `langchain-0.1.9.tar`

### file list

```diff
@@ -1,1326 +1,1326 @@
--rw-r--r--   0        0        0     1067 2024-02-19 20:58:55.553226 langchain-0.1.8/LICENSE
--rw-r--r--   0        0        0     5879 2024-02-19 20:58:55.553226 langchain-0.1.8/README.md
--rw-r--r--   0        0        0    13561 2024-02-19 20:58:55.553226 langchain-0.1.8/langchain/__init__.py
--rw-r--r--   0        0        0      667 2024-02-19 20:58:55.553226 langchain-0.1.8/langchain/_api/__init__.py
--rw-r--r--   0        0        0      471 2024-02-19 20:58:55.553226 langchain-0.1.8/langchain/_api/deprecation.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.553226 langchain-0.1.8/langchain/_api/path.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.553226 langchain-0.1.8/langchain/adapters/__init__.py
--rw-r--r--   0        0        0      653 2024-02-19 20:58:55.553226 langchain-0.1.8/langchain/adapters/openai.py
--rw-r--r--   0        0        0     4813 2024-02-19 20:58:55.553226 langchain-0.1.8/langchain/agents/__init__.py
--rw-r--r--   0        0        0    54729 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent.py
--rw-r--r--   0        0        0    15135 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_iterator.py
--rw-r--r--   0        0        0     3678 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       25 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/ainetwork/__init__.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/ainetwork/toolkit.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0      156 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/base.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/clickup/__init__.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/clickup/toolkit.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0     3235 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/conversational_retrieval/tool.py
--rw-r--r--   0        0        0     1091 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0      177 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0      617 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       22 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/gitlab/__init__.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/gitlab/toolkit.py
--rw-r--r--   0        0        0       21 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/json/base.py
--rw-r--r--   0        0        0      126 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0       23 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0       19 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/nasa/__init__.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/nasa/toolkit.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0       96 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0      530 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0     1153 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0      186 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0      170 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0      157 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0     1104 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0      174 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0      140 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0      269 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0     1094 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0       21 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/slack/__init__.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/slack/toolkit.py
--rw-r--r--   0        0        0     1103 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0       23 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0      123 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0      127 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0      184 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       21 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/steam/__init__.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/steam/toolkit.py
--rw-r--r--   0        0        0       56 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/vectorstore/__init__.py
--rw-r--r--   0        0        0     4211 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/vectorstore/base.py
--rw-r--r--   0        0        0      834 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/vectorstore/prompt.py
--rw-r--r--   0        0        0     3001 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/vectorstore/toolkit.py
--rw-r--r--   0        0        0     1095 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0       22 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0     1948 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/agent_types.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/chat/__init__.py
--rw-r--r--   0        0        0     5084 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/chat/base.py
--rw-r--r--   0        0        0     1977 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/chat/output_parser.py
--rw-r--r--   0        0        0     1158 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/chat/prompt.py
--rw-r--r--   0        0        0       75 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/conversational/__init__.py
--rw-r--r--   0        0        0     4957 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/conversational/base.py
--rw-r--r--   0        0        0     1383 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/conversational/output_parser.py
--rw-r--r--   0        0        0     1859 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/conversational/prompt.py
--rw-r--r--   0        0        0       75 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/conversational_chat/__init__.py
--rw-r--r--   0        0        0     5196 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/conversational_chat/base.py
--rw-r--r--   0        0        0     2398 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/conversational_chat/output_parser.py
--rw-r--r--   0        0        0     2763 2024-02-19 20:58:55.557226 langchain-0.1.8/langchain/agents/conversational_chat/prompt.py
--rw-r--r--   0        0        0      847 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/format_scratchpad/__init__.py
--rw-r--r--   0        0        0      528 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/format_scratchpad/log.py
--rw-r--r--   0        0        0      721 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/format_scratchpad/log_to_messages.py
--rw-r--r--   0        0        0     2203 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/format_scratchpad/openai_functions.py
--rw-r--r--   0        0        0     1885 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/format_scratchpad/openai_tools.py
--rw-r--r--   0        0        0      578 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/format_scratchpad/xml.py
--rw-r--r--   0        0        0     3244 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/initialize.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/json_chat/__init__.py
--rw-r--r--   0        0        0     6832 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/json_chat/base.py
--rw-r--r--   0        0        0      551 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/json_chat/prompt.py
--rw-r--r--   0        0        0    23921 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/load_tools.py
--rw-r--r--   0        0        0     4592 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/loading.py
--rw-r--r--   0        0        0       86 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/mrkl/__init__.py
--rw-r--r--   0        0        0     6046 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/mrkl/base.py
--rw-r--r--   0        0        0     3407 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/mrkl/output_parser.py
--rw-r--r--   0        0        0      641 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/mrkl/prompt.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_assistant/__init__.py
--rw-r--r--   0        0        0    25712 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_assistant/base.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_functions_agent/__init__.py
--rw-r--r--   0        0        0     2567 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py
--rw-r--r--   0        0        0    11522 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_functions_agent/base.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_functions_multi_agent/__init__.py
--rw-r--r--   0        0        0    11944 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_functions_multi_agent/base.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_tools/__init__.py
--rw-r--r--   0        0        0     3388 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/openai_tools/base.py
--rw-r--r--   0        0        0     1270 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/output_parsers/__init__.py
--rw-r--r--   0        0        0     1846 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/output_parsers/json.py
--rw-r--r--   0        0        0     3467 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/output_parsers/openai_functions.py
--rw-r--r--   0        0        0     3492 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/output_parsers/openai_tools.py
--rw-r--r--   0        0        0     2455 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/output_parsers/react_json_single_input.py
--rw-r--r--   0        0        0     3218 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/output_parsers/react_single_input.py
--rw-r--r--   0        0        0     1545 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/output_parsers/self_ask.py
--rw-r--r--   0        0        0     1658 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/output_parsers/xml.py
--rw-r--r--   0        0        0       76 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/react/__init__.py
--rw-r--r--   0        0        0     3903 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/react/agent.py
--rw-r--r--   0        0        0     5714 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/react/base.py
--rw-r--r--   0        0        0     1231 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/react/output_parser.py
--rw-r--r--   0        0        0     1906 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/react/textworld_prompt.py
--rw-r--r--   0        0        0     6127 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/react/wiki_prompt.py
--rw-r--r--   0        0        0     1175 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/schema.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/self_ask_with_search/__init__.py
--rw-r--r--   0        0        0     8099 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/self_ask_with_search/base.py
--rw-r--r--   0        0        0      138 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/self_ask_with_search/output_parser.py
--rw-r--r--   0        0        0     1926 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/self_ask_with_search/prompt.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/structured_chat/__init__.py
--rw-r--r--   0        0        0     9948 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/structured_chat/base.py
--rw-r--r--   0        0        0     3799 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/structured_chat/output_parser.py
--rw-r--r--   0        0        0      992 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/structured_chat/prompt.py
--rw-r--r--   0        0        0     1409 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/tools.py
--rw-r--r--   0        0        0     1475 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/types.py
--rw-r--r--   0        0        0      384 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/utils.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/xml/__init__.py
--rw-r--r--   0        0        0     7258 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/xml/base.py
--rw-r--r--   0        0        0      767 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/agents/xml/prompt.py
--rw-r--r--   0        0        0      217 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/base_language.py
--rw-r--r--   0        0        0      701 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/cache.py
--rw-r--r--   0        0        0     2509 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/__init__.py
--rw-r--r--   0        0        0      211 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/aim_callback.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/argilla_callback.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/arize_callback.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/arthur_callback.py
--rw-r--r--   0        0        0      653 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/base.py
--rw-r--r--   0        0        0      129 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/clearml_callback.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/confident_callback.py
--rw-r--r--   0        0        0      129 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/context_callback.py
--rw-r--r--   0        0        0     2589 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/file.py
--rw-r--r--   0        0        0      123 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/flyte_callback.py
--rw-r--r--   0        0        0      275 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/human.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/infino_callback.py
--rw-r--r--   0        0        0      241 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/labelstudio_callback.py
--rw-r--r--   0        0        0      142 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/llmonitor_callback.py
--rw-r--r--   0        0        0     1777 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/manager.py
--rw-r--r--   0        0        0      305 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/openai_info.py
--rw-r--r--   0        0        0      141 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0      135 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/stdout.py
--rw-r--r--   0        0        0     2399 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/streaming_aiter.py
--rw-r--r--   0        0        0     3371 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/streaming_aiter_final_only.py
--rw-r--r--   0        0        0      173 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     3357 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/streaming_stdout_final_only.py
--rw-r--r--   0        0        0     3190 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0      185 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0      490 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0      589 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0      154 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/tracers/base.py
--rw-r--r--   0        0        0      154 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/tracers/comet.py
--rw-r--r--   0        0        0      233 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0      218 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0      226 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/tracers/log_stream.py
--rw-r--r--   0        0        0     1384 2024-02-19 20:58:55.561226 langchain-0.1.8/langchain/callbacks/tracers/logging.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/tracers/root_listeners.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0      470 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0      168 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0      229 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/trubrics_callback.py
--rw-r--r--   0        0        0      403 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/utils.py
--rw-r--r--   0        0        0      130 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/wandb_callback.py
--rw-r--r--   0        0        0      129 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0     5951 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/__init__.py
--rw-r--r--   0        0        0       84 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/__init__.py
--rw-r--r--   0        0        0     8919 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/base.py
--rw-r--r--   0        0        0     2452 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/news_docs.py
--rw-r--r--   0        0        0     3399 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/open_meteo_docs.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/openapi/__init__.py
--rw-r--r--   0        0        0     8786 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/openapi/chain.py
--rw-r--r--   0        0        0     1791 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/openapi/prompts.py
--rw-r--r--   0        0        0     1975 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/openapi/requests_chain.py
--rw-r--r--   0        0        0     1847 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/openapi/response_chain.py
--rw-r--r--   0        0        0     1920 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/podcast_docs.py
--rw-r--r--   0        0        0     1031 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/prompt.py
--rw-r--r--   0        0        0     1537 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/api/tmdb_docs.py
--rw-r--r--   0        0        0    28434 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/base.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/chat_vector_db/__init__.py
--rw-r--r--   0        0        0      694 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/chat_vector_db/prompts.py
--rw-r--r--   0        0        0      367 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/combine_documents/__init__.py
--rw-r--r--   0        0        0     7963 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/combine_documents/base.py
--rw-r--r--   0        0        0    11739 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/combine_documents/map_reduce.py
--rw-r--r--   0        0        0     8949 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/combine_documents/map_rerank.py
--rw-r--r--   0        0        0    13894 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/combine_documents/reduce.py
--rw-r--r--   0        0        0     9113 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/combine_documents/refine.py
--rw-r--r--   0        0        0    10963 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/combine_documents/stuff.py
--rw-r--r--   0        0        0      107 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/constitutional_ai/__init__.py
--rw-r--r--   0        0        0     6341 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/constitutional_ai/base.py
--rw-r--r--   0        0        0      283 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/constitutional_ai/models.py
--rw-r--r--   0        0        0    21738 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/constitutional_ai/principles.py
--rw-r--r--   0        0        0     8666 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/constitutional_ai/prompts.py
--rw-r--r--   0        0        0       71 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/conversation/__init__.py
--rw-r--r--   0        0        0     2366 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/conversation/base.py
--rw-r--r--   0        0        0      856 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/conversation/memory.py
--rw-r--r--   0        0        0      913 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/conversation/prompt.py
--rw-r--r--   0        0        0       49 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0    17834 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/conversational_retrieval/base.py
--rw-r--r--   0        0        0      720 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/conversational_retrieval/prompts.py
--rw-r--r--   0        0        0      126 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/elasticsearch_database/__init__.py
--rw-r--r--   0        0        0     8287 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/elasticsearch_database/base.py
--rw-r--r--   0        0        0     1425 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/elasticsearch_database/prompts.py
--rw-r--r--   0        0        0      465 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/ernie_functions/__init__.py
--rw-r--r--   0        0        0    23289 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/ernie_functions/base.py
--rw-r--r--   0        0        0      741 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/example_generator.py
--rw-r--r--   0        0        0       51 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/flare/__init__.py
--rw-r--r--   0        0        0     9033 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/flare/base.py
--rw-r--r--   0        0        0     1471 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/flare/prompts.py
--rw-r--r--   0        0        0       49 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/__init__.py
--rw-r--r--   0        0        0     8397 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/arangodb.py
--rw-r--r--   0        0        0     3671 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/base.py
--rw-r--r--   0        0        0    10452 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/cypher.py
--rw-r--r--   0        0        0     9625 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/cypher_utils.py
--rw-r--r--   0        0        0     5272 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/falkordb.py
--rw-r--r--   0        0        0     3717 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/hugegraph.py
--rw-r--r--   0        0        0     3698 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/kuzu.py
--rw-r--r--   0        0        0     3692 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/nebulagraph.py
--rw-r--r--   0        0        0     6890 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/neptune_cypher.py
--rw-r--r--   0        0        0     6610 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/neptune_sparql.py
--rw-r--r--   0        0        0     7226 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/ontotext_graphdb.py
--rw-r--r--   0        0        0    16720 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/prompts.py
--rw-r--r--   0        0        0     5440 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/graph_qa/sparql.py
--rw-r--r--   0        0        0     2662 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/history_aware_retriever.py
--rw-r--r--   0        0        0       75 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/hyde/__init__.py
--rw-r--r--   0        0        0     3341 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/hyde/base.py
--rw-r--r--   0        0        0     1913 2024-02-19 20:58:55.565226 langchain-0.1.8/langchain/chains/hyde/prompts.py
--rw-r--r--   0        0        0    14776 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm.py
--rw-r--r--   0        0        0      450 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_bash/__init__.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_checker/__init__.py
--rw-r--r--   0        0        0     6164 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_checker/base.py
--rw-r--r--   0        0        0     1125 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_checker/prompt.py
--rw-r--r--   0        0        0      143 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_math/__init__.py
--rw-r--r--   0        0        0     6723 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_math/base.py
--rw-r--r--   0        0        0      868 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_math/prompt.py
--rw-r--r--   0        0        0     3193 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_requests.py
--rw-r--r--   0        0        0      352 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_summarization_checker/__init__.py
--rw-r--r--   0        0        0     6582 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_summarization_checker/base.py
--rw-r--r--   0        0        0      654 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
--rw-r--r--   0        0        0      377 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_summarization_checker/prompts/check_facts.txt
--rw-r--r--   0        0        0      128 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_summarization_checker/prompts/create_facts.txt
--rw-r--r--   0        0        0      416 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt
--rw-r--r--   0        0        0      467 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0    25261 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/loading.py
--rw-r--r--   0        0        0     3732 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/mapreduce.py
--rw-r--r--   0        0        0     3086 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/moderation.py
--rw-r--r--   0        0        0       96 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/natbot/__init__.py
--rw-r--r--   0        0        0     4695 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/natbot/base.py
--rw-r--r--   0        0        0    16050 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/natbot/crawler.py
--rw-r--r--   0        0        0     4989 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/natbot/prompt.py
--rw-r--r--   0        0        0     1357 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_functions/__init__.py
--rw-r--r--   0        0        0    10075 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_functions/base.py
--rw-r--r--   0        0        0     3526 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_functions/citation_fuzzy_match.py
--rw-r--r--   0        0        0     4073 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_functions/extraction.py
--rw-r--r--   0        0        0    11306 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_functions/openapi.py
--rw-r--r--   0        0        0     3918 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_functions/qa_with_structure.py
--rw-r--r--   0        0        0     2660 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_functions/tagging.py
--rw-r--r--   0        0        0     1257 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_functions/utils.py
--rw-r--r--   0        0        0      134 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_tools/__init__.py
--rw-r--r--   0        0        0     1665 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/openai_tools/extraction.py
--rw-r--r--   0        0        0     2015 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/prompt_selector.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_generation/__init__.py
--rw-r--r--   0        0        0     2464 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_generation/base.py
--rw-r--r--   0        0        0     1875 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_generation/prompt.py
--rw-r--r--   0        0        0      173 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_with_sources/__init__.py
--rw-r--r--   0        0        0     7976 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_with_sources/base.py
--rw-r--r--   0        0        0     6793 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_with_sources/loading.py
--rw-r--r--   0        0        0     6971 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_with_sources/map_reduce_prompt.py
--rw-r--r--   0        0        0     1318 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_with_sources/refine_prompts.py
--rw-r--r--   0        0        0     2459 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_with_sources/retrieval.py
--rw-r--r--   0        0        0     6581 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_with_sources/stuff_prompt.py
--rw-r--r--   0        0        0     2770 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/qa_with_sources/vector_db.py
--rw-r--r--   0        0        0      131 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/query_constructor/__init__.py
--rw-r--r--   0        0        0    13621 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/query_constructor/base.py
--rw-r--r--   0        0        0     3191 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/query_constructor/ir.py
--rw-r--r--   0        0        0     5707 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/query_constructor/parser.py
--rw-r--r--   0        0        0     6880 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/query_constructor/prompt.py
--rw-r--r--   0        0        0      321 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/query_constructor/schema.py
--rw-r--r--   0        0        0     8503 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/question_answering/__init__.py
--rw-r--r--   0        0        0     8013 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/question_answering/map_reduce_prompt.py
--rw-r--r--   0        0        0     1622 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/question_answering/map_rerank_prompt.py
--rw-r--r--   0        0        0     2378 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/question_answering/refine_prompts.py
--rw-r--r--   0        0        0     1146 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/question_answering/stuff_prompt.py
--rw-r--r--   0        0        0     2742 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/retrieval.py
--rw-r--r--   0        0        0       62 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/retrieval_qa/__init__.py
--rw-r--r--   0        0        0     9952 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/retrieval_qa/base.py
--rw-r--r--   0        0        0      399 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/retrieval_qa/prompt.py
--rw-r--r--   0        0        0      407 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/router/__init__.py
--rw-r--r--   0        0        0     4571 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/router/base.py
--rw-r--r--   0        0        0     1982 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/router/embedding_router.py
--rw-r--r--   0        0        0     4283 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/router/llm_router.py
--rw-r--r--   0        0        0     2245 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/router/multi_prompt.py
--rw-r--r--   0        0        0     1156 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/router/multi_prompt_prompt.py
--rw-r--r--   0        0        0     1079 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/router/multi_retrieval_prompt.py
--rw-r--r--   0        0        0     3659 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/router/multi_retrieval_qa.py
--rw-r--r--   0        0        0     7510 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/sequential.py
--rw-r--r--   0        0        0       47 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/sql_database/__init__.py
--rw-r--r--   0        0        0    15458 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/sql_database/prompt.py
--rw-r--r--   0        0        0     5293 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/sql_database/query.py
--rw-r--r--   0        0        0      204 2024-02-19 20:58:55.569226 langchain-0.1.8/langchain/chains/structured_output/__init__.py
--rw-r--r--   0        0        0    15509 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chains/structured_output/base.py
--rw-r--r--   0        0        0     5804 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chains/summarize/__init__.py
--rw-r--r--   0        0        0      238 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chains/summarize/map_reduce_prompt.py
--rw-r--r--   0        0        0      677 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chains/summarize/refine_prompts.py
--rw-r--r--   0        0        0      238 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chains/summarize/stuff_prompt.py
--rw-r--r--   0        0        0     2369 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chains/transform.py
--rw-r--r--   0        0        0      452 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/__init__.py
--rw-r--r--   0        0        0       95 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/base.py
--rw-r--r--   0        0        0      240 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/facebook_messenger.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/gmail.py
--rw-r--r--   0        0        0      107 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/imessage.py
--rw-r--r--   0        0        0      187 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/langsmith.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/slack.py
--rw-r--r--   0        0        0      107 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/telegram.py
--rw-r--r--   0        0        0      290 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/utils.py
--rw-r--r--   0        0        0      107 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_loaders/whatsapp.py
--rw-r--r--   0        0        0     1979 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/__init__.py
--rw-r--r--   0        0        0      199 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/anthropic.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/anyscale.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/azure_openai.py
--rw-r--r--   0        0        0      189 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0      110 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/baichuan.py
--rw-r--r--   0        0        0      131 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      268 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/base.py
--rw-r--r--   0        0        0      131 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/bedrock.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/cohere.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/databricks.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/ernie.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/everlyai.py
--rw-r--r--   0        0        0      169 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/fake.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/fireworks.py
--rw-r--r--   0        0        0       95 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/gigachat.py
--rw-r--r--   0        0        0      158 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/google_palm.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/human.py
--rw-r--r--   0        0        0      107 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/hunyuan.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/javelin_ai_gateway.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/jinachat.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/konko.py
--rw-r--r--   0        0        0      137 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/litellm.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/meta.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/minimax.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/mlflow.py
--rw-r--r--   0        0        0      156 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/ollama.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/openai.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/pai_eas_endpoint.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/tongyi.py
--rw-r--r--   0        0        0      110 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/vertexai.py
--rw-r--r--   0        0        0      178 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/volcengine_maas.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/chat_models/yandex.py
--rw-r--r--   0        0        0     1184 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/docstore/__init__.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/docstore/base.py
--rw-r--r--   0        0        0       70 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/docstore/document.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/docstore/in_memory.py
--rw-r--r--   0        0        0       86 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/docstore/wikipedia.py
--rw-r--r--   0        0        0     5722 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/acreom.py
--rw-r--r--   0        0        0      554 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/airbyte.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/airtable.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/arcgis_loader.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/arxiv.py
--rw-r--r--   0        0        0      190 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/assemblyai.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/async_html.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/azlyrics.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/azure_ai_data.py
--rw-r--r--   0        0        0      166 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0      151 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0      146 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/baiducloud_bos_directory.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/baiducloud_bos_file.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/base.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/base_o365.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/bibtex.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/bigquery.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/bilibili.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/blackboard.py
--rw-r--r--   0        0        0      374 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0      140 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0      138 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0      172 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/blockchain.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/brave_search.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/browserless.py
--rw-r--r--   0        0        0      138 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/chatgpt.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/chromium.py
--rw-r--r--   0        0        0      146 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/college_confidential.py
--rw-r--r--   0        0        0      118 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/concurrent.py
--rw-r--r--   0        0        0      154 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/confluence.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/conllu.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/couchbase.py
--rw-r--r--   0        0        0      156 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/csv_loader.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0      163 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/dataframe.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/diffbot.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/directory.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/discord.py
--rw-r--r--   0        0        0      119 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/docusaurus.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/dropbox.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0      177 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/email.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/epub.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/etherscan.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/evernote.py
--rw-r--r--   0        0        0      118 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/excel.py
--rw-r--r--   0        0        0      167 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/fauna.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/figma.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/gcs_file.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/generic.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/geodataframe.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/git.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/gitbook.py
--rw-r--r--   0        0        0      160 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/github.py
--rw-r--r--   0        0        0      145 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/google_speech_to_text.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/googledrive.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/gutenberg.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/helpers.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/hn.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/html.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/html_bs.py
--rw-r--r--   0        0        0      144 2024-02-19 20:58:55.573226 langchain-0.1.8/langchain/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/ifixit.py
--rw-r--r--   0        0        0      118 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/image.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/image_captions.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/imsdb.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/iugu.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/joplin.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/json_loader.py
--rw-r--r--   0        0        0      198 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/lakefs.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/larksuite.py
--rw-r--r--   0        0        0      127 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/markdown.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/mastodon.py
--rw-r--r--   0        0        0      110 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/max_compute.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/merge.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/mhtml.py
--rw-r--r--   0        0        0      131 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/mongodb.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/news.py
--rw-r--r--   0        0        0      196 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/notebook.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/notion.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/notiondb.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/nuclia.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/obs_directory.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/obs_file.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/obsidian.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/odt.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/onedrive.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/onenote.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/open_city_data.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/org_mode.py
--rw-r--r--   0        0        0      789 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0      225 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/docai.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0      176 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      136 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/language/cobol.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0      141 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0      136 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/msword.py
--rw-r--r--   0        0        0      494 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0      706 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/pdf.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/polars_dataframe.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/powerpoint.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/psychic.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/pubmed.py
--rw-r--r--   0        0        0      137 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/python.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/quip.py
--rw-r--r--   0        0        0      128 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/readthedocs.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/reddit.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/roam.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/rspace.py
--rw-r--r--   0        0        0       96 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/rss.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/rst.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/rtf.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/s3_directory.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/s3_file.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/sharepoint.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/sitemap.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/slack_directory.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/spreedly.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/srt.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/stripe.py
--rw-r--r--   0        0        0      275 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/telegram.py
--rw-r--r--   0        0        0      147 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0      123 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0      141 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/tensorflow_datasets.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/text.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/toml.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/trello.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/tsv.py
--rw-r--r--   0        0        0      119 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/twitter.py
--rw-r--r--   0        0        0      601 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/unstructured.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/url.py
--rw-r--r--   0        0        0      236 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/url_playwright.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/url_selenium.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/weather.py
--rw-r--r--   0        0        0      110 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/web_base.py
--rw-r--r--   0        0        0      167 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/wikipedia.py
--rw-r--r--   0        0        0      187 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/word_document.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/xml.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/xorbits.py
--rw-r--r--   0        0        0      218 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_loaders/youtube.py
--rw-r--r--   0        0        0     1616 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/__init__.py
--rw-r--r--   0        0        0      155 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/beautiful_soup_transformer.py
--rw-r--r--   0        0        0      149 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0      136 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0      145 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0      487 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0      149 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/google_translate.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/html2text.py
--rw-r--r--   0        0        0      137 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0      144 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0      191 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     6033 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/document_transformers/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0     3598 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/embeddings/__init__.py
--rw-r--r--   0        0        0      248 2024-02-19 20:58:55.577226 langchain-0.1.8/langchain/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0       90 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/awa.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/azure_openai.py
--rw-r--r--   0        0        0      142 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/base.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/bedrock.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/bookend.py
--rw-r--r--   0        0        0     8240 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/cache.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/clarifai.py
--rw-r--r--   0        0        0      148 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/cloudflare_workersai.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/cohere.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/dashscope.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/databricks.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/deepinfra.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/edenai.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/elasticsearch.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/embaas.py
--rw-r--r--   0        0        0       96 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/ernie.py
--rw-r--r--   0        0        0      164 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/fake.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/fastembed.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/google_palm.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/gpt4all.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/gradient_ai.py
--rw-r--r--   0        0        0      344 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/huggingface.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0      200 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/infinity.py
--rw-r--r--   0        0        0      140 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/javelin_ai_gateway.py
--rw-r--r--   0        0        0       93 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/jina.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/johnsnowlabs.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/llamacpp.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/llm_rails.py
--rw-r--r--   0        0        0      118 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/localai.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/minimax.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/mlflow.py
--rw-r--r--   0        0        0      134 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/mosaicml.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/nlpcloud.py
--rw-r--r--   0        0        0      119 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/ollama.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/openai.py
--rw-r--r--   0        0        0      200 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/self_hosted.py
--rw-r--r--   0        0        0      255 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      148 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0      107 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0      130 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/vertexai.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/voyageai.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/embeddings/xinference.py
--rw-r--r--   0        0        0      476 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/env.py
--rw-r--r--   0        0        0     5803 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/__init__.py
--rw-r--r--   0        0        0      165 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/agents/__init__.py
--rw-r--r--   0        0        0    13884 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/agents/trajectory_eval_chain.py
--rw-r--r--   0        0        0     5938 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/agents/trajectory_eval_prompt.py
--rw-r--r--   0        0        0     1400 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/comparison/__init__.py
--rw-r--r--   0        0        0    16056 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/comparison/eval_chain.py
--rw-r--r--   0        0        0     2358 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/comparison/prompt.py
--rw-r--r--   0        0        0     1647 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/criteria/__init__.py
--rw-r--r--   0        0        0    21358 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/criteria/eval_chain.py
--rw-r--r--   0        0        0     1756 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/criteria/prompt.py
--rw-r--r--   0        0        0      323 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/embedding_distance/__init__.py
--rw-r--r--   0        0        0    15503 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/embedding_distance/base.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/exact_match/__init__.py
--rw-r--r--   0        0        0     2751 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/exact_match/base.py
--rw-r--r--   0        0        0     6693 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/loading.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/parsing/__init__.py
--rw-r--r--   0        0        0     5246 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/parsing/base.py
--rw-r--r--   0        0        0     3679 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/parsing/json_distance.py
--rw-r--r--   0        0        0     3197 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/parsing/json_schema.py
--rw-r--r--   0        0        0      344 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/qa/__init__.py
--rw-r--r--   0        0        0    10886 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/qa/eval_chain.py
--rw-r--r--   0        0        0     3911 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/qa/eval_prompt.py
--rw-r--r--   0        0        0     1052 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/qa/generate_chain.py
--rw-r--r--   0        0        0      606 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/qa/generate_prompt.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/regex_match/__init__.py
--rw-r--r--   0        0        0     2407 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/regex_match/base.py
--rw-r--r--   0        0        0    18197 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/schema.py
--rw-r--r--   0        0        0     1112 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/scoring/__init__.py
--rw-r--r--   0        0        0    15656 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/scoring/eval_chain.py
--rw-r--r--   0        0        0     2129 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/scoring/prompt.py
--rw-r--r--   0        0        0      285 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/string_distance/__init__.py
--rw-r--r--   0        0        0    14014 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/evaluation/string_distance/base.py
--rw-r--r--   0        0        0      141 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/example_generator.py
--rw-r--r--   0        0        0      167 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/formatting.py
--rw-r--r--   0        0        0     7435 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/globals/__init__.py
--rw-r--r--   0        0        0     1104 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/graphs/__init__.py
--rw-r--r--   0        0        0      148 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/graphs/arangodb_graph.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/graphs/falkordb_graph.py
--rw-r--r--   0        0        0      141 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/graphs/graph_document.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/graphs/graph_store.py
--rw-r--r--   0        0        0       84 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/graphs/hugegraph.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.581226 langchain-0.1.8/langchain/graphs/kuzu_graph.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/graphs/memgraph_graph.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/graphs/nebula_graph.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/graphs/neo4j_graph.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/graphs/neptune_graph.py
--rw-r--r--   0        0        0      299 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/graphs/networkx_graph.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/graphs/rdf_graph.py
--rw-r--r--   0        0        0     2874 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/hub.py
--rw-r--r--   0        0        0      973 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/__init__.py
--rw-r--r--   0        0        0    22479 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/_api.py
--rw-r--r--   0        0        0    20556 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0     5221 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/base.py
--rw-r--r--   0        0        0     1752 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/graph.py
--rw-r--r--   0        0        0       49 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/prompts/__init__.py
--rw-r--r--   0        0        0     1952 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/prompts/entity_extraction.py
--rw-r--r--   0        0        0     1157 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/prompts/entity_summarization.py
--rw-r--r--   0        0        0     1599 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/prompts/knowledge_triplet_extraction.py
--rw-r--r--   0        0        0     3423 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/indexes/vectorstore.py
--rw-r--r--   0        0        0      282 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/input.py
--rw-r--r--   0        0        0    17110 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/__init__.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/ai21.py
--rw-r--r--   0        0        0       86 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/aleph_alpha.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0       82 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/anthropic.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/anyscale.py
--rw-r--r--   0        0        0       70 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/arcee.py
--rw-r--r--   0        0        0       82 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/aviary.py
--rw-r--r--   0        0        0      507 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/azureml_endpoint.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0       76 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/bananadev.py
--rw-r--r--   0        0        0      228 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/base.py
--rw-r--r--   0        0        0       76 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/baseten.py
--rw-r--r--   0        0        0       67 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/beam.py
--rw-r--r--   0        0        0      128 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/bedrock.py
--rw-r--r--   0        0        0       92 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/bittensor.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/cerebriumai.py
--rw-r--r--   0        0        0       76 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/chatglm.py
--rw-r--r--   0        0        0       79 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/clarifai.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/cloudflare_workersai.py
--rw-r--r--   0        0        0       89 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/cohere.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/ctransformers.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/ctranslate2.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/databricks.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/deepinfra.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/deepsparse.py
--rw-r--r--   0        0        0       73 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/edenai.py
--rw-r--r--   0        0        0      127 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/fake.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/fireworks.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/forefrontai.py
--rw-r--r--   0        0        0       79 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/gigachat.py
--rw-r--r--   0        0        0       86 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/google_palm.py
--rw-r--r--   0        0        0       76 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/gooseai.py
--rw-r--r--   0        0        0       76 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/gpt4all.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/gradient_ai.py
--rw-r--r--   0        0        0      664 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/grammars/json.gbnf
--rw-r--r--   0        0        0      167 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/grammars/list.gbnf
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0      107 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/huggingface_hub.py
--rw-r--r--   0        0        0      129 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0      148 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0       95 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/human.py
--rw-r--r--   0        0        0      123 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/javelin_ai_gateway.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/koboldai.py
--rw-r--r--   0        0        0       79 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/llamacpp.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/loading.py
--rw-r--r--   0        0        0       93 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/manifest.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/minimax.py
--rw-r--r--   0        0        0       73 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/mlflow.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0       70 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/modal.py
--rw-r--r--   0        0        0       95 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/mosaicml.py
--rw-r--r--   0        0        0       79 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/nlpcloud.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/octoai_endpoint.py
--rw-r--r--   0        0        0       82 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/ollama.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/opaqueprompts.py
--rw-r--r--   0        0        0      193 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/openai.py
--rw-r--r--   0        0        0       76 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/openllm.py
--rw-r--r--   0        0        0       73 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/openlm.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/pai_eas_endpoint.py
--rw-r--r--   0        0        0       73 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/petals.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/pipelineai.py
--rw-r--r--   0        0        0       82 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/predibase.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/predictionguard.py
--rw-r--r--   0        0        0      168 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/promptlayer_openai.py
--rw-r--r--   0        0        0       82 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/replicate.py
--rw-r--r--   0        0        0       67 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/rwkv.py
--rw-r--r--   0        0        0      160 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/self_hosted.py
--rw-r--r--   0        0        0      143 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/stochasticai.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/symblai_nebula.py
--rw-r--r--   0        0        0       76 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/textgen.py
--rw-r--r--   0        0        0       92 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/titan_takeoff.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/titan_takeoff_pro.py
--rw-r--r--   0        0        0       79 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/together.py
--rw-r--r--   0        0        0       89 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/tongyi.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/utils.py
--rw-r--r--   0        0        0      147 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/vertexai.py
--rw-r--r--   0        0        0       93 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/vllm.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/volcengine_maas.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/watsonxllm.py
--rw-r--r--   0        0        0       73 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/writer.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/xinference.py
--rw-r--r--   0        0        0       79 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/llms/yandex.py
--rw-r--r--   0        0        0      206 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/load/__init__.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/load/dump.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/load/load.py
--rw-r--r--   0        0        0      412 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/load/serializable.py
--rw-r--r--   0        0        0     3256 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/memory/__init__.py
--rw-r--r--   0        0        0     4861 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/memory/buffer.py
--rw-r--r--   0        0        0     1616 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/memory/buffer_window.py
--rw-r--r--   0        0        0     2245 2024-02-19 20:58:55.585226 langchain-0.1.8/langchain/memory/chat_memory.py
--rw-r--r--   0        0        0     1560 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/__init__.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/astradb.py
--rw-r--r--   0        0        0      145 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0      143 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0      142 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0      157 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/elasticsearch.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/file.py
--rw-r--r--   0        0        0      145 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      118 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/momento.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/neo4j.py
--rw-r--r--   0        0        0      142 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/postgres.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/redis.py
--rw-r--r--   0        0        0      141 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/rocksetdb.py
--rw-r--r--   0        0        0      157 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/singlestoredb.py
--rw-r--r--   0        0        0      248 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/sql.py
--rw-r--r--   0        0        0      145 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0      155 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/upstash_redis.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/xata.py
--rw-r--r--   0        0        0      118 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/chat_message_histories/zep.py
--rw-r--r--   0        0        0     2912 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/combined.py
--rw-r--r--   0        0        0    15677 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/entity.py
--rw-r--r--   0        0        0     5075 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/kg.py
--rw-r--r--   0        0        0     3106 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/motorhead_memory.py
--rw-r--r--   0        0        0     8181 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/prompt.py
--rw-r--r--   0        0        0      794 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/readonly.py
--rw-r--r--   0        0        0      761 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/simple.py
--rw-r--r--   0        0        0     3389 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/summary.py
--rw-r--r--   0        0        0     2949 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/summary_buffer.py
--rw-r--r--   0        0        0     2144 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/token_buffer.py
--rw-r--r--   0        0        0      617 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/utils.py
--rw-r--r--   0        0        0     3002 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/vectorstore.py
--rw-r--r--   0        0        0     5090 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/memory/zep_memory.py
--rw-r--r--   0        0        0     3278 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/model_laboratory.py
--rw-r--r--   0        0        0     2216 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     1084 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/boolean.py
--rw-r--r--   0        0        0     1799 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/combining.py
--rw-r--r--   0        0        0     1974 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1205 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/enum.py
--rw-r--r--   0        0        0      424 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/ernie_functions.py
--rw-r--r--   0        0        0     3153 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/fix.py
--rw-r--r--   0        0        0     3958 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/format_instructions.py
--rw-r--r--   0        0        0      298 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/json.py
--rw-r--r--   0        0        0      310 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/list.py
--rw-r--r--   0        0        0      702 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/loading.py
--rw-r--r--   0        0        0     7989 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/openai_functions.py
--rw-r--r--   0        0        0     3781 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/openai_tools.py
--rw-r--r--   0        0        0     6548 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/pandas_dataframe.py
--rw-r--r--   0        0        0      508 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/prompts.py
--rw-r--r--   0        0        0     1955 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/pydantic.py
--rw-r--r--   0        0        0      129 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/rail_parser.py
--rw-r--r--   0        0        0     1214 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/regex.py
--rw-r--r--   0        0        0     1709 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/regex_dict.py
--rw-r--r--   0        0        0     7792 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/retry.py
--rw-r--r--   0        0        0     3134 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/structured.py
--rw-r--r--   0        0        0       93 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/xml.py
--rw-r--r--   0        0        0     2181 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/output_parsers/yaml.py
--rw-r--r--   0        0        0     2560 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/__init__.py
--rw-r--r--   0        0        0      565 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/base.py
--rw-r--r--   0        0        0     1045 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/chat.py
--rw-r--r--   0        0        0      568 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/example_selector/__init__.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/example_selector/base.py
--rw-r--r--   0        0        0      136 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/example_selector/length_based.py
--rw-r--r--   0        0        0      203 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/example_selector/ngram_overlap.py
--rw-r--r--   0        0        0      288 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/example_selector/semantic_similarity.py
--rw-r--r--   0        0        0      265 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/few_shot.py
--rw-r--r--   0        0        0      128 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0      530 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/loading.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/pipeline.py
--rw-r--r--   0        0        0      153 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/prompts/prompt.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/py.typed
--rw-r--r--   0        0        0      897 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      134 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/pydantic_v1/main.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/python.py
--rw-r--r--   0        0        0      222 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/requests.py
--rw-r--r--   0        0        0     3488 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/__init__.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/arcee.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/arxiv.py
--rw-r--r--   0        0        0      150 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/azure_cognitive_search.py
--rw-r--r--   0        0        0      221 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/bedrock.py
--rw-r--r--   0        0        0      162 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/bm25.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/chaindesk.py
--rw-r--r--   0        0        0      138 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0      126 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/cohere_rag_retriever.py
--rw-r--r--   0        0        0     2298 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/contextual_compression.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/databerry.py
--rw-r--r--   0        0        0      129 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/docarray.py
--rw-r--r--   0        0        0      701 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/document_compressors/__init__.py
--rw-r--r--   0        0        0     3775 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/document_compressors/base.py
--rw-r--r--   0        0        0     3955 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/document_compressors/chain_extract.py
--rw-r--r--   0        0        0      366 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/document_compressors/chain_extract_prompt.py
--rw-r--r--   0        0        0     2757 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/document_compressors/chain_filter.py
--rw-r--r--   0        0        0      231 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/document_compressors/chain_filter_prompt.py
--rw-r--r--   0        0        0     4213 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/document_compressors/cohere_rerank.py
--rw-r--r--   0        0        0     3031 2024-02-19 20:58:55.589226 langchain-0.1.8/langchain/retrievers/document_compressors/embeddings_filter.py
--rw-r--r--   0        0        0     2415 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/document_compressors/flashrank_rerank.py
--rw-r--r--   0        0        0      141 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/embedchain.py
--rw-r--r--   0        0        0     9668 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/ensemble.py
--rw-r--r--   0        0        0      171 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/google_cloud_documentai_warehouse.py
--rw-r--r--   0        0        0      334 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/google_vertex_ai_search.py
--rw-r--r--   0        0        0       92 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/kay.py
--rw-r--r--   0        0        0      803 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/kendra.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/knn.py
--rw-r--r--   0        0        0      177 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/llama_index.py
--rw-r--r--   0        0        0     3489 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/merger_retriever.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/metal.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/milvus.py
--rw-r--r--   0        0        0     6768 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/multi_query.py
--rw-r--r--   0        0        0     3920 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/multi_vector.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/outline.py
--rw-r--r--   0        0        0     5196 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/parent_document_retriever.py
--rw-r--r--   0        0        0      150 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/pubmed.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/pupmed.py
--rw-r--r--   0        0        0     2658 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/re_phraser.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/remote_retriever.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/__init__.py
--rw-r--r--   0        0        0     2194 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/astradb.py
--rw-r--r--   0        0        0     9664 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/base.py
--rw-r--r--   0        0        0     1474 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/chroma.py
--rw-r--r--   0        0        0     1918 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/dashvector.py
--rw-r--r--   0        0        0     2631 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/deeplake.py
--rw-r--r--   0        0        0     3273 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/elasticsearch.py
--rw-r--r--   0        0        0     3352 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/milvus.py
--rw-r--r--   0        0        0     2303 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/mongodb_atlas.py
--rw-r--r--   0        0        0     3636 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/myscale.py
--rw-r--r--   0        0        0     3271 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/opensearch.py
--rw-r--r--   0        0        0     1529 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/pgvector.py
--rw-r--r--   0        0        0     1710 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/pinecone.py
--rw-r--r--   0        0        0     3168 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/qdrant.py
--rw-r--r--   0        0        0     3376 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/redis.py
--rw-r--r--   0        0        0     2974 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/supabase.py
--rw-r--r--   0        0        0     2633 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/timescalevector.py
--rw-r--r--   0        0        0     2164 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/vectara.py
--rw-r--r--   0        0        0     2619 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/self_query/weaviate.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/svm.py
--rw-r--r--   0        0        0      167 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/tavily_search_api.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/tfidf.py
--rw-r--r--   0        0        0     6295 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/time_weighted_retriever.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0      150 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0     8196 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/web_research.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/wikipedia.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/you.py
--rw-r--r--   0        0        0      142 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/zep.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/retrievers/zilliz.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/runnables/__init__.py
--rw-r--r--   0        0        0      809 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/runnables/hub.py
--rw-r--r--   0        0        0     1521 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/runnables/openai_functions.py
--rw-r--r--   0        0        0     2065 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/__init__.py
--rw-r--r--   0        0        0      149 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/agent.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/cache.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/__init__.py
--rw-r--r--   0        0        0      511 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/base.py
--rw-r--r--   0        0        0     1511 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/manager.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/stdout.py
--rw-r--r--   0        0        0      131 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/base.py
--rw-r--r--   0        0        0      176 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0      219 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0      127 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0      226 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/log_stream.py
--rw-r--r--   0        0        0      105 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/root_listeners.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0      470 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0      257 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0       80 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/chat.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/chat_history.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/document.py
--rw-r--r--   0        0        0       75 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/embeddings.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/exceptions.py
--rw-r--r--   0        0        0      367 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/language_model.py
--rw-r--r--   0        0        0       71 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/memory.py
--rw-r--r--   0        0        0     1048 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/messages.py
--rw-r--r--   0        0        0      320 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/output.py
--rw-r--r--   0        0        0      651 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/output_parser.py
--rw-r--r--   0        0        0       80 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/prompt.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/prompt_template.py
--rw-r--r--   0        0        0       81 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/retriever.py
--rw-r--r--   0        0        0     1796 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/__init__.py
--rw-r--r--   0        0        0      781 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/base.py
--rw-r--r--   0        0        0       89 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/branch.py
--rw-r--r--   0        0        0      665 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/config.py
--rw-r--r--   0        0        0      333 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/configurable.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/fallbacks.py
--rw-r--r--   0        0        0      260 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/history.py
--rw-r--r--   0        0        0      205 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/passthrough.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/retry.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/router.py
--rw-r--r--   0        0        0     1118 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/runnable/utils.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/storage.py
--rw-r--r--   0        0        0      137 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/schema/vectorstore.py
--rw-r--r--   0        0        0      130 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/serpapi.py
--rw-r--r--   0        0        0     3544 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/smith/__init__.py
--rw-r--r--   0        0        0     2199 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/smith/evaluation/__init__.py
--rw-r--r--   0        0        0    12480 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/smith/evaluation/config.py
--rw-r--r--   0        0        0     9936 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/smith/evaluation/name_generation.py
--rw-r--r--   0        0        0     3306 2024-02-19 20:58:55.593226 langchain-0.1.8/langchain/smith/evaluation/progress.py
--rw-r--r--   0        0        0    50978 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/smith/evaluation/runner_utils.py
--rw-r--r--   0        0        0    17107 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/smith/evaluation/string_run_evaluator.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/smith/evaluation/utils.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/sql_database.py
--rw-r--r--   0        0        0     1571 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/storage/__init__.py
--rw-r--r--   0        0        0     2517 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/storage/_lc_store.py
--rw-r--r--   0        0        0     2970 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/storage/encoder_backed.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/storage/exceptions.py
--rw-r--r--   0        0        0     4307 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/storage/file_system.py
--rw-r--r--   0        0        0     4448 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/storage/in_memory.py
--rw-r--r--   0        0        0       83 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/storage/redis.py
--rw-r--r--   0        0        0      166 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/storage/upstash_redis.py
--rw-r--r--   0        0        0    55865 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/text_splitter.py
--rw-r--r--   0        0        0     5663 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/__init__.py
--rw-r--r--   0        0        0      166 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/ainetwork/app.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/ainetwork/base.py
--rw-r--r--   0        0        0      119 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/ainetwork/owner.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/ainetwork/rule.py
--rw-r--r--   0        0        0      130 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/ainetwork/transfer.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/ainetwork/value.py
--rw-r--r--   0        0        0      257 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/amadeus/__init__.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/amadeus/base.py
--rw-r--r--   0        0        0      180 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0      170 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0       25 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/arxiv/__init__.py
--rw-r--r--   0        0        0      118 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/arxiv/tool.py
--rw-r--r--   0        0        0      802 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0      156 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0      149 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0      149 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0      175 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/azure_cognitive_services/text_analytics_health.py
--rw-r--r--   0        0        0      332 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/base.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/bearly/__init__.py
--rw-r--r--   0        0        0      229 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/bearly/tool.py
--rw-r--r--   0        0        0      170 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/bing_search/__init__.py
--rw-r--r--   0        0        0      138 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/brave_search/__init__.py
--rw-r--r--   0        0        0       95 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/brave_search/tool.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/clickup/__init__.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/clickup/tool.py
--rw-r--r--   0        0        0      157 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/convert_to_openai.py
--rw-r--r--   0        0        0      268 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0      197 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      147 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0      269 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/ddg_search/tool.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/e2b_data_analysis/__init__.py
--rw-r--r--   0        0        0      240 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/e2b_data_analysis/tool.py
--rw-r--r--   0        0        0     1024 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/__init__.py
--rw-r--r--   0        0        0      127 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/audio_speech_to_text.py
--rw-r--r--   0        0        0      127 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/audio_text_to_speech.py
--rw-r--r--   0        0        0       99 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/edenai_base_tool.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/image_explicitcontent.py
--rw-r--r--   0        0        0      143 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/image_objectdetection.py
--rw-r--r--   0        0        0      119 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/ocr_identityparser.py
--rw-r--r--   0        0        0      128 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/ocr_invoiceparser.py
--rw-r--r--   0        0        0      126 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/edenai/text_moderation.py
--rw-r--r--   0        0        0      164 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/eleven_labs/__init__.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/eleven_labs/models.py
--rw-r--r--   0        0        0      138 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/eleven_labs/text2speech.py
--rw-r--r--   0        0        0      723 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/file_management/__init__.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/file_management/copy.py
--rw-r--r--   0        0        0      155 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/file_management/delete.py
--rw-r--r--   0        0        0      160 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/file_management/file_search.py
--rw-r--r--   0        0        0      175 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/file_management/list_dir.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/file_management/move.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/file_management/read.py
--rw-r--r--   0        0        0      150 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/github/__init__.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/github/tool.py
--rw-r--r--   0        0        0       20 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gitlab/__init__.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gitlab/tool.py
--rw-r--r--   0        0        0      500 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gmail/__init__.py
--rw-r--r--   0        0        0       92 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gmail/base.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gmail/create_draft.py
--rw-r--r--   0        0        0      154 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gmail/get_message.py
--rw-r--r--   0        0        0      136 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gmail/get_thread.py
--rw-r--r--   0        0        0      167 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gmail/search.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/gmail/send_message.py
--rw-r--r--   0        0        0      136 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/golden_query/__init__.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/golden_query/tool.py
--rw-r--r--   0        0        0      171 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/google_cloud/__init__.py
--rw-r--r--   0        0        0      151 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/google_cloud/texttospeech.py
--rw-r--r--   0        0        0      152 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/google_finance/__init__.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/google_finance/tool.py
--rw-r--r--   0        0        0      140 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/google_jobs/__init__.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/google_jobs/tool.py
--rw-r--r--   0        0        0      140 2024-02-19 20:58:55.597226 langchain-0.1.8/langchain/tools/google_lens/__init__.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_lens/tool.py
--rw-r--r--   0        0        0      140 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_places/__init__.py
--rw-r--r--   0        0        0      161 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_places/tool.py
--rw-r--r--   0        0        0      152 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_scholar/__init__.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_scholar/tool.py
--rw-r--r--   0        0        0      195 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_search/__init__.py
--rw-r--r--   0        0        0      161 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_search/tool.py
--rw-r--r--   0        0        0      243 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_serper/__init__.py
--rw-r--r--   0        0        0      161 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_serper/tool.py
--rw-r--r--   0        0        0      148 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_trends/__init__.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/google_trends/tool.py
--rw-r--r--   0        0        0       47 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/graphql/__init__.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/graphql/tool.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/human/__init__.py
--rw-r--r--   0        0        0       92 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/human/tool.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/ifttt.py
--rw-r--r--   0        0        0       43 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/interaction/__init__.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/jira/__init__.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/json/__init__.py
--rw-r--r--   0        0        0      174 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/json/tool.py
--rw-r--r--   0        0        0      134 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/memorize/__init__.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/memorize/tool.py
--rw-r--r--   0        0        0       35 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/merriam_webster/__init__.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/merriam_webster/tool.py
--rw-r--r--   0        0        0      154 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0      118 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0      359 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/multion/__init__.py
--rw-r--r--   0        0        0      170 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/multion/close_session.py
--rw-r--r--   0        0        0      175 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/multion/create_session.py
--rw-r--r--   0        0        0      175 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/multion/update_session.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/nasa/__init__.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/nasa/tool.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/nuclia/__init__.py
--rw-r--r--   0        0        0      135 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/nuclia/tool.py
--rw-r--r--   0        0        0      567 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/office365/__init__.py
--rw-r--r--   0        0        0       94 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/office365/base.py
--rw-r--r--   0        0        0      197 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0      164 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/office365/events_search.py
--rw-r--r--   0        0        0      166 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/office365/messages_search.py
--rw-r--r--   0        0        0      151 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/office365/send_event.py
--rw-r--r--   0        0        0      161 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/office365/send_message.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0      542 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      191 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      162 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      119 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/openweathermap/tool.py
--rw-r--r--   0        0        0      763 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/__init__.py
--rw-r--r--   0        0        0      110 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/base.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/click.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/current_page.py
--rw-r--r--   0        0        0      198 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/extract_text.py
--rw-r--r--   0        0        0      168 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/get_elements.py
--rw-r--r--   0        0        0      152 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/navigate.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0      214 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/plugin.py
--rw-r--r--   0        0        0       52 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/powerbi/__init__.py
--rw-r--r--   0        0        0      189 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/pubmed/__init__.py
--rw-r--r--   0        0        0       95 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/pubmed/tool.py
--rw-r--r--   0        0        0      512 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/python/__init__.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/reddit_search/__init__.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/reddit_search/tool.py
--rw-r--r--   0        0        0     1581 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/render.py
--rw-r--r--   0        0        0       52 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/requests/__init__.py
--rw-r--r--   0        0        0      349 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/requests/tool.py
--rw-r--r--   0        0        0     2494 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/retriever.py
--rw-r--r--   0        0        0       31 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0      140 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/scenexplain/tool.py
--rw-r--r--   0        0        0      214 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/searchapi/__init__.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/searchapi/tool.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/searx_search/__init__.py
--rw-r--r--   0        0        0      156 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/searx_search/tool.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/shell/__init__.py
--rw-r--r--   0        0        0      123 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/shell/tool.py
--rw-r--r--   0        0        0      433 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/slack/__init__.py
--rw-r--r--   0        0        0       92 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/slack/base.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/slack/get_channel.py
--rw-r--r--   0        0        0      164 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/slack/get_message.py
--rw-r--r--   0        0        0      179 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/slack/schedule_message.py
--rw-r--r--   0        0        0      159 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/slack/send_message.py
--rw-r--r--   0        0        0       18 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/sleep/__init__.py
--rw-r--r--   0        0        0      110 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0      304 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/sql_database/prompt.py
--rw-r--r--   0        0        0      337 2024-02-19 20:58:55.601226 langchain-0.1.8/langchain/tools/sql_database/tool.py
--rw-r--r--   0        0        0       33 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/stackexchange/__init__.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/stackexchange/tool.py
--rw-r--r--   0        0        0       24 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/steam/__init__.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/steam/tool.py
--rw-r--r--   0        0        0      186 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0      180 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0      189 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/tavily_search/__init__.py
--rw-r--r--   0        0        0      187 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/tavily_search/tool.py
--rw-r--r--   0        0        0       51 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0      192 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       29 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      156 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0      114 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/yahoo_finance_news.py
--rw-r--r--   0        0        0        0 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/youtube/__init__.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/youtube/search.py
--rw-r--r--   0        0        0      193 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/zapier/__init__.py
--rw-r--r--   0        0        0      162 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/tools/zapier/tool.py
--rw-r--r--   0        0        0     2327 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/__init__.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/alpha_vantage.py
--rw-r--r--   0        0        0      193 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/anthropic.py
--rw-r--r--   0        0        0       89 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/apify.py
--rw-r--r--   0        0        0      361 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/arcee.py
--rw-r--r--   0        0        0       95 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/arxiv.py
--rw-r--r--   0        0        0      274 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/asyncio.py
--rw-r--r--   0        0        0       95 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/awslambda.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/bibtex.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/bing_search.py
--rw-r--r--   0        0        0      108 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/brave_search.py
--rw-r--r--   0        0        0      269 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/clickup.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/dalle_image_generator.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0      129 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/github.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/gitlab.py
--rw-r--r--   0        0        0      123 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/golden_query.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/google_finance.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/google_jobs.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/google_lens.py
--rw-r--r--   0        0        0      121 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/google_places_api.py
--rw-r--r--   0        0        0      120 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/google_scholar.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/google_search.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/google_serper.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/google_trends.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/graphql.py
--rw-r--r--   0        0        0       92 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/jira.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/loading.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/max_compute.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/merriam_webster.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/metaphor_search.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/nasa.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/opaqueprompts.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/openapi.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/openweathermap.py
--rw-r--r--   0        0        0      110 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/outline.py
--rw-r--r--   0        0        0       81 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/portkey.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/powerbi.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/pubmed.py
--rw-r--r--   0        0        0       86 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/python.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/reddit_search.py
--rw-r--r--   0        0        0      201 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/redis.py
--rw-r--r--   0        0        0      181 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/requests.py
--rw-r--r--   0        0        0      113 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/scenexplain.py
--rw-r--r--   0        0        0      107 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/searchapi.py
--rw-r--r--   0        0        0      151 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/searx_search.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/serpapi.py
--rw-r--r--   0        0        0       85 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/spark_sql.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/sql_database.py
--rw-r--r--   0        0        0      119 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/stackexchange.py
--rw-r--r--   0        0        0      101 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/steam.py
--rw-r--r--   0        0        0      126 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/tavily_search.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/tensorflow_datasets.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/twilio.py
--rw-r--r--   0        0        0      276 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/vertexai.py
--rw-r--r--   0        0        0      116 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/wikipedia.py
--rw-r--r--   0        0        0      117 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0       98 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utilities/zapier.py
--rw-r--r--   0        0        0     1221 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/__init__.py
--rw-r--r--   0        0        0      102 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/aiter.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/env.py
--rw-r--r--   0        0        0      325 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/ernie_functions.py
--rw-r--r--   0        0        0       91 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/formatting.py
--rw-r--r--   0        0        0      421 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/html.py
--rw-r--r--   0        0        0      211 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/input.py
--rw-r--r--   0        0        0      139 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/interactive_env.py
--rw-r--r--   0        0        0      133 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/iter.py
--rw-r--r--   0        0        0      258 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/json_schema.py
--rw-r--r--   0        0        0       92 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/loading.py
--rw-r--r--   0        0        0      181 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/math.py
--rw-r--r--   0        0        0       86 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/openai.py
--rw-r--r--   0        0        0      330 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/openai_functions.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/pydantic.py
--rw-r--r--   0        0        0      148 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/strings.py
--rw-r--r--   0        0        0      446 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/utils/utils.py
--rw-r--r--   0        0        0     2768 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/__init__.py
--rw-r--r--   0        0        0      220 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/analyticdb.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/annoy.py
--rw-r--r--   0        0        0      100 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/astradb.py
--rw-r--r--   0        0        0       82 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/atlas.py
--rw-r--r--   0        0        0       78 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/awadb.py
--rw-r--r--   0        0        0      256 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/azure_cosmos_db.py
--rw-r--r--   0        0        0      188 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/azuresearch.py
--rw-r--r--   0        0        0       89 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/bageldb.py
--rw-r--r--   0        0        0      115 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/baiducloud_vector_search.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/base.py
--rw-r--r--   0        0        0      104 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/cassandra.py
--rw-r--r--   0        0        0       90 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/chroma.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/clarifai.py
--rw-r--r--   0        0        0      148 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/clickhouse.py
--rw-r--r--   0        0        0       93 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/dashvector.py
--rw-r--r--   0        0        0      140 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/databricks_vector_search.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/deeplake.py
--rw-r--r--   0        0        0       78 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/dingo.py
--rw-r--r--   0        0        0      236 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0      111 2024-02-19 20:58:55.605226 langchain-0.1.8/langchain/vectorstores/docarray/base.py
--rw-r--r--   0        0        0      112 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0      125 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0      184 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0      362 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/elasticsearch.py
--rw-r--r--   0        0        0       84 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/epsilla.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/faiss.py
--rw-r--r--   0        0        0       78 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/hippo.py
--rw-r--r--   0        0        0       96 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/hologres.py
--rw-r--r--   0        0        0       84 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/lancedb.py
--rw-r--r--   0        0        0      128 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/llm_rails.py
--rw-r--r--   0        0        0       78 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/marqo.py
--rw-r--r--   0        0        0      106 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/matching_engine.py
--rw-r--r--   0        0        0       96 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/meilisearch.py
--rw-r--r--   0        0        0       81 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/milvus.py
--rw-r--r--   0        0        0      128 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/momento_vector_index.py
--rw-r--r--   0        0        0      192 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0      179 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/myscale.py
--rw-r--r--   0        0        0      147 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/neo4j_vector.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/nucliadb.py
--rw-r--r--   0        0        0      147 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0      234 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/pgembedding.py
--rw-r--r--   0        0        0       93 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/pgvecto_rs.py
--rw-r--r--   0        0        0      149 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/pgvector.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/pinecone.py
--rw-r--r--   0        0        0      130 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/qdrant.py
--rw-r--r--   0        0        0      265 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/redis/__init__.py
--rw-r--r--   0        0        0      213 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/redis/base.py
--rw-r--r--   0        0        0      416 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/redis/filters.py
--rw-r--r--   0        0        0      503 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/redis/schema.py
--rw-r--r--   0        0        0       86 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0       87 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/scann.py
--rw-r--r--   0        0        0       81 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/semadb.py
--rw-r--r--   0        0        0      165 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0      364 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/sklearn.py
--rw-r--r--   0        0        0       90 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/sqlitevss.py
--rw-r--r--   0        0        0      154 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/starrocks.py
--rw-r--r--   0        0        0      109 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/supabase.py
--rw-r--r--   0        0        0       75 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/tair.py
--rw-r--r--   0        0        0      191 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/tencentvectordb.py
--rw-r--r--   0        0        0       81 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/tigris.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/tiledb.py
--rw-r--r--   0        0        0      124 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/timescalevector.py
--rw-r--r--   0        0        0       90 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/typesense.py
--rw-r--r--   0        0        0       84 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/usearch.py
--rw-r--r--   0        0        0      227 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/utils.py
--rw-r--r--   0        0        0       75 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/vald.py
--rw-r--r--   0        0        0       81 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/vearch.py
--rw-r--r--   0        0        0      122 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/vectara.py
--rw-r--r--   0        0        0       88 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/vespa.py
--rw-r--r--   0        0        0      103 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/weaviate.py
--rw-r--r--   0        0        0       97 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/xata.py
--rw-r--r--   0        0        0       96 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/yellowbrick.py
--rw-r--r--   0        0        0      132 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/zep.py
--rw-r--r--   0        0        0       81 2024-02-19 20:58:55.609226 langchain-0.1.8/langchain/vectorstores/zilliz.py
--rw-r--r--   0        0        0    11689 2024-02-19 20:58:55.609226 langchain-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    13949 1970-01-01 00:00:00.000000 langchain-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-23 05:45:53.745760 langchain-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5879 2024-02-23 05:45:53.745760 langchain-0.1.9/README.md
+-rw-r--r--   0        0        0    13561 2024-02-23 05:45:53.745760 langchain-0.1.9/langchain/__init__.py
+-rw-r--r--   0        0        0      667 2024-02-23 05:45:53.745760 langchain-0.1.9/langchain/_api/__init__.py
+-rw-r--r--   0        0        0      471 2024-02-23 05:45:53.745760 langchain-0.1.9/langchain/_api/deprecation.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.745760 langchain-0.1.9/langchain/_api/path.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/adapters/__init__.py
+-rw-r--r--   0        0        0      653 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/adapters/openai.py
+-rw-r--r--   0        0        0     4813 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/__init__.py
+-rw-r--r--   0        0        0    54729 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent.py
+-rw-r--r--   0        0        0    15135 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_iterator.py
+-rw-r--r--   0        0        0     3678 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       25 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/ainetwork/__init__.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/ainetwork/toolkit.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0      156 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/base.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/clickup/__init__.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/clickup/toolkit.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0     3235 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/tool.py
+-rw-r--r--   0        0        0     1091 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0      177 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0      617 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       22 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/gitlab/__init__.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/gitlab/toolkit.py
+-rw-r--r--   0        0        0       21 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0      126 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0       23 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0       19 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/nasa/__init__.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/nasa/toolkit.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0       96 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0      530 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0     1153 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0      186 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0      170 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0      157 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0     1104 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0      174 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0      140 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0      269 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0     1094 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0       21 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/slack/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/slack/toolkit.py
+-rw-r--r--   0        0        0     1103 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0       23 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0      123 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0      127 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0      184 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       21 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/steam/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/steam/toolkit.py
+-rw-r--r--   0        0        0       56 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/vectorstore/__init__.py
+-rw-r--r--   0        0        0     4211 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/vectorstore/base.py
+-rw-r--r--   0        0        0      834 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/vectorstore/prompt.py
+-rw-r--r--   0        0        0     3001 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/vectorstore/toolkit.py
+-rw-r--r--   0        0        0     1095 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0       22 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0     1948 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/agent_types.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/chat/__init__.py
+-rw-r--r--   0        0        0     5084 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/chat/base.py
+-rw-r--r--   0        0        0     1977 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/chat/output_parser.py
+-rw-r--r--   0        0        0     1158 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/chat/prompt.py
+-rw-r--r--   0        0        0       75 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/conversational/__init__.py
+-rw-r--r--   0        0        0     4957 2024-02-23 05:45:53.749760 langchain-0.1.9/langchain/agents/conversational/base.py
+-rw-r--r--   0        0        0     1383 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/conversational/output_parser.py
+-rw-r--r--   0        0        0     1859 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/conversational/prompt.py
+-rw-r--r--   0        0        0       75 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/conversational_chat/__init__.py
+-rw-r--r--   0        0        0     5196 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/conversational_chat/base.py
+-rw-r--r--   0        0        0     2398 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/conversational_chat/output_parser.py
+-rw-r--r--   0        0        0     2763 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/conversational_chat/prompt.py
+-rw-r--r--   0        0        0      847 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/format_scratchpad/__init__.py
+-rw-r--r--   0        0        0      528 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/format_scratchpad/log.py
+-rw-r--r--   0        0        0      721 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/format_scratchpad/log_to_messages.py
+-rw-r--r--   0        0        0     2203 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/format_scratchpad/openai_functions.py
+-rw-r--r--   0        0        0     1885 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/format_scratchpad/openai_tools.py
+-rw-r--r--   0        0        0      578 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/format_scratchpad/xml.py
+-rw-r--r--   0        0        0     3244 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/initialize.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/json_chat/__init__.py
+-rw-r--r--   0        0        0     6832 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/json_chat/base.py
+-rw-r--r--   0        0        0      551 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/json_chat/prompt.py
+-rw-r--r--   0        0        0    23975 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/load_tools.py
+-rw-r--r--   0        0        0     4592 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/loading.py
+-rw-r--r--   0        0        0       86 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/mrkl/__init__.py
+-rw-r--r--   0        0        0     6046 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/mrkl/base.py
+-rw-r--r--   0        0        0     3407 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/mrkl/output_parser.py
+-rw-r--r--   0        0        0      641 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/mrkl/prompt.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_assistant/__init__.py
+-rw-r--r--   0        0        0    25712 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_assistant/base.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_functions_agent/__init__.py
+-rw-r--r--   0        0        0     2567 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py
+-rw-r--r--   0        0        0    11522 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_functions_agent/base.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_functions_multi_agent/__init__.py
+-rw-r--r--   0        0        0    11944 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_functions_multi_agent/base.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_tools/__init__.py
+-rw-r--r--   0        0        0     3388 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/openai_tools/base.py
+-rw-r--r--   0        0        0     1270 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1846 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/output_parsers/json.py
+-rw-r--r--   0        0        0     3467 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0     3492 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/output_parsers/openai_tools.py
+-rw-r--r--   0        0        0     2455 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/output_parsers/react_json_single_input.py
+-rw-r--r--   0        0        0     3218 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/output_parsers/react_single_input.py
+-rw-r--r--   0        0        0     1545 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/output_parsers/self_ask.py
+-rw-r--r--   0        0        0     1658 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/output_parsers/xml.py
+-rw-r--r--   0        0        0       76 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/react/__init__.py
+-rw-r--r--   0        0        0     3903 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/react/agent.py
+-rw-r--r--   0        0        0     5714 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/react/base.py
+-rw-r--r--   0        0        0     1231 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/react/output_parser.py
+-rw-r--r--   0        0        0     1906 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/react/textworld_prompt.py
+-rw-r--r--   0        0        0     6127 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/react/wiki_prompt.py
+-rw-r--r--   0        0        0     1175 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/schema.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/self_ask_with_search/__init__.py
+-rw-r--r--   0        0        0     8099 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/self_ask_with_search/base.py
+-rw-r--r--   0        0        0      138 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/self_ask_with_search/output_parser.py
+-rw-r--r--   0        0        0     1926 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/self_ask_with_search/prompt.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/structured_chat/__init__.py
+-rw-r--r--   0        0        0     9948 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/structured_chat/base.py
+-rw-r--r--   0        0        0     3799 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/structured_chat/output_parser.py
+-rw-r--r--   0        0        0      992 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/structured_chat/prompt.py
+-rw-r--r--   0        0        0     1409 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/tools.py
+-rw-r--r--   0        0        0     1475 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/types.py
+-rw-r--r--   0        0        0      384 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/utils.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/xml/__init__.py
+-rw-r--r--   0        0        0     7258 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/xml/base.py
+-rw-r--r--   0        0        0      767 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/agents/xml/prompt.py
+-rw-r--r--   0        0        0      217 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/base_language.py
+-rw-r--r--   0        0        0      701 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/cache.py
+-rw-r--r--   0        0        0     2509 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/__init__.py
+-rw-r--r--   0        0        0      211 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/aim_callback.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/arize_callback.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0      653 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/base.py
+-rw-r--r--   0        0        0      129 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/confident_callback.py
+-rw-r--r--   0        0        0      129 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/context_callback.py
+-rw-r--r--   0        0        0     2589 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/file.py
+-rw-r--r--   0        0        0      123 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0      275 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/human.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/infino_callback.py
+-rw-r--r--   0        0        0      241 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/labelstudio_callback.py
+-rw-r--r--   0        0        0      142 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/llmonitor_callback.py
+-rw-r--r--   0        0        0     1777 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/manager.py
+-rw-r--r--   0        0        0      305 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/openai_info.py
+-rw-r--r--   0        0        0      141 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0      135 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/stdout.py
+-rw-r--r--   0        0        0     2399 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/streaming_aiter.py
+-rw-r--r--   0        0        0     3371 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/streaming_aiter_final_only.py
+-rw-r--r--   0        0        0      173 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     3357 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/streaming_stdout_final_only.py
+-rw-r--r--   0        0        0     3190 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0      490 2024-02-23 05:45:53.753760 langchain-0.1.9/langchain/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0      589 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0      154 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/base.py
+-rw-r--r--   0        0        0      154 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/comet.py
+-rw-r--r--   0        0        0      233 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0      218 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0      226 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/log_stream.py
+-rw-r--r--   0        0        0     1384 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/logging.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/root_listeners.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0      470 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0      168 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0      229 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/trubrics_callback.py
+-rw-r--r--   0        0        0      403 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/utils.py
+-rw-r--r--   0        0        0      130 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0      129 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0     5951 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/__init__.py
+-rw-r--r--   0        0        0       84 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/__init__.py
+-rw-r--r--   0        0        0     8919 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/base.py
+-rw-r--r--   0        0        0     2452 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/news_docs.py
+-rw-r--r--   0        0        0     3399 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/open_meteo_docs.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/openapi/__init__.py
+-rw-r--r--   0        0        0     8786 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/openapi/chain.py
+-rw-r--r--   0        0        0     1791 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/openapi/prompts.py
+-rw-r--r--   0        0        0     1975 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/openapi/requests_chain.py
+-rw-r--r--   0        0        0     1847 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/openapi/response_chain.py
+-rw-r--r--   0        0        0     1920 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/podcast_docs.py
+-rw-r--r--   0        0        0     1031 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/prompt.py
+-rw-r--r--   0        0        0     1537 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/api/tmdb_docs.py
+-rw-r--r--   0        0        0    28451 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/base.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/chat_vector_db/__init__.py
+-rw-r--r--   0        0        0      694 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/chat_vector_db/prompts.py
+-rw-r--r--   0        0        0      367 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/combine_documents/__init__.py
+-rw-r--r--   0        0        0     8005 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/combine_documents/base.py
+-rw-r--r--   0        0        0    11781 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/combine_documents/map_reduce.py
+-rw-r--r--   0        0        0     8991 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/combine_documents/map_rerank.py
+-rw-r--r--   0        0        0    13894 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/combine_documents/reduce.py
+-rw-r--r--   0        0        0     9113 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/combine_documents/refine.py
+-rw-r--r--   0        0        0    10963 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/combine_documents/stuff.py
+-rw-r--r--   0        0        0      107 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/constitutional_ai/__init__.py
+-rw-r--r--   0        0        0     6341 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/constitutional_ai/base.py
+-rw-r--r--   0        0        0      283 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/constitutional_ai/models.py
+-rw-r--r--   0        0        0    21738 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/constitutional_ai/principles.py
+-rw-r--r--   0        0        0     8666 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/constitutional_ai/prompts.py
+-rw-r--r--   0        0        0       71 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/conversation/__init__.py
+-rw-r--r--   0        0        0     2366 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/conversation/base.py
+-rw-r--r--   0        0        0      856 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/conversation/memory.py
+-rw-r--r--   0        0        0      913 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/conversation/prompt.py
+-rw-r--r--   0        0        0       49 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0    17834 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/conversational_retrieval/base.py
+-rw-r--r--   0        0        0      720 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/conversational_retrieval/prompts.py
+-rw-r--r--   0        0        0      126 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/elasticsearch_database/__init__.py
+-rw-r--r--   0        0        0     8287 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/elasticsearch_database/base.py
+-rw-r--r--   0        0        0     1425 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/elasticsearch_database/prompts.py
+-rw-r--r--   0        0        0      465 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/ernie_functions/__init__.py
+-rw-r--r--   0        0        0    23205 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/ernie_functions/base.py
+-rw-r--r--   0        0        0      741 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/example_generator.py
+-rw-r--r--   0        0        0       51 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/flare/__init__.py
+-rw-r--r--   0        0        0     9033 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/flare/base.py
+-rw-r--r--   0        0        0     1471 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/flare/prompts.py
+-rw-r--r--   0        0        0       49 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/__init__.py
+-rw-r--r--   0        0        0     8397 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/arangodb.py
+-rw-r--r--   0        0        0     3671 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/base.py
+-rw-r--r--   0        0        0    10452 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/cypher.py
+-rw-r--r--   0        0        0     9625 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/cypher_utils.py
+-rw-r--r--   0        0        0     5272 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/falkordb.py
+-rw-r--r--   0        0        0     3717 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/hugegraph.py
+-rw-r--r--   0        0        0     3698 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/kuzu.py
+-rw-r--r--   0        0        0     3692 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/nebulagraph.py
+-rw-r--r--   0        0        0     6890 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/neptune_cypher.py
+-rw-r--r--   0        0        0     6610 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/neptune_sparql.py
+-rw-r--r--   0        0        0     7226 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/ontotext_graphdb.py
+-rw-r--r--   0        0        0    16720 2024-02-23 05:45:53.757760 langchain-0.1.9/langchain/chains/graph_qa/prompts.py
+-rw-r--r--   0        0        0     5838 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/graph_qa/sparql.py
+-rw-r--r--   0        0        0     2662 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/history_aware_retriever.py
+-rw-r--r--   0        0        0       75 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/hyde/__init__.py
+-rw-r--r--   0        0        0     3341 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/hyde/base.py
+-rw-r--r--   0        0        0     1913 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/hyde/prompts.py
+-rw-r--r--   0        0        0    14776 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm.py
+-rw-r--r--   0        0        0      450 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_bash/__init__.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_checker/__init__.py
+-rw-r--r--   0        0        0     6164 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_checker/base.py
+-rw-r--r--   0        0        0     1125 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_checker/prompt.py
+-rw-r--r--   0        0        0      143 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_math/__init__.py
+-rw-r--r--   0        0        0     6723 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_math/base.py
+-rw-r--r--   0        0        0      868 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_math/prompt.py
+-rw-r--r--   0        0        0     3193 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_requests.py
+-rw-r--r--   0        0        0      352 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_summarization_checker/__init__.py
+-rw-r--r--   0        0        0     6582 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_summarization_checker/base.py
+-rw-r--r--   0        0        0      654 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
+-rw-r--r--   0        0        0      377 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_summarization_checker/prompts/check_facts.txt
+-rw-r--r--   0        0        0      128 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_summarization_checker/prompts/create_facts.txt
+-rw-r--r--   0        0        0      416 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_summarization_checker/prompts/revise_summary.txt
+-rw-r--r--   0        0        0      467 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0    25261 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/loading.py
+-rw-r--r--   0        0        0     3732 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/mapreduce.py
+-rw-r--r--   0        0        0     3086 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/moderation.py
+-rw-r--r--   0        0        0       96 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/natbot/__init__.py
+-rw-r--r--   0        0        0     4695 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/natbot/base.py
+-rw-r--r--   0        0        0    16050 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/natbot/crawler.py
+-rw-r--r--   0        0        0     4989 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/natbot/prompt.py
+-rw-r--r--   0        0        0     1357 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_functions/__init__.py
+-rw-r--r--   0        0        0    10075 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_functions/base.py
+-rw-r--r--   0        0        0     3526 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_functions/citation_fuzzy_match.py
+-rw-r--r--   0        0        0     4073 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_functions/extraction.py
+-rw-r--r--   0        0        0    11306 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_functions/openapi.py
+-rw-r--r--   0        0        0     3918 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_functions/qa_with_structure.py
+-rw-r--r--   0        0        0     2660 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_functions/tagging.py
+-rw-r--r--   0        0        0     1257 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_functions/utils.py
+-rw-r--r--   0        0        0      134 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_tools/__init__.py
+-rw-r--r--   0        0        0     1665 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/openai_tools/extraction.py
+-rw-r--r--   0        0        0     2015 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/prompt_selector.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_generation/__init__.py
+-rw-r--r--   0        0        0     2464 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_generation/base.py
+-rw-r--r--   0        0        0     1875 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_generation/prompt.py
+-rw-r--r--   0        0        0      173 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_with_sources/__init__.py
+-rw-r--r--   0        0        0     7976 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_with_sources/base.py
+-rw-r--r--   0        0        0     6793 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_with_sources/loading.py
+-rw-r--r--   0        0        0     6971 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_with_sources/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1318 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_with_sources/refine_prompts.py
+-rw-r--r--   0        0        0     2459 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_with_sources/retrieval.py
+-rw-r--r--   0        0        0     6581 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_with_sources/stuff_prompt.py
+-rw-r--r--   0        0        0     2770 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/qa_with_sources/vector_db.py
+-rw-r--r--   0        0        0      131 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/query_constructor/__init__.py
+-rw-r--r--   0        0        0    13621 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/query_constructor/base.py
+-rw-r--r--   0        0        0     3191 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/query_constructor/ir.py
+-rw-r--r--   0        0        0     5707 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/query_constructor/parser.py
+-rw-r--r--   0        0        0     6880 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/query_constructor/prompt.py
+-rw-r--r--   0        0        0      321 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/query_constructor/schema.py
+-rw-r--r--   0        0        0     8503 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/question_answering/__init__.py
+-rw-r--r--   0        0        0     8013 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/question_answering/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1622 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/question_answering/map_rerank_prompt.py
+-rw-r--r--   0        0        0     2378 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/question_answering/refine_prompts.py
+-rw-r--r--   0        0        0     1146 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/question_answering/stuff_prompt.py
+-rw-r--r--   0        0        0     2742 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/retrieval.py
+-rw-r--r--   0        0        0       62 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/retrieval_qa/__init__.py
+-rw-r--r--   0        0        0     9952 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/retrieval_qa/base.py
+-rw-r--r--   0        0        0      399 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/retrieval_qa/prompt.py
+-rw-r--r--   0        0        0      407 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/router/__init__.py
+-rw-r--r--   0        0        0     4571 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/router/base.py
+-rw-r--r--   0        0        0     1982 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/router/embedding_router.py
+-rw-r--r--   0        0        0     4283 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/router/llm_router.py
+-rw-r--r--   0        0        0     2245 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/router/multi_prompt.py
+-rw-r--r--   0        0        0     1156 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/router/multi_prompt_prompt.py
+-rw-r--r--   0        0        0     1079 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/router/multi_retrieval_prompt.py
+-rw-r--r--   0        0        0     3659 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/router/multi_retrieval_qa.py
+-rw-r--r--   0        0        0     7510 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/sequential.py
+-rw-r--r--   0        0        0       47 2024-02-23 05:45:53.761760 langchain-0.1.9/langchain/chains/sql_database/__init__.py
+-rw-r--r--   0        0        0    15458 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/sql_database/prompt.py
+-rw-r--r--   0        0        0     5293 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/sql_database/query.py
+-rw-r--r--   0        0        0      204 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/structured_output/__init__.py
+-rw-r--r--   0        0        0    22263 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/structured_output/base.py
+-rw-r--r--   0        0        0     5804 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/summarize/__init__.py
+-rw-r--r--   0        0        0      238 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/summarize/map_reduce_prompt.py
+-rw-r--r--   0        0        0      677 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/summarize/refine_prompts.py
+-rw-r--r--   0        0        0      238 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/summarize/stuff_prompt.py
+-rw-r--r--   0        0        0     2369 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chains/transform.py
+-rw-r--r--   0        0        0      452 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/__init__.py
+-rw-r--r--   0        0        0       95 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/base.py
+-rw-r--r--   0        0        0      240 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/facebook_messenger.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/gmail.py
+-rw-r--r--   0        0        0      107 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/imessage.py
+-rw-r--r--   0        0        0      187 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/langsmith.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/slack.py
+-rw-r--r--   0        0        0      107 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/telegram.py
+-rw-r--r--   0        0        0      290 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/utils.py
+-rw-r--r--   0        0        0      107 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_loaders/whatsapp.py
+-rw-r--r--   0        0        0     1979 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/__init__.py
+-rw-r--r--   0        0        0      199 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/anthropic.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/anyscale.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/azure_openai.py
+-rw-r--r--   0        0        0      189 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0      110 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/baichuan.py
+-rw-r--r--   0        0        0      131 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      268 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/base.py
+-rw-r--r--   0        0        0      131 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/bedrock.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/cohere.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/databricks.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/ernie.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/everlyai.py
+-rw-r--r--   0        0        0      169 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/fake.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/fireworks.py
+-rw-r--r--   0        0        0       95 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/gigachat.py
+-rw-r--r--   0        0        0      158 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/google_palm.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/human.py
+-rw-r--r--   0        0        0      107 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/hunyuan.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/javelin_ai_gateway.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/jinachat.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/konko.py
+-rw-r--r--   0        0        0      137 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/litellm.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/meta.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/minimax.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/mlflow.py
+-rw-r--r--   0        0        0      156 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/ollama.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/openai.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/pai_eas_endpoint.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/tongyi.py
+-rw-r--r--   0        0        0      110 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/vertexai.py
+-rw-r--r--   0        0        0      178 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/volcengine_maas.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/chat_models/yandex.py
+-rw-r--r--   0        0        0     1184 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/docstore/__init__.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/docstore/base.py
+-rw-r--r--   0        0        0       70 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/docstore/document.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/docstore/in_memory.py
+-rw-r--r--   0        0        0       86 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/docstore/wikipedia.py
+-rw-r--r--   0        0        0     5722 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/acreom.py
+-rw-r--r--   0        0        0      554 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/airbyte.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/airtable.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/arcgis_loader.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/arxiv.py
+-rw-r--r--   0        0        0      190 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/assemblyai.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/async_html.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/azure_ai_data.py
+-rw-r--r--   0        0        0      166 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0      151 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0      146 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/baiducloud_bos_directory.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/baiducloud_bos_file.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/base.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/base_o365.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/bibtex.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/bigquery.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/bilibili.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/blackboard.py
+-rw-r--r--   0        0        0      374 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0      140 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0      138 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0      172 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/blockchain.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/brave_search.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/browserless.py
+-rw-r--r--   0        0        0      138 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/chromium.py
+-rw-r--r--   0        0        0      146 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0      118 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/concurrent.py
+-rw-r--r--   0        0        0      154 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/confluence.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/conllu.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/couchbase.py
+-rw-r--r--   0        0        0      156 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0      163 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/dataframe.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/diffbot.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/directory.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/discord.py
+-rw-r--r--   0        0        0      119 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/docusaurus.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/dropbox.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0      177 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/email.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/epub.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/etherscan.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/evernote.py
+-rw-r--r--   0        0        0      118 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/excel.py
+-rw-r--r--   0        0        0      167 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/fauna.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/figma.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/generic.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.765760 langchain-0.1.9/langchain/document_loaders/git.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/gitbook.py
+-rw-r--r--   0        0        0      160 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/github.py
+-rw-r--r--   0        0        0      145 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/google_speech_to_text.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/helpers.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/hn.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/html.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/html_bs.py
+-rw-r--r--   0        0        0      144 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/ifixit.py
+-rw-r--r--   0        0        0      118 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/image.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/image_captions.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/imsdb.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/iugu.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/joplin.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/json_loader.py
+-rw-r--r--   0        0        0      198 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/lakefs.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/larksuite.py
+-rw-r--r--   0        0        0      127 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/markdown.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/mastodon.py
+-rw-r--r--   0        0        0      110 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/max_compute.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/merge.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/mhtml.py
+-rw-r--r--   0        0        0      131 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/mongodb.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/news.py
+-rw-r--r--   0        0        0      196 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/notebook.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/notion.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/notiondb.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/nuclia.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/obs_file.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/obsidian.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/odt.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/onedrive.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/onenote.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/org_mode.py
+-rw-r--r--   0        0        0      789 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0      225 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/docai.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0      176 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      136 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/language/cobol.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0      141 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0      136 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/msword.py
+-rw-r--r--   0        0        0      494 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0      706 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/pdf.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/polars_dataframe.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/psychic.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/pubmed.py
+-rw-r--r--   0        0        0      137 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/python.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/quip.py
+-rw-r--r--   0        0        0      128 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/reddit.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/roam.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/rspace.py
+-rw-r--r--   0        0        0       96 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/rss.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/rst.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/rtf.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/s3_file.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/sharepoint.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/sitemap.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/spreedly.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/srt.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/stripe.py
+-rw-r--r--   0        0        0      275 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/telegram.py
+-rw-r--r--   0        0        0      147 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0      123 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0      141 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/tensorflow_datasets.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/text.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/toml.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/trello.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/tsv.py
+-rw-r--r--   0        0        0      119 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/twitter.py
+-rw-r--r--   0        0        0      601 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/unstructured.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/url.py
+-rw-r--r--   0        0        0      236 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/weather.py
+-rw-r--r--   0        0        0      110 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/web_base.py
+-rw-r--r--   0        0        0      167 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0      187 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/word_document.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/xml.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/xorbits.py
+-rw-r--r--   0        0        0      218 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_loaders/youtube.py
+-rw-r--r--   0        0        0     1616 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/__init__.py
+-rw-r--r--   0        0        0      155 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/beautiful_soup_transformer.py
+-rw-r--r--   0        0        0      149 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0      136 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0      145 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0      487 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0      149 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/google_translate.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/html2text.py
+-rw-r--r--   0        0        0      137 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0      144 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0      191 2024-02-23 05:45:53.769760 langchain-0.1.9/langchain/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     6033 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/document_transformers/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0     3598 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/__init__.py
+-rw-r--r--   0        0        0      248 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0       90 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/awa.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/azure_openai.py
+-rw-r--r--   0        0        0      142 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/base.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/bedrock.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/bookend.py
+-rw-r--r--   0        0        0     8240 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/cache.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/clarifai.py
+-rw-r--r--   0        0        0      148 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/cloudflare_workersai.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/cohere.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/dashscope.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/databricks.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/deepinfra.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/edenai.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/embaas.py
+-rw-r--r--   0        0        0       96 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/ernie.py
+-rw-r--r--   0        0        0      164 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/fake.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/fastembed.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/google_palm.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/gpt4all.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/gradient_ai.py
+-rw-r--r--   0        0        0      344 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/huggingface.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0      200 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/infinity.py
+-rw-r--r--   0        0        0      140 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/javelin_ai_gateway.py
+-rw-r--r--   0        0        0       93 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/jina.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/johnsnowlabs.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/llamacpp.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/llm_rails.py
+-rw-r--r--   0        0        0      118 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/localai.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/minimax.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/mlflow.py
+-rw-r--r--   0        0        0      134 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/mosaicml.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0      119 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/ollama.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/openai.py
+-rw-r--r--   0        0        0      200 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/self_hosted.py
+-rw-r--r--   0        0        0      255 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      148 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0      107 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0      130 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/vertexai.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/voyageai.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/embeddings/xinference.py
+-rw-r--r--   0        0        0      476 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/env.py
+-rw-r--r--   0        0        0     5803 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/__init__.py
+-rw-r--r--   0        0        0      165 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/agents/__init__.py
+-rw-r--r--   0        0        0    13884 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/agents/trajectory_eval_chain.py
+-rw-r--r--   0        0        0     5938 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/agents/trajectory_eval_prompt.py
+-rw-r--r--   0        0        0     1400 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/comparison/__init__.py
+-rw-r--r--   0        0        0    16056 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/comparison/eval_chain.py
+-rw-r--r--   0        0        0     2358 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/comparison/prompt.py
+-rw-r--r--   0        0        0     1647 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/criteria/__init__.py
+-rw-r--r--   0        0        0    21358 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/criteria/eval_chain.py
+-rw-r--r--   0        0        0     1756 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/criteria/prompt.py
+-rw-r--r--   0        0        0      323 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/embedding_distance/__init__.py
+-rw-r--r--   0        0        0    15503 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/embedding_distance/base.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/exact_match/__init__.py
+-rw-r--r--   0        0        0     2751 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/exact_match/base.py
+-rw-r--r--   0        0        0     6693 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/loading.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/parsing/__init__.py
+-rw-r--r--   0        0        0     5246 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/parsing/base.py
+-rw-r--r--   0        0        0     3679 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/parsing/json_distance.py
+-rw-r--r--   0        0        0     3197 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/parsing/json_schema.py
+-rw-r--r--   0        0        0      344 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/qa/__init__.py
+-rw-r--r--   0        0        0    10886 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/qa/eval_chain.py
+-rw-r--r--   0        0        0     3911 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/qa/eval_prompt.py
+-rw-r--r--   0        0        0     1052 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/qa/generate_chain.py
+-rw-r--r--   0        0        0      606 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/qa/generate_prompt.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/regex_match/__init__.py
+-rw-r--r--   0        0        0     2407 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/regex_match/base.py
+-rw-r--r--   0        0        0    18197 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/schema.py
+-rw-r--r--   0        0        0     1112 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/scoring/__init__.py
+-rw-r--r--   0        0        0    15656 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/scoring/eval_chain.py
+-rw-r--r--   0        0        0     2129 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/scoring/prompt.py
+-rw-r--r--   0        0        0      285 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/string_distance/__init__.py
+-rw-r--r--   0        0        0    14014 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/evaluation/string_distance/base.py
+-rw-r--r--   0        0        0      141 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/example_generator.py
+-rw-r--r--   0        0        0      167 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/formatting.py
+-rw-r--r--   0        0        0     7435 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/globals/__init__.py
+-rw-r--r--   0        0        0     1104 2024-02-23 05:45:53.773760 langchain-0.1.9/langchain/graphs/__init__.py
+-rw-r--r--   0        0        0      148 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/falkordb_graph.py
+-rw-r--r--   0        0        0      141 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/graph_document.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/graph_store.py
+-rw-r--r--   0        0        0       84 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/hugegraph.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/nebula_graph.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/neptune_graph.py
+-rw-r--r--   0        0        0      299 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/networkx_graph.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/graphs/rdf_graph.py
+-rw-r--r--   0        0        0     2874 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/hub.py
+-rw-r--r--   0        0        0      902 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/__init__.py
+-rw-r--r--   0        0        0    22479 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/_api.py
+-rw-r--r--   0        0        0    20556 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0     5221 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/base.py
+-rw-r--r--   0        0        0     1752 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/graph.py
+-rw-r--r--   0        0        0       49 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/prompts/__init__.py
+-rw-r--r--   0        0        0     1952 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/prompts/entity_extraction.py
+-rw-r--r--   0        0        0     1157 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/prompts/entity_summarization.py
+-rw-r--r--   0        0        0     1599 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/prompts/knowledge_triplet_extraction.py
+-rw-r--r--   0        0        0     3423 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/indexes/vectorstore.py
+-rw-r--r--   0        0        0      282 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/input.py
+-rw-r--r--   0        0        0    17110 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/__init__.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/ai21.py
+-rw-r--r--   0        0        0       86 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/aleph_alpha.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0       82 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/anthropic.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/anyscale.py
+-rw-r--r--   0        0        0       70 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/arcee.py
+-rw-r--r--   0        0        0       82 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/aviary.py
+-rw-r--r--   0        0        0      507 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0       76 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/bananadev.py
+-rw-r--r--   0        0        0      228 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/base.py
+-rw-r--r--   0        0        0       76 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/baseten.py
+-rw-r--r--   0        0        0       67 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/beam.py
+-rw-r--r--   0        0        0      128 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/bedrock.py
+-rw-r--r--   0        0        0       92 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/bittensor.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/cerebriumai.py
+-rw-r--r--   0        0        0       76 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/chatglm.py
+-rw-r--r--   0        0        0       79 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/clarifai.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/cloudflare_workersai.py
+-rw-r--r--   0        0        0       89 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/cohere.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/ctransformers.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/ctranslate2.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/databricks.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/deepinfra.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/deepsparse.py
+-rw-r--r--   0        0        0       73 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/edenai.py
+-rw-r--r--   0        0        0      127 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/fake.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/fireworks.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/forefrontai.py
+-rw-r--r--   0        0        0       79 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/gigachat.py
+-rw-r--r--   0        0        0       86 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/google_palm.py
+-rw-r--r--   0        0        0       76 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/gooseai.py
+-rw-r--r--   0        0        0       76 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/gpt4all.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/gradient_ai.py
+-rw-r--r--   0        0        0      664 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/grammars/json.gbnf
+-rw-r--r--   0        0        0      167 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/grammars/list.gbnf
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0      107 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/huggingface_hub.py
+-rw-r--r--   0        0        0      129 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0      148 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0       95 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/human.py
+-rw-r--r--   0        0        0      123 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/javelin_ai_gateway.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/koboldai.py
+-rw-r--r--   0        0        0       79 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/llamacpp.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/loading.py
+-rw-r--r--   0        0        0       93 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/manifest.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/minimax.py
+-rw-r--r--   0        0        0       73 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/mlflow.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0       70 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/modal.py
+-rw-r--r--   0        0        0       95 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/mosaicml.py
+-rw-r--r--   0        0        0       79 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/nlpcloud.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0       82 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/ollama.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/opaqueprompts.py
+-rw-r--r--   0        0        0      193 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/openai.py
+-rw-r--r--   0        0        0       76 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/openllm.py
+-rw-r--r--   0        0        0       73 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/openlm.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/pai_eas_endpoint.py
+-rw-r--r--   0        0        0       73 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/petals.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/pipelineai.py
+-rw-r--r--   0        0        0       82 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/predibase.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/predictionguard.py
+-rw-r--r--   0        0        0      168 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0       82 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/replicate.py
+-rw-r--r--   0        0        0       67 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/rwkv.py
+-rw-r--r--   0        0        0      160 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/self_hosted.py
+-rw-r--r--   0        0        0      143 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/stochasticai.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/symblai_nebula.py
+-rw-r--r--   0        0        0       76 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/textgen.py
+-rw-r--r--   0        0        0       92 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/titan_takeoff.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/titan_takeoff_pro.py
+-rw-r--r--   0        0        0       79 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/together.py
+-rw-r--r--   0        0        0       89 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/tongyi.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/utils.py
+-rw-r--r--   0        0        0      147 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/vertexai.py
+-rw-r--r--   0        0        0       93 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/vllm.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/volcengine_maas.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/watsonxllm.py
+-rw-r--r--   0        0        0       73 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/writer.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/xinference.py
+-rw-r--r--   0        0        0       79 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/llms/yandex.py
+-rw-r--r--   0        0        0      206 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/load/__init__.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/load/dump.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/load/load.py
+-rw-r--r--   0        0        0      412 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/load/serializable.py
+-rw-r--r--   0        0        0     3256 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/memory/__init__.py
+-rw-r--r--   0        0        0     4861 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/memory/buffer.py
+-rw-r--r--   0        0        0     1616 2024-02-23 05:45:53.777760 langchain-0.1.9/langchain/memory/buffer_window.py
+-rw-r--r--   0        0        0     2245 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_memory.py
+-rw-r--r--   0        0        0     1560 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/astradb.py
+-rw-r--r--   0        0        0      145 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0      143 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0      142 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0      157 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/elasticsearch.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/file.py
+-rw-r--r--   0        0        0      145 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      118 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/momento.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/neo4j.py
+-rw-r--r--   0        0        0      142 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/redis.py
+-rw-r--r--   0        0        0      141 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/rocksetdb.py
+-rw-r--r--   0        0        0      157 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/singlestoredb.py
+-rw-r--r--   0        0        0      248 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/sql.py
+-rw-r--r--   0        0        0      145 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0      155 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/upstash_redis.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/xata.py
+-rw-r--r--   0        0        0      118 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     2912 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/combined.py
+-rw-r--r--   0        0        0    15677 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/entity.py
+-rw-r--r--   0        0        0     5075 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/kg.py
+-rw-r--r--   0        0        0     3106 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/motorhead_memory.py
+-rw-r--r--   0        0        0     8181 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/prompt.py
+-rw-r--r--   0        0        0      794 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/readonly.py
+-rw-r--r--   0        0        0      761 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/simple.py
+-rw-r--r--   0        0        0     3389 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/summary.py
+-rw-r--r--   0        0        0     2949 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/summary_buffer.py
+-rw-r--r--   0        0        0     2144 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/token_buffer.py
+-rw-r--r--   0        0        0      617 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/utils.py
+-rw-r--r--   0        0        0     3002 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/vectorstore.py
+-rw-r--r--   0        0        0     5090 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/memory/zep_memory.py
+-rw-r--r--   0        0        0     3278 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/model_laboratory.py
+-rw-r--r--   0        0        0     2216 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1084 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/boolean.py
+-rw-r--r--   0        0        0     1799 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/combining.py
+-rw-r--r--   0        0        0     1974 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1205 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/enum.py
+-rw-r--r--   0        0        0      424 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/ernie_functions.py
+-rw-r--r--   0        0        0     3153 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/fix.py
+-rw-r--r--   0        0        0     3958 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/format_instructions.py
+-rw-r--r--   0        0        0      298 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/json.py
+-rw-r--r--   0        0        0      310 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/list.py
+-rw-r--r--   0        0        0      702 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/loading.py
+-rw-r--r--   0        0        0     7989 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0     5124 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/openai_tools.py
+-rw-r--r--   0        0        0     6548 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/pandas_dataframe.py
+-rw-r--r--   0        0        0      508 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/prompts.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/pydantic.py
+-rw-r--r--   0        0        0      129 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/rail_parser.py
+-rw-r--r--   0        0        0     1214 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/regex.py
+-rw-r--r--   0        0        0     1709 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/regex_dict.py
+-rw-r--r--   0        0        0     7792 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/retry.py
+-rw-r--r--   0        0        0     3134 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/structured.py
+-rw-r--r--   0        0        0       93 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/xml.py
+-rw-r--r--   0        0        0     2181 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/output_parsers/yaml.py
+-rw-r--r--   0        0        0     2560 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/__init__.py
+-rw-r--r--   0        0        0      565 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/base.py
+-rw-r--r--   0        0        0     1045 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/chat.py
+-rw-r--r--   0        0        0      568 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/example_selector/__init__.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/example_selector/base.py
+-rw-r--r--   0        0        0      136 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/example_selector/length_based.py
+-rw-r--r--   0        0        0      203 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/example_selector/ngram_overlap.py
+-rw-r--r--   0        0        0      288 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/example_selector/semantic_similarity.py
+-rw-r--r--   0        0        0      265 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/few_shot.py
+-rw-r--r--   0        0        0      128 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0      530 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/loading.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/pipeline.py
+-rw-r--r--   0        0        0      153 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/prompts/prompt.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/py.typed
+-rw-r--r--   0        0        0      897 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      134 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/pydantic_v1/main.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/python.py
+-rw-r--r--   0        0        0      222 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/requests.py
+-rw-r--r--   0        0        0     3488 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/arcee.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/arxiv.py
+-rw-r--r--   0        0        0      150 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/azure_cognitive_search.py
+-rw-r--r--   0        0        0      221 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/bedrock.py
+-rw-r--r--   0        0        0      162 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/bm25.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/chaindesk.py
+-rw-r--r--   0        0        0      138 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0      126 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/cohere_rag_retriever.py
+-rw-r--r--   0        0        0     2298 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/contextual_compression.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/databerry.py
+-rw-r--r--   0        0        0      129 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/docarray.py
+-rw-r--r--   0        0        0      701 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/__init__.py
+-rw-r--r--   0        0        0     3775 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/base.py
+-rw-r--r--   0        0        0     3955 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/chain_extract.py
+-rw-r--r--   0        0        0      366 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/chain_extract_prompt.py
+-rw-r--r--   0        0        0     2757 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/chain_filter.py
+-rw-r--r--   0        0        0      231 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/chain_filter_prompt.py
+-rw-r--r--   0        0        0     4213 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/cohere_rerank.py
+-rw-r--r--   0        0        0     3031 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/embeddings_filter.py
+-rw-r--r--   0        0        0     2415 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/document_compressors/flashrank_rerank.py
+-rw-r--r--   0        0        0      141 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/embedchain.py
+-rw-r--r--   0        0        0     9668 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/ensemble.py
+-rw-r--r--   0        0        0      171 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/google_cloud_documentai_warehouse.py
+-rw-r--r--   0        0        0      334 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/google_vertex_ai_search.py
+-rw-r--r--   0        0        0       92 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/kay.py
+-rw-r--r--   0        0        0      803 2024-02-23 05:45:53.781760 langchain-0.1.9/langchain/retrievers/kendra.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/knn.py
+-rw-r--r--   0        0        0      177 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/llama_index.py
+-rw-r--r--   0        0        0     3489 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/merger_retriever.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/metal.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/milvus.py
+-rw-r--r--   0        0        0     6768 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/multi_query.py
+-rw-r--r--   0        0        0     3920 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/multi_vector.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/outline.py
+-rw-r--r--   0        0        0     5196 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/parent_document_retriever.py
+-rw-r--r--   0        0        0      150 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/pubmed.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/pupmed.py
+-rw-r--r--   0        0        0     2658 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/re_phraser.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/__init__.py
+-rw-r--r--   0        0        0     2194 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/astradb.py
+-rw-r--r--   0        0        0     9902 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/base.py
+-rw-r--r--   0        0        0     1474 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/chroma.py
+-rw-r--r--   0        0        0     1918 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/dashvector.py
+-rw-r--r--   0        0        0     2631 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/deeplake.py
+-rw-r--r--   0        0        0     3273 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/elasticsearch.py
+-rw-r--r--   0        0        0     3352 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/milvus.py
+-rw-r--r--   0        0        0     2303 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/mongodb_atlas.py
+-rw-r--r--   0        0        0     3636 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/myscale.py
+-rw-r--r--   0        0        0     3271 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/opensearch.py
+-rw-r--r--   0        0        0     1529 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/pgvector.py
+-rw-r--r--   0        0        0     1710 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/pinecone.py
+-rw-r--r--   0        0        0     3168 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/qdrant.py
+-rw-r--r--   0        0        0     3376 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/redis.py
+-rw-r--r--   0        0        0     2974 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/supabase.py
+-rw-r--r--   0        0        0     2633 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/timescalevector.py
+-rw-r--r--   0        0        0     2164 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/vectara.py
+-rw-r--r--   0        0        0     2619 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/self_query/weaviate.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/svm.py
+-rw-r--r--   0        0        0      167 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/tavily_search_api.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/tfidf.py
+-rw-r--r--   0        0        0     6295 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/time_weighted_retriever.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0      150 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0     8196 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/web_research.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/wikipedia.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/you.py
+-rw-r--r--   0        0        0      142 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/zep.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/retrievers/zilliz.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/runnables/__init__.py
+-rw-r--r--   0        0        0      809 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/runnables/hub.py
+-rw-r--r--   0        0        0     1521 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/runnables/openai_functions.py
+-rw-r--r--   0        0        0     2065 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/__init__.py
+-rw-r--r--   0        0        0      149 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/agent.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/cache.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/__init__.py
+-rw-r--r--   0        0        0      511 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/base.py
+-rw-r--r--   0        0        0     1511 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/manager.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/stdout.py
+-rw-r--r--   0        0        0      131 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/base.py
+-rw-r--r--   0        0        0      176 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0      219 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0      127 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0      226 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/log_stream.py
+-rw-r--r--   0        0        0      105 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/root_listeners.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0      470 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0      257 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0       80 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/chat.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/chat_history.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/document.py
+-rw-r--r--   0        0        0       75 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/embeddings.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/exceptions.py
+-rw-r--r--   0        0        0      367 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/language_model.py
+-rw-r--r--   0        0        0       71 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/memory.py
+-rw-r--r--   0        0        0     1048 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/messages.py
+-rw-r--r--   0        0        0      320 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/output.py
+-rw-r--r--   0        0        0      651 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/output_parser.py
+-rw-r--r--   0        0        0       80 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/prompt.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/prompt_template.py
+-rw-r--r--   0        0        0       81 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/retriever.py
+-rw-r--r--   0        0        0     1796 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/__init__.py
+-rw-r--r--   0        0        0      781 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/base.py
+-rw-r--r--   0        0        0       89 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/branch.py
+-rw-r--r--   0        0        0      665 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/config.py
+-rw-r--r--   0        0        0      333 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/configurable.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/fallbacks.py
+-rw-r--r--   0        0        0      260 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/history.py
+-rw-r--r--   0        0        0      205 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/passthrough.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/retry.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/router.py
+-rw-r--r--   0        0        0     1118 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/runnable/utils.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/storage.py
+-rw-r--r--   0        0        0      137 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/schema/vectorstore.py
+-rw-r--r--   0        0        0      130 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/serpapi.py
+-rw-r--r--   0        0        0     3544 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/smith/__init__.py
+-rw-r--r--   0        0        0     2199 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/smith/evaluation/__init__.py
+-rw-r--r--   0        0        0    12480 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/smith/evaluation/config.py
+-rw-r--r--   0        0        0     9936 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/smith/evaluation/name_generation.py
+-rw-r--r--   0        0        0     3306 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/smith/evaluation/progress.py
+-rw-r--r--   0        0        0    50978 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/smith/evaluation/runner_utils.py
+-rw-r--r--   0        0        0    17107 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/smith/evaluation/string_run_evaluator.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/smith/evaluation/utils.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.785760 langchain-0.1.9/langchain/sql_database.py
+-rw-r--r--   0        0        0     1571 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/storage/__init__.py
+-rw-r--r--   0        0        0     2517 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/storage/_lc_store.py
+-rw-r--r--   0        0        0     2970 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/storage/encoder_backed.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/storage/exceptions.py
+-rw-r--r--   0        0        0     4307 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/storage/file_system.py
+-rw-r--r--   0        0        0     4448 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/storage/in_memory.py
+-rw-r--r--   0        0        0       83 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/storage/redis.py
+-rw-r--r--   0        0        0      166 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/storage/upstash_redis.py
+-rw-r--r--   0        0        0    55865 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/text_splitter.py
+-rw-r--r--   0        0        0     5663 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/__init__.py
+-rw-r--r--   0        0        0      166 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/ainetwork/app.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/ainetwork/base.py
+-rw-r--r--   0        0        0      119 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/ainetwork/owner.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/ainetwork/rule.py
+-rw-r--r--   0        0        0      130 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/ainetwork/transfer.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/ainetwork/value.py
+-rw-r--r--   0        0        0      257 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/amadeus/base.py
+-rw-r--r--   0        0        0      180 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0      170 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0       25 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0      118 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/arxiv/tool.py
+-rw-r--r--   0        0        0      802 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0      156 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0      149 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0      149 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0      175 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/azure_cognitive_services/text_analytics_health.py
+-rw-r--r--   0        0        0      332 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/base.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/bearly/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/bearly/tool.py
+-rw-r--r--   0        0        0      170 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0      138 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0       95 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/brave_search/tool.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/clickup/__init__.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/clickup/tool.py
+-rw-r--r--   0        0        0      157 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      268 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0      197 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      147 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0      269 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/e2b_data_analysis/__init__.py
+-rw-r--r--   0        0        0      240 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/e2b_data_analysis/tool.py
+-rw-r--r--   0        0        0     1024 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/__init__.py
+-rw-r--r--   0        0        0      127 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/audio_speech_to_text.py
+-rw-r--r--   0        0        0      127 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/audio_text_to_speech.py
+-rw-r--r--   0        0        0       99 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/edenai_base_tool.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/image_explicitcontent.py
+-rw-r--r--   0        0        0      143 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/image_objectdetection.py
+-rw-r--r--   0        0        0      119 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/ocr_identityparser.py
+-rw-r--r--   0        0        0      128 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/ocr_invoiceparser.py
+-rw-r--r--   0        0        0      126 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/edenai/text_moderation.py
+-rw-r--r--   0        0        0      164 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/eleven_labs/__init__.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/eleven_labs/models.py
+-rw-r--r--   0        0        0      138 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/eleven_labs/text2speech.py
+-rw-r--r--   0        0        0      723 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/file_management/__init__.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/file_management/copy.py
+-rw-r--r--   0        0        0      155 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/file_management/delete.py
+-rw-r--r--   0        0        0      160 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/file_management/file_search.py
+-rw-r--r--   0        0        0      175 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/file_management/move.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/file_management/read.py
+-rw-r--r--   0        0        0      150 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/file_management/write.py
+-rw-r--r--   0        0        0       20 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/github/__init__.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/github/tool.py
+-rw-r--r--   0        0        0       20 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gitlab/__init__.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gitlab/tool.py
+-rw-r--r--   0        0        0      500 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gmail/__init__.py
+-rw-r--r--   0        0        0       92 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gmail/base.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0      154 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gmail/get_message.py
+-rw-r--r--   0        0        0      136 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0      167 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gmail/search.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/gmail/send_message.py
+-rw-r--r--   0        0        0      136 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      171 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_cloud/__init__.py
+-rw-r--r--   0        0        0      151 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_cloud/texttospeech.py
+-rw-r--r--   0        0        0      152 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_finance/__init__.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_finance/tool.py
+-rw-r--r--   0        0        0      140 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_jobs/__init__.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_jobs/tool.py
+-rw-r--r--   0        0        0      140 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_lens/__init__.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_lens/tool.py
+-rw-r--r--   0        0        0      140 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_places/__init__.py
+-rw-r--r--   0        0        0      161 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_places/tool.py
+-rw-r--r--   0        0        0      152 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_scholar/__init__.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_scholar/tool.py
+-rw-r--r--   0        0        0      195 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      161 2024-02-23 05:45:53.789760 langchain-0.1.9/langchain/tools/google_search/tool.py
+-rw-r--r--   0        0        0      243 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0      161 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/google_serper/tool.py
+-rw-r--r--   0        0        0      148 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/google_trends/__init__.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/google_trends/tool.py
+-rw-r--r--   0        0        0       47 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/graphql/__init__.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/graphql/tool.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/human/__init__.py
+-rw-r--r--   0        0        0       92 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/human/tool.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/jira/__init__.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/json/__init__.py
+-rw-r--r--   0        0        0      174 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/json/tool.py
+-rw-r--r--   0        0        0      134 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/memorize/__init__.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/memorize/tool.py
+-rw-r--r--   0        0        0       35 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/merriam_webster/__init__.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/merriam_webster/tool.py
+-rw-r--r--   0        0        0      154 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0      118 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0      359 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/multion/__init__.py
+-rw-r--r--   0        0        0      170 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/multion/close_session.py
+-rw-r--r--   0        0        0      175 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/multion/create_session.py
+-rw-r--r--   0        0        0      175 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/multion/update_session.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/nasa/__init__.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/nasa/tool.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0      135 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/nuclia/tool.py
+-rw-r--r--   0        0        0      567 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/office365/__init__.py
+-rw-r--r--   0        0        0       94 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/office365/base.py
+-rw-r--r--   0        0        0      197 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0      164 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/office365/events_search.py
+-rw-r--r--   0        0        0      166 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/office365/messages_search.py
+-rw-r--r--   0        0        0      151 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/office365/send_event.py
+-rw-r--r--   0        0        0      161 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/office365/send_message.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0      542 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      191 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      162 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      119 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0      763 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/__init__.py
+-rw-r--r--   0        0        0      110 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/base.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/click.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/current_page.py
+-rw-r--r--   0        0        0      198 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0      168 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0      152 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/navigate.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0      214 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/plugin.py
+-rw-r--r--   0        0        0       52 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0      189 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0       95 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/pubmed/tool.py
+-rw-r--r--   0        0        0      512 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/python/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/reddit_search/__init__.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/reddit_search/tool.py
+-rw-r--r--   0        0        0     1581 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/render.py
+-rw-r--r--   0        0        0       52 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/requests/__init__.py
+-rw-r--r--   0        0        0      349 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/requests/tool.py
+-rw-r--r--   0        0        0     2494 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/retriever.py
+-rw-r--r--   0        0        0       31 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0      140 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0      214 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/searchapi/__init__.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/searchapi/tool.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0      156 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/searx_search/tool.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/shell/__init__.py
+-rw-r--r--   0        0        0      123 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/shell/tool.py
+-rw-r--r--   0        0        0      433 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/slack/__init__.py
+-rw-r--r--   0        0        0       92 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/slack/base.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/slack/get_channel.py
+-rw-r--r--   0        0        0      164 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/slack/get_message.py
+-rw-r--r--   0        0        0      179 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/slack/schedule_message.py
+-rw-r--r--   0        0        0      159 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/slack/send_message.py
+-rw-r--r--   0        0        0       18 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/sleep/__init__.py
+-rw-r--r--   0        0        0      110 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0      304 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0      337 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/sql_database/tool.py
+-rw-r--r--   0        0        0       33 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/stackexchange/__init__.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/stackexchange/tool.py
+-rw-r--r--   0        0        0       24 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/steam/__init__.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/steam/tool.py
+-rw-r--r--   0        0        0      186 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0      180 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0      189 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/tavily_search/__init__.py
+-rw-r--r--   0        0        0      187 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/tavily_search/tool.py
+-rw-r--r--   0        0        0       51 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0      192 2024-02-23 05:45:53.793760 langchain-0.1.9/langchain/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       29 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      156 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0      114 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/yahoo_finance_news.py
+-rw-r--r--   0        0        0        0 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/youtube/__init__.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/youtube/search.py
+-rw-r--r--   0        0        0      193 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/zapier/__init__.py
+-rw-r--r--   0        0        0      162 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/tools/zapier/tool.py
+-rw-r--r--   0        0        0     2327 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/__init__.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/alpha_vantage.py
+-rw-r--r--   0        0        0      193 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/anthropic.py
+-rw-r--r--   0        0        0       89 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/apify.py
+-rw-r--r--   0        0        0      361 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/arcee.py
+-rw-r--r--   0        0        0       95 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/arxiv.py
+-rw-r--r--   0        0        0      274 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/asyncio.py
+-rw-r--r--   0        0        0       95 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/awslambda.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/bibtex.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/bing_search.py
+-rw-r--r--   0        0        0      108 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/brave_search.py
+-rw-r--r--   0        0        0      269 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/clickup.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/dalle_image_generator.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0      129 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/github.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/gitlab.py
+-rw-r--r--   0        0        0      123 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/golden_query.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/google_finance.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/google_jobs.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/google_lens.py
+-rw-r--r--   0        0        0      121 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/google_places_api.py
+-rw-r--r--   0        0        0      120 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/google_scholar.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/google_search.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/google_serper.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/google_trends.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/graphql.py
+-rw-r--r--   0        0        0       92 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/jira.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/loading.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/max_compute.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/merriam_webster.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/metaphor_search.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/nasa.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/opaqueprompts.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/openapi.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/openweathermap.py
+-rw-r--r--   0        0        0      110 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/outline.py
+-rw-r--r--   0        0        0       81 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/portkey.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/powerbi.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/pubmed.py
+-rw-r--r--   0        0        0       86 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/python.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/reddit_search.py
+-rw-r--r--   0        0        0      201 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/redis.py
+-rw-r--r--   0        0        0      181 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/requests.py
+-rw-r--r--   0        0        0      113 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/scenexplain.py
+-rw-r--r--   0        0        0      107 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/searchapi.py
+-rw-r--r--   0        0        0      151 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/searx_search.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/serpapi.py
+-rw-r--r--   0        0        0       85 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/spark_sql.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/sql_database.py
+-rw-r--r--   0        0        0      119 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/stackexchange.py
+-rw-r--r--   0        0        0      101 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/steam.py
+-rw-r--r--   0        0        0      126 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/tavily_search.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/tensorflow_datasets.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/twilio.py
+-rw-r--r--   0        0        0      276 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/vertexai.py
+-rw-r--r--   0        0        0      116 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/wikipedia.py
+-rw-r--r--   0        0        0      117 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0       98 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utilities/zapier.py
+-rw-r--r--   0        0        0     1221 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/__init__.py
+-rw-r--r--   0        0        0      102 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/aiter.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/env.py
+-rw-r--r--   0        0        0      325 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/ernie_functions.py
+-rw-r--r--   0        0        0       91 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/formatting.py
+-rw-r--r--   0        0        0      421 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/html.py
+-rw-r--r--   0        0        0      211 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/input.py
+-rw-r--r--   0        0        0      139 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/interactive_env.py
+-rw-r--r--   0        0        0      133 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/iter.py
+-rw-r--r--   0        0        0      258 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/json_schema.py
+-rw-r--r--   0        0        0       92 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/loading.py
+-rw-r--r--   0        0        0      181 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/math.py
+-rw-r--r--   0        0        0       86 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/openai.py
+-rw-r--r--   0        0        0      330 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/openai_functions.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/pydantic.py
+-rw-r--r--   0        0        0      148 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/strings.py
+-rw-r--r--   0        0        0      446 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/utils/utils.py
+-rw-r--r--   0        0        0     2768 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/__init__.py
+-rw-r--r--   0        0        0      220 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/annoy.py
+-rw-r--r--   0        0        0      100 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/astradb.py
+-rw-r--r--   0        0        0       82 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/atlas.py
+-rw-r--r--   0        0        0       78 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/awadb.py
+-rw-r--r--   0        0        0      256 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/azure_cosmos_db.py
+-rw-r--r--   0        0        0      188 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0       89 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/bageldb.py
+-rw-r--r--   0        0        0      115 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/baiducloud_vector_search.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/base.py
+-rw-r--r--   0        0        0      104 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/cassandra.py
+-rw-r--r--   0        0        0       90 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/chroma.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/clarifai.py
+-rw-r--r--   0        0        0      148 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0       93 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/dashvector.py
+-rw-r--r--   0        0        0      140 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/databricks_vector_search.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/deeplake.py
+-rw-r--r--   0        0        0       78 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/dingo.py
+-rw-r--r--   0        0        0      236 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0      111 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0      112 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0      125 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0      184 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0      362 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/elasticsearch.py
+-rw-r--r--   0        0        0       84 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/epsilla.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/faiss.py
+-rw-r--r--   0        0        0       78 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/hippo.py
+-rw-r--r--   0        0        0       96 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/hologres.py
+-rw-r--r--   0        0        0       84 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/lancedb.py
+-rw-r--r--   0        0        0      128 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/llm_rails.py
+-rw-r--r--   0        0        0       78 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/marqo.py
+-rw-r--r--   0        0        0      106 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0       96 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0       81 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/milvus.py
+-rw-r--r--   0        0        0      128 2024-02-23 05:45:53.797760 langchain-0.1.9/langchain/vectorstores/momento_vector_index.py
+-rw-r--r--   0        0        0      192 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0      179 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/myscale.py
+-rw-r--r--   0        0        0      147 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/neo4j_vector.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/nucliadb.py
+-rw-r--r--   0        0        0      147 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0      234 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0       93 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/pgvecto_rs.py
+-rw-r--r--   0        0        0      149 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/pgvector.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/pinecone.py
+-rw-r--r--   0        0        0      130 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/qdrant.py
+-rw-r--r--   0        0        0      265 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/redis/__init__.py
+-rw-r--r--   0        0        0      213 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/redis/base.py
+-rw-r--r--   0        0        0      416 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/redis/filters.py
+-rw-r--r--   0        0        0      503 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/redis/schema.py
+-rw-r--r--   0        0        0       86 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0       87 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/scann.py
+-rw-r--r--   0        0        0       81 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/semadb.py
+-rw-r--r--   0        0        0      165 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0      364 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/sklearn.py
+-rw-r--r--   0        0        0       90 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/sqlitevss.py
+-rw-r--r--   0        0        0      154 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/starrocks.py
+-rw-r--r--   0        0        0      109 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/supabase.py
+-rw-r--r--   0        0        0       75 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/tair.py
+-rw-r--r--   0        0        0      191 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/tencentvectordb.py
+-rw-r--r--   0        0        0       81 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/tigris.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/tiledb.py
+-rw-r--r--   0        0        0      124 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/timescalevector.py
+-rw-r--r--   0        0        0       90 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/typesense.py
+-rw-r--r--   0        0        0       84 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/usearch.py
+-rw-r--r--   0        0        0      227 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/utils.py
+-rw-r--r--   0        0        0       75 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/vald.py
+-rw-r--r--   0        0        0       81 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/vearch.py
+-rw-r--r--   0        0        0      122 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/vectara.py
+-rw-r--r--   0        0        0       88 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/vespa.py
+-rw-r--r--   0        0        0      103 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/weaviate.py
+-rw-r--r--   0        0        0       97 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/xata.py
+-rw-r--r--   0        0        0       96 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/yellowbrick.py
+-rw-r--r--   0        0        0      132 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/zep.py
+-rw-r--r--   0        0        0       81 2024-02-23 05:45:53.801760 langchain-0.1.9/langchain/vectorstores/zilliz.py
+-rw-r--r--   0        0        0    11689 2024-02-23 05:45:53.801760 langchain-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    13949 1970-01-01 00:00:00.000000 langchain-0.1.9/PKG-INFO
```

### Comparing `langchain-0.1.8/LICENSE` & `langchain-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/README.md` & `langchain-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/__init__.py` & `langchain-0.1.9/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/_api/__init__.py` & `langchain-0.1.9/langchain/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/adapters/openai.py` & `langchain-0.1.9/langchain/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/__init__.py` & `langchain-0.1.9/langchain/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent.py` & `langchain-0.1.9/langchain/agents/agent.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_iterator.py` & `langchain-0.1.9/langchain/agents/agent_iterator.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/__init__.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/csv/__init__.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/github/toolkit.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/github/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/openapi/planner.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/openapi/planner.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/openapi/planner_prompt.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/openapi/planner_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/pandas/__init__.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/python/__init__.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/spark/__init__.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/vectorstore/base.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/vectorstore/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/vectorstore/prompt.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/vectorstore/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/vectorstore/toolkit.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/vectorstore/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_toolkits/xorbits/__init__.py` & `langchain-0.1.9/langchain/agents/agent_toolkits/xorbits/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/agent_types.py` & `langchain-0.1.9/langchain/agents/agent_types.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/chat/base.py` & `langchain-0.1.9/langchain/agents/chat/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/chat/output_parser.py` & `langchain-0.1.9/langchain/agents/chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/chat/prompt.py` & `langchain-0.1.9/langchain/agents/chat/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/conversational/base.py` & `langchain-0.1.9/langchain/agents/conversational/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/conversational/output_parser.py` & `langchain-0.1.9/langchain/agents/conversational/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/conversational/prompt.py` & `langchain-0.1.9/langchain/agents/conversational/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/conversational_chat/base.py` & `langchain-0.1.9/langchain/agents/conversational_chat/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/conversational_chat/output_parser.py` & `langchain-0.1.9/langchain/agents/conversational_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/conversational_chat/prompt.py` & `langchain-0.1.9/langchain/agents/conversational_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/format_scratchpad/__init__.py` & `langchain-0.1.9/langchain/agents/format_scratchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/format_scratchpad/log.py` & `langchain-0.1.9/langchain/agents/format_scratchpad/log.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/format_scratchpad/log_to_messages.py` & `langchain-0.1.9/langchain/agents/format_scratchpad/log_to_messages.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/format_scratchpad/openai_functions.py` & `langchain-0.1.9/langchain/agents/format_scratchpad/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/format_scratchpad/openai_tools.py` & `langchain-0.1.9/langchain/agents/format_scratchpad/openai_tools.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/format_scratchpad/xml.py` & `langchain-0.1.9/langchain/agents/format_scratchpad/xml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/initialize.py` & `langchain-0.1.9/langchain/agents/initialize.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/json_chat/base.py` & `langchain-0.1.9/langchain/agents/json_chat/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/json_chat/prompt.py` & `langchain-0.1.9/langchain/agents/json_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/load_tools.py` & `langchain-0.1.9/langchain/agents/load_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,18 @@
     "human": (_get_human_tool, ["prompt_func", "input_func"]),
     "awslambda": (
         _get_lambda_api,
         ["awslambda_tool_name", "awslambda_tool_description", "function_name"],
     ),
     "stackexchange": (_get_stackexchange, []),
     "sceneXplain": (_get_scenexplain, []),
-    "graphql": (_get_graphql_tool, ["graphql_endpoint", "custom_headers"]),
+    "graphql": (
+        _get_graphql_tool,
+        ["graphql_endpoint", "custom_headers", "fetch_schema_from_transport"],
+    ),
     "openweathermap-api": (_get_openweathermap, ["openweathermap_api_key"]),
     "dataforseo-api-search": (
         _get_dataforseo_api_search,
         ["api_login", "api_password", "aiosession"],
     ),
     "dataforseo-api-search-json": (
         _get_dataforseo_api_search_json,
```

### Comparing `langchain-0.1.8/langchain/agents/loading.py` & `langchain-0.1.9/langchain/agents/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/mrkl/base.py` & `langchain-0.1.9/langchain/agents/mrkl/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/mrkl/output_parser.py` & `langchain-0.1.9/langchain/agents/mrkl/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/mrkl/prompt.py` & `langchain-0.1.9/langchain/agents/mrkl/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/openai_assistant/base.py` & `langchain-0.1.9/langchain/agents/openai_assistant/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py` & `langchain-0.1.9/langchain/agents/openai_functions_agent/agent_token_buffer_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/openai_functions_agent/base.py` & `langchain-0.1.9/langchain/agents/openai_functions_agent/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/openai_functions_multi_agent/base.py` & `langchain-0.1.9/langchain/agents/openai_functions_multi_agent/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/openai_tools/base.py` & `langchain-0.1.9/langchain/agents/openai_tools/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/output_parsers/__init__.py` & `langchain-0.1.9/langchain/agents/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/output_parsers/json.py` & `langchain-0.1.9/langchain/agents/output_parsers/json.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/output_parsers/openai_functions.py` & `langchain-0.1.9/langchain/agents/output_parsers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/output_parsers/openai_tools.py` & `langchain-0.1.9/langchain/agents/output_parsers/openai_tools.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/output_parsers/react_json_single_input.py` & `langchain-0.1.9/langchain/agents/output_parsers/react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/output_parsers/react_single_input.py` & `langchain-0.1.9/langchain/agents/output_parsers/react_single_input.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/output_parsers/self_ask.py` & `langchain-0.1.9/langchain/agents/output_parsers/self_ask.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/output_parsers/xml.py` & `langchain-0.1.9/langchain/agents/output_parsers/xml.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/react/agent.py` & `langchain-0.1.9/langchain/agents/react/agent.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/react/base.py` & `langchain-0.1.9/langchain/agents/react/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/react/output_parser.py` & `langchain-0.1.9/langchain/agents/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/react/textworld_prompt.py` & `langchain-0.1.9/langchain/agents/react/textworld_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/react/wiki_prompt.py` & `langchain-0.1.9/langchain/agents/react/wiki_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/schema.py` & `langchain-0.1.9/langchain/agents/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/self_ask_with_search/base.py` & `langchain-0.1.9/langchain/agents/self_ask_with_search/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/self_ask_with_search/prompt.py` & `langchain-0.1.9/langchain/agents/self_ask_with_search/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/structured_chat/base.py` & `langchain-0.1.9/langchain/agents/structured_chat/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/structured_chat/output_parser.py` & `langchain-0.1.9/langchain/agents/structured_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/structured_chat/prompt.py` & `langchain-0.1.9/langchain/agents/structured_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/tools.py` & `langchain-0.1.9/langchain/agents/tools.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/types.py` & `langchain-0.1.9/langchain/agents/types.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/xml/base.py` & `langchain-0.1.9/langchain/agents/xml/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/agents/xml/prompt.py` & `langchain-0.1.9/langchain/agents/xml/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/cache.py` & `langchain-0.1.9/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/__init__.py` & `langchain-0.1.9/langchain/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/base.py` & `langchain-0.1.9/langchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/file.py` & `langchain-0.1.9/langchain/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/manager.py` & `langchain-0.1.9/langchain/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/streaming_aiter.py` & `langchain-0.1.9/langchain/callbacks/streaming_aiter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/streaming_aiter_final_only.py` & `langchain-0.1.9/langchain/callbacks/streaming_aiter_final_only.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/streaming_stdout_final_only.py` & `langchain-0.1.9/langchain/callbacks/streaming_stdout_final_only.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/streamlit/__init__.py` & `langchain-0.1.9/langchain/callbacks/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/tracers/__init__.py` & `langchain-0.1.9/langchain/callbacks/tracers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/callbacks/tracers/logging.py` & `langchain-0.1.9/langchain/callbacks/tracers/logging.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/__init__.py` & `langchain-0.1.9/langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/base.py` & `langchain-0.1.9/langchain/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/news_docs.py` & `langchain-0.1.9/langchain/chains/api/news_docs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/open_meteo_docs.py` & `langchain-0.1.9/langchain/chains/api/open_meteo_docs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/openapi/chain.py` & `langchain-0.1.9/langchain/chains/api/openapi/chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/openapi/prompts.py` & `langchain-0.1.9/langchain/chains/api/openapi/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/openapi/requests_chain.py` & `langchain-0.1.9/langchain/chains/api/openapi/requests_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/openapi/response_chain.py` & `langchain-0.1.9/langchain/chains/api/openapi/response_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/podcast_docs.py` & `langchain-0.1.9/langchain/chains/api/podcast_docs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/prompt.py` & `langchain-0.1.9/langchain/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/api/tmdb_docs.py` & `langchain-0.1.9/langchain/chains/api/tmdb_docs.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/base.py` & `langchain-0.1.9/langchain/chains/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,27 +16,22 @@
     CallbackManager,
     CallbackManagerForChainRun,
     Callbacks,
 )
 from langchain_core.load.dump import dumpd
 from langchain_core.memory import BaseMemory
 from langchain_core.outputs import RunInfo
-from langchain_core.pydantic_v1 import (
-    BaseModel,
-    Field,
-    create_model,
-    root_validator,
-    validator,
-)
+from langchain_core.pydantic_v1 import BaseModel, Field, root_validator, validator
 from langchain_core.runnables import (
     RunnableConfig,
     RunnableSerializable,
     ensure_config,
     run_in_executor,
 )
+from langchain_core.runnables.utils import create_model
 
 from langchain.schema import RUN_KEY
 
 logger = logging.getLogger(__name__)
 
 
 def _get_verbosity() -> bool:
```

### Comparing `langchain-0.1.8/langchain/chains/chat_vector_db/prompts.py` & `langchain-0.1.9/langchain/chains/chat_vector_db/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/combine_documents/base.py` & `langchain-0.1.9/langchain/chains/combine_documents/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain_core.documents import Document
 from langchain_core.prompts import BasePromptTemplate, PromptTemplate
-from langchain_core.pydantic_v1 import BaseModel, Field, create_model
+from langchain_core.pydantic_v1 import BaseModel, Field
 from langchain_core.runnables.config import RunnableConfig
+from langchain_core.runnables.utils import create_model
 
 from langchain.chains.base import Chain
 from langchain.text_splitter import RecursiveCharacterTextSplitter, TextSplitter
 
 DEFAULT_DOCUMENT_SEPARATOR = "\n\n"
 DOCUMENTS_KEY = "context"
 DEFAULT_DOCUMENT_PROMPT = PromptTemplate.from_template("{page_content}")
```

### Comparing `langchain-0.1.8/langchain/chains/combine_documents/map_reduce.py` & `langchain-0.1.9/langchain/chains/combine_documents/map_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Tuple, Type
 
 from langchain_core.callbacks import Callbacks
 from langchain_core.documents import Document
-from langchain_core.pydantic_v1 import BaseModel, Extra, create_model, root_validator
+from langchain_core.pydantic_v1 import BaseModel, Extra, root_validator
 from langchain_core.runnables.config import RunnableConfig
+from langchain_core.runnables.utils import create_model
 
 from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
 from langchain.chains.combine_documents.reduce import ReduceDocumentsChain
 from langchain.chains.llm import LLMChain
 
 
 class MapReduceDocumentsChain(BaseCombineDocumentsChain):
```

### Comparing `langchain-0.1.8/langchain/chains/combine_documents/map_rerank.py` & `langchain-0.1.9/langchain/chains/combine_documents/map_rerank.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union, cast
 
 from langchain_core.callbacks import Callbacks
 from langchain_core.documents import Document
-from langchain_core.pydantic_v1 import BaseModel, Extra, create_model, root_validator
+from langchain_core.pydantic_v1 import BaseModel, Extra, root_validator
 from langchain_core.runnables.config import RunnableConfig
+from langchain_core.runnables.utils import create_model
 
 from langchain.chains.combine_documents.base import BaseCombineDocumentsChain
 from langchain.chains.llm import LLMChain
 from langchain.output_parsers.regex import RegexParser
 
 
 class MapRerankDocumentsChain(BaseCombineDocumentsChain):
```

### Comparing `langchain-0.1.8/langchain/chains/combine_documents/reduce.py` & `langchain-0.1.9/langchain/chains/combine_documents/reduce.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/combine_documents/refine.py` & `langchain-0.1.9/langchain/chains/combine_documents/refine.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/combine_documents/stuff.py` & `langchain-0.1.9/langchain/chains/combine_documents/stuff.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/constitutional_ai/base.py` & `langchain-0.1.9/langchain/chains/constitutional_ai/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/constitutional_ai/principles.py` & `langchain-0.1.9/langchain/chains/constitutional_ai/principles.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/constitutional_ai/prompts.py` & `langchain-0.1.9/langchain/chains/constitutional_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/conversation/base.py` & `langchain-0.1.9/langchain/chains/conversation/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/conversation/memory.py` & `langchain-0.1.9/langchain/chains/conversation/memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/conversation/prompt.py` & `langchain-0.1.9/langchain/chains/conversation/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/conversational_retrieval/base.py` & `langchain-0.1.9/langchain/chains/conversational_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/conversational_retrieval/prompts.py` & `langchain-0.1.9/langchain/chains/conversational_retrieval/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/elasticsearch_database/base.py` & `langchain-0.1.9/langchain/chains/elasticsearch_database/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/elasticsearch_database/prompts.py` & `langchain-0.1.9/langchain/chains/elasticsearch_database/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/ernie_functions/base.py` & `langchain-0.1.9/langchain/chains/ernie_functions/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,39 +306,39 @@
 
     Returns:
         A runnable sequence that will pass the given function to the model when run.
 
     Example:
         .. code-block:: python
 
-                from typing import Optional
+            from typing import Optional
 
-                from langchain.chains.ernie_functions import create_structured_output_chain
-                from langchain_community.chat_models import ErnieBotChat
-                from langchain.prompts import ChatPromptTemplate
-                from langchain.pydantic_v1 import BaseModel, Field
-
-                class Dog(BaseModel):
-                    \"\"\"Identifying information about a dog.\"\"\"
-
-                    name: str = Field(..., description="The dog's name")
-                    color: str = Field(..., description="The dog's color")
-                    fav_food: Optional[str] = Field(None, description="The dog's favorite food")
-
-                llm = ErnieBotChat(model_name="ERNIE-Bot-4")
-                prompt = ChatPromptTemplate.from_messages(
-                    [
-                        ("user", "Use the given format to extract information from the following input: {input}"),
-                        ("assistant", "OK!"),
-                        ("user", "Tip: Make sure to answer in the correct format"),
-                    ]
-                )
-                chain = create_structured_output_chain(Dog, llm, prompt)
-                chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
-                # -> Dog(name="Harry", color="brown", fav_food="chicken")
+            from langchain.chains.ernie_functions import create_structured_output_chain
+            from langchain_community.chat_models import ErnieBotChat
+            from langchain.prompts import ChatPromptTemplate
+            from langchain.pydantic_v1 import BaseModel, Field
+
+            class Dog(BaseModel):
+                \"\"\"Identifying information about a dog.\"\"\"
+
+                name: str = Field(..., description="The dog's name")
+                color: str = Field(..., description="The dog's color")
+                fav_food: Optional[str] = Field(None, description="The dog's favorite food")
+
+            llm = ErnieBotChat(model_name="ERNIE-Bot-4")
+            prompt = ChatPromptTemplate.from_messages(
+                [
+                    ("user", "Use the given format to extract information from the following input: {input}"),
+                    ("assistant", "OK!"),
+                    ("user", "Tip: Make sure to answer in the correct format"),
+                ]
+            )
+            chain = create_structured_output_chain(Dog, llm, prompt)
+            chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
+            # -> Dog(name="Harry", color="brown", fav_food="chicken")
     """  # noqa: E501
     if isinstance(output_schema, dict):
         function: Any = {
             "name": "output_formatter",
             "description": (
                 "Output formatter. Should always be used to format your response to the"
                 " user."
```

### Comparing `langchain-0.1.8/langchain/chains/example_generator.py` & `langchain-0.1.9/langchain/chains/example_generator.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/flare/base.py` & `langchain-0.1.9/langchain/chains/flare/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/flare/prompts.py` & `langchain-0.1.9/langchain/chains/flare/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/arangodb.py` & `langchain-0.1.9/langchain/chains/graph_qa/arangodb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/base.py` & `langchain-0.1.9/langchain/chains/graph_qa/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/cypher.py` & `langchain-0.1.9/langchain/chains/graph_qa/cypher.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/cypher_utils.py` & `langchain-0.1.9/langchain/chains/graph_qa/cypher_utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/falkordb.py` & `langchain-0.1.9/langchain/chains/graph_qa/falkordb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/hugegraph.py` & `langchain-0.1.9/langchain/chains/graph_qa/hugegraph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/kuzu.py` & `langchain-0.1.9/langchain/chains/graph_qa/kuzu.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/nebulagraph.py` & `langchain-0.1.9/langchain/chains/graph_qa/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/neptune_cypher.py` & `langchain-0.1.9/langchain/chains/graph_qa/neptune_cypher.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/neptune_sparql.py` & `langchain-0.1.9/langchain/chains/graph_qa/neptune_sparql.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/ontotext_graphdb.py` & `langchain-0.1.9/langchain/chains/graph_qa/ontotext_graphdb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/prompts.py` & `langchain-0.1.9/langchain/chains/graph_qa/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/graph_qa/sparql.py` & `langchain-0.1.9/langchain/chains/graph_qa/sparql.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,23 +37,33 @@
     """
 
     graph: RdfGraph = Field(exclude=True)
     sparql_generation_select_chain: LLMChain
     sparql_generation_update_chain: LLMChain
     sparql_intent_chain: LLMChain
     qa_chain: LLMChain
+    return_sparql_query: bool = False
     input_key: str = "query"  #: :meta private:
     output_key: str = "result"  #: :meta private:
+    sparql_query_key: str = "sparql_query"  #: :meta private:
 
     @property
     def input_keys(self) -> List[str]:
+        """Return the input keys.
+
+        :meta private:
+        """
         return [self.input_key]
 
     @property
     def output_keys(self) -> List[str]:
+        """Return the output keys.
+
+        :meta private:
+        """
         _output_keys = [self.output_key]
         return _output_keys
 
     @classmethod
     def from_llm(
         cls,
         llm: BaseLanguageModel,
@@ -131,8 +141,12 @@
             )
             res = result[self.qa_chain.output_key]
         elif intent == "UPDATE":
             self.graph.update(generated_sparql)
             res = "Successfully inserted triples into the graph."
         else:
             raise ValueError("Unsupported SPARQL query type.")
-        return {self.output_key: res}
+
+        chain_result: Dict[str, Any] = {self.output_key: res}
+        if self.return_sparql_query:
+            chain_result[self.sparql_query_key] = generated_sparql
+        return chain_result
```

### Comparing `langchain-0.1.8/langchain/chains/history_aware_retriever.py` & `langchain-0.1.9/langchain/chains/history_aware_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/hyde/base.py` & `langchain-0.1.9/langchain/chains/hyde/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/hyde/prompts.py` & `langchain-0.1.9/langchain/chains/hyde/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/llm.py` & `langchain-0.1.9/langchain/chains/llm.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/llm_checker/base.py` & `langchain-0.1.9/langchain/chains/llm_checker/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/llm_checker/prompt.py` & `langchain-0.1.9/langchain/chains/llm_checker/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/llm_math/base.py` & `langchain-0.1.9/langchain/chains/llm_math/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/llm_math/prompt.py` & `langchain-0.1.9/langchain/chains/llm_math/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/llm_requests.py` & `langchain-0.1.9/langchain/chains/llm_requests.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/llm_summarization_checker/base.py` & `langchain-0.1.9/langchain/chains/llm_summarization_checker/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt` & `langchain-0.1.9/langchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/loading.py` & `langchain-0.1.9/langchain/chains/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/mapreduce.py` & `langchain-0.1.9/langchain/chains/mapreduce.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/moderation.py` & `langchain-0.1.9/langchain/chains/moderation.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/natbot/base.py` & `langchain-0.1.9/langchain/chains/natbot/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/natbot/crawler.py` & `langchain-0.1.9/langchain/chains/natbot/crawler.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/natbot/prompt.py` & `langchain-0.1.9/langchain/chains/natbot/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_functions/__init__.py` & `langchain-0.1.9/langchain/chains/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_functions/base.py` & `langchain-0.1.9/langchain/chains/openai_functions/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_functions/citation_fuzzy_match.py` & `langchain-0.1.9/langchain/chains/openai_functions/citation_fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_functions/extraction.py` & `langchain-0.1.9/langchain/chains/openai_functions/extraction.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_functions/openapi.py` & `langchain-0.1.9/langchain/chains/openai_functions/openapi.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_functions/qa_with_structure.py` & `langchain-0.1.9/langchain/chains/openai_functions/qa_with_structure.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_functions/tagging.py` & `langchain-0.1.9/langchain/chains/openai_functions/tagging.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_functions/utils.py` & `langchain-0.1.9/langchain/chains/openai_functions/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/openai_tools/extraction.py` & `langchain-0.1.9/langchain/chains/openai_tools/extraction.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/prompt_selector.py` & `langchain-0.1.9/langchain/chains/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_generation/base.py` & `langchain-0.1.9/langchain/chains/qa_generation/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_generation/prompt.py` & `langchain-0.1.9/langchain/chains/qa_generation/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_with_sources/base.py` & `langchain-0.1.9/langchain/chains/qa_with_sources/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_with_sources/loading.py` & `langchain-0.1.9/langchain/chains/qa_with_sources/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_with_sources/map_reduce_prompt.py` & `langchain-0.1.9/langchain/chains/qa_with_sources/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_with_sources/refine_prompts.py` & `langchain-0.1.9/langchain/chains/qa_with_sources/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_with_sources/retrieval.py` & `langchain-0.1.9/langchain/chains/qa_with_sources/retrieval.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_with_sources/stuff_prompt.py` & `langchain-0.1.9/langchain/chains/qa_with_sources/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/qa_with_sources/vector_db.py` & `langchain-0.1.9/langchain/chains/qa_with_sources/vector_db.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/query_constructor/base.py` & `langchain-0.1.9/langchain/chains/query_constructor/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/query_constructor/ir.py` & `langchain-0.1.9/langchain/chains/query_constructor/ir.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/query_constructor/parser.py` & `langchain-0.1.9/langchain/chains/query_constructor/parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/query_constructor/prompt.py` & `langchain-0.1.9/langchain/chains/query_constructor/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/question_answering/__init__.py` & `langchain-0.1.9/langchain/chains/question_answering/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/question_answering/map_reduce_prompt.py` & `langchain-0.1.9/langchain/chains/question_answering/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/question_answering/map_rerank_prompt.py` & `langchain-0.1.9/langchain/chains/question_answering/map_rerank_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/question_answering/refine_prompts.py` & `langchain-0.1.9/langchain/chains/question_answering/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/question_answering/stuff_prompt.py` & `langchain-0.1.9/langchain/chains/question_answering/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/retrieval.py` & `langchain-0.1.9/langchain/chains/retrieval.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/retrieval_qa/base.py` & `langchain-0.1.9/langchain/chains/retrieval_qa/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/router/base.py` & `langchain-0.1.9/langchain/chains/router/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/router/embedding_router.py` & `langchain-0.1.9/langchain/chains/router/embedding_router.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/router/llm_router.py` & `langchain-0.1.9/langchain/chains/router/llm_router.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/router/multi_prompt.py` & `langchain-0.1.9/langchain/chains/router/multi_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/router/multi_prompt_prompt.py` & `langchain-0.1.9/langchain/chains/router/multi_prompt_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/router/multi_retrieval_prompt.py` & `langchain-0.1.9/langchain/chains/router/multi_retrieval_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/router/multi_retrieval_qa.py` & `langchain-0.1.9/langchain/chains/router/multi_retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/sequential.py` & `langchain-0.1.9/langchain/chains/sequential.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/sql_database/prompt.py` & `langchain-0.1.9/langchain/chains/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/sql_database/query.py` & `langchain-0.1.9/langchain/chains/sql_database/query.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/structured_output/base.py` & `langchain-0.1.9/langchain/chains/structured_output/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,32 +5,39 @@
     BaseGenerationOutputParser,
     BaseOutputParser,
     JsonOutputParser,
 )
 from langchain_core.prompts import BasePromptTemplate
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.runnables import Runnable
-from langchain_core.utils.function_calling import convert_to_openai_function
+from langchain_core.utils.function_calling import (
+    convert_to_openai_function,
+    convert_to_openai_tool,
+)
 
-from langchain.output_parsers import PydanticOutputParser
+from langchain.output_parsers import (
+    JsonOutputKeyToolsParser,
+    PydanticOutputParser,
+    PydanticToolsParser,
+)
 from langchain.output_parsers.openai_functions import (
     JsonOutputFunctionsParser,
     PydanticAttrOutputFunctionsParser,
     PydanticOutputFunctionsParser,
 )
 
 
 def create_openai_fn_runnable(
     functions: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable]],
     llm: Runnable,
     prompt: Optional[BasePromptTemplate] = None,
     *,
     enforce_single_function_usage: bool = True,
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
-    **kwargs: Any,
+    **llm_kwargs: Any,
 ) -> Runnable:
     """Create a runnable sequence that uses OpenAI functions.
 
     Args:
         functions: A sequence of either dictionaries, pydantic.BaseModels classes, or
             Python functions. If dictionaries are passed in, they are assumed to
             already be a valid OpenAI functions. If only a single
@@ -49,14 +56,15 @@
         output_parser: BaseLLMOutputParser to use for parsing model outputs. By default
             will be inferred from the function types. If pydantic.BaseModels are passed
             in, then the OutputParser will try to parse outputs using those. Otherwise
             model outputs will simply be parsed as JSON. If multiple functions are
             passed in and they are not pydantic.BaseModels, the chain output will
             include both the name of the function that was returned and the arguments
             to pass to the function.
+        **llm_kwargs: Additional named arguments to pass to the language model.
 
     Returns:
         A runnable sequence that will pass in the given functions to the model when run.
 
     Example:
         .. code-block:: python
 
@@ -87,33 +95,35 @@
                 structured_llm = create_openai_fn_runnable([RecordPerson, RecordDog], llm)
                 structured_llm.invoke("Harry was a chubby brown beagle who loved chicken)
                 # -> RecordDog(name="Harry", color="brown", fav_food="chicken")
     """  # noqa: E501
     if not functions:
         raise ValueError("Need to pass in at least one function. Received zero.")
     openai_functions = [convert_to_openai_function(f) for f in functions]
-    llm_kwargs: Dict[str, Any] = {"functions": openai_functions, **kwargs}
+    llm_kwargs_: Dict[str, Any] = {"functions": openai_functions, **llm_kwargs}
     if len(openai_functions) == 1 and enforce_single_function_usage:
-        llm_kwargs["function_call"] = {"name": openai_functions[0]["name"]}
+        llm_kwargs_["function_call"] = {"name": openai_functions[0]["name"]}
     output_parser = output_parser or get_openai_output_parser(functions)
     if prompt:
-        return prompt | llm.bind(**llm_kwargs) | output_parser
+        return prompt | llm.bind(**llm_kwargs_) | output_parser
     else:
-        return llm.bind(**llm_kwargs) | output_parser
+        return llm.bind(**llm_kwargs_) | output_parser
 
 
-# TODO: implement mode='openai-tools'.
 def create_structured_output_runnable(
     output_schema: Union[Dict[str, Any], Type[BaseModel]],
     llm: Runnable,
     prompt: Optional[BasePromptTemplate] = None,
     *,
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
-    mode: Literal["openai-functions", "openai-json"] = "openai-functions",
-    enforce_single_function_usage: bool = True,
+    enforce_function_usage: bool = True,
+    return_single: bool = True,
+    mode: Literal[
+        "openai-functions", "openai-tools", "openai-json"
+    ] = "openai-functions",
     **kwargs: Any,
 ) -> Runnable:
     """Create a runnable for extracting structured outputs.
 
     Args:
         output_schema: Either a dictionary or pydantic.BaseModel class. If a dictionary
             is passed in, it's assumed to already be a valid JsonSchema.
@@ -126,27 +136,115 @@
             prompt has input variable 'output_schema' then the given output_schema 
             will be converted to a JsonSchema and inserted in the prompt.
         output_parser: Output parser to use for parsing model outputs. By default
             will be inferred from the function types. If pydantic.BaseModel is passed
             in, then the OutputParser will try to parse outputs using the pydantic 
             class. Otherwise model outputs will be parsed as JSON.
         mode: How structured outputs are extracted from the model. If 'openai-functions' 
-            then OpenAI function calling is used. If 'openai-json' then OpenAI model 
+            then OpenAI function calling is used with the deprecated 'functions', 
+            'function_call' schema. If 'openai-tools' then OpenAI function 
+            calling with the latest 'tools', 'tool_choice' schema is used. This is 
+            recommended over 'openai-functions'. If 'openai-json' then OpenAI model 
             with response_format set to JSON is used.
-        enforce_single_function_usage: Only used if mode is 'openai-functions'. Only 
-            used if a single function is passed in. If
-            True, then the model will be forced to use the given function. If False,
-            then the model will be given the option to use the given function or not.
+        enforce_function_usage: Only applies when mode is 'openai-tools' or 
+            'openai-functions'. If True, then the model will be forced to use the given 
+            output schema. If False, then the model can elect whether to use the output 
+            schema.
+        return_single: Only applies when mode is 'openai-tools'. Whether to a list of 
+            structured outputs or a single one. If True and model does not return any 
+            structured outputs then chain output is None. If False and model does not 
+            return any structured outputs then chain output is an empty list.
         **kwargs: Additional named arguments.
 
     Returns:
-        A runnable sequence that will return a structured output matching the given 
+        A runnable sequence that will return a structured output(s) matching the given 
             output_schema.
+    
+    OpenAI tools example with Pydantic schema (mode='openai-tools'):
+        .. code-block:: python
+        
+                from typing import Optional
+
+                from langchain.chains import create_structured_output_runnable
+                from langchain_openai import ChatOpenAI
+                from langchain_core.pydantic_v1 import BaseModel, Field
+
+
+                class RecordDog(BaseModel):
+                    '''Record some identifying information about a dog.'''
+
+                    name: str = Field(..., description="The dog's name")
+                    color: str = Field(..., description="The dog's color")
+                    fav_food: Optional[str] = Field(None, description="The dog's favorite food")
+
+                llm = ChatOpenAI(model="gpt-3.5-turbo-0125", temperature=0)
+                prompt = ChatPromptTemplate.from_messages(
+                    [
+                        ("system", "You are an extraction algorithm. Please extract every possible instance"), 
+                        ('human', '{input}')
+                    ]
+                )
+                structured_llm = create_structured_output_runnable(
+                    RecordDog, 
+                    llm, 
+                    mode="openai-tools", 
+                    enforce_function_usage=True, 
+                    return_single=True
+                )
+                structured_llm.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
+                # -> RecordDog(name="Harry", color="brown", fav_food="chicken")
+                
+    OpenAI tools example with dict schema (mode="openai-tools"):
+        .. code-block:: python
+        
+                from typing import Optional
+
+                from langchain.chains import create_structured_output_runnable
+                from langchain_openai import ChatOpenAI
 
-    OpenAI functions example:
+
+                dog_schema = {
+                    "type": "function",
+                    "function": {
+                        "name": "record_dog",
+                        "description": "Record some identifying information about a dog.",
+                        "parameters": {
+                            "type": "object",
+                            "properties": {
+                                "name": {
+                                    "description": "The dog's name",
+                                    "type": "string"
+                                },
+                                "color": {
+                                    "description": "The dog's color",
+                                    "type": "string"
+                                },
+                                "fav_food": {
+                                    "description": "The dog's favorite food",
+                                    "type": "string"
+                                }
+                            },
+                            "required": ["name", "color"]
+                        }
+                    }
+                }
+
+
+                llm = ChatOpenAI(model="gpt-3.5-turbo-0125", temperature=0)
+                structured_llm = create_structured_output_runnable(
+                    doc_schema, 
+                    llm, 
+                    mode="openai-tools", 
+                    enforce_function_usage=True, 
+                    return_single=True
+                )
+                structured_llm.invoke("Harry was a chubby brown beagle who loved chicken")
+                # -> {'name': 'Harry', 'color': 'brown', 'fav_food': 'chicken'}
+    
+    OpenAI functions example (mode="openai-functions"):
         .. code-block:: python
 
                 from typing import Optional
 
                 from langchain.chains import create_structured_output_runnable
                 from langchain_openai import ChatOpenAI
                 from langchain_core.pydantic_v1 import BaseModel, Field
@@ -185,15 +283,15 @@
                 system = '''Extract information about any dogs mentioned in the user input.'''
                 prompt = ChatPromptTemplate.from_messages(
                     [("system", system), ("human", "{input}"),]
                 )
                 chain = prompt | structured_llm
                 chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
                 # -> Dog(name="Harry", color="brown", fav_food="chicken")
-    OpenAI json response format example:
+    OpenAI json response format example (mode="openai-json"):
         .. code-block:: python
         
                 from typing import Optional
 
                 from langchain.chains import create_structured_output_runnable
                 from langchain_openai import ChatOpenAI
                 from langchain_core.prompts import ChatPromptTemplate
@@ -215,34 +313,104 @@
                 {output_schema}'''
                 prompt = ChatPromptTemplate.from_messages(
                     [("system", system), ("human", "{input}"),]
                 )
                 chain = prompt | structured_llm
                 chain.invoke({"input": "Harry was a chubby brown beagle who loved chicken"})
     """  # noqa: E501
-    if mode == "openai-functions":
+    # for backwards compatibility
+    force_function_usage = kwargs.get(
+        "enforce_single_function_usage", enforce_function_usage
+    )
+
+    if mode == "openai-tools":
+        # Protect against typos in kwargs
+        keys_in_kwargs = set(kwargs.keys())
+        # Backwards compatibility keys
+        unrecognized_keys = keys_in_kwargs - {"enforce_single_function_usage"}
+        if unrecognized_keys:
+            raise TypeError(
+                f"Got an unexpected keyword argument(s): {unrecognized_keys}."
+            )
+
+        return _create_openai_tools_runnable(
+            output_schema,
+            llm,
+            prompt=prompt,
+            output_parser=output_parser,
+            enforce_tool_usage=force_function_usage,
+            first_tool_only=return_single,
+        )
+
+    elif mode == "openai-functions":
         return _create_openai_functions_structured_output_runnable(
             output_schema,
             llm,
             prompt=prompt,
             output_parser=output_parser,
-            enforce_single_function_usage=enforce_single_function_usage,
-            **kwargs,
+            enforce_single_function_usage=force_function_usage,
+            **kwargs,  # llm-specific kwargs
         )
     elif mode == "openai-json":
+        if force_function_usage:
+            raise ValueError(
+                "enforce_single_function_usage is not supported for mode='openai-json'."
+            )
         return _create_openai_json_runnable(
             output_schema, llm, prompt=prompt, output_parser=output_parser, **kwargs
         )
     else:
         raise ValueError(
-            f"Invalid mode {mode}. Expected one of 'openai-functions', "
+            f"Invalid mode {mode}. Expected one of 'openai-tools', 'openai-functions', "
             f"'openai-json'."
         )
 
 
+def _create_openai_tools_runnable(
+    tool: Union[Dict[str, Any], Type[BaseModel], Callable],
+    llm: Runnable,
+    *,
+    prompt: Optional[BasePromptTemplate],
+    output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]],
+    enforce_tool_usage: bool,
+    first_tool_only: bool,
+) -> Runnable:
+    oai_tool = convert_to_openai_tool(tool)
+    llm_kwargs: Dict[str, Any] = {"tools": [oai_tool]}
+    if enforce_tool_usage:
+        llm_kwargs["tool_choice"] = {
+            "type": "function",
+            "function": {"name": oai_tool["function"]["name"]},
+        }
+    output_parser = output_parser or _get_openai_tool_output_parser(
+        tool, first_tool_only=first_tool_only
+    )
+    if prompt:
+        return prompt | llm.bind(**llm_kwargs) | output_parser
+    else:
+        return llm.bind(**llm_kwargs) | output_parser
+
+
+def _get_openai_tool_output_parser(
+    tool: Union[Dict[str, Any], Type[BaseModel], Callable],
+    *,
+    first_tool_only: bool = False,
+) -> Union[BaseOutputParser, BaseGenerationOutputParser]:
+    if isinstance(tool, type) and issubclass(tool, BaseModel):
+        output_parser: Union[
+            BaseOutputParser, BaseGenerationOutputParser
+        ] = PydanticToolsParser(tools=[tool], first_tool_only=first_tool_only)
+    else:
+        key_name = convert_to_openai_tool(tool)["function"]["name"]
+        output_parser = JsonOutputKeyToolsParser(
+            first_tool_only=first_tool_only, key_name=key_name
+        )
+    return output_parser
+
+
 def get_openai_output_parser(
     functions: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable]],
 ) -> Union[BaseOutputParser, BaseGenerationOutputParser]:
     """Get the appropriate function output parser given the user functions.
 
     Args:
         functions: Sequence where element is a dictionary, a pydantic.BaseModel class,
@@ -251,19 +419,18 @@
 
     Returns:
         A PydanticOutputFunctionsParser if functions are Pydantic classes, otherwise
             a JsonOutputFunctionsParser. If there's only one function and it is
             not a Pydantic class, then the output parser will automatically extract
             only the function arguments and not the function name.
     """
-    function_names = [convert_to_openai_function(f)["name"] for f in functions]
     if isinstance(functions[0], type) and issubclass(functions[0], BaseModel):
         if len(functions) > 1:
             pydantic_schema: Union[Dict, Type[BaseModel]] = {
-                name: fn for name, fn in zip(function_names, functions)
+                convert_to_openai_function(fn)["name"]: fn for fn in functions
             }
         else:
             pydantic_schema = functions[0]
         output_parser: Union[
             BaseOutputParser, BaseGenerationOutputParser
         ] = PydanticOutputFunctionsParser(pydantic_schema=pydantic_schema)
     else:
@@ -300,15 +467,15 @@
 
 def _create_openai_functions_structured_output_runnable(
     output_schema: Union[Dict[str, Any], Type[BaseModel]],
     llm: Runnable,
     prompt: Optional[BasePromptTemplate] = None,
     *,
     output_parser: Optional[Union[BaseOutputParser, BaseGenerationOutputParser]] = None,
-    **kwargs: Any,
+    **llm_kwargs: Any,
 ) -> Runnable:
     if isinstance(output_schema, dict):
         function: Any = {
             "name": "output_formatter",
             "description": (
                 "Output formatter. Should always be used to format your response to the"
                 " user."
@@ -327,9 +494,9 @@
             pydantic_schema=_OutputFormatter, attr_name="output"
         )
     return create_openai_fn_runnable(
         [function],
         llm,
         prompt=prompt,
         output_parser=output_parser,
-        **kwargs,
+        **llm_kwargs,
     )
```

### Comparing `langchain-0.1.8/langchain/chains/summarize/__init__.py` & `langchain-0.1.9/langchain/chains/summarize/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/summarize/refine_prompts.py` & `langchain-0.1.9/langchain/chains/summarize/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chains/transform.py` & `langchain-0.1.9/langchain/chains/transform.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/chat_models/__init__.py` & `langchain-0.1.9/langchain/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/docstore/__init__.py` & `langchain-0.1.9/langchain/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/document_loaders/__init__.py` & `langchain-0.1.9/langchain/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/document_loaders/airbyte.py` & `langchain-0.1.9/langchain/document_loaders/airbyte.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/document_loaders/parsers/__init__.py` & `langchain-0.1.9/langchain/document_loaders/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/document_loaders/pdf.py` & `langchain-0.1.9/langchain/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/document_loaders/unstructured.py` & `langchain-0.1.9/langchain/document_loaders/unstructured.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/document_transformers/__init__.py` & `langchain-0.1.9/langchain/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/document_transformers/xsl/html_chunks_with_headers.xslt` & `langchain-0.1.9/langchain/document_transformers/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/embeddings/__init__.py` & `langchain-0.1.9/langchain/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/embeddings/cache.py` & `langchain-0.1.9/langchain/embeddings/cache.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/__init__.py` & `langchain-0.1.9/langchain/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/agents/trajectory_eval_chain.py` & `langchain-0.1.9/langchain/evaluation/agents/trajectory_eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/agents/trajectory_eval_prompt.py` & `langchain-0.1.9/langchain/evaluation/agents/trajectory_eval_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/comparison/__init__.py` & `langchain-0.1.9/langchain/evaluation/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/comparison/eval_chain.py` & `langchain-0.1.9/langchain/evaluation/comparison/eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/comparison/prompt.py` & `langchain-0.1.9/langchain/evaluation/comparison/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/criteria/__init__.py` & `langchain-0.1.9/langchain/evaluation/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/criteria/eval_chain.py` & `langchain-0.1.9/langchain/evaluation/criteria/eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/criteria/prompt.py` & `langchain-0.1.9/langchain/evaluation/criteria/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/embedding_distance/base.py` & `langchain-0.1.9/langchain/evaluation/embedding_distance/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/exact_match/base.py` & `langchain-0.1.9/langchain/evaluation/exact_match/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/loading.py` & `langchain-0.1.9/langchain/evaluation/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/parsing/base.py` & `langchain-0.1.9/langchain/evaluation/parsing/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/parsing/json_distance.py` & `langchain-0.1.9/langchain/evaluation/parsing/json_distance.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/parsing/json_schema.py` & `langchain-0.1.9/langchain/evaluation/parsing/json_schema.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/qa/eval_chain.py` & `langchain-0.1.9/langchain/evaluation/qa/eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/qa/eval_prompt.py` & `langchain-0.1.9/langchain/evaluation/qa/eval_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/qa/generate_chain.py` & `langchain-0.1.9/langchain/evaluation/qa/generate_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/qa/generate_prompt.py` & `langchain-0.1.9/langchain/evaluation/qa/generate_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/regex_match/base.py` & `langchain-0.1.9/langchain/evaluation/regex_match/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/schema.py` & `langchain-0.1.9/langchain/evaluation/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/scoring/__init__.py` & `langchain-0.1.9/langchain/evaluation/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/scoring/eval_chain.py` & `langchain-0.1.9/langchain/evaluation/scoring/eval_chain.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/scoring/prompt.py` & `langchain-0.1.9/langchain/evaluation/scoring/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/evaluation/string_distance/base.py` & `langchain-0.1.9/langchain/evaluation/string_distance/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/globals/__init__.py` & `langchain-0.1.9/langchain/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/graphs/__init__.py` & `langchain-0.1.9/langchain/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/hub.py` & `langchain-0.1.9/langchain/hub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/indexes/__init__.py` & `langchain-0.1.9/langchain/indexes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-"""Code to support various indexing workflows.
+"""**Index** is used to avoid writing duplicated content
+into the vectostore and to avoid over-writing content if it's unchanged.
 
-Provides code to:
+Indexes also :
 
 * Create knowledge graphs from data.
 
 * Support indexing workflows from LangChain data loaders to vectorstores.
 
-For indexing workflows, this code is used to avoid writing duplicated content
-into the vectostore and to avoid over-writing content if it's unchanged.
-
-Importantly, this keeps on working even if the content being written is derived
+Importantly, Index keeps on working even if the content being written is derived
 via a set of transformations from some source content (e.g., indexing children
 documents that were derived from parent documents by chunking.)
 """
 from langchain.indexes._api import IndexingResult, aindex, index
 from langchain.indexes._sql_record_manager import SQLRecordManager
 from langchain.indexes.graph import GraphIndexCreator
 from langchain.indexes.vectorstore import VectorstoreIndexCreator
```

### Comparing `langchain-0.1.8/langchain/indexes/_api.py` & `langchain-0.1.9/langchain/indexes/_api.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/indexes/_sql_record_manager.py` & `langchain-0.1.9/langchain/indexes/_sql_record_manager.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/indexes/base.py` & `langchain-0.1.9/langchain/indexes/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/indexes/graph.py` & `langchain-0.1.9/langchain/indexes/graph.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/indexes/prompts/entity_extraction.py` & `langchain-0.1.9/langchain/indexes/prompts/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/indexes/prompts/entity_summarization.py` & `langchain-0.1.9/langchain/indexes/prompts/entity_summarization.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/indexes/prompts/knowledge_triplet_extraction.py` & `langchain-0.1.9/langchain/indexes/prompts/knowledge_triplet_extraction.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/indexes/vectorstore.py` & `langchain-0.1.9/langchain/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/llms/__init__.py` & `langchain-0.1.9/langchain/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/llms/grammars/json.gbnf` & `langchain-0.1.9/langchain/llms/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/__init__.py` & `langchain-0.1.9/langchain/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/buffer.py` & `langchain-0.1.9/langchain/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/buffer_window.py` & `langchain-0.1.9/langchain/memory/buffer_window.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/chat_memory.py` & `langchain-0.1.9/langchain/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/chat_message_histories/__init__.py` & `langchain-0.1.9/langchain/memory/chat_message_histories/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/combined.py` & `langchain-0.1.9/langchain/memory/combined.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/entity.py` & `langchain-0.1.9/langchain/memory/entity.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/kg.py` & `langchain-0.1.9/langchain/memory/kg.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/motorhead_memory.py` & `langchain-0.1.9/langchain/memory/motorhead_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/prompt.py` & `langchain-0.1.9/langchain/memory/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/readonly.py` & `langchain-0.1.9/langchain/memory/readonly.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/simple.py` & `langchain-0.1.9/langchain/memory/simple.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/summary.py` & `langchain-0.1.9/langchain/memory/summary.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/summary_buffer.py` & `langchain-0.1.9/langchain/memory/summary_buffer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/token_buffer.py` & `langchain-0.1.9/langchain/memory/token_buffer.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/utils.py` & `langchain-0.1.9/langchain/memory/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/vectorstore.py` & `langchain-0.1.9/langchain/memory/vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/memory/zep_memory.py` & `langchain-0.1.9/langchain/memory/zep_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/model_laboratory.py` & `langchain-0.1.9/langchain/model_laboratory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/__init__.py` & `langchain-0.1.9/langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/boolean.py` & `langchain-0.1.9/langchain/output_parsers/boolean.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/combining.py` & `langchain-0.1.9/langchain/output_parsers/combining.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/datetime.py` & `langchain-0.1.9/langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/enum.py` & `langchain-0.1.9/langchain/output_parsers/enum.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/fix.py` & `langchain-0.1.9/langchain/output_parsers/fix.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/format_instructions.py` & `langchain-0.1.9/langchain/output_parsers/format_instructions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/loading.py` & `langchain-0.1.9/langchain/output_parsers/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/openai_functions.py` & `langchain-0.1.9/langchain/output_parsers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/pandas_dataframe.py` & `langchain-0.1.9/langchain/output_parsers/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/pydantic.py` & `langchain-0.1.9/langchain/output_parsers/yaml.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 import json
-from typing import Any, List, Type
+import re
+from typing import Type, TypeVar
 
+import yaml
 from langchain_core.exceptions import OutputParserException
-from langchain_core.output_parsers import JsonOutputParser
-from langchain_core.outputs import Generation
+from langchain_core.output_parsers import BaseOutputParser
 from langchain_core.pydantic_v1 import BaseModel, ValidationError
 
-from langchain.output_parsers.format_instructions import PYDANTIC_FORMAT_INSTRUCTIONS
+from langchain.output_parsers.format_instructions import YAML_FORMAT_INSTRUCTIONS
 
+T = TypeVar("T", bound=BaseModel)
 
-class PydanticOutputParser(JsonOutputParser):
-    """Parse an output using a pydantic model."""
 
-    pydantic_object: Type[BaseModel]
-    """The pydantic model to parse.
-    
-    Attention: To avoid potential compatibility issues, it's recommended to use
-        pydantic <2 or leverage the v1 namespace in pydantic >= 2.
-    """
+class YamlOutputParser(BaseOutputParser[T]):
+    """Parse YAML output using a pydantic model."""
 
-    def parse_result(self, result: List[Generation], *, partial: bool = False) -> Any:
-        json_object = super().parse_result(result)
+    pydantic_object: Type[T]
+    """The pydantic model to parse."""
+    pattern: re.Pattern = re.compile(
+        r"^```(?:ya?ml)?(?P<yaml>[^`]*)", re.MULTILINE | re.DOTALL
+    )
+    """Regex pattern to match yaml code blocks 
+    within triple backticks with optional yaml or yml prefix."""
+
+    def parse(self, text: str) -> T:
         try:
+            # Greedy search for 1st yaml candidate.
+            match = re.search(self.pattern, text.strip())
+            yaml_str = ""
+            if match:
+                yaml_str = match.group("yaml")
+            else:
+                # If no backticks were present, try to parse the entire output as yaml.
+                yaml_str = text
+
+            json_object = yaml.safe_load(yaml_str)
             return self.pydantic_object.parse_obj(json_object)
-        except ValidationError as e:
+
+        except (yaml.YAMLError, ValidationError) as e:
             name = self.pydantic_object.__name__
-            msg = f"Failed to parse {name} from completion {json_object}. Got: {e}"
-            raise OutputParserException(msg, llm_output=json_object)
+            msg = f"Failed to parse {name} from completion {text}. Got: {e}"
+            raise OutputParserException(msg, llm_output=text) from e
 
     def get_format_instructions(self) -> str:
         # Copy schema to avoid altering original Pydantic schema.
         schema = {k: v for k, v in self.pydantic_object.schema().items()}
 
         # Remove extraneous fields.
         reduced_schema = schema
         if "title" in reduced_schema:
             del reduced_schema["title"]
         if "type" in reduced_schema:
             del reduced_schema["type"]
-        # Ensure json in context is well-formed with double quotes.
+        # Ensure yaml in context is well-formed with double quotes.
         schema_str = json.dumps(reduced_schema)
 
-        return PYDANTIC_FORMAT_INSTRUCTIONS.format(schema=schema_str)
+        return YAML_FORMAT_INSTRUCTIONS.format(schema=schema_str)
 
     @property
     def _type(self) -> str:
-        return "pydantic"
-
-    @property
-    def OutputType(self) -> Type[BaseModel]:
-        """Return the pydantic model."""
-        return self.pydantic_object
+        return "yaml"
```

### Comparing `langchain-0.1.8/langchain/output_parsers/regex.py` & `langchain-0.1.9/langchain/output_parsers/regex.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/regex_dict.py` & `langchain-0.1.9/langchain/output_parsers/regex_dict.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/retry.py` & `langchain-0.1.9/langchain/output_parsers/retry.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/output_parsers/structured.py` & `langchain-0.1.9/langchain/output_parsers/structured.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/prompts/__init__.py` & `langchain-0.1.9/langchain/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/prompts/base.py` & `langchain-0.1.9/langchain/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/prompts/chat.py` & `langchain-0.1.9/langchain/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/prompts/example_selector/__init__.py` & `langchain-0.1.9/langchain/prompts/example_selector/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/prompts/loading.py` & `langchain-0.1.9/langchain/prompts/loading.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/pydantic_v1/__init__.py` & `langchain-0.1.9/langchain/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/__init__.py` & `langchain-0.1.9/langchain/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/contextual_compression.py` & `langchain-0.1.9/langchain/retrievers/contextual_compression.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/document_compressors/__init__.py` & `langchain-0.1.9/langchain/retrievers/document_compressors/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/document_compressors/base.py` & `langchain-0.1.9/langchain/retrievers/document_compressors/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/document_compressors/chain_extract.py` & `langchain-0.1.9/langchain/retrievers/document_compressors/chain_extract.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/document_compressors/chain_filter.py` & `langchain-0.1.9/langchain/retrievers/document_compressors/chain_filter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/document_compressors/cohere_rerank.py` & `langchain-0.1.9/langchain/retrievers/document_compressors/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/document_compressors/embeddings_filter.py` & `langchain-0.1.9/langchain/retrievers/document_compressors/embeddings_filter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/document_compressors/flashrank_rerank.py` & `langchain-0.1.9/langchain/retrievers/document_compressors/flashrank_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/ensemble.py` & `langchain-0.1.9/langchain/retrievers/ensemble.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/kendra.py` & `langchain-0.1.9/langchain/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/merger_retriever.py` & `langchain-0.1.9/langchain/retrievers/merger_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/multi_query.py` & `langchain-0.1.9/langchain/retrievers/multi_query.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/multi_vector.py` & `langchain-0.1.9/langchain/retrievers/multi_vector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/parent_document_retriever.py` & `langchain-0.1.9/langchain/retrievers/parent_document_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/re_phraser.py` & `langchain-0.1.9/langchain/retrievers/re_phraser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/astradb.py` & `langchain-0.1.9/langchain/retrievers/self_query/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/base.py` & `langchain-0.1.9/langchain/retrievers/self_query/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,23 +72,32 @@
         ElasticsearchStore: ElasticsearchTranslator,
         Milvus: MilvusTranslator,
         SupabaseVectorStore: SupabaseVectorTranslator,
         TimescaleVector: TimescaleVectorTranslator,
         OpenSearchVectorSearch: OpenSearchTranslator,
         MongoDBAtlasVectorSearch: MongoDBAtlasTranslator,
     }
+
     if isinstance(vectorstore, Qdrant):
         return QdrantTranslator(metadata_key=vectorstore.metadata_payload_key)
     elif isinstance(vectorstore, MyScale):
         return MyScaleTranslator(metadata_key=vectorstore.metadata_column)
     elif isinstance(vectorstore, Redis):
         return RedisTranslator.from_vectorstore(vectorstore)
     elif vectorstore.__class__ in BUILTIN_TRANSLATORS:
         return BUILTIN_TRANSLATORS[vectorstore.__class__]()
     else:
+        try:
+            from langchain_astradb.vectorstores import AstraDBVectorStore
+
+            if isinstance(vectorstore, AstraDBVectorStore):
+                return AstraDBTranslator()
+        except ImportError:
+            pass
+
         raise ValueError(
             f"Self query retriever with Vector Store type {vectorstore.__class__}"
             f" not supported."
         )
 
 
 class SelfQueryRetriever(BaseRetriever):
```

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/chroma.py` & `langchain-0.1.9/langchain/retrievers/self_query/chroma.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/dashvector.py` & `langchain-0.1.9/langchain/retrievers/self_query/dashvector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/deeplake.py` & `langchain-0.1.9/langchain/retrievers/self_query/deeplake.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/elasticsearch.py` & `langchain-0.1.9/langchain/retrievers/self_query/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/milvus.py` & `langchain-0.1.9/langchain/retrievers/self_query/milvus.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/mongodb_atlas.py` & `langchain-0.1.9/langchain/retrievers/self_query/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/myscale.py` & `langchain-0.1.9/langchain/retrievers/self_query/myscale.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/opensearch.py` & `langchain-0.1.9/langchain/retrievers/self_query/opensearch.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/pgvector.py` & `langchain-0.1.9/langchain/retrievers/self_query/pgvector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/pinecone.py` & `langchain-0.1.9/langchain/retrievers/self_query/pinecone.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/qdrant.py` & `langchain-0.1.9/langchain/retrievers/self_query/qdrant.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/redis.py` & `langchain-0.1.9/langchain/retrievers/self_query/redis.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/supabase.py` & `langchain-0.1.9/langchain/retrievers/self_query/supabase.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/timescalevector.py` & `langchain-0.1.9/langchain/retrievers/self_query/timescalevector.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/vectara.py` & `langchain-0.1.9/langchain/retrievers/self_query/vectara.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/self_query/weaviate.py` & `langchain-0.1.9/langchain/retrievers/self_query/weaviate.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/time_weighted_retriever.py` & `langchain-0.1.9/langchain/retrievers/time_weighted_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/retrievers/web_research.py` & `langchain-0.1.9/langchain/retrievers/web_research.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/runnables/hub.py` & `langchain-0.1.9/langchain/runnables/hub.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/runnables/openai_functions.py` & `langchain-0.1.9/langchain/runnables/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/schema/__init__.py` & `langchain-0.1.9/langchain/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/schema/callbacks/manager.py` & `langchain-0.1.9/langchain/schema/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/schema/messages.py` & `langchain-0.1.9/langchain/schema/messages.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/schema/output_parser.py` & `langchain-0.1.9/langchain/schema/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/schema/runnable/__init__.py` & `langchain-0.1.9/langchain/schema/runnable/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/schema/runnable/base.py` & `langchain-0.1.9/langchain/schema/runnable/base.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/schema/runnable/config.py` & `langchain-0.1.9/langchain/schema/runnable/config.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/schema/runnable/utils.py` & `langchain-0.1.9/langchain/schema/runnable/utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/smith/__init__.py` & `langchain-0.1.9/langchain/smith/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/smith/evaluation/__init__.py` & `langchain-0.1.9/langchain/smith/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/smith/evaluation/config.py` & `langchain-0.1.9/langchain/smith/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/smith/evaluation/name_generation.py` & `langchain-0.1.9/langchain/smith/evaluation/name_generation.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/smith/evaluation/progress.py` & `langchain-0.1.9/langchain/smith/evaluation/progress.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/smith/evaluation/runner_utils.py` & `langchain-0.1.9/langchain/smith/evaluation/runner_utils.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/smith/evaluation/string_run_evaluator.py` & `langchain-0.1.9/langchain/smith/evaluation/string_run_evaluator.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/storage/__init__.py` & `langchain-0.1.9/langchain/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/storage/_lc_store.py` & `langchain-0.1.9/langchain/storage/_lc_store.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/storage/encoder_backed.py` & `langchain-0.1.9/langchain/storage/encoder_backed.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/storage/file_system.py` & `langchain-0.1.9/langchain/storage/file_system.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/storage/in_memory.py` & `langchain-0.1.9/langchain/storage/in_memory.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/text_splitter.py` & `langchain-0.1.9/langchain/text_splitter.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/__init__.py` & `langchain-0.1.9/langchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/azure_cognitive_services/__init__.py` & `langchain-0.1.9/langchain/tools/azure_cognitive_services/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/edenai/__init__.py` & `langchain-0.1.9/langchain/tools/edenai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/file_management/__init__.py` & `langchain-0.1.9/langchain/tools/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/office365/__init__.py` & `langchain-0.1.9/langchain/tools/office365/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/openapi/utils/api_models.py` & `langchain-0.1.9/langchain/tools/openapi/utils/api_models.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/playwright/__init__.py` & `langchain-0.1.9/langchain/tools/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/python/__init__.py` & `langchain-0.1.9/langchain/tools/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/render.py` & `langchain-0.1.9/langchain/tools/render.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/tools/retriever.py` & `langchain-0.1.9/langchain/tools/retriever.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/utilities/__init__.py` & `langchain-0.1.9/langchain/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/utils/__init__.py` & `langchain-0.1.9/langchain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/langchain/vectorstores/__init__.py` & `langchain-0.1.9/langchain/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain-0.1.8/pyproject.toml` & `langchain-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain"
-version = "0.1.8"
+version = "0.1.9"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 
 [tool.poetry.scripts]
 langchain-server = "langchain.server:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = ">=0.1.24,<0.2"
+langchain-core = ">=0.1.26,<0.2"
 langchain-community = ">=0.0.21,<0.1"
 langsmith = "^0.1.0"
 pydantic = ">=1,<3"
 SQLAlchemy = ">=1.4,<3"
 requests = "^2"
 PyYAML = ">=5.3"
 numpy = "^1"
```

### Comparing `langchain-0.1.8/PKG-INFO` & `langchain-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain
-Version: 0.1.8
+Version: 0.1.9
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -68,15 +68,15 @@
 Requires-Dist: huggingface_hub (>=0,<1) ; extra == "llms"
 Requires-Dist: javelin-sdk (>=0.1.8,<0.2.0) ; extra == "extended-testing"
 Requires-Dist: jinja2 (>=3,<4) ; extra == "extended-testing"
 Requires-Dist: jq (>=1.4.1,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: jsonpatch (>=1.33,<2.0)
 Requires-Dist: jsonschema (>1) ; extra == "extended-testing"
 Requires-Dist: langchain-community (>=0.0.21,<0.1)
-Requires-Dist: langchain-core (>=0.1.24,<0.2)
+Requires-Dist: langchain-core (>=0.1.26,<0.2)
 Requires-Dist: langchain-openai (>=0.0.2,<0.1) ; extra == "extended-testing"
 Requires-Dist: langsmith (>=0.1.0,<0.2.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0) ; extra == "extended-testing"
 Requires-Dist: manifest-ml (>=0.0.1,<0.0.2) ; extra == "llms"
 Requires-Dist: markdownify (>=0.11.6,<0.12.0) ; extra == "extended-testing"
 Requires-Dist: motor (>=3.3.1,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: msal (>=1.25.0,<2.0.0) ; extra == "extended-testing"
```

