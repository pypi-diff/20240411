# Comparing `tmp/komodo_sdk-0.0.90.tar.gz` & `tmp/komodo_sdk-0.0.91.tar.gz`

## Comparing `komodo_sdk-0.0.90.tar` & `komodo_sdk-0.0.91.tar`

### file list

```diff
@@ -1,441 +1,443 @@
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/.dockerignore
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/requirements.txt
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/.github/workflows/deploy-all.yml
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/.github/workflows/publish-container.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/README.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/config.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/chatdoc_agent.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/collection_builder.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/coordinator_agent.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/default.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/difference_agent.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/echo_agent.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/elastic_agent.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/groot_agent.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/librarian_agent.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/mongo_agent.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/pdf_generator.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/sample_agent.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/summarizer_agent.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/translator_agent.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/agents/widget_builder_agent.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/sources/filesystem.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/sources/s3bucketkey.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/sources/webpages.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/sources/website_crawler.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/elastic/elastic_connect.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/elastic/elastic_count.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/elastic/elastic_get.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/elastic/elastic_search.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/files/collection_builder.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/files/collection_lister.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/files/collection_reader.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/files/directory_reader.py
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/files/file_reader.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/files/file_writer.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/markets/polygon_search.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_connect.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_databases.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_query.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_schema.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_unique.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/search/vector_search.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/search/vector_search_runtime.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/utils/agent_tool.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/utils/sample_tool.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/utils/thought_tool.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/utils/workflow_tool.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/web/data_fetcher.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/web/serpapi_search.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/web/tavily_search.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/tools/web/web_scraper.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/utils/agent_helper.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/utils/indexer.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/utils/play.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/utils/rag_context.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/vector_stores/pinecone_store.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/vector_stores/qdrant_store.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/vector_stores/vector_store_helper.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/core/workflows/sample_workflow.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/data/agents/planner/personal_finance_profile.yml
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/data/appliances/citibank/personal_finance_profile.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/data/appliances/komodo/dir1/hello.txt
--rw-r--r--   0        0        0  1139092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/data/workflows/analyzer/personal_finance_profile.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/checker/agent.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/checker/context.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/checker/dictionary.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/checker/instructions.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/planner/agent.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/planner/context.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/planner/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/planner/instructions.txt
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/planner/role.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/planner/tools/income_calculator.yml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/planner/tools/income_contributions.yml
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/appliances/citibank/appliance.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/appliances/komodo/appliance.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/appliances/sample/appliance.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/appliances/sample/context.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/appliances/sample/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/appliances/sample/instructions.txt
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/workflows/analyzer/context.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/workflows/analyzer/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/workflows/analyzer/instructions.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/definitions/workflows/analyzer/workflow.yml
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_agent.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_app.py
--rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_collection.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_config.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_context.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_datasource.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_features.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_locations.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_runnable.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_runtime.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_tool.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_tool_registry.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_user.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_vector.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_vectorstore.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/framework/komodo_workflow.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/database/agent_loader.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/database/appliance_loader.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/database/tool_loader.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/database/user_loader.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/filesystem/agent_loader.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/filesystem/appliance_loader.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/filesystem/loader_helper.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/filesystem/loader_locations.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/loaders/filesystem/workflow_loader.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/azure/azure.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/azure/azure_openai.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/bedrock/bedrock.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/bedrock/bedrock_claude.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/bedrock/bedrock_cohere.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/bedrock/bedrock_model.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/bedrock/bedrock_titan.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/agent_runner.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/appliance_utils.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/chat_message.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/chat_metadata.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/model_request.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/model_response.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/models.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/responder.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/workflow_executor.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/workflow_runner.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/framework/workflow_selector.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/openai/openai_api.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/openai/openai_api_streamed.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/openai/openai_api_streamed_tool_call.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/openai/openai_completion.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/openai/openai_debug.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/models/openai/openai_process_actions.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/collection.proto
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/data.proto
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/model.proto
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/report.proto
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/sample.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/generated/collection_pb2.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/generated/collection_pb2.pyi
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/generated/data_pb2.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/generated/data_pb2.pyi
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/generated/model_pb2.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/generated/model_pb2.pyi
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/generated/report_pb2.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/proto/generated/report_pb2.pyi
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/scripts/run_agent_runner.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/scripts/run_agent_runner_2.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/scripts/run_difference_agent.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/scripts/run_librarian_agent.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/scripts/run_sample_agent.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/scripts/run_streaming_test.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/scripts/run_widget_builder.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/agent_router.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/appliance_router.py
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/ask_request.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/audio_router.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/collections_router.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/conversation_router.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/fast.py
--rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/globals.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/logo_router.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/report_router.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/server/user_router.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/directory/assistants_helpers.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/documents/file_writer_helper.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/documents/text_convert_helper.py
--rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/documents/text_extract.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/documents/text_extract_helper.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/documents/text_html.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/embeddings/faiss_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/embeddings/openai.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/embeddings/pinecone_store.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/mssql/mssql.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/api_query.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/digest.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/filestats.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/globber.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/hidden_prints.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/lambda_entry.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/lambda_utils.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/logconfig.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/pathutils.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/s3_file_utils.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/sentry_utils.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/switchdir.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/tags.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/term_colors.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/timebox.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/shared/utils/watcher.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/agent_store.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/appliance_store.py
--rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/collection_store.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/conversations_store.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/logo_store.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/proto_utils.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/redis_database.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/tool_store.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/store/user_store.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/core/test_elastic_agent.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/core/test_elastic_sample.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/core/test_elastic_tools.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/core/test_groot_agent.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/core/test_mongo_agent.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/core/test_mongo_sample.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/core/test_mongo_tools.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/core/test_serpapi_search.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/models/test_azure.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/models/test_bedrock.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/models/test_openai.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/models/test_workflow_runner.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/shared/test_mssql.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/komodo/tests/store/test_conversation_store.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/pdf2html/Dockerfile
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/pdf2html/docker-compose.yml
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/pdf2html/server.py
--rw-r--r--   0        0        0   480357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/pdf2html/data/sample.html
--rw-r--r--   0        0        0   599041 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/pdf2html/data/sample.pdf
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/Dockerfile
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/README.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/docker-compose.yml
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/docker-production.yml
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/appliance/appliance.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/appliance/config.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/appliance/seed.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/appliance/server.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/appliance/workflow.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/definitions/agents/dasher_v1/agent.yml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/definitions/agents/dasher_v1/instructions.txt
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/definitions/agents/dasher_v2/agent.yml
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/definitions/agents/dasher_v2/instructions.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/definitions/appliances/sample/appliance.yml
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/app.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/globals.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/server.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/themes.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/assets/custom.css
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/agent.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/analytics.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/appliance.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/archive.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/dasher_v1.py
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/dasher_v2.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/department.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/home.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/not_found_404.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/present.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/report.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/side_bar.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/topic_1.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/reports/bar_chart.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/reports/line_chart.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/sample/widgets/pages/reports/pie_chart.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/.gitignore
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/Dockerfile
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/README.md
--rw-r--r--   0        0        0   953941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/package-lock.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/package.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/tailwind.config.js
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/deployment/nginx.default.conf
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/chaticon.png
--rw-r--r--   0        0        0    66364 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/faqbg.png
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/favicon.ico
--rw-r--r--   0        0        0    84772 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/footer.png
--rw-r--r--   0        0        0   230014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/home.png
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/index.html
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/logo192.png
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/logo512.png
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/manifest.json
--rw-r--r--   0        0        0   318284 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/pricingBg.png
--rw-r--r--   0        0        0   189260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/pricingBg1.png
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/robots.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Read Me.txt
--rw-r--r--   0        0        0    84336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf
--rw-r--r--   0        0        0   291948 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf
--rw-r--r--   0        0        0    80288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf
--rw-r--r--   0        0        0   275104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf
--rw-r--r--   0        0        0    85092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf
--rw-r--r--   0        0        0   291180 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf
--rw-r--r--   0        0        0    80172 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf
--rw-r--r--   0        0        0   273580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf
--rw-r--r--   0        0        0    82008 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf
--rw-r--r--   0        0        0   418296 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf
--rw-r--r--   0        0        0    78624 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf
--rw-r--r--   0        0        0   411148 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf
--rw-r--r--   0        0        0    81940 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf
--rw-r--r--   0        0        0   279500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf
--rw-r--r--   0        0        0    78360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf
--rw-r--r--   0        0        0   257728 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf
--rw-r--r--   0        0        0    78480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf
--rw-r--r--   0        0        0   313920 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf
--rw-r--r--   0        0        0    82916 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf
--rw-r--r--   0        0        0   367128 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf
--rw-r--r--   0        0        0    79536 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf
--rw-r--r--   0        0        0   349188 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf
--rw-r--r--   0        0        0    83092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf
--rw-r--r--   0        0        0   309704 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf
--rw-r--r--   0        0        0    79480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf
--rw-r--r--   0        0        0   291444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf
--rw-r--r--   0        0        0    81828 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf
--rw-r--r--   0        0        0   331432 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf
--rw-r--r--   0        0        0    83560 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf
--rw-r--r--   0        0        0   301516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf
--rw-r--r--   0        0        0    79800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf
--rw-r--r--   0        0        0   283064 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    79864 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf
--rw-r--r--   0        0        0   459400 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf
--rw-r--r--   0        0        0    77840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf
--rw-r--r--   0        0        0   455000 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/App.css
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/App.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/App.test.js
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/RouterMain.js
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/index.css
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/index.js
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/logo.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/reportWebVitals.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/setupTests.js
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/API/API_data.js
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/API/ApiComment.js
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/Frame.svg
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/ai.png
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/arrowLeft.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/aubergine.png
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/barbra.svg
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/blue.svg
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/blueTick.svg
--rw-r--r--   0        0        0  1709204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/botAvatar.svg
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/chatListIcon.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/clementine.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/close.svg
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/docs.svg
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/docx.png
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/folder.svg
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/gallery.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/gray.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/green.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/grey.svg
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/headphone.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/indigo.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/jade.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/lagoon.svg
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/magicpen-1.svg
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/magicpen.svg
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/message.svg
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/multi.png
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/odt.png
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/orange.png
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/parrot.svg
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/pdf.png
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/pdf.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/pink.svg
--rw-r--r--   0        0        0   378813 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/pricingBg.png
--rw-r--r--   0        0        0    48909 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/profile.png
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/send.png
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/setting-1.svg
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/setting.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/sky.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/square.svg
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/text.png
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/text.svg
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/trash.svg
--rw-r--r--   0        0        0  1884519 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/userProfile.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/assets/yellow.svg
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/auth/Login.js
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/auth/Signup.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/DocumentView.js
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/Header.js
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/HeaderSideBar.js
--rw-r--r--   0        0        0    20984 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/Home.jsx
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/LayoutHeader.js
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/NavigateBack.js
--rw-r--r--   0        0        0    30197 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/Sidebar.js
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/DocumentBox/Table.js
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/chat/Chat.js
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/chat/Details.js
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/chat/EnhancedPrompt.js
--rw-r--r--   0        0        0    14804 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/chatBot/Chat.js
--rw-r--r--   0        0        0    16338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/chatBot/ChatBotById.js
--rw-r--r--   0        0        0    63153 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/chatBot/ChatBotSideBar.js
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/chatBot/EnhancedBot.js
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/document/DocumentSidebar.js
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/helpers/Toast.js
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/components/inputs/CustomInputs.jsx
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/contexts/roleContext.js
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/helpers/Toast.js
--rw-r--r--   0        0        0    33366 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/Ellipsis.gif
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/chat.png
--rw-r--r--   0        0        0   214322 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/chatgpt.png
--rw-r--r--   0        0        0   101078 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/chatimg.png
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/chattick.png
--rw-r--r--   0        0        0    21789 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/content.png
--rw-r--r--   0        0        0    53673 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/copy.png
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/doc.png
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/docprofile.png
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/docwave.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/dots.png
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/dummy.txt
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/first.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/homemenu.png
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/imgLogo.jpg
--rw-r--r--   0        0        0   371173 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/login.png
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/pdf.png
--rw-r--r--   0        0        0   177241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/person.png
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/portfolio.png
--rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/pptLogo.png
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/profile.png
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/robot.png
--rw-r--r--   0        0        0    96034 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/sample.pdf
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/second.png
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/send.png
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/setting.png
--rw-r--r--   0        0        0    61070 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/summary.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/tick.png
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/tik.png
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/txt.png
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/upload.png
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/upload2.png
--rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/user.png
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/wave.png
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/wave1.png
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/word.png
--rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/images/xlsxLogo.png
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/layout/CollectionLayout.js
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/layout/PrimaryLayout.js
--rw-r--r--   0        0        0    32712 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/Document.js
--rw-r--r--   0        0        0    42860 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/chatBot.js
--rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/chat/Chat.js
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/chat/Details.js
--rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/pricing/Pricing.jsx
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/privacy/Privacy.jsx
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/privacy/Terms.jsx
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/profile/Profile.jsx
--rw-r--r--   0        0        0    23023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/website/src/pages/settings/Settings.jsx
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/.gitignore
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/README.md
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/pyproject.toml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.90/PKG-INFO
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/.dockerignore
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/requirements.txt
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/.github/workflows/deploy-all.yml
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/.github/workflows/publish-container.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/README.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/config.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/chatdoc_agent.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/collection_builder.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/coordinator_agent.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/default.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/difference_agent.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/echo_agent.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/elastic_agent.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/groot_agent.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/librarian_agent.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/mongo_agent.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/pdf_generator.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/sample_agent.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/summarizer_agent.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/translator_agent.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/widget_builder_agent.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/sources/filesystem.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/sources/s3bucketkey.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/sources/webpages.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/sources/website_crawler.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_connect.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_count.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_get.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_search.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/collection_builder.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/collection_lister.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/collection_reader.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/directory_reader.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/file_reader.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/file_writer.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/markets/polygon_search.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_connect.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_databases.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_query.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_schema.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_unique.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/search/vector_search.py
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/search/vector_search_runtime.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/utils/agent_tool.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/utils/sample_tool.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/utils/thought_tool.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/utils/workflow_tool.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/web/data_fetcher.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/web/serpapi_search.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/web/tavily_search.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/web/web_scraper.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/utils/agent_helper.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/utils/indexer.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/utils/play.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/utils/rag_context.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/vector_stores/pinecone_store.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/vector_stores/qdrant_store.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/vector_stores/vector_store_helper.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/workflows/sample_workflow.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/agents/planner/personal_finance_profile.yml
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/appliances/citibank/personal_finance_profile.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/appliances/komodo/dir1/hello.txt
+-rw-r--r--   0        0        0  1139092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/workflows/analyzer/personal_finance_profile.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/checker/agent.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/checker/context.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/checker/dictionary.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/checker/instructions.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/agent.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/context.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/instructions.txt
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/role.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/tools/income_calculator.yml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/tools/income_contributions.yml
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/citibank/appliance.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/komodo/appliance.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/sample/appliance.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/sample/context.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/sample/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/sample/instructions.txt
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/context.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/instructions.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/workflow.yml
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_agent.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_app.py
+-rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_collection.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_config.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_context.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_datasource.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_features.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_locations.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_runnable.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_runtime.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_tool.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_tool_registry.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_user.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_vector.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_vectorstore.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_workflow.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/database/agent_loader.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/database/appliance_loader.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/database/tool_loader.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/database/user_loader.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/agent_loader.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/appliance_loader.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/loader_helper.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/loader_locations.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/workflow_loader.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/azure/azure.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/azure/azure_openai.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_claude.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_cohere.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_model.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_titan.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/agent_runner.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/appliance_utils.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/chat_message.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/chat_metadata.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/model_request.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/model_response.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/models.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/responder.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/workflow_executor.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/workflow_runner.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/workflow_selector.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_api.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_api_streamed.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_api_streamed_tool_call.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_completion.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_debug.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_process_actions.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/collection.proto
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/data.proto
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/model.proto
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/report.proto
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/sample.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/collection_pb2.py
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/collection_pb2.pyi
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/data_pb2.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/data_pb2.pyi
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/model_pb2.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/model_pb2.pyi
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/report_pb2.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/report_pb2.pyi
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_agent_runner.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_agent_runner_2.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_difference_agent.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_librarian_agent.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_sample_agent.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_streaming_test.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_widget_builder.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/agent_router.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/appliance_router.py
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/ask_request.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/audio_router.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/collections_router.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/conversation_router.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/fast.py
+-rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/globals.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/logo_router.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/report_router.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/user_router.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/directory/assistants_helpers.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/file_writer_helper.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/text_convert_helper.py
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/text_extract.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/text_extract_helper.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/text_html.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/embeddings/faiss_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/embeddings/openai.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/embeddings/pinecone_store.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/mssql/mssql.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/api_query.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/digest.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/filestats.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/globber.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/hidden_prints.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/lambda_entry.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/lambda_utils.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/logconfig.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/pathutils.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/s3_file_utils.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/sentry_utils.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/switchdir.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/tags.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/term_colors.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/timebox.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/watcher.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/agent_store.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/appliance_store.py
+-rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/collection_store.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/conversations_store.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/logo_store.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/proto_utils.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/redis_database.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/tool_store.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/user_store.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_elastic_agent.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_elastic_sample.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_elastic_tools.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_groot_agent.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_mongo_agent.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_mongo_sample.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_mongo_tools.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_serpapi_search.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/models/test_azure.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/models/test_bedrock.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/models/test_openai.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/models/test_workflow_runner.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/shared/test_mssql.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/store/test_conversation_store.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/Dockerfile
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/docker-compose.yml
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/server.py
+-rw-r--r--   0        0        0   480357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/data/sample.html
+-rw-r--r--   0        0        0   599041 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/data/sample.pdf
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/Dockerfile
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/README.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/docker-compose.yml
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/docker-production.yml
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/appliance.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/config.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/seed.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/server.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/workflow.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/agents/dasher_v1/agent.yml
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/agents/dasher_v1/instructions.txt
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/agents/dasher_v2/agent.yml
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/agents/dasher_v2/instructions.txt
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/appliances/sample/appliance.yml
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/app.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/globals.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/server.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/themes.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/assets/custom.css
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/agent.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/analytics.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/appliance.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/archive.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/dasher_v1.py
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/dasher_v2.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/department.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/home.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/not_found_404.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/present.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/report.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/side_bar.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/topic_1.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/reports/bar_chart.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/reports/line_chart.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/reports/pie_chart.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/Dockerfile
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/README.md
+-rw-r--r--   0        0        0   953941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/package-lock.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/package.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/tailwind.config.js
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/deployment/nginx.default.conf
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/chaticon.png
+-rw-r--r--   0        0        0    66364 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/faqbg.png
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/favicon.ico
+-rw-r--r--   0        0        0    84772 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/footer.png
+-rw-r--r--   0        0        0   230014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/home.png
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/index.html
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/logo192.png
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/logo512.png
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/manifest.json
+-rw-r--r--   0        0        0   318284 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/pricingBg.png
+-rw-r--r--   0        0        0   189260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/pricingBg1.png
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/robots.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Read Me.txt
+-rw-r--r--   0        0        0    84336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf
+-rw-r--r--   0        0        0   291948 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf
+-rw-r--r--   0        0        0    80288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf
+-rw-r--r--   0        0        0   275104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf
+-rw-r--r--   0        0        0    85092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf
+-rw-r--r--   0        0        0   291180 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf
+-rw-r--r--   0        0        0    80172 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf
+-rw-r--r--   0        0        0   273580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf
+-rw-r--r--   0        0        0    82008 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf
+-rw-r--r--   0        0        0   418296 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf
+-rw-r--r--   0        0        0    78624 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf
+-rw-r--r--   0        0        0   411148 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf
+-rw-r--r--   0        0        0    81940 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf
+-rw-r--r--   0        0        0   279500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf
+-rw-r--r--   0        0        0    78360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf
+-rw-r--r--   0        0        0   257728 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf
+-rw-r--r--   0        0        0    78480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf
+-rw-r--r--   0        0        0   313920 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf
+-rw-r--r--   0        0        0    82916 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf
+-rw-r--r--   0        0        0   367128 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf
+-rw-r--r--   0        0        0    79536 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf
+-rw-r--r--   0        0        0   349188 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf
+-rw-r--r--   0        0        0    83092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf
+-rw-r--r--   0        0        0   309704 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf
+-rw-r--r--   0        0        0    79480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf
+-rw-r--r--   0        0        0   291444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf
+-rw-r--r--   0        0        0    81828 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf
+-rw-r--r--   0        0        0   331432 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf
+-rw-r--r--   0        0        0    83560 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf
+-rw-r--r--   0        0        0   301516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf
+-rw-r--r--   0        0        0    79800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf
+-rw-r--r--   0        0        0   283064 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    79864 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf
+-rw-r--r--   0        0        0   459400 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf
+-rw-r--r--   0        0        0    77840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf
+-rw-r--r--   0        0        0   455000 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/App.css
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/App.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/App.test.js
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/RouterMain.js
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/index.css
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/index.js
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/logo.svg
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/reportWebVitals.js
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/setupTests.js
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/API/API_data.js
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/API/ApiComment.js
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/Frame.svg
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/ai.png
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/arrowLeft.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/aubergine.png
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/barbra.svg
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/blue.svg
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/blueTick.svg
+-rw-r--r--   0        0        0  1709204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/botAvatar.svg
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/chatListIcon.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/clementine.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/close.svg
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/docs.svg
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/docx.png
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/folder.svg
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/gallery.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/gray.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/green.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/grey.svg
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/headphone.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/indigo.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/jade.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/lagoon.svg
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/magicpen-1.svg
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/magicpen.svg
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/message.svg
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/multi.png
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/odt.png
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/orange.png
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/parrot.svg
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/pdf.png
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/pdf.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/pink.svg
+-rw-r--r--   0        0        0   378813 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/pricingBg.png
+-rw-r--r--   0        0        0    48909 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/profile.png
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/send.png
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/setting-1.svg
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/setting.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/sky.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/square.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/text.png
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/text.svg
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/trash.svg
+-rw-r--r--   0        0        0  1884519 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/userProfile.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/yellow.svg
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/auth/Login.js
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/auth/Signup.js
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/ChartDashboard.js
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/Dashboard.js
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/DocumentView.js
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/Header.js
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/HeaderSideBar.js
+-rw-r--r--   0        0        0    20984 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/Home.jsx
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/LayoutHeader.js
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/NavigateBack.js
+-rw-r--r--   0        0        0    36368 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/Sidebar.js
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/DocumentBox/Table.js
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chat/Chat.js
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chat/Details.js
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chat/EnhancedPrompt.js
+-rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chatBot/Chat.js
+-rw-r--r--   0        0        0    15498 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chatBot/ChatBotById.js
+-rw-r--r--   0        0        0    64401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chatBot/ChatBotSideBar.js
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chatBot/EnhancedBot.js
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/document/DocumentSidebar.js
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/helpers/Toast.js
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/inputs/CustomInputs.jsx
+-rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/contexts/roleContext.js
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/helpers/Toast.js
+-rw-r--r--   0        0        0    33366 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/Ellipsis.gif
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/chat.png
+-rw-r--r--   0        0        0   214322 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/chatgpt.png
+-rw-r--r--   0        0        0   101078 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/chatimg.png
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/chattick.png
+-rw-r--r--   0        0        0    21789 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/content.png
+-rw-r--r--   0        0        0    53673 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/copy.png
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/doc.png
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/docprofile.png
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/docwave.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/dots.png
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/dummy.txt
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/first.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/homemenu.png
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/imgLogo.jpg
+-rw-r--r--   0        0        0   371173 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/login.png
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/pdf.png
+-rw-r--r--   0        0        0   177241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/person.png
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/portfolio.png
+-rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/pptLogo.png
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/profile.png
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/robot.png
+-rw-r--r--   0        0        0    96034 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/sample.pdf
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/second.png
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/send.png
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/setting.png
+-rw-r--r--   0        0        0    61070 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/summary.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/tick.png
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/tik.png
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/txt.png
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/upload.png
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/upload2.png
+-rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/user.png
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/wave.png
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/wave1.png
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/word.png
+-rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/xlsxLogo.png
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/layout/CollectionLayout.js
+-rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/layout/PrimaryLayout.js
+-rw-r--r--   0        0        0    32803 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/Document.js
+-rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/chatBot.js
+-rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/chat/Chat.js
+-rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/chat/Details.js
+-rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/pricing/Pricing.jsx
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/privacy/Privacy.jsx
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/privacy/Terms.jsx
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/profile/Profile.jsx
+-rw-r--r--   0        0        0    23023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/settings/Settings.jsx
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/.gitignore
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/README.md
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pyproject.toml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/PKG-INFO
```

### Comparing `komodo_sdk-0.0.90/.dockerignore` & `komodo_sdk-0.0.91/.dockerignore`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/requirements.txt` & `komodo_sdk-0.0.91/requirements.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/.github/workflows/deploy-all.yml` & `komodo_sdk-0.0.91/.github/workflows/deploy-all.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/.github/workflows/publish-container.yml` & `komodo_sdk-0.0.91/.github/workflows/publish-container.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/README.md` & `komodo_sdk-0.0.91/komodo/README.md`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/config.py` & `komodo_sdk-0.0.91/komodo/config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/chatdoc_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/chatdoc_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/collection_builder.py` & `komodo_sdk-0.0.91/komodo/core/agents/collection_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/coordinator_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/coordinator_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/default.py` & `komodo_sdk-0.0.91/komodo/core/agents/default.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/difference_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/difference_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/elastic_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/groot_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/groot_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/librarian_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/librarian_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/mongo_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/mongo_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/pdf_generator.py` & `komodo_sdk-0.0.91/komodo/core/agents/pdf_generator.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/sample_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/sample_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/summarizer_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/summarizer_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/translator_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/translator_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/agents/widget_builder_agent.py` & `komodo_sdk-0.0.91/komodo/core/agents/widget_builder_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/sources/filesystem.py` & `komodo_sdk-0.0.91/komodo/core/sources/filesystem.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/sources/s3bucketkey.py` & `komodo_sdk-0.0.91/komodo/core/sources/s3bucketkey.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/sources/webpages.py` & `komodo_sdk-0.0.91/komodo/core/sources/webpages.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/sources/website_crawler.py` & `komodo_sdk-0.0.91/komodo/core/sources/website_crawler.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/elastic/elastic_count.py` & `komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_count.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/elastic/elastic_get.py` & `komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_get.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/elastic/elastic_search.py` & `komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/files/collection_builder.py` & `komodo_sdk-0.0.91/komodo/core/tools/files/collection_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/files/collection_lister.py` & `komodo_sdk-0.0.91/komodo/core/tools/files/collection_lister.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/files/collection_reader.py` & `komodo_sdk-0.0.91/komodo/core/tools/files/collection_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/files/directory_reader.py` & `komodo_sdk-0.0.91/komodo/core/tools/files/directory_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/files/file_reader.py` & `komodo_sdk-0.0.91/komodo/core/tools/files/file_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/files/file_writer.py` & `komodo_sdk-0.0.91/komodo/core/tools/files/file_writer.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/markets/polygon_search.py` & `komodo_sdk-0.0.91/komodo/core/tools/markets/polygon_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_databases.py` & `komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_databases.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_query.py` & `komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_query.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_schema.py` & `komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_schema.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/mongo/mongo_unique.py` & `komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_unique.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/search/vector_search.py` & `komodo_sdk-0.0.91/komodo/core/tools/search/vector_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/search/vector_search_runtime.py` & `komodo_sdk-0.0.91/komodo/core/tools/search/vector_search_runtime.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/utils/agent_tool.py` & `komodo_sdk-0.0.91/komodo/core/tools/utils/agent_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/utils/sample_tool.py` & `komodo_sdk-0.0.91/komodo/core/tools/utils/sample_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/utils/thought_tool.py` & `komodo_sdk-0.0.91/komodo/core/tools/utils/thought_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/utils/workflow_tool.py` & `komodo_sdk-0.0.91/komodo/core/tools/utils/workflow_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/web/data_fetcher.py` & `komodo_sdk-0.0.91/komodo/core/tools/web/data_fetcher.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/web/serpapi_search.py` & `komodo_sdk-0.0.91/komodo/core/tools/web/serpapi_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/web/tavily_search.py` & `komodo_sdk-0.0.91/komodo/core/tools/web/tavily_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/tools/web/web_scraper.py` & `komodo_sdk-0.0.91/komodo/core/tools/web/web_scraper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/utils/agent_helper.py` & `komodo_sdk-0.0.91/komodo/core/utils/agent_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/utils/indexer.py` & `komodo_sdk-0.0.91/komodo/core/utils/indexer.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/utils/play.py` & `komodo_sdk-0.0.91/komodo/core/utils/play.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/utils/rag_context.py` & `komodo_sdk-0.0.91/komodo/core/utils/rag_context.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/vector_stores/pinecone_store.py` & `komodo_sdk-0.0.91/komodo/core/vector_stores/pinecone_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/vector_stores/qdrant_store.py` & `komodo_sdk-0.0.91/komodo/core/vector_stores/qdrant_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/vector_stores/vector_store_helper.py` & `komodo_sdk-0.0.91/komodo/core/vector_stores/vector_store_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/core/workflows/sample_workflow.py` & `komodo_sdk-0.0.91/komodo/core/workflows/sample_workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/data/agents/planner/personal_finance_profile.yml` & `komodo_sdk-0.0.91/komodo/data/agents/planner/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/data/appliances/citibank/personal_finance_profile.yml` & `komodo_sdk-0.0.91/komodo/data/appliances/citibank/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf` & `komodo_sdk-0.0.91/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/data/workflows/analyzer/personal_finance_profile.yml` & `komodo_sdk-0.0.91/komodo/data/workflows/analyzer/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/definitions/agents/planner/context.yml` & `komodo_sdk-0.0.91/komodo/definitions/agents/planner/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/definitions/agents/planner/role.yml` & `komodo_sdk-0.0.91/komodo/definitions/agents/planner/role.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml` & `komodo_sdk-0.0.91/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/definitions/appliances/sample/context.yml` & `komodo_sdk-0.0.91/komodo/definitions/appliances/sample/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/definitions/workflows/analyzer/context.yml` & `komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_agent.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_app.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_app.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,17 +50,38 @@
 
     def get_agent(self, shortcode):
         for a in self.get_all_agents():
             if a.shortcode == shortcode:
                 return a
         return None
 
+    def get_user_profile(self, user):
+        return user.to_dict()
+
     def generate_context(self, prompt=None, runtime=None):
         return self.context
 
+    def configuration(self, user: KomodoUser):
+        print("Retrieving default configuration")
+        return {
+            "shortcode": self.shortcode,
+            "name": self.name,
+            "company": self.company,
+            "type": self.type.name,
+            "purpose": self.purpose,
+            "user": user.email if user else None,
+            "configuration": [
+                {
+                    "feature": KomodoFeatures.chat.name,
+                    "description": "Chat with the agents",
+                    "agents": [a.summary() for a in self.get_all_agents()]
+                }
+            ]
+        }
+
     def index(self, reindex=False):
         for agent in self.agents:
             agent.index(reindex=reindex)
 
     @staticmethod
     def default(config=None):
         return KomodoApp(name="Placeholder", shortcode="placeholder", purpose="Placeholder", config=config)
```

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_collection.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_collection.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_config.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_context.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_context.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_datasource.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_datasource.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_locations.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_locations.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_runnable.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_runnable.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_runtime.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_runtime.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_tool.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_tool_registry.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_tool_registry.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_user.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         self.verified = kwargs.get('verified', False)
         self.provider_id = kwargs.get('provider_id', 'komodo')
         self.token = kwargs.get('token', '')
 
         self.allowed_assistants = kwargs.get('allowed_assistants', [])
         self.preferred_assistant = kwargs.get('preferred_assistant', '')
         self.show_tool_progress = kwargs.get('show_tool_progress', None)
+        self.is_power_user = kwargs.get('is_power_user', False)
 
         # each user has a home folder / collection and a default downloads folder
         self.guid = get_text_digest(email)
         self.home_shortcode = self.guid + "_home"
         self.downloads_shortcode = self.guid + "_downloads"
 
     def __str__(self):
@@ -38,12 +39,7 @@
             'preferred_assistant': self.preferred_assistant,
             'show_tool_progress': self.show_tool_progress}
 
     @staticmethod
     def default():
         email = "ryan.oberoi@komodoapp.ai"
         return KomodoUser(email=email, name="Ryan Oberoi")
-
-    @staticmethod
-    def poweruser():
-        email = "ryan@kmdo.app"
-        return KomodoUser(email=email, name="Ryan", show_tool_progress="details")
```

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_vector.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_vector.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_vectorstore.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_vectorstore.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/framework/komodo_workflow.py` & `komodo_sdk-0.0.91/komodo/framework/komodo_workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/loaders/database/agent_loader.py` & `komodo_sdk-0.0.91/komodo/loaders/database/agent_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/loaders/database/appliance_loader.py` & `komodo_sdk-0.0.91/komodo/loaders/database/appliance_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/loaders/database/user_loader.py` & `komodo_sdk-0.0.91/komodo/loaders/database/user_loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 class UserLoader:
 
     def __init__(self, appliance):
         self.appliance = appliance
 
     def get_user(self, email):
         user = UserLoader.load(email) or next((x for x in self.appliance.users if x.email == email), None)
-        if UserLoader.is_power_user(email):
+        if user and UserLoader.is_power_user(email):
+            user.is_power_user = True
             user.show_tool_progress = "details"
         return user
 
     @classmethod
     def load(cls, email) -> [KomodoUser, None]:
         user = cls.load_appliance_user(email) or cls.load_system_user(email) or cls.load_firebase_user(email)
         return user
```

### Comparing `komodo_sdk-0.0.90/komodo/loaders/filesystem/agent_loader.py` & `komodo_sdk-0.0.91/komodo/loaders/filesystem/agent_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/loaders/filesystem/appliance_loader.py` & `komodo_sdk-0.0.91/komodo/loaders/filesystem/appliance_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/loaders/filesystem/loader_helper.py` & `komodo_sdk-0.0.91/komodo/loaders/filesystem/loader_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/loaders/filesystem/loader_locations.py` & `komodo_sdk-0.0.91/komodo/loaders/filesystem/loader_locations.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/loaders/filesystem/workflow_loader.py` & `komodo_sdk-0.0.91/komodo/loaders/filesystem/workflow_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/azure/azure.py` & `komodo_sdk-0.0.91/komodo/models/azure/azure.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/azure/azure_openai.py` & `komodo_sdk-0.0.91/komodo/models/azure/azure_openai.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/bedrock/bedrock.py` & `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/bedrock/bedrock_claude.py` & `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_claude.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/bedrock/bedrock_cohere.py` & `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_cohere.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/bedrock/bedrock_model.py` & `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_model.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/bedrock/bedrock_titan.py` & `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_titan.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/framework/agent_runner.py` & `komodo_sdk-0.0.91/komodo/models/framework/agent_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/framework/appliance_utils.py` & `komodo_sdk-0.0.91/komodo/models/framework/appliance_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/framework/chat_message.py` & `komodo_sdk-0.0.91/komodo/models/framework/chat_message.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/framework/model_request.py` & `komodo_sdk-0.0.91/komodo/models/framework/model_request.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/framework/model_response.py` & `komodo_sdk-0.0.91/komodo/models/framework/model_response.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/framework/responder.py` & `komodo_sdk-0.0.91/komodo/models/framework/responder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/framework/workflow_executor.py` & `komodo_sdk-0.0.91/komodo/models/framework/workflow_executor.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/framework/workflow_runner.py` & `komodo_sdk-0.0.91/komodo/models/framework/workflow_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/openai/openai_api.py` & `komodo_sdk-0.0.91/komodo/models/openai/openai_api.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/openai/openai_api_streamed.py` & `komodo_sdk-0.0.91/komodo/models/openai/openai_api_streamed.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/openai/openai_api_streamed_tool_call.py` & `komodo_sdk-0.0.91/komodo/models/openai/openai_api_streamed_tool_call.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/openai/openai_debug.py` & `komodo_sdk-0.0.91/komodo/models/openai/openai_debug.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/models/openai/openai_process_actions.py` & `komodo_sdk-0.0.91/komodo/models/openai/openai_process_actions.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/collection.proto` & `komodo_sdk-0.0.91/komodo/proto/collection.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/data.proto` & `komodo_sdk-0.0.91/komodo/proto/data.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/model.proto` & `komodo_sdk-0.0.91/komodo/proto/model.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/report.proto` & `komodo_sdk-0.0.91/komodo/proto/report.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/sample.py` & `komodo_sdk-0.0.91/komodo/proto/sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/generated/collection_pb2.py` & `komodo_sdk-0.0.91/komodo/proto/generated/collection_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/generated/collection_pb2.pyi` & `komodo_sdk-0.0.91/komodo/proto/generated/collection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/generated/data_pb2.py` & `komodo_sdk-0.0.91/komodo/proto/generated/data_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/generated/data_pb2.pyi` & `komodo_sdk-0.0.91/komodo/proto/generated/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/generated/model_pb2.py` & `komodo_sdk-0.0.91/komodo/proto/generated/model_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/generated/model_pb2.pyi` & `komodo_sdk-0.0.91/komodo/proto/generated/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/generated/report_pb2.py` & `komodo_sdk-0.0.91/komodo/proto/generated/report_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/proto/generated/report_pb2.pyi` & `komodo_sdk-0.0.91/komodo/proto/generated/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/scripts/run_agent_runner.py` & `komodo_sdk-0.0.91/komodo/scripts/run_agent_runner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from komodo.framework.komodo_agent import KomodoAgent
+from komodo.framework.komodo_runtime import KomodoRuntime
 from komodo.framework.komodo_user import KomodoUser
 from komodo.models.framework.agent_runner import AgentRunner
 
 if __name__ == '__main__':
     from komodo.core.tools.utils.thought_tool import ChainOfThought
     from komodo.models.framework.models import OPENAI_GPT4_MODEL
 
     agent = KomodoAgent.default()
     agent.model = OPENAI_GPT4_MODEL
     agent.add_tool(ChainOfThought())
-    runner = AgentRunner(agent, user=KomodoUser.poweruser())
-    
+
+    runtime = KomodoRuntime(agent=agent, user=KomodoUser.default())
+    runner = AgentRunner(runtime)
+
     prompt = "Tell me 5 jokes, and invoke the thought tool exactly after telling each joke."
     for response in runner.run_streamed(prompt):
         print(response, end="")
     print()
```

### Comparing `komodo_sdk-0.0.90/komodo/scripts/run_agent_runner_2.py` & `komodo_sdk-0.0.91/komodo/scripts/run_agent_runner_2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/scripts/run_difference_agent.py` & `komodo_sdk-0.0.91/komodo/scripts/run_difference_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/scripts/run_librarian_agent.py` & `komodo_sdk-0.0.91/komodo/scripts/run_librarian_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/scripts/run_streaming_test.py` & `komodo_sdk-0.0.91/komodo/scripts/run_streaming_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from komodo.core.tools.utils.sample_tool import SampleTool
 from komodo.core.tools.utils.thought_tool import ChainOfThought
 from komodo.framework.komodo_agent import KomodoAgent
+from komodo.framework.komodo_runtime import KomodoRuntime
 from komodo.framework.komodo_user import KomodoUser
 from komodo.models.framework.agent_runner import AgentRunner
 
 
 def run_stream_1():
     prompt = "whats up in nyc today? search for event and then search for additional details on the first event found"
     agent = KomodoAgent.default()
     agent.tools = [SampleTool("."), ChainOfThought()]
-    runner = AgentRunner(agent, user=KomodoUser.poweruser())
+
+    runtime = KomodoRuntime(agent=agent, user=KomodoUser.default())
+    runner = AgentRunner(runtime)
     for response in runner.run_streamed(prompt):
         print(response, end="")
     print()
 
 
 if __name__ == "__main__":
     run_stream_1()
```

### Comparing `komodo_sdk-0.0.90/komodo/scripts/run_widget_builder.py` & `komodo_sdk-0.0.91/komodo/scripts/run_widget_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/agent_router.py` & `komodo_sdk-0.0.91/komodo/server/agent_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/appliance_router.py` & `komodo_sdk-0.0.91/sample/appliance/appliance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,77 @@
-import datetime
-
-from fastapi import Depends, APIRouter
-
+from komodo import KomodoApp
 from komodo.core.agents.chatdoc_agent import ChatdocAgent
+from komodo.core.agents.collection_builder import CollectionBuilderAgent
+from komodo.core.agents.default import translator_agent, summarizer_agent
+
+from komodo.framework.komodo_context import KomodoContext
 from komodo.framework.komodo_features import KomodoFeatures
-from komodo.server.globals import get_appliance, get_email
+from komodo.framework.komodo_user import KomodoUser
+from komodo.loaders.filesystem.appliance_loader import ApplianceLoader
+from sample.appliance.workflow import SampleWorkflow
+
+
+class SampleAppliance(KomodoApp):
+    shortcode = 'sample'
+    name = 'Sample Appliance'
+    purpose = 'To test the Komodo Appliances SDK'
+
+    def __init__(self, config):
+        base = ApplianceLoader(config.definitions_directory, config.data_directory).load(self.shortcode)
+        super().__init__(**base)
+        self.config = config
+
+        self.add_agent(summarizer_agent())
+        self.add_agent(translator_agent())
+
+        chatdoc = ChatdocAgent()
+        chatdoc.max_tokens_per_file = 500
+        chatdoc.max_total_tokens = 2000
+
+        self.add_agent(chatdoc)
+        self.add_agent(CollectionBuilderAgent())
+        self.add_workflow(SampleWorkflow())
+
+    def generate_context(self, prompt=None, runtime=None):
+        context = KomodoContext()
+        context.add("Sample", f"Develop context for the {self.name} appliance")
+        return context
+
+    def configuration(self, user: KomodoUser):
+        print(f"Generating configuration for {user.email}")
+        config = self.configuration_for_power_user() if user.is_power_user else self.configuration_for_normal_user()
+        return {
+            "shortcode": self.shortcode,
+            "name": self.name,
+            "company": self.company,
+            "type": self.type.name,
+            "purpose": self.purpose,
+            "user": user.email,
+            "configuration": config
+        }
+
+    def configuration_for_normal_user(self):
+        shortcodes = ['summarizer', 'translator']
+        agents = [a for a in self.get_all_agents() if a.shortcode in shortcodes]
+        return [
+            {
+                "feature": KomodoFeatures.chat.name,
+                "description": "Chat with the agents",
+                "agents": [a.summary() for a in agents]
+            },
+            {
+                "feature": KomodoFeatures.chatdoc.name,
+                "description": "Chat with documents",
+                "agents": [ChatdocAgent().summary()]
+            }
+        ]
 
-router = APIRouter(
-    prefix='/api/v1/appliance',
-    tags=['Appliance']
-)
-
-
-@router.get('/description', response_model=dict, summary='Get appliance description',
-            description='Get the description of the appliance.')
-def get_appliance_description(appliance=Depends(get_appliance)):
-    agents = appliance.get_all_agents()
-    return {
-        "shortcode": appliance.shortcode,
-        "name": appliance.name,
-        "company": appliance.company,
-        "type": appliance.type.name,
-        "features": ", ".join([f.name for f in appliance.features]),
-        "version": get_version(),
-        "purpose": appliance.purpose,
-        "agents": [a.summary() for a in agents]
-    }
-
-
-@router.get('/configuration', response_model=dict, summary='Get appliance configuration',
-            description='Get the configuration of the appliance.')
-def get_appliance_configuration(email=Depends(get_email), appliance=Depends(get_appliance)):
-    agents = appliance.get_all_agents()
-    return {
-        "shortcode": appliance.shortcode,
-        "name": appliance.name,
-        "company": appliance.company,
-        "type": appliance.type.name,
-        "version": get_version(),
-        "purpose": appliance.purpose,
-        "user": email,
-        "configuration": [
+    def configuration_for_power_user(self):
+        agents = self.get_all_agents()
+        return [
             {
                 "feature": KomodoFeatures.chat.name,
                 "description": "Chat with the agents",
                 "agents": [a.summary() for a in agents]
             },
             {
                 "feature": KomodoFeatures.chatdoc.name,
@@ -78,37 +105,7 @@
                 "agents": []
             }, {
                 "feature": KomodoFeatures.dashboard.name,
                 "description": "Komodo Dashboard #2",
                 "agents": []
             }
         ]
-    }
-
-
-def get_version():
-    import importlib.metadata
-    try:
-        return importlib.metadata.version('komodo-sdk')
-    except importlib.metadata.PackageNotFoundError:
-        return "0.0.0." + str(datetime.datetime.now().strftime('%Y%m%d'))
-
-
-@router.get('/index', summary='Index all data sources',
-            description='Index all data sources for the appliance.')
-def index_all_data_sources(appliance=Depends(get_appliance)):
-    appliance.index(reindex=False)
-    return {"status": "success"}
-
-
-@router.get('/reindex', summary='Re-index all data sources.',
-            description='Deletes all existing data and re-indexes all data sources for the appliance.')
-def re_index_all_data_sources(appliance=Depends(get_appliance)):
-    appliance.index(reindex=True)
-    return {"status": "success"}
-
-
-@router.get('/available-agents', summary='Get available agents',
-            description='Get available agents for the appliance for a given feature.')
-def get_available_agents(email=Depends(get_email), appliance=Depends(get_appliance)):
-    agents = appliance.get_all_agents()
-    return {"status": "success"}
```

### Comparing `komodo_sdk-0.0.90/komodo/server/ask_request.py` & `komodo_sdk-0.0.91/komodo/server/ask_request.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/audio_router.py` & `komodo_sdk-0.0.91/komodo/server/audio_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/collections_router.py` & `komodo_sdk-0.0.91/komodo/server/collections_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/conversation_router.py` & `komodo_sdk-0.0.91/komodo/server/conversation_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/fast.py` & `komodo_sdk-0.0.91/komodo/server/fast.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/globals.py` & `komodo_sdk-0.0.91/komodo/server/globals.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/logo_router.py` & `komodo_sdk-0.0.91/komodo/server/logo_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/server/report_router.py` & `komodo_sdk-0.0.91/komodo/server/report_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/directory/assistants_helpers.py` & `komodo_sdk-0.0.91/komodo/shared/directory/assistants_helpers.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/documents/file_writer_helper.py` & `komodo_sdk-0.0.91/komodo/shared/documents/file_writer_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/documents/text_convert_helper.py` & `komodo_sdk-0.0.91/komodo/shared/documents/text_convert_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/documents/text_extract.py` & `komodo_sdk-0.0.91/komodo/shared/documents/text_extract.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/documents/text_extract_helper.py` & `komodo_sdk-0.0.91/komodo/shared/documents/text_extract_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/documents/text_html.py` & `komodo_sdk-0.0.91/komodo/shared/documents/text_html.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/embeddings/faiss_store.py` & `komodo_sdk-0.0.91/komodo/shared/embeddings/faiss_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/embeddings/pinecone_store.py` & `komodo_sdk-0.0.91/komodo/shared/embeddings/pinecone_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/mssql/mssql.py` & `komodo_sdk-0.0.91/komodo/shared/mssql/mssql.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/api_query.py` & `komodo_sdk-0.0.91/komodo/shared/utils/api_query.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/digest.py` & `komodo_sdk-0.0.91/komodo/shared/utils/digest.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/filestats.py` & `komodo_sdk-0.0.91/komodo/shared/utils/filestats.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/globber.py` & `komodo_sdk-0.0.91/komodo/shared/utils/globber.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/lambda_entry.py` & `komodo_sdk-0.0.91/komodo/shared/utils/lambda_entry.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/lambda_utils.py` & `komodo_sdk-0.0.91/komodo/shared/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/logconfig.py` & `komodo_sdk-0.0.91/komodo/shared/utils/logconfig.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/s3_file_utils.py` & `komodo_sdk-0.0.91/komodo/shared/utils/s3_file_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/tags.py` & `komodo_sdk-0.0.91/komodo/shared/utils/tags.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/term_colors.py` & `komodo_sdk-0.0.91/komodo/shared/utils/term_colors.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/timebox.py` & `komodo_sdk-0.0.91/komodo/shared/utils/timebox.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/shared/utils/watcher.py` & `komodo_sdk-0.0.91/komodo/shared/utils/watcher.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/store/agent_store.py` & `komodo_sdk-0.0.91/komodo/store/agent_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/store/appliance_store.py` & `komodo_sdk-0.0.91/komodo/store/appliance_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/store/collection_store.py` & `komodo_sdk-0.0.91/komodo/store/collection_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/store/conversations_store.py` & `komodo_sdk-0.0.91/komodo/store/conversations_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/store/logo_store.py` & `komodo_sdk-0.0.91/komodo/store/logo_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/store/redis_database.py` & `komodo_sdk-0.0.91/komodo/store/redis_database.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/store/tool_store.py` & `komodo_sdk-0.0.91/komodo/store/tool_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/store/user_store.py` & `komodo_sdk-0.0.91/komodo/store/user_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/core/test_elastic_agent.py` & `komodo_sdk-0.0.91/komodo/tests/core/test_elastic_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/core/test_elastic_sample.py` & `komodo_sdk-0.0.91/komodo/tests/core/test_elastic_sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/core/test_elastic_tools.py` & `komodo_sdk-0.0.91/komodo/tests/core/test_elastic_tools.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/core/test_mongo_sample.py` & `komodo_sdk-0.0.91/komodo/tests/core/test_mongo_sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/core/test_mongo_tools.py` & `komodo_sdk-0.0.91/komodo/tests/core/test_mongo_tools.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/core/test_serpapi_search.py` & `komodo_sdk-0.0.91/komodo/tests/core/test_serpapi_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/models/test_bedrock.py` & `komodo_sdk-0.0.91/komodo/tests/models/test_bedrock.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/models/test_workflow_runner.py` & `komodo_sdk-0.0.91/komodo/tests/models/test_workflow_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/shared/test_mssql.py` & `komodo_sdk-0.0.91/komodo/tests/shared/test_mssql.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/komodo/tests/store/test_conversation_store.py` & `komodo_sdk-0.0.91/komodo/tests/store/test_conversation_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/pdf2html/Dockerfile` & `komodo_sdk-0.0.91/pdf2html/Dockerfile`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/pdf2html/server.py` & `komodo_sdk-0.0.91/pdf2html/server.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/pdf2html/data/sample.html` & `komodo_sdk-0.0.91/pdf2html/data/sample.html`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/pdf2html/data/sample.pdf` & `komodo_sdk-0.0.91/pdf2html/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/Dockerfile` & `komodo_sdk-0.0.91/sample/Dockerfile`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/docker-compose.yml` & `komodo_sdk-0.0.91/sample/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/docker-production.yml` & `komodo_sdk-0.0.91/sample/docker-production.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/appliance/config.py` & `komodo_sdk-0.0.91/sample/appliance/config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/appliance/seed.py` & `komodo_sdk-0.0.91/sample/appliance/seed.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/appliance/server.py` & `komodo_sdk-0.0.91/sample/appliance/server.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/appliance/workflow.py` & `komodo_sdk-0.0.91/sample/appliance/workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/definitions/agents/dasher_v1/instructions.txt` & `komodo_sdk-0.0.91/sample/definitions/agents/dasher_v1/instructions.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/definitions/agents/dasher_v2/instructions.txt` & `komodo_sdk-0.0.91/sample/definitions/agents/dasher_v2/instructions.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/app.py` & `komodo_sdk-0.0.91/sample/widgets/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     navbar,
     html.Div(dash.page_container, className='container-padding-margin'),
     html.Link(rel='stylesheet', id='theme-link', href=dbc.themes.BOOTSTRAP)
 ])
 
 
 # Callback to update the theme based on selection
-@app.callback(
+@dash.callback(
     [Output('theme-link', 'href'), Output('theme-dropdown', 'label')],
     [Input(f"theme-{theme.name}", "n_clicks") for theme in Themes],
     prevent_initial_call=True,
 )
 def update_theme(*args):
     ctx = dash.callback_context
     theme_name = Themes.BOOTSTRAP.name
```

### Comparing `komodo_sdk-0.0.90/sample/widgets/globals.py` & `komodo_sdk-0.0.91/sample/widgets/globals.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/themes.py` & `komodo_sdk-0.0.91/sample/widgets/themes.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/assets/custom.css` & `komodo_sdk-0.0.91/sample/widgets/assets/custom.css`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     padding: 30px;
 }
 
 
 .response p {
     margin: 20px 0;
 }
+.dasher-input, .dasher-input *  {
+    border-radius: 10px;
+}
 
-.response, .response *, .dasher-input, .dasher-input *  {
+.dasher-input, .dasher-input svg  {
     border-radius: 10px;
 }
 
 .response h1,
 .response h2,
 .response h3,
 .response h4,
```

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/agent.py` & `komodo_sdk-0.0.91/sample/widgets/pages/agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/analytics.py` & `komodo_sdk-0.0.91/sample/widgets/pages/analytics.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/appliance.py` & `komodo_sdk-0.0.91/sample/widgets/pages/appliance.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/dasher_v1.py` & `komodo_sdk-0.0.91/sample/widgets/pages/dasher_v1.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/dasher_v2.py` & `komodo_sdk-0.0.91/sample/widgets/pages/dasher_v2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/department.py` & `komodo_sdk-0.0.91/sample/widgets/pages/department.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/present.py` & `komodo_sdk-0.0.91/sample/widgets/pages/present.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/report.py` & `komodo_sdk-0.0.91/sample/widgets/pages/report.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/side_bar.py` & `komodo_sdk-0.0.91/sample/widgets/pages/side_bar.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/reports/bar_chart.py` & `komodo_sdk-0.0.91/sample/widgets/pages/reports/bar_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/reports/line_chart.py` & `komodo_sdk-0.0.91/sample/widgets/pages/reports/line_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/sample/widgets/pages/reports/pie_chart.py` & `komodo_sdk-0.0.91/sample/widgets/pages/reports/pie_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/README.md` & `komodo_sdk-0.0.91/website/README.md`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/package-lock.json` & `komodo_sdk-0.0.91/website/package-lock.json`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/package.json` & `komodo_sdk-0.0.91/website/package.json`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/tailwind.config.js` & `komodo_sdk-0.0.91/website/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/deployment/nginx.default.conf` & `komodo_sdk-0.0.91/website/deployment/nginx.default.conf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/chaticon.png` & `komodo_sdk-0.0.91/website/public/chaticon.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/faqbg.png` & `komodo_sdk-0.0.91/website/public/faqbg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/favicon.ico` & `komodo_sdk-0.0.91/website/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/footer.png` & `komodo_sdk-0.0.91/website/public/footer.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/home.png` & `komodo_sdk-0.0.91/website/public/home.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/index.html` & `komodo_sdk-0.0.91/website/public/index.html`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/logo192.png` & `komodo_sdk-0.0.91/website/public/logo192.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/logo512.png` & `komodo_sdk-0.0.91/website/public/logo512.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/pricingBg.png` & `komodo_sdk-0.0.91/website/public/pricingBg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/pricingBg1.png` & `komodo_sdk-0.0.91/website/public/pricingBg1.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf` & `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/App.css` & `komodo_sdk-0.0.91/website/src/App.css`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/RouterMain.js` & `komodo_sdk-0.0.91/website/src/RouterMain.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -23,14 +23,15 @@
 import Document from "./pages/Document";
 import {
     Helmet
 } from "react-helmet";
 import roleContext from "../src/contexts/roleContext";
 import NavigateBack from "./components/NavigateBack";
 import ChatBotById from "./components/chatBot/ChatBotById";
+import Dashboard from "./components/Dashboard";
 
 function Authorization() {
     const user = JSON.parse(localStorage.getItem("komodoUser"));
     return user?.email !== null &&
         user?.email !== undefined &&
         user?.email !== "" ? ( <
             Outlet / >
@@ -183,14 +184,19 @@
 
         <
         Route path = "/profile"
         element = {
             < Profile / >
         }
         /> <
+        Route path = "/dashboard"
+        element = {
+            < Dashboard / >
+        }
+        /> <
         Route path = "/settings"
         element = {
             < Settings / >
         }
         /> <
         Route path = "/privacy"
         element = {
```

### Comparing `komodo_sdk-0.0.90/website/src/index.css` & `komodo_sdk-0.0.91/website/src/index.css`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,16 @@
 }
 .settingbox .css-8fj6w9-placeholder {
   font-size: 16px;
 }
 .chatDrawer {
   display: flex;
   position: relative;
-  width: 290px !important;
+  /* width: auto !important; */
+  width: 330px !important;
 }
 
 .collectionDraw {
   height: calc(100vh - 94px) !important;
   top: 93px !important;
 }
 
@@ -247,12 +248,12 @@
 }
 @media (max-width: 700px) {
   .removemargin table {
     width: 150%;
     overflow-x: auto;
   }
 }
-@media (max-width: 1000px) {
+@media (max-width: 1024px) {
   .collectpanel {
     display: block !important;
   }
 }
```

### Comparing `komodo_sdk-0.0.90/website/src/index.js` & `komodo_sdk-0.0.91/website/src/index.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/logo.svg` & `komodo_sdk-0.0.91/website/src/logo.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/API/API_data.js` & `komodo_sdk-0.0.91/website/src/API/API_data.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -21,16 +21,15 @@
 }
 
 export function ApiGet(path, email) {
     const user = JSON.parse(localStorage.getItem("komodoUser"));
     return new Promise((resolve, reject) => {
         let headers = {
             "Content-Type": "application/json",
-            "X-User-Email": user?.email || "test@example.com",
-            "X-User-Email": user?.email || "test@kmdo.app",
+            "X-User-Email": user?.email || email,
         };
         axios
             .get(`${path}`, {
                 headers: headers,
             })
             .then((response) => {
                 resolve(response);
```

### Comparing `komodo_sdk-0.0.90/website/src/API/ApiComment.js` & `komodo_sdk-0.0.91/website/src/API/ApiComment.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/Frame.svg` & `komodo_sdk-0.0.91/website/src/assets/Frame.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/ai.png` & `komodo_sdk-0.0.91/website/src/assets/ai.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/blue.svg` & `komodo_sdk-0.0.91/website/src/assets/blue.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/botAvatar.svg` & `komodo_sdk-0.0.91/website/src/assets/botAvatar.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/chatListIcon.svg` & `komodo_sdk-0.0.91/website/src/assets/chatListIcon.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/docs.svg` & `komodo_sdk-0.0.91/website/src/assets/docs.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/docx.png` & `komodo_sdk-0.0.91/website/src/assets/docx.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/folder.svg` & `komodo_sdk-0.0.91/website/src/assets/folder.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/gallery.svg` & `komodo_sdk-0.0.91/website/src/assets/gallery.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/headphone.svg` & `komodo_sdk-0.0.91/website/src/assets/headphone.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/magicpen-1.svg` & `komodo_sdk-0.0.91/website/src/assets/magicpen-1.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/magicpen.svg` & `komodo_sdk-0.0.91/website/src/assets/magicpen.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/message.svg` & `komodo_sdk-0.0.91/website/src/assets/message.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/multi.png` & `komodo_sdk-0.0.91/website/src/assets/multi.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/odt.png` & `komodo_sdk-0.0.91/website/src/assets/odt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/pdf.png` & `komodo_sdk-0.0.91/website/src/assets/pdf.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/pdf.svg` & `komodo_sdk-0.0.91/website/src/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/pricingBg.png` & `komodo_sdk-0.0.91/website/src/assets/pricingBg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/profile.png` & `komodo_sdk-0.0.91/website/src/assets/profile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/send.png` & `komodo_sdk-0.0.91/website/src/assets/send.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/setting-1.svg` & `komodo_sdk-0.0.91/website/src/assets/setting-1.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/setting.svg` & `komodo_sdk-0.0.91/website/src/assets/setting.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/text.png` & `komodo_sdk-0.0.91/website/src/assets/text.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/text.svg` & `komodo_sdk-0.0.91/website/src/assets/text.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/trash.svg` & `komodo_sdk-0.0.91/website/src/assets/trash.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/assets/userProfile.svg` & `komodo_sdk-0.0.91/website/src/assets/userProfile.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/auth/Login.js` & `komodo_sdk-0.0.91/website/src/auth/Login.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/auth/Signup.js` & `komodo_sdk-0.0.91/website/src/auth/Signup.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/Header.js` & `komodo_sdk-0.0.91/website/src/components/Header.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -62,53 +62,38 @@
         placeholder: (defaultStyles) => {
             return {
                 ...defaultStyles,
                 fontSize: "21px",
             };
         },
     };
-    // console.log(
-    //   "selectContext?.agentList?.agents :>> ",
-    //   selectContext?.agentList?.agents
-    // );
-    // const agents = selectContext?.agentList?.agents || [];
-
-    // const options = agents.map(agent => ({
-    //   value: agent.shortcode,
-    //   label: agent.name
-    // }));
-
-    // flex flex-row md:flex-col-reverse justify-between border-b-[0.5px] border-[#CDCDCD] h-[93px] md:h-auto items-center px-5 md:px-0 md:mx-4 sm:mx-2
-
-    // console.log(
-    //   "selectContext?.agentList[searchParams ?? 0]?.agents :>> ",
-    //   selectContext?.agentList[searchParams ?? 0]?.agents
-    // );
 
     return ( <
         div className = "flex flex-row md:flex-col-reverse justify-between border-b-[0.5px] border-[#CDCDCD] h-[93px] items-center px-5 xl:justify-center" >
         <
         div className = "w-full xl:flex xl:justify-center xl:items-center xl:flex-col sm:ms-20" > {
+            selectContext?.agentList?.length &&
             selectContext?.agentList[searchParams ?? 0]?.agents?.length > 0 ? (
                 // {selectContext?.reactSelect?.purpose !== undefined ? (
                 <
                 >
                 <
-                div className = "w-fit" >
+                div className = "min-w-[200px] max-w-fit" >
                 <
                 Select className = "font-cerebriregular selectstyle"
                 // value={selectContext?.agentList[searchParams ?? 0]?.agents?.[0]}
                 value = {
                     selectContext?.reactSelect
                 }
                 onChange = {
                     handleChange
                 }
                 // options={location?.state?.agent}
                 options = {
+                    selectContext?.agentList?.length &&
                     selectContext?.agentList[searchParams ?? 0]?.agents
                 }
                 // options={selectContext?.agentList?.agents}
                 styles = {
                     style
                 }
                 getOptionLabel = {
```

### Comparing `komodo_sdk-0.0.90/website/src/components/HeaderSideBar.js` & `komodo_sdk-0.0.91/website/src/components/HeaderSideBar.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/Home.jsx` & `komodo_sdk-0.0.91/website/src/components/Home.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/LayoutHeader.js` & `komodo_sdk-0.0.91/website/src/components/LayoutHeader.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -106,14 +106,16 @@
         onClick = {
             toggleDrawer
         }
         /> <
         /div>
 
         <
+        div className = "xl:block hidden" >
+        <
         Drawer open = {
             isDrawerOpen
         }
         onClose = {
             toggleDrawer
         }
         direction = "left"
@@ -137,30 +139,30 @@
         /div> <
         div className = "p-5 mt-3" >
         <
         Link to = "/home" >
         <
         p className = {
             `text-[20px] font-cerebriregular leading-[24px] mb-5 ${
-                  location?.pathname === "/home"
-                    ? "text-[#316FF6]"
-                    : "text-[#333333]"
-                }`
+                    location?.pathname === "/home"
+                      ? "text-[#316FF6]"
+                      : "text-[#333333]"
+                  }`
         } >
         Home <
         /p> <
         /Link> <
         Link to = "/pricing" >
         <
         p className = {
             `text-[20px] font-cerebriregular leading-[24px] mb-5 ${
-                  location?.pathname === "/pricing"
-                    ? "text-[#316FF6]"
-                    : "text-[#333333]"
-                }`
+                    location?.pathname === "/pricing"
+                      ? "text-[#316FF6]"
+                      : "text-[#333333]"
+                  }`
         } >
         Pricing <
         /p> <
         /Link> <
         hr / >
         <
         div className = "mt-5" > {
@@ -192,12 +194,13 @@
         Try Now <
         /button> <
         /Link> <
         /div> <
         /div> <
         /div> <
         /Drawer> <
+        /div> <
         />
     );
 };
 
 export default LayoutHeader;
```

### Comparing `komodo_sdk-0.0.90/website/src/components/NavigateBack.js` & `komodo_sdk-0.0.91/website/src/components/NavigateBack.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/Sidebar.js` & `komodo_sdk-0.0.91/website/src/components/Sidebar.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -77,14 +77,15 @@
     const handleConfig = (val, i) => {
         // const user = JSON.parse(localStorage.getItem("komodoUser"));
         // localStorage.setItem(
         //   "komodoUser",
         //   JSON.stringify({ ...user, select: val.agents[0] })
         // );
         agentContext.setReactSelect(val.agents[0]);
+        localStorage?.removeItem("react-resizable-panels:example");
         navigate(`/${val.feature}?feature=${i}`);
     };
 
     const customIcon = (index) => {};
 
     const icon = {
         0: ( <
@@ -181,20 +182,93 @@
             clip - rule = "evenodd"
             d = "M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
             fill = "white" /
             >
             <
             /svg>
         ),
+        6: ( <
+            svg xmlns = "http://www.w3.org/2000/svg"
+            width = "26"
+            height = "26"
+            viewBox = "0 0 26 26"
+            fill = "none" >
+            <
+            path d = "M22.4359 8.79666V18.9908C22.4359 21.6558 20.2584 23.8333 17.5934 23.8333H8.40671C5.74171 23.8333 3.56421 21.6558 3.56421 18.9908V8.79666C3.56421 6.94416 4.60421 5.32999 6.13171 4.51749C6.66254 4.23583 7.32338 4.61499 7.32338 5.22166C7.32338 6.94416 8.73171 8.35249 10.4542 8.35249H15.5459C17.2684 8.35249 18.6767 6.94416 18.6767 5.22166C18.6767 4.61499 19.3267 4.23583 19.8684 4.51749C21.3959 5.32999 22.4359 6.94416 22.4359 8.79666Z"
+            fill = "white" /
+            >
+            <
+            path d = "M15.5459 2.16667H10.4542C9.32757 2.16667 8.40674 3.07667 8.40674 4.20334V5.22167C8.40674 6.34834 9.31674 7.25834 10.4434 7.25834H15.5459C16.6726 7.25834 17.5826 6.34834 17.5826 5.22167V4.20334C17.5934 3.07667 16.6726 2.16667 15.5459 2.16667Z"
+            fill = "white" /
+            >
+            <
+            /svg>
+        ),
+        7: ( <
+            svg xmlns = "http://www.w3.org/2000/svg"
+            width = "26"
+            height = "26"
+            viewBox = "0 0 26 26"
+            fill = "none" >
+            <
+            path d = "M17.5391 2.16667H8.46079C4.51746 2.16667 2.16663 4.5175 2.16663 8.46084V17.5283C2.16663 21.4825 4.51746 23.8333 8.46079 23.8333H17.5283C21.4716 23.8333 23.8225 21.4825 23.8225 17.5392V8.46084C23.8333 4.5175 21.4825 2.16667 17.5391 2.16667ZM7.04163 13.6175H10.0425C10.4866 13.6175 10.855 13.9858 10.855 14.43C10.855 14.8742 10.4866 15.2425 10.0425 15.2425H7.04163C6.59746 15.2425 6.22913 14.8742 6.22913 14.43C6.22913 13.9858 6.59746 13.6175 7.04163 13.6175ZM14.0508 19.3158H7.04163C6.59746 19.3158 6.22913 18.9475 6.22913 18.5033C6.22913 18.0592 6.59746 17.6908 7.04163 17.6908H14.0508C14.495 17.6908 14.8633 18.0592 14.8633 18.5033C14.8633 18.9475 14.5058 19.3158 14.0508 19.3158ZM18.9583 19.3158H16.9541C16.51 19.3158 16.1416 18.9475 16.1416 18.5033C16.1416 18.0592 16.51 17.6908 16.9541 17.6908H18.9583C19.4025 17.6908 19.7708 18.0592 19.7708 18.5033C19.7708 18.9475 19.4025 19.3158 18.9583 19.3158ZM18.9583 15.2425H12.9675C12.5233 15.2425 12.155 14.8742 12.155 14.43C12.155 13.9858 12.5233 13.6175 12.9675 13.6175H18.9583C19.4025 13.6175 19.7708 13.9858 19.7708 14.43C19.7708 14.8742 19.4025 15.2425 18.9583 15.2425Z"
+            fill = "white" /
+            >
+            <
+            /svg>
+        ),
+        8: ( <
+            svg xmlns = "http://www.w3.org/2000/svg"
+            width = "26"
+            height = "26"
+            viewBox = "0 0 26 26"
+            fill = "none" >
+            <
+            path d = "M17.5391 2.16667H8.46079C4.51746 2.16667 2.16663 4.5175 2.16663 8.46084V17.5283C2.16663 21.4825 4.51746 23.8333 8.46079 23.8333H17.5283C21.4716 23.8333 23.8225 21.4825 23.8225 17.5392V8.46084C23.8333 4.5175 21.4825 2.16667 17.5391 2.16667ZM20.0416 17.7667C20.0416 19.3917 19.3916 20.0417 17.7666 20.0417H13.65C12.025 20.0417 11.375 19.3917 11.375 17.7667V15.8167C11.375 14.1917 12.025 13.5417 13.65 13.5417H17.7666C19.3916 13.5417 20.0416 14.1917 20.0416 15.8167V17.7667Z"
+            fill = "white" /
+            >
+            <
+            /svg>
+        ),
+        9: ( <
+            svg xmlns = "http://www.w3.org/2000/svg"
+            width = "26"
+            height = "26"
+            viewBox = "0 0 31 27"
+            fill = "none" >
+            <
+            path fill - rule = "evenodd"
+            clip - rule = "evenodd"
+            d = "M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
+            fill = "white" /
+            >
+            <
+            /svg>
+        ),
+        10: ( <
+            svg xmlns = "http://www.w3.org/2000/svg"
+            width = "26"
+            height = "26"
+            viewBox = "0 0 31 27"
+            fill = "none" >
+            <
+            path fill - rule = "evenodd"
+            clip - rule = "evenodd"
+            d = "M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
+            fill = "white" /
+            >
+            <
+            /svg>
+        ),
     };
 
     return ( <
         div className = " bg-darkBg px-5 pt-5 max-w-[68px] min-w-[68px] xl:w-[60px] h-screen flex flex-col justify-between items-center" >
         <
-        div className = "flex flex-col justify-center items-center gap-8" > {
+        div className = "flex flex-col justify-center items-center gap-6" > {
             pathname !== "/" ? ( <
                 > {
                     configData?.map((v, i) => {
                         return ( <
                             div title = {
                                 v?.description
                             }
@@ -209,15 +283,16 @@
                             onClick = {
                                 () => handleConfig(v, i)
                             } >
                             {
                                 " "
                             } {
                                 icon[i]
-                            } <
+                            } {
+                                /* {v?.feature} */ } <
                             /div> <
                             /div>
                         );
                     })
                 }
 
                 {
```

### Comparing `komodo_sdk-0.0.90/website/src/components/DocumentBox/Table.js` & `komodo_sdk-0.0.91/website/src/components/DocumentBox/Table.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/chat/Chat.js` & `komodo_sdk-0.0.91/website/src/components/chat/Chat.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/chat/Details.js` & `komodo_sdk-0.0.91/website/src/components/chat/Details.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/chat/EnhancedPrompt.js` & `komodo_sdk-0.0.91/website/src/components/chat/EnhancedPrompt.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/chatBot/Chat.js` & `komodo_sdk-0.0.91/website/src/components/chatBot/Chat.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -183,19 +183,19 @@
                     ...prevData, {
                         sender: user.email,
                         text: prompt
                     },
                 ]);
             }
             setText(prompt);
+            setSend(true);
+            setApiActive(true);
         }
         setPrompt("");
         scrollToBottom();
-        setSend(true);
-        setApiActive(true);
     };
 
     const handleKeyPress = (e) => {
         if (e.key === "Enter") {
             sendPrompt();
         }
         // if (e.key === "Enter" && !e.shiftKey) {
@@ -282,16 +282,15 @@
           }`
         }
         // className="chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-10 mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
         ref = {
             chatContainerRef
         } >
         {
-            allChatData &&
-            allChatData.length > 0 &&
+            allChatData && allChatData.length > 0 ?
             allChatData.map((val, index) => {
                 return ( <
                     div key = {
                         index
                     }
                     className = "flex flex-col" > {
                         val?.sender === user.email && ( <
@@ -371,15 +370,16 @@
                         )
                     }
 
                     {
                         /* //   )} */ } <
                     /div>
                 );
-            })
+            }) :
+                null
         } {
             text !== "" && (
                 // {text !== "" && fullMessage && (
                 <
                 div className = "flex items-start w-full mt-2 gap-2" >
                 <
                 div className = "bg-customBgDark p-1.5 rounded-full min-w-[31px] h-[30px] mt-2" >
@@ -493,15 +493,22 @@
                       onClick={sendPrompt}
                     >
                       <RiSendPlaneFill className="text-[21px] rotate-45" />
                     </div> */
         } <
         div > {
             !send ? ( <
-                div className = "cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4"
+                div className = {
+                    `${
+                prompt.trim() !== ""
+                  ? "bg-customBgDark cursor-pointer"
+                  : "bg-slate-400"
+              }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4`
+                }
+                // className="cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4"
                 onClick = {
                     sendPrompt
                 } >
                 <
                 RiSendPlaneFill className = "text-[21px] rotate-45" / >
                 <
                 /div>
```

### Comparing `komodo_sdk-0.0.90/website/src/components/chatBot/ChatBotById.js` & `komodo_sdk-0.0.91/website/src/components/chatBot/ChatBotById.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -34,33 +34,59 @@
 } from "@cyntler/react-doc-viewer";
 import {
     Panel,
     PanelGroup,
     PanelResizeHandle
 } from "react-resizable-panels";
 import DocumentView from "../DocumentView";
+import {
+    HiDocumentText
+} from "react-icons/hi";
+import {
+    Box,
+    Modal
+} from "@mui/material";
+import {
+    IoClose
+} from "react-icons/io5";
 
+const style = {
+    position: "absolute",
+    top: "50%",
+    left: "50%",
+    transform: "translate(-50%, -50%)",
+    width: "80%",
+    bgcolor: "#fff",
+    boxShadow: 20,
+    // p: 4,
+    // borderRadius: "20px",
+    outline: "none",
+};
 
 const ChatBotById = () => {
     const chatContext = useContext(roleContext);
     const [prompt, setPrompt] = useState("");
     const [text, setText] = useState("");
     const [allChatData, setAllChatData] = useState([]);
     const [send, setSend] = useState(false);
     const location = useLocation();
-    const parts = location?.pathname.split('/');
+    const parts = location?.pathname.split("/");
     const chatId = parts[3];
     const user = JSON.parse(localStorage.getItem("komodoUser"));
     const [loader, setLoader] = useState(false);
     const [newDetails, setNewDetails] = useState({
         gId: "",
         chatRes: ""
     });
     const chatContainerRef = useRef(null);
     const [apiActive, setApiActive] = useState(true);
+    const [open, setOpen] = useState(false);
+
+    const handleOpen = () => setOpen(true);
+    const handleClose = () => setOpen(false);
 
     const stopRes = () => {
         setApiActive(false);
         setSend(false);
     };
 
     const scrollToBottom = () => {
@@ -82,15 +108,15 @@
                 ...newDetails,
                 gId: chatId,
             });
         }
     }, [location?.pathname]);
 
     const getConversationByGuid = async (guid) => {
-        console.log('guid :>> ', guid);
+        console.log("guid :>> ", guid);
         try {
             setLoader(true);
             const res = await ApiGet(API_Path.conversationsGetUrl(guid));
             if (res?.status === 200) {
                 setAllChatData(res?.data[0]?.messages);
             }
         } catch (error) {
@@ -104,15 +130,15 @@
 
     const sendPrompt = async () => {
         if (prompt.trim() !== "") {
             if (newDetails.chatRes !== "") {
                 setAllChatData((prevData) => [
                     ...prevData, {
                         sender: chatContext?.reactSelect?.shortcode,
-                        text: newDetails.chatRes
+                        text: newDetails.chatRes,
                     }, {
                         sender: user.email,
                         text: prompt
                     },
                 ]);
                 setNewDetails({
                     ...newDetails,
@@ -123,19 +149,19 @@
                     ...prevData, {
                         sender: user.email,
                         text: prompt
                     },
                 ]);
             }
             setText(prompt);
+            setSend(true);
+            setApiActive(true);
         }
         setPrompt("");
         scrollToBottom();
-        setSend(true);
-        setApiActive(true);
     };
 
     const handleKeyPress = (e) => {
         if (e.key === "Enter" && !e.shiftKey) {
             sendPrompt();
             e.preventDefault();
             sendMessage();
@@ -153,29 +179,60 @@
     return ( <
         >
         <
         CollectionLayout >
         <
         PanelGroup autoSaveId = "example"
         direction = "horizontal"
-        className = "panelgroup" >
+        className = "collectpanel" >
         <
         Panel defaultSize = {
             50
         }
         id = "sources-explorer-panel"
         // className="min-w-[30%]"
         className = {
             `xl:border-l xl:border-[#E8E9EA] ${chatContext?.isDoc === true
-                            ? // location?.state?.openChat === true
-                            "min-w-[30%] xl:w-full"
-                            : "min-w-full"
-                            }`
+              ? // location?.state?.openChat === true
+              "min-w-[30%] xl:w-full"
+              : "min-w-full"
+              }`
         } >
         <
+        div className = {
+            `${chatContext?.isDoc === true
+              ?
+              "block"
+              : "hidden"
+              }`
+        } >
+        <
+        div className = "hidden lg:block absolute top-6 right-7 z-10 text-[40px] cursor-pointer bg-customColor p-2 rounded-full"
+        onClick = {
+            handleOpen
+        } >
+        {
+            /* <HiDocumentText /> */ } <
+        svg xmlns = "http://www.w3.org/2000/svg"
+        width = "26"
+        height = "26"
+        viewBox = "0 0 26 26"
+        fill = "none" >
+        <
+        path d = "M22.4359 8.79666V18.9908C22.4359 21.6558 20.2584 23.8333 17.5934 23.8333H8.40671C5.74171 23.8333 3.56421 21.6558 3.56421 18.9908V8.79666C3.56421 6.94416 4.60421 5.32999 6.13171 4.51749C6.66254 4.23583 7.32338 4.61499 7.32338 5.22166C7.32338 6.94416 8.73171 8.35249 10.4542 8.35249H15.5459C17.2684 8.35249 18.6767 6.94416 18.6767 5.22166C18.6767 4.61499 19.3267 4.23583 19.8684 4.51749C21.3959 5.32999 22.4359 6.94416 22.4359 8.79666Z"
+        fill = "white" /
+        >
+        <
+        path d = "M15.5459 2.16667H10.4542C9.32757 2.16667 8.40674 3.07667 8.40674 4.20334V5.22167C8.40674 6.34834 9.31674 7.25834 10.4434 7.25834H15.5459C16.6726 7.25834 17.5826 6.34834 17.5826 5.22167V4.20334C17.5934 3.07667 16.6726 2.16667 15.5459 2.16667Z"
+        fill = "white" /
+        >
+        <
+        /svg> <
+        /div> <
+        /div> <
         div
         // className={`grid lg:grid-cols-1 ${location?.state?.openChat === true ? "grid-cols-2" : ""
         //     }`}
         >
         <
         div
         //  className={`xl:border-l xl:border-[#E8E9EA] ${location?.state?.openChat === true ? "col-span-1" : ""
@@ -184,29 +241,28 @@
         <
         div className = "h-[calc(100vh-177px)] pt-1 flex items-center flex-col" >
         <
         div
         // className={`chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-8 mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4`}
         className = {
             `chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-8 ${chatContext?.isDoc === true
-                                                // location?.state?.openChat === true
-                                                ? "w-full px-5"
-                                                : "mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
-                                            }`
+                      ? // location?.state?.openChat === true
+                      "w-full px-5"
+                      : "mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
+                      }`
         }
         // className={`chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-8 ${location?.state?.openChat === true
         //     ? "w-full px-5"
         //     : "mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
         //     }`}
         ref = {
             chatContainerRef
         } >
         {
-            allChatData &&
-            allChatData.length > 0 &&
+            allChatData && allChatData.length > 0 ?
             allChatData.map((val, index) => {
                 return ( <
                     div key = {
                         index
                     }
                     className = "flex flex-col" > {
                         val?.sender === user.email && ( <
@@ -229,72 +285,68 @@
                             /div> <
                             /div> <
                             /div> <
                             /div>
                         )
                     }
 
-
                     {
-                        val?.sender === chatContext?.reactSelect?.shortcode && ( <
-                            div className = "flex items-start w-full mt-2 gap-2" >
-                            <
-                            div className = "bg-customBgDark p-1.5 rounded-full min-w-[31px] h-[30px] mt-2" >
-                            <
-                            img src = {
-                                wave
-                            }
-                            alt = "wave"
-                            className = "w-[20px] h-[20px]" /
-                            >
-                            <
-                            /div> <
-                            div className = "flex flex-col" >
-                            <
-                            div >
-                            <
-                            MarkdownRenderer markdown = {
-                                val?.text
-                            }
-                            className = "font-cerebriregular text-[15px] px-3 text-blackText removemargin" /
-                            >
-                            <
-                            /div>
-
-                            <
-                            div className = "text-blackText font-cerebri font-normal text-[12px] text-right mt-1" >
-
-                            <
-                            /div> <
-                            /div> <
-                            /div>
-                        )
-                    }
-
-                    <
+                        val?.sender ===
+                            chatContext?.reactSelect?.shortcode && ( <
+                                div className = "flex items-start w-full mt-2 gap-2" >
+                                <
+                                div className = "bg-customBgDark p-1.5 rounded-full min-w-[31px] h-[30px] mt-2" >
+                                <
+                                img src = {
+                                    wave
+                                }
+                                alt = "wave"
+                                className = "w-[20px] h-[20px]" /
+                                >
+                                <
+                                /div> <
+                                div className = "flex flex-col" >
+                                <
+                                div >
+                                <
+                                MarkdownRenderer markdown = {
+                                    val?.text
+                                }
+                                className = "font-cerebriregular text-[15px] px-3 text-blackText removemargin" /
+                                >
+                                <
+                                /div>
+
+                                <
+                                div className = "text-blackText font-cerebri font-normal text-[12px] text-right mt-1" > < /div> <
+                                /div> <
+                                /div>
+                            )
+                    } <
                     /div>
                 );
-            })
+            }) :
+                null
         } {
             text !== "" && ( <
                 div className = "flex items-start w-full mt-2 gap-2" >
                 <
                 div className = "bg-customBgDark p-1.5 rounded-full min-w-[31px] h-[30px] mt-2" >
                 <
                 img src = {
                     wave
                 }
                 alt = "wave"
-                className = "w-[20px] h-[20px]" / >
+                className = "w-[20px] h-[20px]" /
+                >
                 <
                 /div> <
                 div className = "flex flex-col" >
                 <
                 div >
-
                 <
                 EnhancedBot prompt = {
                     text
                 }
                 guid = {
                     newDetails?.gId
                 }
@@ -307,26 +359,22 @@
                 apiActive = {
                     apiActive
                 }
                 /> <
                 /div>
 
                 <
-                div className = "text-blackText font-cerebri font-normal text-[12px] text-right mt-1" >
-                <
-                /div> <
+                div className = "text-blackText font-cerebri font-normal text-[12px] text-right mt-1" > < /div> <
                 /div> <
                 /div>
             )
         } <
         div className = {
             `flex flex-col mt-4 mb-5 `
-        } >
-        <
-        /div> <
+        } > < /div> <
         /div> <
         /div> <
         div className = "relative px-5 border-t-[0.5px] border-[#CDCDCD] py-5 flex items-center justify-center gap-4 bg-white" >
         <
         div className = "w-[14px] sm:w-[40px]" >
         <
         img src = {
@@ -348,15 +396,21 @@
             handleKeyPress
         }
         />
 
         <
         div > {
             !send ? ( <
-                div className = "cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4"
+                div className = {
+                    `${prompt.trim() !== ""
+                          ? "bg-customBgDark cursor-pointer"
+                          : "bg-slate-400"
+                          }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4`
+                }
+                // className="cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4"
                 onClick = {
                     sendPrompt
                 } >
                 <
                 RiSendPlaneFill className = "text-[21px] rotate-45" / >
                 <
                 /div>
@@ -401,31 +455,64 @@
         <
         Panel defaultSize = {
             50
         }
         id = "console-panel"
         className = {
             `border-l border-[#E8E9EA] ${chatContext?.isDoc === true
-                            ? // location?.state?.openChat === true
-                            "w-[50%] block xl:w-full"
-                            : "hidden"
-                            }`
+              ? // location?.state?.openChat === true
+              "w-[50%] block xl:w-full"
+              : "hidden"
+              }`
         } >
         <
-        DocumentView / >
+        DocumentView foo = "bar" / >
         <
         /Panel> <
-        /PanelGroup> <
+        /PanelGroup>
+
+        <
+        Modal open = {
+            open
+        }
+        onClose = {
+            handleClose
+        }
+        aria - labelledby = "modal-modal-title"
+        aria - describedby = "modal-modal-description" >
+        <
+        Box sx = {
+            style
+        } >
+        <
+        div className = "flex justify-between items-center font-cerebri text-[18px] text-[#3C3C3C] mb-2 p-5" >
+        <
+        div >
+        File Preview <
+        /div> <
+        div onClick = {
+            handleClose
+        }
+        className = "text-[25px]" >
+        <
+        IoClose / >
+        <
+        /div> <
+        /div> <
+        DocumentView foo = "bar" / >
+        <
+        /Box> <
+        /Modal> <
         /CollectionLayout> <
         style > {
             `
                 .EZDrawer__overlay {
                 background-color: transparent !important;
                 }
                 `
         } <
         /style> <
         />
-    )
+    );
 };
 
 export default ChatBotById;
```

### Comparing `komodo_sdk-0.0.90/website/src/components/chatBot/ChatBotSideBar.js` & `komodo_sdk-0.0.91/website/src/components/chatBot/ChatBotSideBar.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -61,28 +61,31 @@
 
 const ChatBotSideBar = ({
     uploadedFiles = [],
     // setIsCollections,
     // isCollections,
     setSelectedCollectionName,
     setSelectedFileName,
+    setIsDrawerOpen,
+    textWidth,
     // filesData,
     // setFilesData,
     // getUserFiles,
 }) => {
     const user = JSON.parse(localStorage.getItem("komodoUser"));
     const fileInputRef = useRef(null);
     const [open, setOpen] = useState(false);
     const collectFileName = localStorage?.getItem("collectName");
     const [collection, setCollection] = useState("");
     const [description, setDescription] = useState("");
     // const [fileData, setFileData] = useState("");
     // console.log("fileData :>> ", fileData);
     const [collectName, setCollectName] = useState("");
     const [collect, setCollect] = useState([]);
+    console.log("collect :>> ", collect);
     const [deleteChat, setDeleteChat] = useState(false);
     const [deleteChatId, setDeleteChatId] = useState(null);
     const [deleteChat1, setDeleteChat1] = useState(false);
     const [deleteChatId1, setDeleteChatId1] = useState(null);
     const handleOpen = () => setOpen(true);
     const handleClose = () => setOpen(false);
     const navigate = useNavigate();
@@ -147,15 +150,21 @@
     useEffect(() => {
         CollectionData();
     }, []);
 
     const CollectionData = async () => {
         try {
             const collection = await ApiGet(API_Path.collectionsGetUrl);
-            setCollect(collection?.data);
+            const dataA = await collection?.data?.map((v) => {
+                return {
+                    ...v,
+                    name: v?.name?.replace(/[_-]/g, " ")
+                };
+            });
+            setCollect(dataA);
         } catch (error) {
             console.log("error", error);
         }
     };
 
     const getFileIcon = (fileType, path) => {
         if (fileType?.includes("pdf")) {
@@ -176,32 +185,37 @@
                 //     fill="var(--primary-color)"
                 //   />
                 // </svg>
                 <
                 img src = {
                     pdf
                 }
-                alt = "pdf" / >
+                alt = "pdf"
+                className = "min-w-[25px]" / >
             );
         } else if (fileType.includes("sheet")) {
             return < img src = {
                 xlsx
             }
             width = {
                 25
             }
-            alt = "xlsx" / > ;
+            alt = "xlsx"
+            className = "min-w-[25px]" / > ;
         } else if (fileType.includes("presentation")) {
-            return < img src = {
-                pptLogo
-            }
-            width = {
-                25
-            }
-            alt = "ppt" / > ;
+            return ( <
+                img src = {
+                    pptLogo
+                }
+                width = {
+                    25
+                }
+                alt = "ppt"
+                className = "min-w-[25px]" / >
+            );
         } else if (fileType.includes("doc") || fileType.includes("msword")) {
             return (
                 // <svg
                 //   xmlns="http://www.w3.org/2000/svg"
                 //   width="20"
                 //   height="20"
                 //   viewBox="0 0 43 43"
@@ -216,15 +230,16 @@
                 //     fill="var(--primary-color)"
                 //   />
                 // </svg>
                 <
                 img src = {
                     word
                 }
-                alt = "word" / >
+                alt = "word"
+                className = "min-w-[25px]" / >
             );
         } else if (fileType.includes("text")) {
             return (
                 // <svg
                 //   xmlns="http://www.w3.org/2000/svg"
                 //   width="20"
                 //   height="20"
@@ -243,29 +258,35 @@
                 <
                 img src = {
                     txt
                 }
                 alt = "txt" / >
             );
         } else if (fileType.includes("image")) {
-            return < img src = {
-                imgLogo
-            }
-            width = {
-                25
-            }
-            alt = "imgLogo" / > ;
+            return ( <
+                img src = {
+                    imgLogo
+                }
+                width = {
+                    25
+                }
+                alt = "imgLogo"
+                className = "min-w-[25px]" / >
+            );
         } else {
-            return < img src = {
-                odtIcon
-            }
-            width = {
-                25
-            }
-            alt = "txt" / > ;
+            return ( <
+                img src = {
+                    odtIcon
+                }
+                width = {
+                    25
+                }
+                alt = "txt"
+                className = "min-w-[25px]" / >
+            );
         }
     };
 
     const handleSelectItem = (name) => {
         setSelectedCollectionName(name);
     };
 
@@ -437,19 +458,19 @@
             return "Today";
         } else if (valDate.toDateString() === yesterday.toDateString()) {
             return "Yesterday";
         } else {
             return "Previous";
         }
     };
-    const [isDrawerOpen, setIsDrawerOpen] = useState(false);
+    // const [isDrawerOpen, setIsDrawerOpen] = useState(false);
 
-    const toggleDrawer = () => {
-        setIsDrawerOpen(!isDrawerOpen);
-    };
+    // const toggleDrawer = () => {
+    //   setIsDrawerOpen(!isDrawerOpen);
+    // };
 
     const renderChatItems = () => {
         let todayDisplayed = false;
         let yesterdayDisplayed = false;
         let previousDisplayed = false;
         return listData?.list?.map((val, i) => {
             const formattedDate = formatDate(val?.createdAt);
@@ -512,14 +533,15 @@
         div key = {
             val?.guid
         }
         // onClick={() => handleDetails(val)}
         onClick = {
             () => {
                 navigate(`/chatdoc/${contextFiles?.oldChatId}/${val?.guid}`);
+                localStorage?.removeItem("react-resizable-panels:example");
                 setIsCollections(false);
             }
         }
         className = {
             `px-5 border-b-[0.5px] border-[#F6F6F9] py-5 text-[#5A636C] text-[14px] leading-[17.78px] flex justify-between items-center font-cerebriregular cursor-pointer ${
         id === val?.guid ? "bg-[#F6F6F9]" : ""
       }`
@@ -569,15 +591,17 @@
                                 
                           
                                 <img src={chatListIcon}/>
                             </span> */
         }
 
         <
-        div className = "text-wrap"
+        div className = "line-clamp-1"
+        // className="truncate"
+        // style={{ width: textWidth + "px" }}
         // className="w-[200px] lg:w-[110px] xl:w-[60px] xxl:w-[100px] truncate"
         onClick = {
             () => setIsDrawerOpen(false)
         } >
         {
             val?.title
         } <
@@ -854,15 +878,15 @@
                 <
                 div className = "flex items-center justify-between pt-4 px-5 border-t-[0.5px] border-[#F6F6F9]" >
                 <
                 div className = "text-blackText text-[18px] mt-4 mb-3 -ml-2 font-cerebriMedium" >
                 Collections <
                 /div> <
                 /div> <
-                div >
+                div id = "collectionWidth" >
                 <
                 div className = "sidebar h-[calc(100vh-251px)] 1xl:h-[calc(100vh-278px)] overflow-auto" > {
                     collect.map((item, index) => {
                         return ( <
                             div className = {
                                 `flex items-center justify-between px-3 py-4 mt-1 cursor-pointer overflow-hidden`
                             }
@@ -933,15 +957,18 @@
 
                             <
                             div >
                             <
                             div title = {
                                 item?.description
                             }
-                            className = "text-blackText font-cerebriregular text-[16px] capitalize w-[110px] whitespace-nowrap overflow-hidden text-ellipsis" >
+                            // style={{ width: textWidth + "px" }}
+                            className = "text-blackText font-cerebriregular text-[16px] capitalize line-clamp-1"
+                            // className="text-blackText font-cerebriregular text-[16px] capitalize w-[110px] whitespace-nowrap overflow-hidden text-ellipsis"
+                            >
                             {
                                 item?.name
                             } <
                             /div> <
                             /div> <
                             /div> <
                             div >
@@ -1049,15 +1076,17 @@
                                 </span> */
                 } <
                 /div>
 
                 <
                 div > {
                     activeTab === 1 && ( <
-                        div className = "sidebar h-[calc(100vh-358px)] 1xl:h-[calc(100vh-381px)] overflow-auto" > {
+                        div id = "collectionWidth"
+                        className = "sidebar h-[calc(100vh-358px)] 1xl:h-[calc(100vh-381px)] overflow-auto scrollbar" >
+                        {
                             contextFiles?.filesData?.files?.map((val, index) => {
                                 return ( <
                                     div className = {
                                         ` flex items-center justify-between px-3 py-3 mt-1 cursor-pointer overflow-hidden ${
                         val?.guid === contextFiles?.resFileId
                           ? // val?.guid === location?.state?.fileId
                             "bg-[#F6F6F9]"
@@ -1067,14 +1096,15 @@
                                     onClick = {
                                         () => {
                                             handleSelectedFileName(val.name);
                                             contextFiles?.handleFileData(id, val?.guid, val?.magic);
                                             // handleFileData(val?.guid);
                                             contextFiles?.setIsdoc(true);
                                             contextFiles?.setResFileId(val?.guid);
+                                            setIsDrawerOpen(false);
                                             // navigate(`/chatdoc/${id}`, {
                                             //   state: {
                                             //     fileId: val?.guid,
                                             //     fileName: val.name,
                                             //     openChat: true,
                                             //   },
                                             // });
@@ -1112,15 +1142,20 @@
                                         getFileIcon(val?.magic, val?.path)
                                     } <
                                     /span>
 
                                     <
                                     div >
                                     <
-                                    div className = "text-blackText font-cerebriregular text-[14px] capitalize w-[110px] whitespace-nowrap overflow-hidden text-ellipsis" > {
+                                    div
+                                    // style={{ width: textWidth + "px" }}
+                                    className = "text-blackText font-cerebriregular text-[14px] capitalize line-clamp-1"
+                                    // className="text-blackText font-cerebriregular text-[14px] capitalize w-[110px] whitespace-nowrap overflow-hidden text-ellipsis"
+                                    >
+                                    {
                                         val.name
                                     } <
                                     /div> <
                                     /div> <
                                     /div>
 
                                     <
@@ -1183,28 +1218,30 @@
                     )
                 }
 
                 {
                     activeTab === 2 && ( <
                         div className = "sidebar" >
                         <
-                        div className = "font-cerebri w-[-webkit-fill-available] flex flex-col justify-between" >
+                        div id = "collectionWidth"
+                        className = "font-cerebri w-[-webkit-fill-available] flex flex-col justify-between" >
                         <
                         div > {
                             /* <h1 className="text-[21px] font-cerebri text-[#495057] leading-[27px] mt-5 mx-5">
                                                   Chat
                                                 </h1> */
                         } <
                         div className = "text-center my-1.5 px-3" >
                         <
                         button onClick = {
                             () => {
                                 // listData?.setChatHistory(false);
                                 listData?.setChatGuid("");
                                 navigate(`/chatdoc/${contextFiles?.oldChatId}`);
+                                setIsDrawerOpen(false);
                             }
                         }
                         className = "bg-customBgDark text-[#fff] rounded-md w-full px-24 pb-2 pt-3 text-[15px] font-cerebriregular xxl:px-10" >
                         New Chat <
                         /button> <
                         /div> {
                             /* <div className="h-[calc(100vh-247px)] overflow-auto scrollbar"> */ } <
@@ -1316,15 +1353,15 @@
                         <
                         /svg> <
                         span class = "sr-only" > Loading... < /span> <
                         /div> <
                         p title = {
                             fileName
                         }
-                        className = "text-wrap cursor-pointer"
+                        className = "line-clamp-1 cursor-pointer"
                         // className="w-[200px] lg:w-[110px] xl:w-[60px] xxl:w-[100px] truncate cursor-pointer"
                         >
                         {
                             fileName
                         } <
                         /p> <
                         /div>
```

### Comparing `komodo_sdk-0.0.90/website/src/components/chatBot/EnhancedBot.js` & `komodo_sdk-0.0.91/website/src/components/chatBot/EnhancedBot.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/components/document/DocumentSidebar.js` & `komodo_sdk-0.0.91/website/src/components/document/DocumentSidebar.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/contexts/roleContext.js` & `komodo_sdk-0.0.91/website/src/contexts/roleContext.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -23,14 +23,15 @@
 export function RoleStore(props) {
     const [reactSelect, setReactSelect] = useState();
     const [configSelect, setConfigSelect] = useState();
     const [user, setUser] = useState("");
     const [agentList, setAgentList] = useState();
     const [configure, setConfigure] = useState();
     const [list, setList] = useState([]);
+    console.log("list :>> ", list);
     const [chatHistory, setChatHistory] = useState(false);
     const [chatGuid, setChatGuid] = useState("");
     const [chatRes, setChatRes] = useState("");
     const [company, setCompany] = useState("");
     const [agentType, setAgentType] = useState("");
     const [filesData, setFilesData] = useState({});
     const [pdfData, setPdfData] = useState("");
@@ -111,14 +112,15 @@
         } catch (error) {
             console.log("user details get ::error", error);
             ErrorToast(error?.data?.detail || "Something went wrong");
         }
     };
 
     const conversations = async (flag) => {
+        setList([]);
         try {
             const agent = await ApiGet(
                 API_Path.agentConversationsGetUrl(reactSelect?.shortcode)
             );
             if (agent?.status === 200) {
                 let sortedArray = agent?.data.sort((item1, item2) => {
                     return new Date(item2.createdAt) - new Date(item1.createdAt);
@@ -137,15 +139,30 @@
     };
 
     const getUserFiles = async (shortcode) => {
         try {
             const files = await ApiGet(
                 API_Path.collectionsGetCollectionUrl(shortcode)
             );
-            setFilesData(files?.data);
+            // const dataA = await files?.data?.files?.map((v) => {
+            //   return v?.name?.replace(/[_-]/g, " ");
+            // });
+            // console.log("dataA :>> ", dataA);
+            // setFilesData(files?.data);
+            const dataA = await files?.data?.files?.map((v) => {
+                return {
+                    ...v,
+                    name: v?.name?.replace(/[_-]/g, " ")
+                };
+            });
+            console.log("dataA :>> ", dataA);
+            setFilesData({
+                ...files?.data,
+                files: dataA
+            });
             // setFirstPdfData(files?.data?.files[0]);
         } catch (error) {
             console.log("error", error);
         }
     };
 
     const companyData = async () => {
```

### Comparing `komodo_sdk-0.0.90/website/src/images/Ellipsis.gif` & `komodo_sdk-0.0.91/website/src/images/Ellipsis.gif`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/chat.png` & `komodo_sdk-0.0.91/website/src/images/chat.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/chatgpt.png` & `komodo_sdk-0.0.91/website/src/images/chatgpt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/chatimg.png` & `komodo_sdk-0.0.91/website/src/images/chatimg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/chattick.png` & `komodo_sdk-0.0.91/website/src/images/chattick.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/content.png` & `komodo_sdk-0.0.91/website/src/images/content.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/copy.png` & `komodo_sdk-0.0.91/website/src/images/copy.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/doc.png` & `komodo_sdk-0.0.91/website/src/images/doc.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/docprofile.png` & `komodo_sdk-0.0.91/website/src/images/docprofile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/docwave.png` & `komodo_sdk-0.0.91/website/src/images/docwave.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/first.png` & `komodo_sdk-0.0.91/website/src/images/first.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/imgLogo.jpg` & `komodo_sdk-0.0.91/website/src/images/imgLogo.jpg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/login.png` & `komodo_sdk-0.0.91/website/src/images/login.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/pdf.png` & `komodo_sdk-0.0.91/website/src/images/pdf.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/person.png` & `komodo_sdk-0.0.91/website/src/images/person.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/portfolio.png` & `komodo_sdk-0.0.91/website/src/images/portfolio.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/pptLogo.png` & `komodo_sdk-0.0.91/website/src/images/pptLogo.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/profile.png` & `komodo_sdk-0.0.91/website/src/images/profile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/robot.png` & `komodo_sdk-0.0.91/website/src/images/robot.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/sample.pdf` & `komodo_sdk-0.0.91/website/src/images/sample.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/second.png` & `komodo_sdk-0.0.91/website/src/images/second.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/send.png` & `komodo_sdk-0.0.91/website/src/images/send.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/setting.png` & `komodo_sdk-0.0.91/website/src/images/setting.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/summary.png` & `komodo_sdk-0.0.91/website/src/images/summary.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/tik.png` & `komodo_sdk-0.0.91/website/src/images/tik.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/txt.png` & `komodo_sdk-0.0.91/website/src/images/txt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/user.png` & `komodo_sdk-0.0.91/website/src/images/user.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/wave.png` & `komodo_sdk-0.0.91/website/src/images/wave.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/wave1.png` & `komodo_sdk-0.0.91/website/src/images/wave1.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/word.png` & `komodo_sdk-0.0.91/website/src/images/word.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/images/xlsxLogo.png` & `komodo_sdk-0.0.91/website/src/images/xlsxLogo.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/layout/CollectionLayout.js` & `komodo_sdk-0.0.91/website/src/layout/CollectionLayout.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,11 @@
 import React, {
     Children,
     useContext,
+    useEffect,
     useState
 } from "react";
 import Sidebar from "../components/Sidebar";
 import {
     BiMinus
 } from "react-icons/bi";
 import menuIcon from "../assets/Frame.svg";
@@ -81,34 +82,47 @@
 
     const [searchText, setSearchText] = useState("");
     const [isSearchVisible, setIsSearchVisible] = useState(false);
     const [numPages, setNumPages] = useState(null);
     const [isDrawerOpen, setIsDrawerOpen] = useState(false);
     const [selectedCollectionName, setSelectedCollectionName] = useState("");
     const [selectedFileName, setSelectedFileName] = useState("");
+    const [textWidth, setTextWidth] = useState();
+
     // const [filesData, setFilesData] = useState({});
     // console.log("filesData :>> ", filesData);
     const chatCollection = useContext(roleContext);
     const isCollections = chatCollection?.isCollections;
     const setIsCollections = chatCollection?.setIsCollections;
 
     const docs = [{
         uri: pdf
     }];
 
     const toggleDrawer = () => {
         setIsDrawerOpen(!isDrawerOpen);
     };
+    useEffect(() => {
+        setTextWidth(200);
+    }, []);
 
     return ( <
         div className = "flex" >
         <
         PanelGroup autoSaveId = "example"
         direction = "horizontal"
-        className = "panelgroup" >
+        className = "panelgroup"
+        onLayout = {
+            () => {
+                const sidebarWidth = document.getElementById("collectionWidth");
+                if (sidebarWidth) {
+                    setTextWidth(sidebarWidth?.offsetWidth - 110);
+                }
+            }
+        } >
         <
         div className = "z-[999]" >
         <
         img src = {
             menuIcon
         }
         // className="hidden xl:flex w-[24px] h-[24px] m-3"
@@ -147,14 +161,20 @@
         }
         setSelectedCollectionName = {
             setSelectedCollectionName
         }
         setSelectedFileName = {
             setSelectedFileName
         }
+        textWidth = {
+            textWidth
+        }
+        setIsDrawerOpen = {
+            setIsDrawerOpen
+        }
         // setFilesData={setFilesData}
         // filesData={filesData}
         // getUserFiles={getUserFiles}
         /> <
         /Panel> <
         PanelResizeHandle / > {
             /* </div> */ }
@@ -201,14 +221,16 @@
         } {
             children
         } <
         /div> <
         /Panel>
 
         <
+        div className = "xl:block hidden" >
+        <
         Drawer open = {
             isDrawerOpen
         }
         onClose = {
             toggleDrawer
         }
         direction = "left"
@@ -240,19 +262,26 @@
         }
         setSelectedCollectionName = {
             setSelectedCollectionName
         }
         setSelectedFileName = {
             setSelectedFileName
         }
+        textWidth = {
+            textWidth
+        }
+        setIsDrawerOpen = {
+            setIsDrawerOpen
+        }
         // setFilesData={setFilesData}
         // filesData={filesData}
         // getUserFiles={getUserFiles}
         /> <
         /div> <
         /Drawer> <
+        /div> <
         /PanelGroup> <
         /div>
     );
 };
 
 export default CollectionLayout;
```

### Comparing `komodo_sdk-0.0.90/website/src/layout/PrimaryLayout.js` & `komodo_sdk-0.0.91/website/src/layout/PrimaryLayout.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -35,15 +35,15 @@
 }) => {
     const user = JSON.parse(localStorage.getItem("komodoUser"));
     const listData = useContext(roleContext);
     const navigate = useNavigate();
     const modalRef = useRef(null);
     const [deleteChat, setDeleteChat] = useState(false);
     const [deleteChatId, setDeleteChatId] = useState(null);
-    const [textWidth, setTextWidth] = useState()
+    const [textWidth, setTextWidth] = useState();
     const pathname = window.location.hash;
     const match = pathname.match(/\/details\/([^/]+)/);
     const id = match ? match[1] : null;
 
     const handleDetails = (val) => {
         navigate(`/details/${val?.guid}`);
     };
@@ -78,21 +78,25 @@
         if (!["close", "close1"].includes(e?.target?.id)) {
             setDeleteChat(false);
         }
     };
 
     useEffect(() => {
         document.addEventListener("mousedown", handleClickOutside);
-        const sidebarWidth = document.getElementById("sidebarWidth");
-        setTextWidth(200)
+        // const sidebarWidth = document.getElementById("sidebarWidth");
+
         return () => {
             document.removeEventListener("mousedown", handleClickOutside);
         };
     }, []);
 
+    useEffect(() => {
+        setTextWidth(200);
+    });
+
     const formatDate = (date) => {
         const today = new Date();
         const yesterday = new Date(today);
         yesterday.setDate(today.getDate() - 1);
         const valDate = new Date(date);
         if (valDate.toDateString() === today.toDateString()) {
             return "Today";
@@ -172,16 +176,17 @@
         div key = {
             val?.guid
         }
         onClick = {
             () => handleDetails(val)
         }
         className = {
-            `px-5 border-b-[0.5px] border-[#F6F6F9] py-5 text-[#5A636C] text-[14px] leading-[17.78px] flex justify-between items-center font-cerebriregular cursor-pointer ${id === val?.guid ? "bg-[#F6F6F9]" : ""
-        }`
+            `px-5 border-b-[0.5px] border-[#F6F6F9] py-5 text-[#5A636C] text-[14px] leading-[17.78px] flex justify-between items-center font-cerebriregular cursor-pointer ${
+        id === val?.guid ? "bg-[#F6F6F9]" : ""
+      }`
         } >
         <
         div className = "flex items-center gap-3" >
         <
         span className = "bg-customBg p-2 rounded-[5px]" >
         <
         svg xmlns = "http://www.w3.org/2000/svg"
@@ -224,20 +229,17 @@
                                 
                           
                                 <img src={chatListIcon}/>
                             </span> */
         }
 
         <
-        div className = "truncate"
-        style = {
-            {
-                width: textWidth + "px"
-            }
-        }
+        div className = "line-clamp-1"
+        // className="truncate"
+        // style={{ width: textWidth + "px" }}
         onClick = {
             () => setIsDrawerOpen(false)
         } >
         {
             val?.title
         } <
         /div> <
@@ -280,26 +282,27 @@
         <
         PanelGroup autoSaveId = "example"
         direction = "horizontal"
         className = "panelgroup"
         onLayout = {
             () => {
                 const sidebarWidth = document.getElementById("sidebarWidth");
-                setTextWidth(sidebarWidth.offsetWidth - 110)
+                setTextWidth(sidebarWidth.offsetWidth - 110);
             }
         } >
         <
         div className = "z-[999]" >
         <
         img src = {
             menuIcon
         }
         className = {
-            `hidden xl:flex xl:absolute w-[27px] h-[27px] mx-4 my-8 ${isDrawerOpen === true ? "xl:hidden" : ""
-                }`
+            `hidden xl:flex xl:absolute w-[27px] h-[27px] mx-4 my-8 ${
+                isDrawerOpen === true ? "xl:hidden" : ""
+              }`
         }
         // className="hidden lg:flex lg:absolute w-[24px] h-[24px] mx-4 my-8"
         onClick = {
             toggleDrawer
         }
         alt = "" /
         >
@@ -316,15 +319,15 @@
             /* <div className="xl:hidden w-1/5 font-cerebri flex border-r-[0.5px] border-[#CDCDCD]"> */ } <
         Sidebar / >
         <
         div className = "font-cerebri w-[-webkit-fill-available] flex flex-col justify-between" >
         <
         div id = "sidebarWidth" >
         <
-        h1 className = "text-[21px] font-cerebri text-[#495057] leading-[27px] mb-9 mt-5 mx-5" >
+        h1 className = "text-[21px] font-cerebri text-[#495057] leading-[27px] mb-5 mt-5 mx-5" >
         Chat <
         /h1> <
         div className = "text-center" >
         <
         button onClick = {
             () => {
                 listData?.setChatHistory(false);
@@ -355,14 +358,17 @@
         } <
         /h1> <
         /div> <
         /div> <
         /div> <
         /Panel> <
         PanelResizeHandle / >
+
+        <
+        div className = "xl:block hidden" >
         <
         Drawer open = {
             isDrawerOpen
         }
         onClose = {
             toggleDrawer
         }
@@ -416,19 +422,20 @@
         <
         h1 className = "text-[18px] leading-[25.4px] font-cerebri text-[#495057]" > {
             user?.name
         } <
         /h1> <
         /div> <
         /div> <
-        /Drawer>
+        /Drawer> <
+        /div>
 
         <
         Panel defaultSize = {
-            85
+            80
         }
         id = "console-panel" >
         <
         div className = "w-full" > {
             /* <div className="w-4/5 xl:w-full"> */ } <
         Header / > {
             children
```

### Comparing `komodo_sdk-0.0.90/website/src/pages/Document.js` & `komodo_sdk-0.0.91/website/src/pages/Document.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -291,14 +291,16 @@
         <
         DocumentSidebar / >
         <
         /div> {
             /* </Panel>
                       <PanelResizeHandle /> */
         } <
+        div className = "xl:block hidden" >
+        <
         Drawer open = {
             isDrawerOpen
         }
         onClose = {
             toggleDrawer
         }
         direction = "left"
@@ -317,15 +319,16 @@
         }
         alt = "" /
         >
         <
         DocumentSidebar / >
         <
         /div> <
-        /Drawer> {
+        /Drawer> <
+        /div> {
             /* <Panel defaultSize={70} id="console-panel"> */ } <
         div className = "w-full" >
         <
         Header / >
         <
         div className = "flex lg:flex-col" >
         <
```

### Comparing `komodo_sdk-0.0.90/website/src/pages/chatBot.js` & `komodo_sdk-0.0.91/website/src/pages/chatBot.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -58,14 +58,25 @@
 } from "react-excel-renderer";
 import {
     Panel,
     PanelGroup,
     PanelResizeHandle
 } from "react-resizable-panels";
 import DocumentView from "../components/DocumentView";
+import {
+    HiDocumentText
+} from "react-icons/hi";
+import {
+    Box,
+    Modal
+} from "@mui/material";
+import {
+    IoClose
+} from "react-icons/io5";
+
 
 // import {
 //   Document,
 //   Page,
 //   Text,
 //   View,
 //   StyleSheet,
@@ -85,19 +96,19 @@
 // });
 
 const style = {
     position: "absolute",
     top: "50%",
     left: "50%",
     transform: "translate(-50%, -50%)",
-    width: "fit-content",
+    width: "80%",
     bgcolor: "#fff",
     boxShadow: 20,
     // p: 4,
-    borderRadius: "20px",
+    // borderRadius: "20px",
     outline: "none",
 };
 
 const ChatBot = () => {
     // "https://nett.umich.edu/sites/default/files/docs/pdf_files_scan_create_reducefilesize.pdf"
     // "https://medicine-storage.s3.ap-southeast-2.amazonaws.com/pdfs/p9973001.pdf"
 
@@ -147,14 +158,15 @@
     const [searchText, setSearchText] = useState("");
     const [isSearchVisible, setIsSearchVisible] = useState(false);
     const [numPages, setNumPages] = useState(null);
     const [isDrawerOpen, setIsDrawerOpen] = useState(false);
     const [selectedCollectionName, setSelectedCollectionName] = useState("");
     const [selectedFileName, setSelectedFileName] = useState("");
     const [filesData, setFilesData] = useState({});
+
     const contextFiles = useContext(roleContext);
     const handleDelete = (chatId, e) => {
         e.stopPropagation();
         setDeleteChat(true);
         setDeleteChatId(chatId);
     };
 
@@ -463,22 +475,52 @@
         } <
         Panel defaultSize = {
             50
         }
         id = "sources-explorer-panel"
         // className="min-w-[30%]"
         className = {
-            `xl:border-l xl:border-[#E8E9EA] ${
-                contextFiles?.isDoc === true
-                  ? // location?.state?.openChat === true
-                    "min-w-[30%] xl:w-full"
-                  : "min-w-full"
-              }`
+            `xl:border-l xl:border-[#E8E9EA] ${contextFiles?.isDoc === true
+                ? // location?.state?.openChat === true
+                "min-w-[30%] xl:w-full"
+                : "min-w-full"
+                }`
+        } >
+        <
+        div className = {
+            `${contextFiles?.isDoc === true
+                ?
+                "block"
+                : "hidden"
+                }`
+        } >
+        <
+        div className = "hidden lg:block absolute top-6 right-7 z-10 text-[40px] cursor-pointer  bg-customColor p-2 rounded-full"
+        onClick = {
+            handleOpen
         } >
         {
+            /* <HiDocumentText /> */ } <
+        svg xmlns = "http://www.w3.org/2000/svg"
+        width = "26"
+        height = "26"
+        viewBox = "0 0 26 26"
+        fill = "none" >
+        <
+        path d = "M22.4359 8.79666V18.9908C22.4359 21.6558 20.2584 23.8333 17.5934 23.8333H8.40671C5.74171 23.8333 3.56421 21.6558 3.56421 18.9908V8.79666C3.56421 6.94416 4.60421 5.32999 6.13171 4.51749C6.66254 4.23583 7.32338 4.61499 7.32338 5.22166C7.32338 6.94416 8.73171 8.35249 10.4542 8.35249H15.5459C17.2684 8.35249 18.6767 6.94416 18.6767 5.22166C18.6767 4.61499 19.3267 4.23583 19.8684 4.51749C21.3959 5.32999 22.4359 6.94416 22.4359 8.79666Z"
+        fill = "white" /
+        >
+        <
+        path d = "M15.5459 2.16667H10.4542C9.32757 2.16667 8.40674 3.07667 8.40674 4.20334V5.22167C8.40674 6.34834 9.31674 7.25834 10.4434 7.25834H15.5459C16.6726 7.25834 17.5826 6.34834 17.5826 5.22167V4.20334C17.5934 3.07667 16.6726 2.16667 15.5459 2.16667Z"
+        fill = "white" /
+        >
+        <
+        /svg> <
+        /div> <
+        /div> {
             /* <div className="col-span-1 xl:border-l xl:border-[#E8E9EA]"> */ } <
         Chat selectedItemName = {
             location?.state?.collectionName
         }
         // selectedItemName={selectedCollectionName}
         selectedFileName = {
             selectedFileName
@@ -497,24 +539,23 @@
                       > */
         } <
         Panel defaultSize = {
             50
         }
         id = "console-panel"
         className = {
-            `border-l border-[#E8E9EA] ${
-                contextFiles?.isDoc === true
-                  ? // location?.state?.openChat === true
-                    "w-[50%] block xl:w-full"
-                  : "hidden"
-              }`
+            `border-l border-[#E8E9EA] ${contextFiles?.isDoc === true
+                ? // location?.state?.openChat === true
+                "w-[50%] block xl:w-full"
+                : "hidden"
+                }`
         } >
         {
             /* <div className="col-span-1 border-l border-[#E8E9EA]"> */ } <
-        DocumentView / > {
+        DocumentView foo = "bar" / > {
             /* <div
                             className={`bg-[#FFFFFF] h-[calc(100vh-93px)] overflow-auto scrollbarCustom px-3 `}
                           >
                             {contextFiles?.pdfURL ? (
                               contextFiles?.pdfURL?.rows && contextFiles?.pdfURL?.cols ? (
                                 <OutTable
                                   data={contextFiles?.pdfURL?.rows || []}
@@ -926,15 +967,51 @@
                             </Drawer>
                           </div>
                         </div> */
         } {
             /* </div> */ } <
         /Panel> <
         /PanelGroup> <
+        /div>
+
+
+        <
+        Modal open = {
+            open
+        }
+        onClose = {
+            handleClose
+        }
+        aria - labelledby = "modal-modal-title"
+        aria - describedby = "modal-modal-description" >
+        <
+        Box sx = {
+            style
+        } >
+        <
+        div className = "flex justify-between items-center font-cerebri text-[18px] text-[#3C3C3C] mb-2 p-5" >
+        <
+        div >
+        File Preview <
         /div> <
+        div onClick = {
+            handleClose
+        }
+        className = "text-[25px]" >
+        <
+        IoClose / >
+        <
+        /div> <
+        /div> <
+        DocumentView foo = "bar" / >
+        <
+        /Box> <
+        /Modal>
+
+        <
         /CollectionLayout>
 
         <
         style > {
             `
         .EZDrawer__overlay {
           background-color: transparent !important;
```

### Comparing `komodo_sdk-0.0.90/website/src/pages/chat/Chat.js` & `komodo_sdk-0.0.91/website/src/pages/chat/Chat.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -106,19 +106,19 @@
                     ...prevData, {
                         sender: user.email,
                         text: prompt
                     },
                 ]);
             }
             setText(prompt);
+            setSend(true);
+            setApiActive(true);
         }
         setPrompt("");
         scrollToBottom();
-        setSend(true);
-        setApiActive(true);
     };
 
     const handleKeyPress = (e) => {
         if (e.key === "Enter" && !e.shiftKey) {
             sendPrompt();
             e.preventDefault();
         }
@@ -151,16 +151,15 @@
                 div ref = {
                     chatContainerRef
                 }
                 className = "mt-10 mx-8 overflow-y-auto h-[calc(100vh-217px)] scrollbar w-[1017px] xl:w-[950px] lg:w-[800px] md:w-full md:mx-4 sm:mx-2 lg:px-4"
                 // className="mt-10 mx-8 overflow-y-auto h-[700px] scrollbar w-[1017px] xl:w-[950px] lg:w-[800px] md:w-full md:mx-4 sm:mx-2"
                 >
                 {
-                    allChatData &&
-                    allChatData.length &&
+                    allChatData && allChatData.length ?
                     allChatData.map((val, i) => {
                         return ( <
                             div className = "mb-5"
                             key = {
                                 i
                             } > {
                                 val?.sender === user?.email && ( <
@@ -168,15 +167,15 @@
                                     <
                                     div >
                                     <
                                     img src = {
                                         profile
                                     }
                                     alt = "profile"
-                                    className = "w-[30px] h-[30px]" /
+                                    className = "min-w-[30px] max-w-[30px] h-[30px]" /
                                     >
                                     <
                                     /div> <
                                     div className = "text-[15px] font-cerebriregular rounded-md bg-customBg px-4 py-3 text-customColor" > {
                                         val?.text
                                     } <
                                     /div> <
@@ -212,15 +211,16 @@
                                         /div> <
                                         /div> <
                                         /div>
                                     )
                             } <
                             /div>
                         );
-                    })
+                    }) :
+                        null
                 } {
                     text !== "" && ( <
                         div className = "mb-7" >
                         <
                         div >
                         <
                         div className = "flex gap-5" >
@@ -306,15 +306,21 @@
                                           className="cursor-pointer w-[44px] h-[43px]"
                                         /> */
                 }
 
                 <
                 div > {
                     !send ? ( <
-                        div className = "cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2 pr-3.5"
+                        div className = {
+                            `${
+                            prompt.trim() !== ""
+                              ? "bg-customBgDark cursor-pointer"
+                              : "bg-slate-400"
+                          }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2 pr-3.5`
+                        }
                         onClick = {
                             sendPrompt
                         } >
                         <
                         RiSendPlaneFill className = "text-[21px] rotate-45" / >
                         <
                         /div>
@@ -368,15 +374,22 @@
                 }
                 className = "border border-[#CFD4D8] rounded-md px-4 pt-3 pb-[10px] text-[15px] font-cerebriregular leading-[19.05px] outline-none w-full" /
                 >
 
                 <
                 div > {
                     !send ? ( <
-                        div className = "cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2 pr-3.5"
+                        div className = {
+                            `${
+                          prompt.trim() !== ""
+                            ? "bg-customBgDark cursor-pointer"
+                            : "bg-slate-400"
+                        }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2 pr-3.5`
+                        }
+                        // className="cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2 pr-3.5"
                         onClick = {
                             sendPrompt
                         } >
                         <
                         RiSendPlaneFill className = "text-[21px] rotate-45" / >
                         <
                         /div>
```

### Comparing `komodo_sdk-0.0.90/website/src/pages/chat/Details.js` & `komodo_sdk-0.0.91/website/src/pages/chat/Details.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -111,19 +111,21 @@
                     ...prevData, {
                         sender: user.email,
                         text: prompt
                     },
                 ]);
             }
             setText(prompt);
+            setSend(true);
+            setApiActive(true);
         }
         setPrompt("");
         scrollToBottom();
-        setSend(true);
-        setApiActive(true);
+        // setSend(true);
+        // setApiActive(true);
     };
 
     const handleKeyPress = (e) => {
         if (e.key === "Enter" && !e.shiftKey) {
             sendPrompt();
             e.preventDefault();
             sendMessage();
@@ -165,15 +167,15 @@
                                         <
                                         div >
                                         <
                                         img src = {
                                             profile
                                         }
                                         alt = "profile"
-                                        className = "w-[30px] h-[30px]" /
+                                        className = "min-w-[30px] max-w-[30px] h-[30px]" /
                                         >
                                         <
                                         /div> <
                                         div className = "text-[15px] font-cerebriregular rounded-md bg-customBg px-4 py-3 text-customColor" > {
                                             val?.text
                                         } <
                                         /div> <
@@ -292,15 +294,21 @@
             handleKeyPress
         }
         className = "w-[892px] xl:w-[700px] border border-[#CFD4D8] rounded-md px-4 pt-[13px] pb-[10px] text-[14px] font-cerebriregular leading-[17.78px] outline-none flex justify-center items-center" /
         >
         <
         div > {
             !send ? ( <
-                div className = "cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2 pr-3.5"
+                div className = {
+                    `${
+                  prompt.trim() !== ""
+                    ? "bg-customBgDark cursor-pointer"
+                    : "bg-slate-400"
+                }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2 pr-3.5`
+                }
                 onClick = {
                     sendPrompt
                 } >
                 <
                 RiSendPlaneFill className = "text-[21px] rotate-45" / >
                 <
                 /div>
```

### Comparing `komodo_sdk-0.0.90/website/src/pages/pricing/Pricing.jsx` & `komodo_sdk-0.0.91/website/src/pages/pricing/Pricing.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/pages/privacy/Privacy.jsx` & `komodo_sdk-0.0.91/website/src/pages/privacy/Privacy.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/pages/privacy/Terms.jsx` & `komodo_sdk-0.0.91/website/src/pages/privacy/Terms.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/pages/profile/Profile.jsx` & `komodo_sdk-0.0.91/website/src/pages/profile/Profile.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/website/src/pages/settings/Settings.jsx` & `komodo_sdk-0.0.91/website/src/pages/settings/Settings.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/.gitignore` & `komodo_sdk-0.0.91/.gitignore`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.90/pyproject.toml` & `komodo_sdk-0.0.91/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "komodo-sdk"
-version = "0.0.90"
+version = "0.0.91"
 authors = [
     { name = "Ryan Oberoi", email = "ryan.oberoi@komodoapp.ai" },
 ]
 description = "Komodo SDK"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `komodo_sdk-0.0.90/PKG-INFO` & `komodo_sdk-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: komodo-sdk
-Version: 0.0.90
+Version: 0.0.91
 Summary: Komodo SDK
 Project-URL: Homepage, https://github.com/Komodo-AI/komodo-sdk.git
 Author-email: Ryan Oberoi <ryan.oberoi@komodoapp.ai>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: aiofiles~=23.2.1
```

