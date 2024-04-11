# Comparing `tmp/komodo_sdk-0.0.91.tar.gz` & `tmp/komodo_sdk-0.0.92.tar.gz`

## Comparing `komodo_sdk-0.0.91.tar` & `komodo_sdk-0.0.92.tar`

### file list

```diff
@@ -1,443 +1,443 @@
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/.dockerignore
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/requirements.txt
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/.github/workflows/deploy-all.yml
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/.github/workflows/publish-container.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/README.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/config.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/chatdoc_agent.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/collection_builder.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/coordinator_agent.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/default.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/difference_agent.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/echo_agent.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/elastic_agent.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/groot_agent.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/librarian_agent.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/mongo_agent.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/pdf_generator.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/sample_agent.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/summarizer_agent.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/translator_agent.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/agents/widget_builder_agent.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/sources/filesystem.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/sources/s3bucketkey.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/sources/webpages.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/sources/website_crawler.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_connect.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_count.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_get.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_search.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/collection_builder.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/collection_lister.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/collection_reader.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/directory_reader.py
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/file_reader.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/files/file_writer.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/markets/polygon_search.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_connect.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_databases.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_query.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_schema.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_unique.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/search/vector_search.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/search/vector_search_runtime.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/utils/agent_tool.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/utils/sample_tool.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/utils/thought_tool.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/utils/workflow_tool.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/web/data_fetcher.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/web/serpapi_search.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/web/tavily_search.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/tools/web/web_scraper.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/utils/agent_helper.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/utils/indexer.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/utils/play.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/utils/rag_context.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/vector_stores/pinecone_store.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/vector_stores/qdrant_store.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/vector_stores/vector_store_helper.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/core/workflows/sample_workflow.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/agents/planner/personal_finance_profile.yml
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/appliances/citibank/personal_finance_profile.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/appliances/komodo/dir1/hello.txt
--rw-r--r--   0        0        0  1139092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/data/workflows/analyzer/personal_finance_profile.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/checker/agent.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/checker/context.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/checker/dictionary.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/checker/instructions.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/agent.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/context.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/instructions.txt
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/role.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/tools/income_calculator.yml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/tools/income_contributions.yml
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/citibank/appliance.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/komodo/appliance.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/sample/appliance.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/sample/context.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/sample/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/appliances/sample/instructions.txt
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/context.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/instructions.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/workflow.yml
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_agent.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_app.py
--rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_collection.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_config.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_context.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_datasource.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_features.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_locations.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_runnable.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_runtime.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_tool.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_tool_registry.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_user.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_vector.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_vectorstore.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/framework/komodo_workflow.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/database/agent_loader.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/database/appliance_loader.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/database/tool_loader.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/database/user_loader.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/agent_loader.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/appliance_loader.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/loader_helper.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/loader_locations.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/loaders/filesystem/workflow_loader.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/azure/azure.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/azure/azure_openai.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_claude.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_cohere.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_model.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_titan.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/agent_runner.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/appliance_utils.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/chat_message.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/chat_metadata.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/model_request.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/model_response.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/models.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/responder.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/workflow_executor.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/workflow_runner.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/framework/workflow_selector.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_api.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_api_streamed.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_api_streamed_tool_call.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_completion.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_debug.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/models/openai/openai_process_actions.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/collection.proto
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/data.proto
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/model.proto
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/report.proto
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/sample.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/collection_pb2.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/collection_pb2.pyi
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/data_pb2.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/data_pb2.pyi
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/model_pb2.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/model_pb2.pyi
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/report_pb2.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/proto/generated/report_pb2.pyi
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_agent_runner.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_agent_runner_2.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_difference_agent.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_librarian_agent.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_sample_agent.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_streaming_test.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/scripts/run_widget_builder.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/agent_router.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/appliance_router.py
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/ask_request.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/audio_router.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/collections_router.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/conversation_router.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/fast.py
--rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/globals.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/logo_router.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/report_router.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/server/user_router.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/directory/assistants_helpers.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/file_writer_helper.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/text_convert_helper.py
--rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/text_extract.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/text_extract_helper.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/documents/text_html.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/embeddings/faiss_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/embeddings/openai.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/embeddings/pinecone_store.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/mssql/mssql.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/api_query.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/digest.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/filestats.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/globber.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/hidden_prints.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/lambda_entry.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/lambda_utils.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/logconfig.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/pathutils.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/s3_file_utils.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/sentry_utils.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/switchdir.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/tags.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/term_colors.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/timebox.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/shared/utils/watcher.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/agent_store.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/appliance_store.py
--rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/collection_store.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/conversations_store.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/logo_store.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/proto_utils.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/redis_database.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/tool_store.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/store/user_store.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_elastic_agent.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_elastic_sample.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_elastic_tools.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_groot_agent.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_mongo_agent.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_mongo_sample.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_mongo_tools.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/core/test_serpapi_search.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/models/test_azure.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/models/test_bedrock.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/models/test_openai.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/models/test_workflow_runner.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/shared/test_mssql.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/komodo/tests/store/test_conversation_store.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/Dockerfile
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/docker-compose.yml
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/server.py
--rw-r--r--   0        0        0   480357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/data/sample.html
--rw-r--r--   0        0        0   599041 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pdf2html/data/sample.pdf
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/Dockerfile
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/README.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/docker-compose.yml
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/docker-production.yml
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/appliance.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/config.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/seed.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/server.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/appliance/workflow.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/agents/dasher_v1/agent.yml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/agents/dasher_v1/instructions.txt
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/agents/dasher_v2/agent.yml
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/agents/dasher_v2/instructions.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/definitions/appliances/sample/appliance.yml
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/app.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/globals.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/server.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/themes.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/assets/custom.css
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/agent.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/analytics.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/appliance.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/archive.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/dasher_v1.py
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/dasher_v2.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/department.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/home.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/not_found_404.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/present.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/report.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/side_bar.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/topic_1.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/reports/bar_chart.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/reports/line_chart.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/sample/widgets/pages/reports/pie_chart.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/.gitignore
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/Dockerfile
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/README.md
--rw-r--r--   0        0        0   953941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/package-lock.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/package.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/tailwind.config.js
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/deployment/nginx.default.conf
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/chaticon.png
--rw-r--r--   0        0        0    66364 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/faqbg.png
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/favicon.ico
--rw-r--r--   0        0        0    84772 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/footer.png
--rw-r--r--   0        0        0   230014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/home.png
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/index.html
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/logo192.png
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/logo512.png
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/manifest.json
--rw-r--r--   0        0        0   318284 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/pricingBg.png
--rw-r--r--   0        0        0   189260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/pricingBg1.png
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/robots.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Read Me.txt
--rw-r--r--   0        0        0    84336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf
--rw-r--r--   0        0        0   291948 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf
--rw-r--r--   0        0        0    80288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf
--rw-r--r--   0        0        0   275104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf
--rw-r--r--   0        0        0    85092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf
--rw-r--r--   0        0        0   291180 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf
--rw-r--r--   0        0        0    80172 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf
--rw-r--r--   0        0        0   273580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf
--rw-r--r--   0        0        0    82008 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf
--rw-r--r--   0        0        0   418296 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf
--rw-r--r--   0        0        0    78624 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf
--rw-r--r--   0        0        0   411148 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf
--rw-r--r--   0        0        0    81940 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf
--rw-r--r--   0        0        0   279500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf
--rw-r--r--   0        0        0    78360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf
--rw-r--r--   0        0        0   257728 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf
--rw-r--r--   0        0        0    78480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf
--rw-r--r--   0        0        0   313920 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf
--rw-r--r--   0        0        0    82916 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf
--rw-r--r--   0        0        0   367128 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf
--rw-r--r--   0        0        0    79536 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf
--rw-r--r--   0        0        0   349188 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf
--rw-r--r--   0        0        0    83092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf
--rw-r--r--   0        0        0   309704 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf
--rw-r--r--   0        0        0    79480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf
--rw-r--r--   0        0        0   291444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf
--rw-r--r--   0        0        0    81828 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf
--rw-r--r--   0        0        0   331432 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf
--rw-r--r--   0        0        0    83560 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf
--rw-r--r--   0        0        0   301516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf
--rw-r--r--   0        0        0    79800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf
--rw-r--r--   0        0        0   283064 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    79864 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf
--rw-r--r--   0        0        0   459400 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf
--rw-r--r--   0        0        0    77840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf
--rw-r--r--   0        0        0   455000 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/App.css
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/App.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/App.test.js
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/RouterMain.js
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/index.css
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/index.js
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/logo.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/reportWebVitals.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/setupTests.js
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/API/API_data.js
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/API/ApiComment.js
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/Frame.svg
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/ai.png
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/arrowLeft.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/aubergine.png
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/barbra.svg
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/blue.svg
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/blueTick.svg
--rw-r--r--   0        0        0  1709204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/botAvatar.svg
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/chatListIcon.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/clementine.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/close.svg
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/docs.svg
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/docx.png
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/folder.svg
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/gallery.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/gray.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/green.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/grey.svg
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/headphone.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/indigo.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/jade.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/lagoon.svg
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/magicpen-1.svg
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/magicpen.svg
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/message.svg
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/multi.png
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/odt.png
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/orange.png
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/parrot.svg
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/pdf.png
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/pdf.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/pink.svg
--rw-r--r--   0        0        0   378813 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/pricingBg.png
--rw-r--r--   0        0        0    48909 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/profile.png
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/send.png
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/setting-1.svg
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/setting.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/sky.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/square.svg
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/text.png
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/text.svg
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/trash.svg
--rw-r--r--   0        0        0  1884519 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/userProfile.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/assets/yellow.svg
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/auth/Login.js
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/auth/Signup.js
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/ChartDashboard.js
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/Dashboard.js
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/DocumentView.js
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/Header.js
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/HeaderSideBar.js
--rw-r--r--   0        0        0    20984 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/Home.jsx
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/LayoutHeader.js
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/NavigateBack.js
--rw-r--r--   0        0        0    36368 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/Sidebar.js
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/DocumentBox/Table.js
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chat/Chat.js
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chat/Details.js
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chat/EnhancedPrompt.js
--rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chatBot/Chat.js
--rw-r--r--   0        0        0    15498 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chatBot/ChatBotById.js
--rw-r--r--   0        0        0    64401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chatBot/ChatBotSideBar.js
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/chatBot/EnhancedBot.js
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/document/DocumentSidebar.js
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/helpers/Toast.js
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/components/inputs/CustomInputs.jsx
--rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/contexts/roleContext.js
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/helpers/Toast.js
--rw-r--r--   0        0        0    33366 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/Ellipsis.gif
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/chat.png
--rw-r--r--   0        0        0   214322 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/chatgpt.png
--rw-r--r--   0        0        0   101078 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/chatimg.png
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/chattick.png
--rw-r--r--   0        0        0    21789 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/content.png
--rw-r--r--   0        0        0    53673 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/copy.png
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/doc.png
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/docprofile.png
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/docwave.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/dots.png
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/dummy.txt
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/first.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/homemenu.png
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/imgLogo.jpg
--rw-r--r--   0        0        0   371173 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/login.png
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/pdf.png
--rw-r--r--   0        0        0   177241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/person.png
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/portfolio.png
--rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/pptLogo.png
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/profile.png
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/robot.png
--rw-r--r--   0        0        0    96034 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/sample.pdf
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/second.png
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/send.png
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/setting.png
--rw-r--r--   0        0        0    61070 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/summary.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/tick.png
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/tik.png
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/txt.png
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/upload.png
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/upload2.png
--rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/user.png
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/wave.png
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/wave1.png
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/word.png
--rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/images/xlsxLogo.png
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/layout/CollectionLayout.js
--rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/layout/PrimaryLayout.js
--rw-r--r--   0        0        0    32803 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/Document.js
--rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/chatBot.js
--rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/chat/Chat.js
--rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/chat/Details.js
--rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/pricing/Pricing.jsx
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/privacy/Privacy.jsx
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/privacy/Terms.jsx
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/profile/Profile.jsx
--rw-r--r--   0        0        0    23023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/website/src/pages/settings/Settings.jsx
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/.gitignore
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/README.md
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/pyproject.toml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.91/PKG-INFO
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/.dockerignore
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/requirements.txt
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/.github/workflows/deploy-all.yml
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/.github/workflows/publish-container.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/README.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/config.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/chatdoc_agent.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/collection_builder.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/coordinator_agent.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/default.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/difference_agent.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/echo_agent.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/elastic_agent.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/groot_agent.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/librarian_agent.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/mongo_agent.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/pdf_generator.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/sample_agent.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/summarizer_agent.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/translator_agent.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/widget_builder_agent.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/sources/filesystem.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/sources/s3bucketkey.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/sources/webpages.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/sources/website_crawler.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_connect.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_count.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_get.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_search.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/collection_builder.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/collection_lister.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/collection_reader.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/directory_reader.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/file_reader.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/file_writer.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/markets/polygon_search.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_connect.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_databases.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_query.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_schema.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_unique.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/search/vector_search.py
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/search/vector_search_runtime.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/utils/agent_tool.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/utils/sample_tool.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/utils/thought_tool.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/utils/workflow_tool.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/web/data_fetcher.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/web/serpapi_search.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/web/tavily_search.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/web/web_scraper.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/utils/agent_helper.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/utils/indexer.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/utils/play.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/utils/rag_context.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/vector_stores/pinecone_store.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/vector_stores/qdrant_store.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/vector_stores/vector_store_helper.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/workflows/sample_workflow.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/agents/planner/personal_finance_profile.yml
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/appliances/citibank/personal_finance_profile.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/appliances/komodo/dir1/hello.txt
+-rw-r--r--   0        0        0  1139092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/workflows/analyzer/personal_finance_profile.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/checker/agent.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/checker/context.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/checker/dictionary.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/checker/instructions.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/agent.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/context.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/instructions.txt
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/role.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/tools/income_calculator.yml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/tools/income_contributions.yml
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/citibank/appliance.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/komodo/appliance.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/sample/appliance.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/sample/context.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/sample/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/sample/instructions.txt
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/context.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/instructions.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/workflow.yml
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_agent.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_app.py
+-rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_collection.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_config.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_context.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_datasource.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_features.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_locations.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_runnable.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_runtime.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_tool.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_tool_registry.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_user.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_vector.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_vectorstore.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_workflow.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/database/agent_loader.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/database/appliance_loader.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/database/tool_loader.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/database/user_loader.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/agent_loader.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/appliance_loader.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/loader_helper.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/loader_locations.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/workflow_loader.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/azure/azure.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/azure/azure_openai.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_claude.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_cohere.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_model.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_titan.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/agent_runner.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/appliance_utils.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/chat_message.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/chat_metadata.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/model_request.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/model_response.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/models.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/responder.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/workflow_executor.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/workflow_runner.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/workflow_selector.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_api.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_api_streamed.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_api_streamed_tool_call.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_completion.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_debug.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_process_actions.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/collection.proto
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/data.proto
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/model.proto
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/report.proto
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/sample.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/collection_pb2.py
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/collection_pb2.pyi
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/data_pb2.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/data_pb2.pyi
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/model_pb2.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/model_pb2.pyi
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/report_pb2.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/report_pb2.pyi
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_agent_runner.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_agent_runner_2.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_difference_agent.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_librarian_agent.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_sample_agent.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_streaming_test.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_widget_builder.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/agent_router.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/appliance_router.py
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/ask_request.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/audio_router.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/collections_router.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/conversation_router.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/fast.py
+-rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/globals.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/logo_router.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/report_router.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/user_router.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/directory/assistants_helpers.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/file_writer_helper.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/text_convert_helper.py
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/text_extract.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/text_extract_helper.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/text_html.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/embeddings/faiss_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/embeddings/openai.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/embeddings/pinecone_store.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/mssql/mssql.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/api_query.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/digest.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/filestats.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/globber.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/hidden_prints.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/lambda_entry.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/lambda_utils.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/logconfig.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/pathutils.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/s3_file_utils.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/sentry_utils.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/switchdir.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/tags.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/term_colors.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/timebox.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/watcher.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/agent_store.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/appliance_store.py
+-rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/collection_store.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/conversations_store.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/logo_store.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/proto_utils.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/redis_database.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/tool_store.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/user_store.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_elastic_agent.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_elastic_sample.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_elastic_tools.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_groot_agent.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_mongo_agent.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_mongo_sample.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_mongo_tools.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_serpapi_search.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/models/test_azure.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/models/test_bedrock.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/models/test_openai.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/models/test_workflow_runner.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/shared/test_mssql.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/store/test_conversation_store.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/Dockerfile
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/docker-compose.yml
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/server.py
+-rw-r--r--   0        0        0   480357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/data/sample.html
+-rw-r--r--   0        0        0   599041 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/data/sample.pdf
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/Dockerfile
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/README.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/docker-compose.yml
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/docker-production.yml
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/appliance.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/config.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/seed.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/server.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/workflow.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/agents/dasher_v1/agent.yml
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/agents/dasher_v1/instructions.txt
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/agents/dasher_v2/agent.yml
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/agents/dasher_v2/instructions.txt
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/appliances/sample/appliance.yml
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/app.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/globals.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/server.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/themes.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/assets/custom.css
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/agent.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/analytics.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/appliance.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/archive.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/dasher_v1.py
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/dasher_v2.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/department.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/home.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/not_found_404.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/present.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/report.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/side_bar.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/topic_1.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/reports/bar_chart.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/reports/line_chart.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/reports/pie_chart.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/Dockerfile
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/README.md
+-rw-r--r--   0        0        0   953941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/package-lock.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/package.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/tailwind.config.js
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/deployment/nginx.default.conf
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/chaticon.png
+-rw-r--r--   0        0        0    66364 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/faqbg.png
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/favicon.ico
+-rw-r--r--   0        0        0    84772 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/footer.png
+-rw-r--r--   0        0        0   230014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/home.png
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/index.html
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/logo192.png
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/logo512.png
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/manifest.json
+-rw-r--r--   0        0        0   318284 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/pricingBg.png
+-rw-r--r--   0        0        0   189260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/pricingBg1.png
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/robots.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Read Me.txt
+-rw-r--r--   0        0        0    84336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf
+-rw-r--r--   0        0        0   291948 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf
+-rw-r--r--   0        0        0    80288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf
+-rw-r--r--   0        0        0   275104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf
+-rw-r--r--   0        0        0    85092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf
+-rw-r--r--   0        0        0   291180 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf
+-rw-r--r--   0        0        0    80172 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf
+-rw-r--r--   0        0        0   273580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf
+-rw-r--r--   0        0        0    82008 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf
+-rw-r--r--   0        0        0   418296 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf
+-rw-r--r--   0        0        0    78624 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf
+-rw-r--r--   0        0        0   411148 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf
+-rw-r--r--   0        0        0    81940 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf
+-rw-r--r--   0        0        0   279500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf
+-rw-r--r--   0        0        0    78360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf
+-rw-r--r--   0        0        0   257728 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf
+-rw-r--r--   0        0        0    78480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf
+-rw-r--r--   0        0        0   313920 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf
+-rw-r--r--   0        0        0    82916 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf
+-rw-r--r--   0        0        0   367128 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf
+-rw-r--r--   0        0        0    79536 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf
+-rw-r--r--   0        0        0   349188 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf
+-rw-r--r--   0        0        0    83092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf
+-rw-r--r--   0        0        0   309704 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf
+-rw-r--r--   0        0        0    79480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf
+-rw-r--r--   0        0        0   291444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf
+-rw-r--r--   0        0        0    81828 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf
+-rw-r--r--   0        0        0   331432 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf
+-rw-r--r--   0        0        0    83560 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf
+-rw-r--r--   0        0        0   301516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf
+-rw-r--r--   0        0        0    79800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf
+-rw-r--r--   0        0        0   283064 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    79864 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf
+-rw-r--r--   0        0        0   459400 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf
+-rw-r--r--   0        0        0    77840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf
+-rw-r--r--   0        0        0   455000 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/App.css
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/App.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/App.test.js
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/RouterMain.js
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/index.css
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/index.js
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/logo.svg
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/reportWebVitals.js
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/setupTests.js
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/API/API_data.js
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/API/ApiComment.js
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/Frame.svg
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/ai.png
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/arrowLeft.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/aubergine.png
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/barbra.svg
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/blue.svg
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/blueTick.svg
+-rw-r--r--   0        0        0  1709204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/botAvatar.svg
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/chatListIcon.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/clementine.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/close.svg
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/docs.svg
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/docx.png
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/folder.svg
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/gallery.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/gray.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/green.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/grey.svg
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/headphone.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/indigo.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/jade.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/lagoon.svg
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/magicpen-1.svg
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/magicpen.svg
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/message.svg
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/multi.png
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/odt.png
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/orange.png
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/parrot.svg
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/pdf.png
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/pdf.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/pink.svg
+-rw-r--r--   0        0        0   378813 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/pricingBg.png
+-rw-r--r--   0        0        0    48909 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/profile.png
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/send.png
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/setting-1.svg
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/setting.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/sky.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/square.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/text.png
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/text.svg
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/trash.svg
+-rw-r--r--   0        0        0  1884519 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/userProfile.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/yellow.svg
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/auth/Login.js
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/auth/Signup.js
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/ChartDashboard.js
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/Dashboard.js
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/DocumentView.js
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/Header.js
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/HeaderSideBar.js
+-rw-r--r--   0        0        0    20984 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/Home.jsx
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/LayoutHeader.js
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/NavigateBack.js
+-rw-r--r--   0        0        0    36368 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/Sidebar.js
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/DocumentBox/Table.js
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chat/Chat.js
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chat/Details.js
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chat/EnhancedPrompt.js
+-rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chatBot/Chat.js
+-rw-r--r--   0        0        0    15498 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chatBot/ChatBotById.js
+-rw-r--r--   0        0        0    64401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chatBot/ChatBotSideBar.js
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chatBot/EnhancedBot.js
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/document/DocumentSidebar.js
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/helpers/Toast.js
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/inputs/CustomInputs.jsx
+-rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/contexts/roleContext.js
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/helpers/Toast.js
+-rw-r--r--   0        0        0    33366 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/Ellipsis.gif
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/chat.png
+-rw-r--r--   0        0        0   214322 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/chatgpt.png
+-rw-r--r--   0        0        0   101078 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/chatimg.png
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/chattick.png
+-rw-r--r--   0        0        0    21789 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/content.png
+-rw-r--r--   0        0        0    53673 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/copy.png
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/doc.png
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/docprofile.png
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/docwave.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/dots.png
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/dummy.txt
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/first.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/homemenu.png
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/imgLogo.jpg
+-rw-r--r--   0        0        0   371173 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/login.png
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/pdf.png
+-rw-r--r--   0        0        0   177241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/person.png
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/portfolio.png
+-rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/pptLogo.png
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/profile.png
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/robot.png
+-rw-r--r--   0        0        0    96034 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/sample.pdf
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/second.png
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/send.png
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/setting.png
+-rw-r--r--   0        0        0    61070 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/summary.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/tick.png
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/tik.png
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/txt.png
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/upload.png
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/upload2.png
+-rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/user.png
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/wave.png
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/wave1.png
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/word.png
+-rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/xlsxLogo.png
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/layout/CollectionLayout.js
+-rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/layout/PrimaryLayout.js
+-rw-r--r--   0        0        0    32803 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/Document.js
+-rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/chatBot.js
+-rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/chat/Chat.js
+-rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/chat/Details.js
+-rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/pricing/Pricing.jsx
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/privacy/Privacy.jsx
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/privacy/Terms.jsx
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/profile/Profile.jsx
+-rw-r--r--   0        0        0    23023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/settings/Settings.jsx
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/.gitignore
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/README.md
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pyproject.toml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/PKG-INFO
```

### Comparing `komodo_sdk-0.0.91/.dockerignore` & `komodo_sdk-0.0.92/.dockerignore`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/requirements.txt` & `komodo_sdk-0.0.92/requirements.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/.github/workflows/deploy-all.yml` & `komodo_sdk-0.0.92/.github/workflows/deploy-all.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/.github/workflows/publish-container.yml` & `komodo_sdk-0.0.92/.github/workflows/publish-container.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/README.md` & `komodo_sdk-0.0.92/komodo/README.md`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/config.py` & `komodo_sdk-0.0.92/komodo/config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/chatdoc_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/chatdoc_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/collection_builder.py` & `komodo_sdk-0.0.92/komodo/core/agents/collection_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/coordinator_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/coordinator_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/default.py` & `komodo_sdk-0.0.92/komodo/core/agents/default.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/difference_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/difference_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/elastic_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/groot_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/groot_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/librarian_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/librarian_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/mongo_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/mongo_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/pdf_generator.py` & `komodo_sdk-0.0.92/komodo/core/agents/pdf_generator.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/sample_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/sample_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/summarizer_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/summarizer_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/translator_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/translator_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/agents/widget_builder_agent.py` & `komodo_sdk-0.0.92/komodo/core/agents/widget_builder_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/sources/filesystem.py` & `komodo_sdk-0.0.92/komodo/core/sources/filesystem.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/sources/s3bucketkey.py` & `komodo_sdk-0.0.92/komodo/core/sources/s3bucketkey.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/sources/webpages.py` & `komodo_sdk-0.0.92/komodo/core/sources/webpages.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/sources/website_crawler.py` & `komodo_sdk-0.0.92/komodo/core/sources/website_crawler.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_count.py` & `komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_count.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_get.py` & `komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_get.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/elastic/elastic_search.py` & `komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/files/collection_builder.py` & `komodo_sdk-0.0.92/komodo/core/tools/files/collection_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/files/collection_lister.py` & `komodo_sdk-0.0.92/komodo/core/tools/files/collection_lister.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/files/collection_reader.py` & `komodo_sdk-0.0.92/komodo/core/tools/files/collection_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/files/directory_reader.py` & `komodo_sdk-0.0.92/komodo/core/tools/files/directory_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/files/file_reader.py` & `komodo_sdk-0.0.92/komodo/core/tools/files/file_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/files/file_writer.py` & `komodo_sdk-0.0.92/komodo/core/tools/files/file_writer.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/markets/polygon_search.py` & `komodo_sdk-0.0.92/komodo/core/tools/markets/polygon_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_databases.py` & `komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_databases.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_query.py` & `komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_query.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_schema.py` & `komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_schema.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/mongo/mongo_unique.py` & `komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_unique.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/search/vector_search.py` & `komodo_sdk-0.0.92/komodo/core/tools/search/vector_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/search/vector_search_runtime.py` & `komodo_sdk-0.0.92/komodo/core/tools/search/vector_search_runtime.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/utils/agent_tool.py` & `komodo_sdk-0.0.92/komodo/core/tools/utils/agent_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/utils/sample_tool.py` & `komodo_sdk-0.0.92/komodo/core/tools/utils/sample_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/utils/thought_tool.py` & `komodo_sdk-0.0.92/komodo/core/tools/utils/thought_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/utils/workflow_tool.py` & `komodo_sdk-0.0.92/komodo/core/tools/utils/workflow_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/web/data_fetcher.py` & `komodo_sdk-0.0.92/komodo/core/tools/web/data_fetcher.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/web/serpapi_search.py` & `komodo_sdk-0.0.92/komodo/core/tools/web/serpapi_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/web/tavily_search.py` & `komodo_sdk-0.0.92/komodo/core/tools/web/tavily_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/tools/web/web_scraper.py` & `komodo_sdk-0.0.92/komodo/core/tools/web/web_scraper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/utils/agent_helper.py` & `komodo_sdk-0.0.92/komodo/core/utils/agent_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/utils/indexer.py` & `komodo_sdk-0.0.92/komodo/core/utils/indexer.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/utils/play.py` & `komodo_sdk-0.0.92/komodo/core/utils/play.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/utils/rag_context.py` & `komodo_sdk-0.0.92/komodo/core/utils/rag_context.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/vector_stores/pinecone_store.py` & `komodo_sdk-0.0.92/komodo/core/vector_stores/pinecone_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/vector_stores/qdrant_store.py` & `komodo_sdk-0.0.92/komodo/core/vector_stores/qdrant_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/vector_stores/vector_store_helper.py` & `komodo_sdk-0.0.92/komodo/core/vector_stores/vector_store_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/core/workflows/sample_workflow.py` & `komodo_sdk-0.0.92/komodo/core/workflows/sample_workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/data/agents/planner/personal_finance_profile.yml` & `komodo_sdk-0.0.92/komodo/data/agents/planner/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/data/appliances/citibank/personal_finance_profile.yml` & `komodo_sdk-0.0.92/komodo/data/appliances/citibank/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf` & `komodo_sdk-0.0.92/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/data/workflows/analyzer/personal_finance_profile.yml` & `komodo_sdk-0.0.92/komodo/data/workflows/analyzer/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/definitions/agents/planner/context.yml` & `komodo_sdk-0.0.92/komodo/definitions/agents/planner/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/definitions/agents/planner/role.yml` & `komodo_sdk-0.0.92/komodo/definitions/agents/planner/role.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml` & `komodo_sdk-0.0.92/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/definitions/appliances/sample/context.yml` & `komodo_sdk-0.0.92/komodo/definitions/appliances/sample/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/definitions/workflows/analyzer/context.yml` & `komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_agent.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_app.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_app.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_collection.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_collection.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_config.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_context.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_context.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_datasource.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_datasource.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_locations.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_locations.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_runnable.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_runnable.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_runtime.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_runtime.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_tool.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_tool_registry.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_tool_registry.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_user.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from komodo.shared.utils.digest import get_text_digest
 
 
 class KomodoUser:
     def __init__(self, *, email, name, **kwargs):
         self.email = email
         self.name = name
-        self.uid = kwargs.get('uid', None)
-        self.role = kwargs.get('role', 'user')
-        self.plan = kwargs.get('plan', 'free')
-        self.verified = kwargs.get('verified', False)
-        self.provider_id = kwargs.get('provider_id', 'komodo')
-        self.token = kwargs.get('token', '')
-
-        self.allowed_assistants = kwargs.get('allowed_assistants', [])
-        self.preferred_assistant = kwargs.get('preferred_assistant', '')
-        self.show_tool_progress = kwargs.get('show_tool_progress', None)
-        self.is_power_user = kwargs.get('is_power_user', False)
+        self.uid = kwargs.pop('uid', None)
+        self.groups = kwargs.pop('groups', [])
+        self.is_power_user = kwargs.pop('is_power_user', False)
+
+        self.role = kwargs.pop('role', 'user')
+        self.plan = kwargs.pop('plan', 'free')
+        self.verified = kwargs.pop('verified', False)
+        self.provider_id = kwargs.pop('provider_id', 'komodo')
+        self.token = kwargs.pop('token', '')
+
+        self.allowed_assistants = kwargs.pop('allowed_assistants', [])
+        self.preferred_assistant = kwargs.pop('preferred_assistant', '')
+        self.show_tool_progress = kwargs.pop('show_tool_progress', None)
+        self.kwargs = kwargs
 
         # each user has a home folder / collection and a default downloads folder
         self.guid = get_text_digest(email)
         self.home_shortcode = self.guid + "_home"
         self.downloads_shortcode = self.guid + "_downloads"
 
     def __str__(self):
@@ -32,14 +35,13 @@
             'email': self.email,
             'name': self.name,
             'role': self.role,
             'plan': self.plan,
             'verified': self.verified,
             'default_collection': self.home_shortcode,
             'allowed_assistants': self.allowed_assistants,
-            'preferred_assistant': self.preferred_assistant,
-            'show_tool_progress': self.show_tool_progress}
+            'preferred_assistant': self.preferred_assistant}
 
     @staticmethod
     def default():
         email = "ryan.oberoi@komodoapp.ai"
         return KomodoUser(email=email, name="Ryan Oberoi")
```

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_vector.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_vector.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_vectorstore.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_vectorstore.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/framework/komodo_workflow.py` & `komodo_sdk-0.0.92/komodo/framework/komodo_workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/loaders/database/agent_loader.py` & `komodo_sdk-0.0.92/komodo/loaders/database/agent_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/loaders/database/appliance_loader.py` & `komodo_sdk-0.0.92/komodo/loaders/database/appliance_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/loaders/database/user_loader.py` & `komodo_sdk-0.0.92/komodo/loaders/database/user_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/loaders/filesystem/agent_loader.py` & `komodo_sdk-0.0.92/komodo/loaders/filesystem/agent_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/loaders/filesystem/appliance_loader.py` & `komodo_sdk-0.0.92/komodo/loaders/filesystem/appliance_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/loaders/filesystem/loader_helper.py` & `komodo_sdk-0.0.92/komodo/loaders/filesystem/loader_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/loaders/filesystem/loader_locations.py` & `komodo_sdk-0.0.92/komodo/loaders/filesystem/loader_locations.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/loaders/filesystem/workflow_loader.py` & `komodo_sdk-0.0.92/komodo/loaders/filesystem/workflow_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/azure/azure.py` & `komodo_sdk-0.0.92/komodo/models/azure/azure.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/azure/azure_openai.py` & `komodo_sdk-0.0.92/komodo/models/azure/azure_openai.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock.py` & `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_claude.py` & `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_claude.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_cohere.py` & `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_cohere.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_model.py` & `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_model.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/bedrock/bedrock_titan.py` & `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_titan.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/framework/agent_runner.py` & `komodo_sdk-0.0.92/komodo/models/framework/agent_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/framework/appliance_utils.py` & `komodo_sdk-0.0.92/komodo/models/framework/appliance_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/framework/chat_message.py` & `komodo_sdk-0.0.92/komodo/models/framework/chat_message.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/framework/model_request.py` & `komodo_sdk-0.0.92/komodo/models/framework/model_request.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/framework/model_response.py` & `komodo_sdk-0.0.92/komodo/models/framework/model_response.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/framework/responder.py` & `komodo_sdk-0.0.92/komodo/models/framework/responder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/framework/workflow_executor.py` & `komodo_sdk-0.0.92/komodo/models/framework/workflow_executor.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/framework/workflow_runner.py` & `komodo_sdk-0.0.92/komodo/models/framework/workflow_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/openai/openai_api.py` & `komodo_sdk-0.0.92/komodo/models/openai/openai_api.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/openai/openai_api_streamed.py` & `komodo_sdk-0.0.92/komodo/models/openai/openai_api_streamed.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/openai/openai_api_streamed_tool_call.py` & `komodo_sdk-0.0.92/komodo/models/openai/openai_api_streamed_tool_call.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/openai/openai_debug.py` & `komodo_sdk-0.0.92/komodo/models/openai/openai_debug.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/models/openai/openai_process_actions.py` & `komodo_sdk-0.0.92/komodo/models/openai/openai_process_actions.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/collection.proto` & `komodo_sdk-0.0.92/komodo/proto/collection.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/data.proto` & `komodo_sdk-0.0.92/komodo/proto/data.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/model.proto` & `komodo_sdk-0.0.92/komodo/proto/model.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/report.proto` & `komodo_sdk-0.0.92/komodo/proto/report.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/sample.py` & `komodo_sdk-0.0.92/komodo/proto/sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/generated/collection_pb2.py` & `komodo_sdk-0.0.92/komodo/proto/generated/collection_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/generated/collection_pb2.pyi` & `komodo_sdk-0.0.92/komodo/proto/generated/collection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/generated/data_pb2.py` & `komodo_sdk-0.0.92/komodo/proto/generated/data_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/generated/data_pb2.pyi` & `komodo_sdk-0.0.92/komodo/proto/generated/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/generated/model_pb2.py` & `komodo_sdk-0.0.92/komodo/proto/generated/model_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/generated/model_pb2.pyi` & `komodo_sdk-0.0.92/komodo/proto/generated/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/generated/report_pb2.py` & `komodo_sdk-0.0.92/komodo/proto/generated/report_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/proto/generated/report_pb2.pyi` & `komodo_sdk-0.0.92/komodo/proto/generated/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/scripts/run_agent_runner.py` & `komodo_sdk-0.0.92/komodo/scripts/run_agent_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/scripts/run_agent_runner_2.py` & `komodo_sdk-0.0.92/komodo/scripts/run_agent_runner_2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/scripts/run_difference_agent.py` & `komodo_sdk-0.0.92/komodo/scripts/run_difference_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/scripts/run_librarian_agent.py` & `komodo_sdk-0.0.92/komodo/scripts/run_librarian_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/scripts/run_streaming_test.py` & `komodo_sdk-0.0.92/komodo/scripts/run_streaming_test.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/scripts/run_widget_builder.py` & `komodo_sdk-0.0.92/komodo/scripts/run_widget_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/agent_router.py` & `komodo_sdk-0.0.92/komodo/server/agent_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/appliance_router.py` & `komodo_sdk-0.0.92/komodo/server/appliance_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/ask_request.py` & `komodo_sdk-0.0.92/komodo/server/ask_request.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/audio_router.py` & `komodo_sdk-0.0.92/komodo/server/audio_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/collections_router.py` & `komodo_sdk-0.0.92/komodo/server/collections_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/conversation_router.py` & `komodo_sdk-0.0.92/komodo/server/conversation_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/fast.py` & `komodo_sdk-0.0.92/komodo/server/fast.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/globals.py` & `komodo_sdk-0.0.92/komodo/server/globals.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/logo_router.py` & `komodo_sdk-0.0.92/komodo/server/logo_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/report_router.py` & `komodo_sdk-0.0.92/komodo/server/report_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/server/user_router.py` & `komodo_sdk-0.0.92/komodo/server/user_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/directory/assistants_helpers.py` & `komodo_sdk-0.0.92/komodo/shared/directory/assistants_helpers.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/documents/file_writer_helper.py` & `komodo_sdk-0.0.92/komodo/shared/documents/file_writer_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/documents/text_convert_helper.py` & `komodo_sdk-0.0.92/komodo/shared/documents/text_convert_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/documents/text_extract.py` & `komodo_sdk-0.0.92/komodo/shared/documents/text_extract.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/documents/text_extract_helper.py` & `komodo_sdk-0.0.92/komodo/shared/documents/text_extract_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/documents/text_html.py` & `komodo_sdk-0.0.92/komodo/shared/documents/text_html.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/embeddings/faiss_store.py` & `komodo_sdk-0.0.92/komodo/shared/embeddings/faiss_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/embeddings/pinecone_store.py` & `komodo_sdk-0.0.92/komodo/shared/embeddings/pinecone_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/mssql/mssql.py` & `komodo_sdk-0.0.92/komodo/shared/mssql/mssql.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/api_query.py` & `komodo_sdk-0.0.92/komodo/shared/utils/api_query.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/digest.py` & `komodo_sdk-0.0.92/komodo/shared/utils/digest.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/filestats.py` & `komodo_sdk-0.0.92/komodo/shared/utils/filestats.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/globber.py` & `komodo_sdk-0.0.92/komodo/shared/utils/globber.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/lambda_entry.py` & `komodo_sdk-0.0.92/komodo/shared/utils/lambda_entry.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/lambda_utils.py` & `komodo_sdk-0.0.92/komodo/shared/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/logconfig.py` & `komodo_sdk-0.0.92/komodo/shared/utils/logconfig.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/s3_file_utils.py` & `komodo_sdk-0.0.92/komodo/shared/utils/s3_file_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/tags.py` & `komodo_sdk-0.0.92/komodo/shared/utils/tags.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/term_colors.py` & `komodo_sdk-0.0.92/komodo/shared/utils/term_colors.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/timebox.py` & `komodo_sdk-0.0.92/komodo/shared/utils/timebox.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/shared/utils/watcher.py` & `komodo_sdk-0.0.92/komodo/shared/utils/watcher.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/store/agent_store.py` & `komodo_sdk-0.0.92/komodo/store/agent_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/store/appliance_store.py` & `komodo_sdk-0.0.92/komodo/store/appliance_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/store/collection_store.py` & `komodo_sdk-0.0.92/komodo/store/collection_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/store/conversations_store.py` & `komodo_sdk-0.0.92/komodo/store/conversations_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/store/logo_store.py` & `komodo_sdk-0.0.92/komodo/store/logo_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/store/redis_database.py` & `komodo_sdk-0.0.92/komodo/store/redis_database.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/store/tool_store.py` & `komodo_sdk-0.0.92/komodo/store/tool_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/store/user_store.py` & `komodo_sdk-0.0.92/komodo/store/user_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/core/test_elastic_agent.py` & `komodo_sdk-0.0.92/komodo/tests/core/test_elastic_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/core/test_elastic_sample.py` & `komodo_sdk-0.0.92/komodo/tests/core/test_elastic_sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/core/test_elastic_tools.py` & `komodo_sdk-0.0.92/komodo/tests/core/test_elastic_tools.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/core/test_mongo_sample.py` & `komodo_sdk-0.0.92/komodo/tests/core/test_mongo_sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/core/test_mongo_tools.py` & `komodo_sdk-0.0.92/komodo/tests/core/test_mongo_tools.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/core/test_serpapi_search.py` & `komodo_sdk-0.0.92/komodo/tests/core/test_serpapi_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/models/test_bedrock.py` & `komodo_sdk-0.0.92/komodo/tests/models/test_bedrock.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/models/test_workflow_runner.py` & `komodo_sdk-0.0.92/komodo/tests/models/test_workflow_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/shared/test_mssql.py` & `komodo_sdk-0.0.92/komodo/tests/shared/test_mssql.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/komodo/tests/store/test_conversation_store.py` & `komodo_sdk-0.0.92/komodo/tests/store/test_conversation_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/pdf2html/Dockerfile` & `komodo_sdk-0.0.92/pdf2html/Dockerfile`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/pdf2html/server.py` & `komodo_sdk-0.0.92/pdf2html/server.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/pdf2html/data/sample.html` & `komodo_sdk-0.0.92/pdf2html/data/sample.html`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/pdf2html/data/sample.pdf` & `komodo_sdk-0.0.92/pdf2html/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/Dockerfile` & `komodo_sdk-0.0.92/sample/Dockerfile`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/docker-compose.yml` & `komodo_sdk-0.0.92/sample/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/docker-production.yml` & `komodo_sdk-0.0.92/sample/docker-production.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/appliance/appliance.py` & `komodo_sdk-0.0.92/sample/appliance/appliance.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/appliance/config.py` & `komodo_sdk-0.0.92/sample/appliance/config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/appliance/seed.py` & `komodo_sdk-0.0.92/sample/appliance/seed.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/appliance/server.py` & `komodo_sdk-0.0.92/sample/appliance/server.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/appliance/workflow.py` & `komodo_sdk-0.0.92/sample/appliance/workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/definitions/agents/dasher_v1/instructions.txt` & `komodo_sdk-0.0.92/sample/definitions/agents/dasher_v1/instructions.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/definitions/agents/dasher_v2/instructions.txt` & `komodo_sdk-0.0.92/sample/definitions/agents/dasher_v2/instructions.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/app.py` & `komodo_sdk-0.0.92/sample/widgets/app.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/globals.py` & `komodo_sdk-0.0.92/sample/widgets/globals.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/themes.py` & `komodo_sdk-0.0.92/sample/widgets/themes.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/assets/custom.css` & `komodo_sdk-0.0.92/sample/widgets/assets/custom.css`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/agent.py` & `komodo_sdk-0.0.92/sample/widgets/pages/agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/analytics.py` & `komodo_sdk-0.0.92/sample/widgets/pages/analytics.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/appliance.py` & `komodo_sdk-0.0.92/sample/widgets/pages/appliance.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/dasher_v1.py` & `komodo_sdk-0.0.92/sample/widgets/pages/dasher_v1.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/dasher_v2.py` & `komodo_sdk-0.0.92/sample/widgets/pages/dasher_v2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/department.py` & `komodo_sdk-0.0.92/sample/widgets/pages/department.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/present.py` & `komodo_sdk-0.0.92/sample/widgets/pages/present.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/report.py` & `komodo_sdk-0.0.92/sample/widgets/pages/report.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/side_bar.py` & `komodo_sdk-0.0.92/sample/widgets/pages/side_bar.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/reports/bar_chart.py` & `komodo_sdk-0.0.92/sample/widgets/pages/reports/bar_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/reports/line_chart.py` & `komodo_sdk-0.0.92/sample/widgets/pages/reports/line_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/sample/widgets/pages/reports/pie_chart.py` & `komodo_sdk-0.0.92/sample/widgets/pages/reports/pie_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/README.md` & `komodo_sdk-0.0.92/website/README.md`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/package-lock.json` & `komodo_sdk-0.0.92/website/package-lock.json`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/package.json` & `komodo_sdk-0.0.92/website/package.json`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/tailwind.config.js` & `komodo_sdk-0.0.92/website/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/deployment/nginx.default.conf` & `komodo_sdk-0.0.92/website/deployment/nginx.default.conf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/chaticon.png` & `komodo_sdk-0.0.92/website/public/chaticon.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/faqbg.png` & `komodo_sdk-0.0.92/website/public/faqbg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/favicon.ico` & `komodo_sdk-0.0.92/website/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/footer.png` & `komodo_sdk-0.0.92/website/public/footer.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/home.png` & `komodo_sdk-0.0.92/website/public/home.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/index.html` & `komodo_sdk-0.0.92/website/public/index.html`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/logo192.png` & `komodo_sdk-0.0.92/website/public/logo192.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/logo512.png` & `komodo_sdk-0.0.92/website/public/logo512.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/pricingBg.png` & `komodo_sdk-0.0.92/website/public/pricingBg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/pricingBg1.png` & `komodo_sdk-0.0.92/website/public/pricingBg1.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf` & `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/App.css` & `komodo_sdk-0.0.92/website/src/App.css`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/RouterMain.js` & `komodo_sdk-0.0.92/website/src/RouterMain.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/index.css` & `komodo_sdk-0.0.92/website/src/index.css`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/index.js` & `komodo_sdk-0.0.92/website/src/index.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/logo.svg` & `komodo_sdk-0.0.92/website/src/logo.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/API/API_data.js` & `komodo_sdk-0.0.92/website/src/API/API_data.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/API/ApiComment.js` & `komodo_sdk-0.0.92/website/src/API/ApiComment.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/Frame.svg` & `komodo_sdk-0.0.92/website/src/assets/Frame.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/ai.png` & `komodo_sdk-0.0.92/website/src/assets/ai.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/blue.svg` & `komodo_sdk-0.0.92/website/src/assets/blue.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/botAvatar.svg` & `komodo_sdk-0.0.92/website/src/assets/botAvatar.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/chatListIcon.svg` & `komodo_sdk-0.0.92/website/src/assets/chatListIcon.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/docs.svg` & `komodo_sdk-0.0.92/website/src/assets/docs.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/docx.png` & `komodo_sdk-0.0.92/website/src/assets/docx.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/folder.svg` & `komodo_sdk-0.0.92/website/src/assets/folder.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/gallery.svg` & `komodo_sdk-0.0.92/website/src/assets/gallery.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/headphone.svg` & `komodo_sdk-0.0.92/website/src/assets/headphone.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/magicpen-1.svg` & `komodo_sdk-0.0.92/website/src/assets/magicpen-1.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/magicpen.svg` & `komodo_sdk-0.0.92/website/src/assets/magicpen.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/message.svg` & `komodo_sdk-0.0.92/website/src/assets/message.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/multi.png` & `komodo_sdk-0.0.92/website/src/assets/multi.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/odt.png` & `komodo_sdk-0.0.92/website/src/assets/odt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/pdf.png` & `komodo_sdk-0.0.92/website/src/assets/pdf.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/pdf.svg` & `komodo_sdk-0.0.92/website/src/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/pricingBg.png` & `komodo_sdk-0.0.92/website/src/assets/pricingBg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/profile.png` & `komodo_sdk-0.0.92/website/src/assets/profile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/send.png` & `komodo_sdk-0.0.92/website/src/assets/send.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/setting-1.svg` & `komodo_sdk-0.0.92/website/src/assets/setting-1.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/setting.svg` & `komodo_sdk-0.0.92/website/src/assets/setting.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/text.png` & `komodo_sdk-0.0.92/website/src/assets/text.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/text.svg` & `komodo_sdk-0.0.92/website/src/assets/text.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/trash.svg` & `komodo_sdk-0.0.92/website/src/assets/trash.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/assets/userProfile.svg` & `komodo_sdk-0.0.92/website/src/assets/userProfile.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/auth/Login.js` & `komodo_sdk-0.0.92/website/src/auth/Login.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/auth/Signup.js` & `komodo_sdk-0.0.92/website/src/auth/Signup.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/Dashboard.js` & `komodo_sdk-0.0.92/website/src/components/Dashboard.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/DocumentView.js` & `komodo_sdk-0.0.92/website/src/components/DocumentView.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/Header.js` & `komodo_sdk-0.0.92/website/src/components/Header.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/HeaderSideBar.js` & `komodo_sdk-0.0.92/website/src/components/HeaderSideBar.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/Home.jsx` & `komodo_sdk-0.0.92/website/src/components/Home.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/LayoutHeader.js` & `komodo_sdk-0.0.92/website/src/components/LayoutHeader.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/NavigateBack.js` & `komodo_sdk-0.0.92/website/src/components/NavigateBack.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/Sidebar.js` & `komodo_sdk-0.0.92/website/src/components/Sidebar.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/DocumentBox/Table.js` & `komodo_sdk-0.0.92/website/src/components/DocumentBox/Table.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/chat/Chat.js` & `komodo_sdk-0.0.92/website/src/components/chat/Chat.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/chat/Details.js` & `komodo_sdk-0.0.92/website/src/components/chat/Details.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/chat/EnhancedPrompt.js` & `komodo_sdk-0.0.92/website/src/components/chat/EnhancedPrompt.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/chatBot/Chat.js` & `komodo_sdk-0.0.92/website/src/components/chatBot/Chat.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/chatBot/ChatBotById.js` & `komodo_sdk-0.0.92/website/src/components/chatBot/ChatBotById.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/chatBot/ChatBotSideBar.js` & `komodo_sdk-0.0.92/website/src/components/chatBot/ChatBotSideBar.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/chatBot/EnhancedBot.js` & `komodo_sdk-0.0.92/website/src/components/chatBot/EnhancedBot.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/components/document/DocumentSidebar.js` & `komodo_sdk-0.0.92/website/src/components/document/DocumentSidebar.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/contexts/roleContext.js` & `komodo_sdk-0.0.92/website/src/contexts/roleContext.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/Ellipsis.gif` & `komodo_sdk-0.0.92/website/src/images/Ellipsis.gif`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/chat.png` & `komodo_sdk-0.0.92/website/src/images/chat.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/chatgpt.png` & `komodo_sdk-0.0.92/website/src/images/chatgpt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/chatimg.png` & `komodo_sdk-0.0.92/website/src/images/chatimg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/chattick.png` & `komodo_sdk-0.0.92/website/src/images/chattick.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/content.png` & `komodo_sdk-0.0.92/website/src/images/content.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/copy.png` & `komodo_sdk-0.0.92/website/src/images/copy.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/doc.png` & `komodo_sdk-0.0.92/website/src/images/doc.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/docprofile.png` & `komodo_sdk-0.0.92/website/src/images/docprofile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/docwave.png` & `komodo_sdk-0.0.92/website/src/images/docwave.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/first.png` & `komodo_sdk-0.0.92/website/src/images/first.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/imgLogo.jpg` & `komodo_sdk-0.0.92/website/src/images/imgLogo.jpg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/login.png` & `komodo_sdk-0.0.92/website/src/images/login.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/pdf.png` & `komodo_sdk-0.0.92/website/src/images/pdf.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/person.png` & `komodo_sdk-0.0.92/website/src/images/person.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/portfolio.png` & `komodo_sdk-0.0.92/website/src/images/portfolio.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/pptLogo.png` & `komodo_sdk-0.0.92/website/src/images/pptLogo.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/profile.png` & `komodo_sdk-0.0.92/website/src/images/profile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/robot.png` & `komodo_sdk-0.0.92/website/src/images/robot.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/sample.pdf` & `komodo_sdk-0.0.92/website/src/images/sample.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/second.png` & `komodo_sdk-0.0.92/website/src/images/second.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/send.png` & `komodo_sdk-0.0.92/website/src/images/send.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/setting.png` & `komodo_sdk-0.0.92/website/src/images/setting.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/summary.png` & `komodo_sdk-0.0.92/website/src/images/summary.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/tik.png` & `komodo_sdk-0.0.92/website/src/images/tik.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/txt.png` & `komodo_sdk-0.0.92/website/src/images/txt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/user.png` & `komodo_sdk-0.0.92/website/src/images/user.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/wave.png` & `komodo_sdk-0.0.92/website/src/images/wave.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/wave1.png` & `komodo_sdk-0.0.92/website/src/images/wave1.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/word.png` & `komodo_sdk-0.0.92/website/src/images/word.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/images/xlsxLogo.png` & `komodo_sdk-0.0.92/website/src/images/xlsxLogo.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/layout/CollectionLayout.js` & `komodo_sdk-0.0.92/website/src/layout/CollectionLayout.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/layout/PrimaryLayout.js` & `komodo_sdk-0.0.92/website/src/layout/PrimaryLayout.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/Document.js` & `komodo_sdk-0.0.92/website/src/pages/Document.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/chatBot.js` & `komodo_sdk-0.0.92/website/src/pages/chatBot.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/chat/Chat.js` & `komodo_sdk-0.0.92/website/src/pages/chat/Chat.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/chat/Details.js` & `komodo_sdk-0.0.92/website/src/pages/chat/Details.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/pricing/Pricing.jsx` & `komodo_sdk-0.0.92/website/src/pages/pricing/Pricing.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/privacy/Privacy.jsx` & `komodo_sdk-0.0.92/website/src/pages/privacy/Privacy.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/privacy/Terms.jsx` & `komodo_sdk-0.0.92/website/src/pages/privacy/Terms.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/profile/Profile.jsx` & `komodo_sdk-0.0.92/website/src/pages/profile/Profile.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/website/src/pages/settings/Settings.jsx` & `komodo_sdk-0.0.92/website/src/pages/settings/Settings.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/.gitignore` & `komodo_sdk-0.0.92/.gitignore`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.91/pyproject.toml` & `komodo_sdk-0.0.92/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "komodo-sdk"
-version = "0.0.91"
+version = "0.0.92"
 authors = [
     { name = "Ryan Oberoi", email = "ryan.oberoi@komodoapp.ai" },
 ]
 description = "Komodo SDK"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `komodo_sdk-0.0.91/PKG-INFO` & `komodo_sdk-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: komodo-sdk
-Version: 0.0.91
+Version: 0.0.92
 Summary: Komodo SDK
 Project-URL: Homepage, https://github.com/Komodo-AI/komodo-sdk.git
 Author-email: Ryan Oberoi <ryan.oberoi@komodoapp.ai>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: aiofiles~=23.2.1
```

