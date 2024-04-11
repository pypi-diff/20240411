# Comparing `tmp/komodo_sdk-0.0.92.tar.gz` & `tmp/komodo_sdk-0.0.93.tar.gz`

## Comparing `komodo_sdk-0.0.92.tar` & `komodo_sdk-0.0.93.tar`

### file list

```diff
@@ -1,443 +1,443 @@
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/.dockerignore
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/requirements.txt
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/.github/workflows/deploy-all.yml
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/.github/workflows/publish-container.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/README.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/config.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/chatdoc_agent.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/collection_builder.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/coordinator_agent.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/default.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/difference_agent.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/echo_agent.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/elastic_agent.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/groot_agent.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/librarian_agent.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/mongo_agent.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/pdf_generator.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/sample_agent.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/summarizer_agent.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/translator_agent.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/agents/widget_builder_agent.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/sources/filesystem.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/sources/s3bucketkey.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/sources/webpages.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/sources/website_crawler.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_connect.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_count.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_get.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_search.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/collection_builder.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/collection_lister.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/collection_reader.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/directory_reader.py
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/file_reader.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/files/file_writer.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/markets/polygon_search.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_connect.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_databases.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_query.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_schema.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_unique.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/search/vector_search.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/search/vector_search_runtime.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/utils/agent_tool.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/utils/sample_tool.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/utils/thought_tool.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/utils/workflow_tool.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/web/data_fetcher.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/web/serpapi_search.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/web/tavily_search.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/tools/web/web_scraper.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/utils/agent_helper.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/utils/indexer.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/utils/play.py
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/utils/rag_context.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/vector_stores/pinecone_store.py
--rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/vector_stores/qdrant_store.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/vector_stores/vector_store_helper.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/core/workflows/sample_workflow.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/agents/planner/personal_finance_profile.yml
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/appliances/citibank/personal_finance_profile.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/appliances/komodo/dir1/hello.txt
--rw-r--r--   0        0        0  1139092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/data/workflows/analyzer/personal_finance_profile.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/checker/agent.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/checker/context.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/checker/dictionary.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/checker/instructions.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/agent.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/context.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/instructions.txt
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/role.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/tools/income_calculator.yml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/tools/income_contributions.yml
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/citibank/appliance.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/komodo/appliance.yml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/sample/appliance.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/sample/context.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/sample/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/appliances/sample/instructions.txt
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/context.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/dictionary.yml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/instructions.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/workflow.yml
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_agent.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_app.py
--rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_collection.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_config.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_context.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_datasource.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_features.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_locations.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_runnable.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_runtime.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_tool.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_tool_registry.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_user.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_vector.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_vectorstore.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/framework/komodo_workflow.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/database/agent_loader.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/database/appliance_loader.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/database/tool_loader.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/database/user_loader.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/agent_loader.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/appliance_loader.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/loader_helper.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/loader_locations.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/loaders/filesystem/workflow_loader.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/azure/azure.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/azure/azure_openai.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_claude.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_cohere.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_model.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_titan.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/agent_runner.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/appliance_utils.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/chat_message.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/chat_metadata.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/model_request.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/model_response.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/models.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/responder.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/workflow_executor.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/workflow_runner.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/framework/workflow_selector.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_api.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_api_streamed.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_api_streamed_tool_call.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_completion.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_debug.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/models/openai/openai_process_actions.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/collection.proto
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/data.proto
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/model.proto
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/report.proto
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/sample.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/collection_pb2.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/collection_pb2.pyi
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/data_pb2.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/data_pb2.pyi
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/model_pb2.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/model_pb2.pyi
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/report_pb2.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/proto/generated/report_pb2.pyi
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_agent_runner.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_agent_runner_2.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_difference_agent.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_librarian_agent.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_sample_agent.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_streaming_test.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/scripts/run_widget_builder.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/agent_router.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/appliance_router.py
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/ask_request.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/audio_router.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/collections_router.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/conversation_router.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/fast.py
--rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/globals.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/logo_router.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/report_router.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/server/user_router.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/directory/assistants_helpers.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/file_writer_helper.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/text_convert_helper.py
--rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/text_extract.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/text_extract_helper.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/documents/text_html.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/embeddings/faiss_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/embeddings/openai.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/embeddings/pinecone_store.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/mssql/mssql.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/api_query.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/digest.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/filestats.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/globber.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/hidden_prints.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/lambda_entry.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/lambda_utils.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/logconfig.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/pathutils.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/s3_file_utils.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/sentry_utils.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/switchdir.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/tags.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/term_colors.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/timebox.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/shared/utils/watcher.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/agent_store.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/appliance_store.py
--rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/collection_store.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/conversations_store.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/logo_store.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/proto_utils.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/redis_database.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/tool_store.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/store/user_store.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_elastic_agent.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_elastic_sample.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_elastic_tools.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_groot_agent.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_mongo_agent.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_mongo_sample.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_mongo_tools.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/core/test_serpapi_search.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/models/test_azure.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/models/test_bedrock.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/models/test_openai.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/models/test_workflow_runner.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/shared/test_mssql.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/komodo/tests/store/test_conversation_store.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/Dockerfile
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/docker-compose.yml
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/server.py
--rw-r--r--   0        0        0   480357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/data/sample.html
--rw-r--r--   0        0        0   599041 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pdf2html/data/sample.pdf
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/Dockerfile
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/README.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/docker-compose.yml
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/docker-production.yml
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/appliance.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/config.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/seed.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/server.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/appliance/workflow.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/agents/dasher_v1/agent.yml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/agents/dasher_v1/instructions.txt
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/agents/dasher_v2/agent.yml
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/agents/dasher_v2/instructions.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/definitions/appliances/sample/appliance.yml
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/app.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/globals.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/server.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/themes.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/assets/custom.css
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/agent.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/analytics.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/appliance.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/archive.py
--rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/dasher_v1.py
--rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/dasher_v2.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/department.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/home.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/not_found_404.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/present.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/report.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/side_bar.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/topic_1.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/reports/bar_chart.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/reports/line_chart.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/sample/widgets/pages/reports/pie_chart.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/.gitignore
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/Dockerfile
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/README.md
--rw-r--r--   0        0        0   953941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/package-lock.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/package.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/tailwind.config.js
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/deployment/nginx.default.conf
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/chaticon.png
--rw-r--r--   0        0        0    66364 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/faqbg.png
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/favicon.ico
--rw-r--r--   0        0        0    84772 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/footer.png
--rw-r--r--   0        0        0   230014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/home.png
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/index.html
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/logo192.png
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/logo512.png
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/manifest.json
--rw-r--r--   0        0        0   318284 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/pricingBg.png
--rw-r--r--   0        0        0   189260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/pricingBg1.png
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/robots.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Read Me.txt
--rw-r--r--   0        0        0    84336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf
--rw-r--r--   0        0        0   291948 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf
--rw-r--r--   0        0        0    80288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf
--rw-r--r--   0        0        0   275104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf
--rw-r--r--   0        0        0    85092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf
--rw-r--r--   0        0        0   291180 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf
--rw-r--r--   0        0        0    80172 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf
--rw-r--r--   0        0        0   273580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf
--rw-r--r--   0        0        0    82008 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf
--rw-r--r--   0        0        0   418296 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf
--rw-r--r--   0        0        0    78624 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf
--rw-r--r--   0        0        0   411148 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf
--rw-r--r--   0        0        0    81940 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf
--rw-r--r--   0        0        0   279500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf
--rw-r--r--   0        0        0    78360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf
--rw-r--r--   0        0        0   257728 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf
--rw-r--r--   0        0        0    78480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf
--rw-r--r--   0        0        0   313920 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf
--rw-r--r--   0        0        0    82916 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf
--rw-r--r--   0        0        0   367128 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf
--rw-r--r--   0        0        0    79536 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf
--rw-r--r--   0        0        0   349188 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf
--rw-r--r--   0        0        0    83092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf
--rw-r--r--   0        0        0   309704 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf
--rw-r--r--   0        0        0    79480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf
--rw-r--r--   0        0        0   291444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf
--rw-r--r--   0        0        0    81828 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf
--rw-r--r--   0        0        0   331432 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf
--rw-r--r--   0        0        0    83560 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf
--rw-r--r--   0        0        0   301516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf
--rw-r--r--   0        0        0    79800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf
--rw-r--r--   0        0        0   283064 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    79864 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf
--rw-r--r--   0        0        0   459400 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf
--rw-r--r--   0        0        0    77840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf
--rw-r--r--   0        0        0   455000 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/App.css
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/App.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/App.test.js
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/RouterMain.js
--rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/index.css
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/index.js
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/logo.svg
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/reportWebVitals.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/setupTests.js
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/API/API_data.js
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/API/ApiComment.js
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/Frame.svg
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/ai.png
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/arrowLeft.svg
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/aubergine.png
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/barbra.svg
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/blue.svg
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/blueTick.svg
--rw-r--r--   0        0        0  1709204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/botAvatar.svg
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/chatListIcon.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/clementine.svg
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/close.svg
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/docs.svg
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/docx.png
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/folder.svg
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/gallery.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/gray.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/green.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/grey.svg
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/headphone.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/indigo.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/jade.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/lagoon.svg
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/magicpen-1.svg
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/magicpen.svg
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/message.svg
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/multi.png
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/odt.png
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/orange.png
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/parrot.svg
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/pdf.png
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/pdf.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/pink.svg
--rw-r--r--   0        0        0   378813 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/pricingBg.png
--rw-r--r--   0        0        0    48909 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/profile.png
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/send.png
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/setting-1.svg
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/setting.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/sky.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/square.svg
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/text.png
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/text.svg
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/trash.svg
--rw-r--r--   0        0        0  1884519 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/userProfile.svg
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/assets/yellow.svg
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/auth/Login.js
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/auth/Signup.js
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/ChartDashboard.js
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/Dashboard.js
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/DocumentView.js
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/Header.js
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/HeaderSideBar.js
--rw-r--r--   0        0        0    20984 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/Home.jsx
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/LayoutHeader.js
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/NavigateBack.js
--rw-r--r--   0        0        0    36368 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/Sidebar.js
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/DocumentBox/Table.js
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chat/Chat.js
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chat/Details.js
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chat/EnhancedPrompt.js
--rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chatBot/Chat.js
--rw-r--r--   0        0        0    15498 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chatBot/ChatBotById.js
--rw-r--r--   0        0        0    64401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chatBot/ChatBotSideBar.js
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/chatBot/EnhancedBot.js
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/document/DocumentSidebar.js
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/helpers/Toast.js
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/components/inputs/CustomInputs.jsx
--rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/contexts/roleContext.js
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/helpers/Toast.js
--rw-r--r--   0        0        0    33366 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/Ellipsis.gif
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/chat.png
--rw-r--r--   0        0        0   214322 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/chatgpt.png
--rw-r--r--   0        0        0   101078 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/chatimg.png
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/chattick.png
--rw-r--r--   0        0        0    21789 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/content.png
--rw-r--r--   0        0        0    53673 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/copy.png
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/doc.png
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/docprofile.png
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/docwave.png
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/dots.png
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/dummy.txt
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/first.png
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/homemenu.png
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/imgLogo.jpg
--rw-r--r--   0        0        0   371173 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/login.png
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/pdf.png
--rw-r--r--   0        0        0   177241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/person.png
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/portfolio.png
--rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/pptLogo.png
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/profile.png
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/robot.png
--rw-r--r--   0        0        0    96034 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/sample.pdf
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/second.png
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/send.png
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/setting.png
--rw-r--r--   0        0        0    61070 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/summary.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/tick.png
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/tik.png
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/txt.png
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/upload.png
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/upload2.png
--rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/user.png
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/wave.png
--rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/wave1.png
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/word.png
--rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/images/xlsxLogo.png
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/layout/CollectionLayout.js
--rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/layout/PrimaryLayout.js
--rw-r--r--   0        0        0    32803 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/Document.js
--rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/chatBot.js
--rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/chat/Chat.js
--rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/chat/Details.js
--rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/pricing/Pricing.jsx
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/privacy/Privacy.jsx
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/privacy/Terms.jsx
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/profile/Profile.jsx
--rw-r--r--   0        0        0    23023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/website/src/pages/settings/Settings.jsx
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/.gitignore
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/README.md
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/pyproject.toml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.92/PKG-INFO
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/.dockerignore
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/requirements.txt
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/.github/workflows/deploy-all.yml
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/.github/workflows/publish-container.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/README.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/config.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/chatdoc_agent.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/collection_builder.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/coordinator_agent.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/default.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/difference_agent.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/echo_agent.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/elastic_agent.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/groot_agent.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/librarian_agent.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/mongo_agent.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/pdf_generator.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/sample_agent.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/summarizer_agent.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/translator_agent.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/agents/widget_builder_agent.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/sources/filesystem.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/sources/s3bucketkey.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/sources/webpages.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/sources/website_crawler.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/elastic/elastic_connect.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/elastic/elastic_count.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/elastic/elastic_get.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/elastic/elastic_search.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/files/collection_builder.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/files/collection_lister.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/files/collection_reader.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/files/directory_reader.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/files/file_reader.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/files/file_writer.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/markets/polygon_search.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/mongo/mongo_connect.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/mongo/mongo_databases.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/mongo/mongo_query.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/mongo/mongo_schema.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/mongo/mongo_unique.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/search/vector_search.py
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/search/vector_search_runtime.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/utils/agent_tool.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/utils/sample_tool.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/utils/thought_tool.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/utils/workflow_tool.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/web/data_fetcher.py
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/web/serpapi_search.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/web/tavily_search.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/tools/web/web_scraper.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/utils/agent_helper.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/utils/indexer.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/utils/play.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/utils/rag_context.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/vector_stores/pinecone_store.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/vector_stores/qdrant_store.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/vector_stores/vector_store_helper.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/core/workflows/sample_workflow.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/data/agents/planner/personal_finance_profile.yml
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/data/appliances/citibank/personal_finance_profile.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/data/appliances/komodo/dir1/hello.txt
+-rw-r--r--   0        0        0  1139092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/data/workflows/analyzer/personal_finance_profile.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/checker/agent.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/checker/context.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/checker/dictionary.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/checker/instructions.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/planner/agent.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/planner/context.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/planner/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/planner/instructions.txt
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/planner/role.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/planner/tools/income_calculator.yml
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/planner/tools/income_contributions.yml
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/appliances/citibank/appliance.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/appliances/komodo/appliance.yml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/appliances/sample/appliance.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/appliances/sample/context.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/appliances/sample/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/appliances/sample/instructions.txt
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/workflows/analyzer/context.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/workflows/analyzer/dictionary.yml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/workflows/analyzer/instructions.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/definitions/workflows/analyzer/workflow.yml
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_agent.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_app.py
+-rw-r--r--   0        0        0     6771 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_collection.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_config.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_context.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_datasource.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_features.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_locations.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_runnable.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_runtime.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_tool.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_tool_registry.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_user.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_vector.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_vectorstore.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/framework/komodo_workflow.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/database/agent_loader.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/database/appliance_loader.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/database/tool_loader.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/database/user_loader.py
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/filesystem/agent_loader.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/filesystem/appliance_loader.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/filesystem/loader_helper.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/filesystem/loader_locations.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/loaders/filesystem/workflow_loader.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/azure/azure.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/azure/azure_openai.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/bedrock/bedrock.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/bedrock/bedrock_claude.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/bedrock/bedrock_cohere.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/bedrock/bedrock_model.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/bedrock/bedrock_titan.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/agent_runner.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/appliance_utils.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/chat_message.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/chat_metadata.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/model_request.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/model_response.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/models.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/responder.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/workflow_executor.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/workflow_runner.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/framework/workflow_selector.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/openai/openai_api.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/openai/openai_api_streamed.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/openai/openai_api_streamed_tool_call.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/openai/openai_completion.py
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/openai/openai_debug.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/models/openai/openai_process_actions.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/collection.proto
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/data.proto
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/model.proto
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/report.proto
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/sample.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/generated/collection_pb2.py
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/generated/collection_pb2.pyi
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/generated/data_pb2.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/generated/data_pb2.pyi
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/generated/model_pb2.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/generated/model_pb2.pyi
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/generated/report_pb2.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/proto/generated/report_pb2.pyi
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/scripts/run_agent_runner.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/scripts/run_agent_runner_2.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/scripts/run_difference_agent.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/scripts/run_librarian_agent.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/scripts/run_sample_agent.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/scripts/run_streaming_test.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/scripts/run_widget_builder.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/agent_router.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/appliance_router.py
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/ask_request.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/audio_router.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/collections_router.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/conversation_router.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/fast.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/globals.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/logo_router.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/report_router.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/server/user_router.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/directory/assistants_helpers.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/documents/file_writer_helper.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/documents/text_convert_helper.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/documents/text_extract.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/documents/text_extract_helper.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/documents/text_html.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/embeddings/faiss_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/embeddings/openai.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/embeddings/pinecone_store.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/mssql/mssql.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/api_query.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/digest.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/filestats.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/globber.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/hidden_prints.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/lambda_entry.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/lambda_utils.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/logconfig.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/pathutils.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/s3_file_utils.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/sentry_utils.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/switchdir.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/tags.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/term_colors.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/timebox.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/shared/utils/watcher.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/agent_store.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/appliance_store.py
+-rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/collection_store.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/conversations_store.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/logo_store.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/proto_utils.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/redis_database.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/tool_store.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/store/user_store.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/core/test_elastic_agent.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/core/test_elastic_sample.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/core/test_elastic_tools.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/core/test_groot_agent.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/core/test_mongo_agent.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/core/test_mongo_sample.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/core/test_mongo_tools.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/core/test_serpapi_search.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/models/test_azure.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/models/test_bedrock.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/models/test_openai.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/models/test_workflow_runner.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/shared/test_mssql.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/komodo/tests/store/test_conversation_store.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/pdf2html/Dockerfile
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/pdf2html/docker-compose.yml
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/pdf2html/server.py
+-rw-r--r--   0        0        0   480357 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/pdf2html/data/sample.html
+-rw-r--r--   0        0        0   599041 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/pdf2html/data/sample.pdf
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/Dockerfile
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/README.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/docker-compose.yml
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/docker-production.yml
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/appliance/appliance.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/appliance/config.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/appliance/seed.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/appliance/server.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/appliance/workflow.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/definitions/agents/dasher_v1/agent.yml
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/definitions/agents/dasher_v1/instructions.txt
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/definitions/agents/dasher_v2/agent.yml
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/definitions/agents/dasher_v2/instructions.txt
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/definitions/appliances/sample/appliance.yml
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/app.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/globals.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/server.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/themes.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/assets/custom.css
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/agent.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/analytics.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/appliance.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/archive.py
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/dasher_v1.py
+-rw-r--r--   0        0        0     9580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/dasher_v2.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/department.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/home.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/not_found_404.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/present.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/report.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/side_bar.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/topic_1.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/reports/bar_chart.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/reports/line_chart.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/sample/widgets/pages/reports/pie_chart.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/Dockerfile
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/README.md
+-rw-r--r--   0        0        0   953941 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/package-lock.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/package.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/tailwind.config.js
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/deployment/nginx.default.conf
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/chaticon.png
+-rw-r--r--   0        0        0    66364 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/faqbg.png
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/favicon.ico
+-rw-r--r--   0        0        0    84772 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/footer.png
+-rw-r--r--   0        0        0   230014 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/home.png
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/index.html
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/logo192.png
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/logo512.png
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/manifest.json
+-rw-r--r--   0        0        0   318284 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/pricingBg.png
+-rw-r--r--   0        0        0   189260 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/pricingBg1.png
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/robots.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Read Me.txt
+-rw-r--r--   0        0        0    84336 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf
+-rw-r--r--   0        0        0   291948 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf
+-rw-r--r--   0        0        0    80288 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf
+-rw-r--r--   0        0        0   275104 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf
+-rw-r--r--   0        0        0    85092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf
+-rw-r--r--   0        0        0   291180 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf
+-rw-r--r--   0        0        0    80172 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf
+-rw-r--r--   0        0        0   273580 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf
+-rw-r--r--   0        0        0    82008 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf
+-rw-r--r--   0        0        0   418296 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf
+-rw-r--r--   0        0        0    78624 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf
+-rw-r--r--   0        0        0   411148 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf
+-rw-r--r--   0        0        0    81940 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf
+-rw-r--r--   0        0        0   279500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf
+-rw-r--r--   0        0        0    78360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf
+-rw-r--r--   0        0        0   257728 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf
+-rw-r--r--   0        0        0    78480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf
+-rw-r--r--   0        0        0   313920 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf
+-rw-r--r--   0        0        0    82916 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf
+-rw-r--r--   0        0        0   367128 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf
+-rw-r--r--   0        0        0    79536 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf
+-rw-r--r--   0        0        0   349188 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf
+-rw-r--r--   0        0        0    83092 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf
+-rw-r--r--   0        0        0   309704 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf
+-rw-r--r--   0        0        0    79480 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf
+-rw-r--r--   0        0        0   291444 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf
+-rw-r--r--   0        0        0    81828 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf
+-rw-r--r--   0        0        0   331432 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf
+-rw-r--r--   0        0        0    83560 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf
+-rw-r--r--   0        0        0   301516 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf
+-rw-r--r--   0        0        0    79800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf
+-rw-r--r--   0        0        0   283064 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    79864 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf
+-rw-r--r--   0        0        0   459400 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf
+-rw-r--r--   0        0        0    77840 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf
+-rw-r--r--   0        0        0   455000 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/App.css
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/App.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/App.test.js
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/RouterMain.js
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/index.css
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/index.js
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/logo.svg
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/reportWebVitals.js
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/setupTests.js
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/API/API_data.js
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/API/ApiComment.js
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/Frame.svg
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/ai.png
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/arrowLeft.svg
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/aubergine.png
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/barbra.svg
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/blue.svg
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/blueTick.svg
+-rw-r--r--   0        0        0  1709204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/botAvatar.svg
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/chatListIcon.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/clementine.svg
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/close.svg
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/docs.svg
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/docx.png
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/folder.svg
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/gallery.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/gray.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/green.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/grey.svg
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/headphone.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/indigo.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/jade.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/lagoon.svg
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/magicpen-1.svg
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/magicpen.svg
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/message.svg
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/multi.png
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/odt.png
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/orange.png
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/parrot.svg
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/pdf.png
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/pdf.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/pink.svg
+-rw-r--r--   0        0        0   378813 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/pricingBg.png
+-rw-r--r--   0        0        0    48909 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/profile.png
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/send.png
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/setting-1.svg
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/setting.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/sky.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/square.svg
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/text.png
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/text.svg
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/trash.svg
+-rw-r--r--   0        0        0  1884519 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/userProfile.svg
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/assets/yellow.svg
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/auth/Login.js
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/auth/Signup.js
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/ChartDashboard.js
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/Dashboard.js
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/DocumentView.js
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/Header.js
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/HeaderSideBar.js
+-rw-r--r--   0        0        0    20984 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/Home.jsx
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/LayoutHeader.js
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/NavigateBack.js
+-rw-r--r--   0        0        0    36800 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/Sidebar.js
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/DocumentBox/Table.js
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/chat/Chat.js
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/chat/Details.js
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/chat/EnhancedPrompt.js
+-rw-r--r--   0        0        0    15403 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/chatBot/Chat.js
+-rw-r--r--   0        0        0    16187 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/chatBot/ChatBotById.js
+-rw-r--r--   0        0        0    64553 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/chatBot/ChatBotSideBar.js
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/chatBot/EnhancedBot.js
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/document/DocumentSidebar.js
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/helpers/Toast.js
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/components/inputs/CustomInputs.jsx
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/contexts/roleContext.js
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/helpers/Toast.js
+-rw-r--r--   0        0        0    33366 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/Ellipsis.gif
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/chat.png
+-rw-r--r--   0        0        0   214322 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/chatgpt.png
+-rw-r--r--   0        0        0   101078 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/chatimg.png
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/chattick.png
+-rw-r--r--   0        0        0    21789 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/content.png
+-rw-r--r--   0        0        0    53673 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/copy.png
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/doc.png
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/docprofile.png
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/docwave.png
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/dots.png
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/dummy.txt
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/first.png
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/homemenu.png
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/imgLogo.jpg
+-rw-r--r--   0        0        0   371173 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/login.png
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/pdf.png
+-rw-r--r--   0        0        0   177241 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/person.png
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/portfolio.png
+-rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/pptLogo.png
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/profile.png
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/robot.png
+-rw-r--r--   0        0        0    96034 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/sample.pdf
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/second.png
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/send.png
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/setting.png
+-rw-r--r--   0        0        0    61070 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/summary.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/tick.png
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/tik.png
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/txt.png
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/upload.png
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/upload2.png
+-rw-r--r--   0        0        0    20593 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/user.png
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/wave.png
+-rw-r--r--   0        0        0    52515 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/wave1.png
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/word.png
+-rw-r--r--   0        0        0    16022 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/images/xlsxLogo.png
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/layout/CollectionLayout.js
+-rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/layout/PrimaryLayout.js
+-rw-r--r--   0        0        0    32803 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/Document.js
+-rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/chatBot.js
+-rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/chat/Chat.js
+-rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/chat/Details.js
+-rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/pricing/Pricing.jsx
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/privacy/Privacy.jsx
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/privacy/Terms.jsx
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/profile/Profile.jsx
+-rw-r--r--   0        0        0    23023 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/website/src/pages/settings/Settings.jsx
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/.gitignore
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/README.md
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/pyproject.toml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 komodo_sdk-0.0.93/PKG-INFO
```

### Comparing `komodo_sdk-0.0.92/.dockerignore` & `komodo_sdk-0.0.93/.dockerignore`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/requirements.txt` & `komodo_sdk-0.0.93/requirements.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/.github/workflows/deploy-all.yml` & `komodo_sdk-0.0.93/.github/workflows/deploy-all.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/.github/workflows/publish-container.yml` & `komodo_sdk-0.0.93/.github/workflows/publish-container.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/README.md` & `komodo_sdk-0.0.93/komodo/README.md`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/config.py` & `komodo_sdk-0.0.93/komodo/config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/chatdoc_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/chatdoc_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/collection_builder.py` & `komodo_sdk-0.0.93/komodo/core/agents/collection_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/coordinator_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/coordinator_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/default.py` & `komodo_sdk-0.0.93/komodo/core/agents/default.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/difference_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/difference_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/elastic_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/groot_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/groot_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/librarian_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/librarian_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/mongo_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/mongo_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/pdf_generator.py` & `komodo_sdk-0.0.93/komodo/core/agents/pdf_generator.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/sample_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/sample_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/summarizer_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/summarizer_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/translator_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/translator_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/agents/widget_builder_agent.py` & `komodo_sdk-0.0.93/komodo/core/agents/widget_builder_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/sources/filesystem.py` & `komodo_sdk-0.0.93/komodo/core/sources/filesystem.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/sources/s3bucketkey.py` & `komodo_sdk-0.0.93/komodo/core/sources/s3bucketkey.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/sources/webpages.py` & `komodo_sdk-0.0.93/komodo/core/sources/webpages.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/sources/website_crawler.py` & `komodo_sdk-0.0.93/komodo/core/sources/website_crawler.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_count.py` & `komodo_sdk-0.0.93/komodo/core/tools/elastic/elastic_count.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_get.py` & `komodo_sdk-0.0.93/komodo/core/tools/elastic/elastic_get.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/elastic/elastic_search.py` & `komodo_sdk-0.0.93/komodo/core/tools/elastic/elastic_search.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,15 +41,24 @@
                             "description": "The starting point (offset) from the first result you want to retrieve",
                             "default": 0
                         },
                         "size": {
                             "type": "integer",
                             "description": "The the number of search hits to return. Defaults to 20.",
                             "default": 20
+                        },
+                        "sort_field": {
+                            "type": "string",
+                            "description": "The field to sort the results by. Defaults to '@timestamp'."
+                        },
+                        "sort_order": {
+                            "type": "string",
+                            "description": "The order to sort the results by. Defaults to desc."
                         }
+
                     },
                     "required": ["index", "body"]
                 },
                 "returns": {
                     "type": "string",
                     "description": "The base64 encoded results of the query."
                 }
@@ -76,22 +85,24 @@
                         indexes.append(index)
                         break
             index = ",".join(indexes)
 
             body = args["body"]
             offset = args.get("from", 0)
             size = args.get("size", 20)
+            sort_field = args.get("sort_field", "@timestamp")
+            sort_order = args.get("sort_order", "desc")
 
             # ensure only pageSize number of results are returned
             body = json.loads(body)
             body["from"] = offset
             body["size"] = size
 
             # Adding a sort clause for '@timestamp' in descending order
-            sort_condition = runtime.config.get_value("elastic_sort_condition", [{"@timestamp": {"order": "desc"}}])
+            sort_condition = runtime.config.get_value("elastic_sort_condition", [{sort_field: {"order": sort_order}}])
             body["sort"] = body.get("sort", []) + sort_condition
 
             print(f"Executing Elastic query with {index} and {body}, original index: {args['index']}")
             results = client.search(index=index, body=body)
             client.close()
 
             # Custom JSON Encoder to handle ObjectId and datetime
```

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/files/collection_builder.py` & `komodo_sdk-0.0.93/komodo/core/tools/files/collection_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/files/collection_lister.py` & `komodo_sdk-0.0.93/komodo/core/tools/files/collection_lister.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/files/collection_reader.py` & `komodo_sdk-0.0.93/komodo/core/tools/files/collection_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/files/directory_reader.py` & `komodo_sdk-0.0.93/komodo/core/tools/files/directory_reader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/files/file_reader.py` & `komodo_sdk-0.0.93/komodo/core/tools/files/file_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,19 +40,28 @@
         shortcode = self.shortcode
         super().__init__(shortcode=shortcode,
                          name=self.name,
                          definition=self.definition(shortcode),
                          action=self.action)
 
     def action(self, args, runtime: KomodoRuntime):
-        folder = Path(args.get('folder'))
-        filename = Path(args.get("filename")).name
+        folder = args.get('folder', None)
+        filename = args.get("filename", None)
         collection = runtime.selected_collection or runtime.home_folder
         path = None
 
+        if folder is None or filename is None:
+            return "Please provide folder and filename."
+
+        folder = Path(folder)
+        if not folder.exists():
+            return f"Could not find folder: {str(folder)}"
+
+        filename = Path(filename).name
+
         if folder.is_absolute():
             path = Path(folder) / filename
         elif folder.name == collection.path.name:
             path = collection.path / filename
 
         if not path or not path.exists():
             return f"Could not find folder or filename. folder: {str(folder)}, filename: {str(filename)}"
```

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/files/file_writer.py` & `komodo_sdk-0.0.93/komodo/core/tools/files/file_writer.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/markets/polygon_search.py` & `komodo_sdk-0.0.93/komodo/core/tools/markets/polygon_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_databases.py` & `komodo_sdk-0.0.93/komodo/core/tools/mongo/mongo_databases.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_schema.py` & `komodo_sdk-0.0.93/komodo/core/tools/mongo/mongo_schema.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/mongo/mongo_unique.py` & `komodo_sdk-0.0.93/komodo/core/tools/mongo/mongo_unique.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/search/vector_search.py` & `komodo_sdk-0.0.93/komodo/core/tools/search/vector_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/search/vector_search_runtime.py` & `komodo_sdk-0.0.93/komodo/core/tools/search/vector_search_runtime.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/utils/agent_tool.py` & `komodo_sdk-0.0.93/komodo/core/tools/utils/agent_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/utils/sample_tool.py` & `komodo_sdk-0.0.93/komodo/core/tools/utils/sample_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/utils/thought_tool.py` & `komodo_sdk-0.0.93/komodo/core/tools/utils/thought_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/utils/workflow_tool.py` & `komodo_sdk-0.0.93/komodo/core/tools/utils/workflow_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/web/data_fetcher.py` & `komodo_sdk-0.0.93/komodo/core/tools/web/data_fetcher.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/web/serpapi_search.py` & `komodo_sdk-0.0.93/komodo/core/tools/web/serpapi_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/web/tavily_search.py` & `komodo_sdk-0.0.93/komodo/core/tools/web/tavily_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/tools/web/web_scraper.py` & `komodo_sdk-0.0.93/komodo/core/tools/web/web_scraper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/utils/agent_helper.py` & `komodo_sdk-0.0.93/komodo/core/utils/agent_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/utils/indexer.py` & `komodo_sdk-0.0.93/komodo/core/utils/indexer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,78 @@
+import datetime
 import time
-from datetime import datetime
+from pathlib import Path
+
+from dateutil import parser
 
 from komodo.core.utils.rag_context import RagContext
 from komodo.shared.utils.filestats import file_details
 from komodo.shared.utils.globber import Globber
 
 
 class Indexer:
     def __init__(self, rag_context: RagContext):
         self.rag_context = rag_context
         self.globber = Globber(rag_context.path, self.__on_created, self.__on_deleted)
 
     def __on_created(self, filepath):
         print("Reviewing status of file: " + filepath)
-        file = self.rag_context.find_file(filepath)
-        if file and file.indexed_at:
-            print(f"Already indexed: {filepath} in collection: {self.rag_context.shortcode} at {file.indexed_at}")
+        if not self.needs_indexing(filepath):
             return
 
         # index the file
         self.rag_context.index(filepath)
 
         # update the file details
         file = file_details(filepath)
-        file.indexed_at = datetime.utcnow().isoformat() + 'Z'
+        file.indexed_at = datetime.datetime.utcnow().isoformat() + 'Z'
         self.rag_context.update_file(filepath, file)
 
     def __on_deleted(self, filepath):
         print("Removing deleted file: " + filepath)
         self.rag_context.remove(filepath)
 
     def add_intelligence(self, filepath):
         print("Adding intelligence to: " + filepath)
 
+    def needs_indexing(self, filepath):
+        print("Checking if file needs indexing: " + filepath)
+        file = self.rag_context.find_file(filepath)
+        if not file or not file.indexed_at:
+            return True
+
+        datetime_indexed_at = parser.parse(file.indexed_at)
+        datetime_modified = datetime.datetime.fromtimestamp(Path(filepath).stat().st_mtime, datetime.timezone.utc)
+
+        print(f"Indexed at: {datetime_indexed_at}")
+        print(f"Modified at: {datetime_modified}")
+
+        if datetime_indexed_at >= datetime_modified:
+            print(f"Already indexed: {filepath} in collection: {self.rag_context.shortcode} at {file.indexed_at}")
+            return False
+        else:
+            print(f"File has been updated since last index: {filepath} in collection. Re-indexing...")
+            return True
+
     def run(self, max_updates=1, update_interval=5, reindex=False):
         if reindex:
             print("Reindexing...")
             self.rag_context.reset_all()
 
+        # ensure that there have not been any files deleted since the last run
+        files = self.globber.get_files_recursively_pathlib()
+        print("Files: " + str(files))
+        ragged_files = self.rag_context.get_all_indexed_files()
+        print("Ragged Files: " + str(ragged_files))
+
+        for file in ragged_files:
+            if file not in files:
+                print("File has been deleted: " + file)
+                self.rag_context.remove(file)
+
         self.globber.start()
         update_count = 1  # start runs the initial update
         while update_count < max_updates or max_updates == 0:
             time.sleep(update_interval)
             self.globber.updates()
             update_count += 1
```

### Comparing `komodo_sdk-0.0.92/komodo/core/utils/play.py` & `komodo_sdk-0.0.93/komodo/core/utils/play.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/utils/rag_context.py` & `komodo_sdk-0.0.93/komodo/core/utils/rag_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     def get_rag_collection(self):
         collection_store = CollectionStore()
         name = os.path.basename(self.path)
         description = f"Collection for {name}"
         return collection_store.get_or_create_collection(shortcode=self.shortcode, path=self.path, name=name,
                                                          description=description)
 
+    def get_all_indexed_files(self):
+        collection = self.get_rag_collection()
+        return [file.path for file in collection.files]
+
     def find_file(self, filepath):
         print("Searching for: " + filepath + " in collection: " + self.shortcode)
         collection = self.get_rag_collection()
         collection_store = CollectionStore()
         return collection_store.find_file_in_collection(collection, filepath)
 
     def update_file(self, filepath, file):
@@ -38,14 +42,16 @@
         collection = self.get_rag_collection()
         collection_store = CollectionStore()
         collection_store.upsert_file_in_collection(collection, file)
         collection_store.store_collection(collection)
 
     def index(self, filepath):
         print("Indexing: " + filepath + " into collection: " + self.shortcode)
+        self.remove_existing_vectors(filepath)
+
         helper = VectorStoreFileHelper(filepath, self.cache_path, self.recache)
         try:
             helper.vectorize()
             if data := helper.data:
                 print("Vectors are being created for file: " + filepath)
                 self.get_vector_store().upsert_batched(data)
             else:
@@ -63,21 +69,25 @@
 
     def get_count(self):
         return self.get_vector_store().get_count()
 
     def remove(self, filepath):
         print("Removing: " + filepath + " from rag context: " + self.shortcode)
         print("Removing from index: " + filepath)
-        self.get_vector_store().delete_all_by_source(filepath)
+        self.remove_existing_vectors(filepath)
 
         print("Removing from collection: " + filepath)
         file = self.find_file(filepath)
         if file:
             collection = self.get_rag_collection()
             collection.files.remove(file)
             collection_store = CollectionStore()
             collection_store.store_collection(collection)
 
+    def remove_existing_vectors(self, filepath):
+        print("Removing existing records from index: " + filepath)
+        self.get_vector_store().delete_all_by_source(VectorStoreFileHelper.source(filepath))
+
     def reset_all(self):
         self.get_vector_store().delete_all()
         collection_store = CollectionStore()
         collection_store.remove_collection(self.shortcode)
```

### Comparing `komodo_sdk-0.0.92/komodo/core/vector_stores/pinecone_store.py` & `komodo_sdk-0.0.93/komodo/core/vector_stores/pinecone_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/vector_stores/qdrant_store.py` & `komodo_sdk-0.0.93/komodo/core/vector_stores/qdrant_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/core/vector_stores/vector_store_helper.py` & `komodo_sdk-0.0.93/komodo/core/vector_stores/vector_store_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,30 @@
         text = helper.extract_text()
         if text and len(text) > 0:
             self.chunks = self.split(text=text, chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap)
             self.data = self.create_vectors(chunks=self.chunks, path=self.path, chunk_size=self.chunk_size)
             self.update_vector_embeddings(vectors=self.data, batch_size=100)
 
     @staticmethod
+    def source(path):
+        return str(Path(path).absolute())
+
+    @staticmethod
     def split(text, chunk_size=1200, chunk_overlap=100):
         text_splitter = NLTKTextSplitter(chunk_size=chunk_size, chunk_overlap=chunk_overlap)
         chunks = text_splitter.split_text(text)
         print_gray("Split text into {} chunks of target size: {}".format(len(chunks), chunk_size))
         return chunks
 
     @staticmethod
     def create_vectors(chunks, path, chunk_size=1200):
         vectors = []
         for i, chunk in enumerate(chunks):
             metadata = MetaData(chunk=i, text=chunk, folder=path.parent.name, filename=path.name,
-                                source=str(path.absolute()), position=i * chunk_size)
+                                source=VectorStoreFileHelper.source(path), position=i * chunk_size)
             vector = Vector(chunk, metadata, None)
             vectors.append(vector)
         return vectors
 
     @staticmethod
     def update_vector_embeddings(vectors, batch_size):
         embeddings_model = get_embeddings()
```

### Comparing `komodo_sdk-0.0.92/komodo/core/workflows/sample_workflow.py` & `komodo_sdk-0.0.93/komodo/core/workflows/sample_workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/data/agents/planner/personal_finance_profile.yml` & `komodo_sdk-0.0.93/komodo/data/agents/planner/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/data/appliances/citibank/personal_finance_profile.yml` & `komodo_sdk-0.0.93/komodo/data/appliances/citibank/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf` & `komodo_sdk-0.0.93/komodo/data/appliances/komodo/dir2/InflationChapter1.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/data/workflows/analyzer/personal_finance_profile.yml` & `komodo_sdk-0.0.93/komodo/data/workflows/analyzer/personal_finance_profile.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/definitions/agents/planner/context.yml` & `komodo_sdk-0.0.93/komodo/definitions/agents/planner/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/definitions/agents/planner/role.yml` & `komodo_sdk-0.0.93/komodo/definitions/agents/planner/role.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml` & `komodo_sdk-0.0.93/komodo/definitions/agents/planner/tools/savings_monte_carlo.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/definitions/appliances/sample/context.yml` & `komodo_sdk-0.0.93/komodo/definitions/appliances/sample/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/definitions/workflows/analyzer/context.yml` & `komodo_sdk-0.0.93/komodo/definitions/workflows/analyzer/context.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_agent.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_app.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_app.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_collection.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_collection.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_config.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_context.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_context.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_datasource.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_datasource.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_locations.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_locations.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_runnable.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_runnable.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_runtime.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     def get_user_collections(self):
         if not self.user or not self.config.locations().user_collections(self.user.email).exists():
             return
 
         for item in self.config.locations().user_collections(self.user.email).iterdir():
             if item.is_dir() and item.name not in [self.user.home_shortcode, self.user.downloads_shortcode]:
-                collection = KomodoCollection(path=item, name=Path(item).stem,
+                collection = KomodoCollection(path=item, name=Path(item).stem, user=self.user,
                                               description=f"User: {item.name}", cache=self.config.cache())
                 yield collection
 
     def get_available_collections(self):
         return list(self.get_user_home()) + list(self.get_user_downloads()) + list(
             self.get_shared_collections()) + list(self.get_user_collections())
```

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_tool.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_tool.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_tool_registry.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_tool_registry.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_user.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.plan = kwargs.pop('plan', 'free')
         self.verified = kwargs.pop('verified', False)
         self.provider_id = kwargs.pop('provider_id', 'komodo')
         self.token = kwargs.pop('token', '')
 
         self.allowed_assistants = kwargs.pop('allowed_assistants', [])
         self.preferred_assistant = kwargs.pop('preferred_assistant', '')
-        self.show_tool_progress = kwargs.pop('show_tool_progress', None)
+        self.show_tool_progress = kwargs.pop('show_tool_progress', False)
         self.kwargs = kwargs
 
         # each user has a home folder / collection and a default downloads folder
         self.guid = get_text_digest(email)
         self.home_shortcode = self.guid + "_home"
         self.downloads_shortcode = self.guid + "_downloads"
```

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_vector.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_vector.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_vectorstore.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_vectorstore.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/framework/komodo_workflow.py` & `komodo_sdk-0.0.93/komodo/framework/komodo_workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/loaders/database/agent_loader.py` & `komodo_sdk-0.0.93/komodo/loaders/database/agent_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/loaders/database/appliance_loader.py` & `komodo_sdk-0.0.93/komodo/loaders/database/appliance_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/loaders/database/user_loader.py` & `komodo_sdk-0.0.93/komodo/loaders/database/user_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/loaders/filesystem/agent_loader.py` & `komodo_sdk-0.0.93/komodo/loaders/filesystem/agent_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/loaders/filesystem/appliance_loader.py` & `komodo_sdk-0.0.93/komodo/loaders/filesystem/appliance_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/loaders/filesystem/loader_helper.py` & `komodo_sdk-0.0.93/komodo/loaders/filesystem/loader_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/loaders/filesystem/loader_locations.py` & `komodo_sdk-0.0.93/komodo/loaders/filesystem/loader_locations.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/loaders/filesystem/workflow_loader.py` & `komodo_sdk-0.0.93/komodo/loaders/filesystem/workflow_loader.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/azure/azure.py` & `komodo_sdk-0.0.93/komodo/models/azure/azure.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/azure/azure_openai.py` & `komodo_sdk-0.0.93/komodo/models/azure/azure_openai.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock.py` & `komodo_sdk-0.0.93/komodo/models/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_claude.py` & `komodo_sdk-0.0.93/komodo/models/bedrock/bedrock_claude.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_cohere.py` & `komodo_sdk-0.0.93/komodo/models/bedrock/bedrock_cohere.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_model.py` & `komodo_sdk-0.0.93/komodo/models/bedrock/bedrock_model.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/bedrock/bedrock_titan.py` & `komodo_sdk-0.0.93/komodo/models/bedrock/bedrock_titan.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/framework/agent_runner.py` & `komodo_sdk-0.0.93/komodo/models/framework/agent_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/framework/appliance_utils.py` & `komodo_sdk-0.0.93/komodo/models/framework/appliance_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/framework/chat_message.py` & `komodo_sdk-0.0.93/komodo/models/framework/chat_message.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/framework/model_request.py` & `komodo_sdk-0.0.93/komodo/models/framework/model_request.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/framework/model_response.py` & `komodo_sdk-0.0.93/komodo/models/framework/model_response.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/framework/responder.py` & `komodo_sdk-0.0.93/komodo/models/framework/responder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/framework/workflow_executor.py` & `komodo_sdk-0.0.93/komodo/models/framework/workflow_executor.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/framework/workflow_runner.py` & `komodo_sdk-0.0.93/komodo/models/framework/workflow_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/openai/openai_api.py` & `komodo_sdk-0.0.93/komodo/models/openai/openai_api.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/openai/openai_api_streamed.py` & `komodo_sdk-0.0.93/komodo/models/openai/openai_api_streamed.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/openai/openai_api_streamed_tool_call.py` & `komodo_sdk-0.0.93/komodo/models/openai/openai_api_streamed_tool_call.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/models/openai/openai_debug.py` & `komodo_sdk-0.0.93/komodo/models/openai/openai_debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class OpenAIProcessDebug():
 
     def __init__(self, runtime: KomodoRuntime):
         self.tools = runtime.agent.tools
         self.show_tool_progress = runtime.user.show_tool_progress
 
     def debug_enabled(self):
-        return self.show_tool_progress and self.show_tool_progress.lower() != 'none'
+        return self.show_tool_progress
 
     def debug_invoke(self, call):
         if not self.debug_enabled():
             return ""
 
         message = self.debug_invoke_internal(call)
         return debug_print(message)
@@ -52,15 +52,19 @@
             return f"""Received response from {tool.name}.
     {contents_display}"""
 
         return f"Received response from {tool.name}: {contents_display}"
 
     def debug_message_tokens(self, message, tokens):
         snippet = message['content'].replace("\n", " ")[:80]
-        print_info(f"Tokens: {tokens:6}: {message['role']}: {snippet}")
+        if message['role'] == 'function':
+            print_info(f"Tokens: {tokens:6}: name: {message['name']}, "
+                       f"tool_call_id: {message['tool_call_id']} {message['role']}: {snippet}")
+        else:
+            print_info(f"Tokens: {tokens:6}: {message['role']}: {snippet}")
 
     def debug_input_tokens(self, total_input_tokens):
         print_info(f"Tokens: {total_input_tokens:6}: Total input tokens")
 
     def debug_output_tokens(self, total_output_tokens):
         print_info(f"Tokens: {total_output_tokens:6}: Total output tokens")
```

### Comparing `komodo_sdk-0.0.92/komodo/models/openai/openai_process_actions.py` & `komodo_sdk-0.0.93/komodo/models/openai/openai_process_actions.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/collection.proto` & `komodo_sdk-0.0.93/komodo/proto/collection.proto`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     string name = 2;
     string description = 3;
     string path = 4;
     string created_at = 5;
     string modified_at = 6;
     repeated File files = 7;
 
+    int32 ctime = 5;
+    int32 mtime = 6;
+
     string summary = 32;
     string query = 51;
     repeated QnA questions = 52;
 }
 
 message File {
     string guid = 1;
```

### Comparing `komodo_sdk-0.0.92/komodo/proto/data.proto` & `komodo_sdk-0.0.93/komodo/proto/data.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/model.proto` & `komodo_sdk-0.0.93/komodo/proto/model.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/report.proto` & `komodo_sdk-0.0.93/komodo/proto/report.proto`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/sample.py` & `komodo_sdk-0.0.93/komodo/proto/sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/generated/collection_pb2.py` & `komodo_sdk-0.0.93/komodo/proto/generated/collection_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/generated/collection_pb2.pyi` & `komodo_sdk-0.0.93/komodo/proto/generated/collection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/generated/data_pb2.py` & `komodo_sdk-0.0.93/komodo/proto/generated/data_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/generated/data_pb2.pyi` & `komodo_sdk-0.0.93/komodo/proto/generated/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/generated/model_pb2.py` & `komodo_sdk-0.0.93/komodo/proto/generated/model_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/generated/model_pb2.pyi` & `komodo_sdk-0.0.93/komodo/proto/generated/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/generated/report_pb2.py` & `komodo_sdk-0.0.93/komodo/proto/generated/report_pb2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/proto/generated/report_pb2.pyi` & `komodo_sdk-0.0.93/komodo/proto/generated/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/scripts/run_agent_runner.py` & `komodo_sdk-0.0.93/komodo/scripts/run_agent_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/scripts/run_agent_runner_2.py` & `komodo_sdk-0.0.93/komodo/scripts/run_agent_runner_2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/scripts/run_difference_agent.py` & `komodo_sdk-0.0.93/komodo/scripts/run_difference_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/scripts/run_librarian_agent.py` & `komodo_sdk-0.0.93/komodo/scripts/run_librarian_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/scripts/run_streaming_test.py` & `komodo_sdk-0.0.93/komodo/scripts/run_streaming_test.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/scripts/run_widget_builder.py` & `komodo_sdk-0.0.93/komodo/scripts/run_widget_builder.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/agent_router.py` & `komodo_sdk-0.0.93/komodo/server/agent_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/appliance_router.py` & `komodo_sdk-0.0.93/komodo/server/appliance_router.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import datetime
-
 from fastapi import Depends, APIRouter
 
-from komodo.server.globals import get_appliance, get_email, get_user
+from komodo.server.globals import get_appliance, get_email, get_user, get_version
 
 router = APIRouter(
     prefix='/api/v1/appliance',
     tags=['Appliance']
 )
 
 
@@ -28,22 +26,14 @@
 
 @router.get('/configuration', response_model=dict, summary='Get appliance configuration',
             description='Get the configuration of the appliance.')
 def get_appliance_configuration(user=Depends(get_user), appliance=Depends(get_appliance)):
     return appliance.configuration(user)
 
 
-def get_version():
-    import importlib.metadata
-    try:
-        return importlib.metadata.version('komodo-sdk')
-    except importlib.metadata.PackageNotFoundError:
-        return "0.0.0." + str(datetime.datetime.now().strftime('%Y%m%d'))
-
-
 @router.get('/index', summary='Index all data sources',
             description='Index all data sources for the appliance.')
 def index_all_data_sources(appliance=Depends(get_appliance)):
     appliance.index(reindex=False)
     return {"status": "success"}
```

### Comparing `komodo_sdk-0.0.92/komodo/server/ask_request.py` & `komodo_sdk-0.0.93/komodo/server/ask_request.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/audio_router.py` & `komodo_sdk-0.0.93/komodo/server/audio_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/collections_router.py` & `komodo_sdk-0.0.93/komodo/server/collections_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/conversation_router.py` & `komodo_sdk-0.0.93/komodo/server/conversation_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/fast.py` & `komodo_sdk-0.0.93/komodo/server/fast.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/globals.py` & `komodo_sdk-0.0.93/komodo/server/globals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import datetime
+
 from fastapi import HTTPException, Depends, Header, Body
 
 from komodo.framework.komodo_app import KomodoApp
 from komodo.framework.komodo_collection import KomodoCollection
 from komodo.framework.komodo_runtime import KomodoRuntime
 from komodo.framework.komodo_user import KomodoUser
 from komodo.loaders.database.user_loader import UserLoader
@@ -54,14 +56,22 @@
     return user.email
 
 
 def get_appliance_runtime(user=Depends(get_user), appliance=Depends(get_appliance)):
     return KomodoRuntime(appliance=appliance, user=user)
 
 
+def get_version():
+    import importlib.metadata
+    try:
+        return importlib.metadata.version('komodo-sdk')
+    except importlib.metadata.PackageNotFoundError:
+        return "0.0.0." + str(datetime.datetime.now().strftime('%Y%m%d'))
+
+
 def get_selected_collection(shortcode, runtime=Depends(get_appliance_runtime)) -> KomodoCollection:
     if collection := runtime.get_collection(shortcode):
         return collection
 
     raise HTTPException(status_code=404, detail="Collection not found: " + shortcode)
```

### Comparing `komodo_sdk-0.0.92/komodo/server/logo_router.py` & `komodo_sdk-0.0.93/komodo/server/logo_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/report_router.py` & `komodo_sdk-0.0.93/komodo/server/report_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/server/user_router.py` & `komodo_sdk-0.0.93/komodo/server/user_router.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/directory/assistants_helpers.py` & `komodo_sdk-0.0.93/komodo/shared/directory/assistants_helpers.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/documents/file_writer_helper.py` & `komodo_sdk-0.0.93/komodo/shared/documents/file_writer_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/documents/text_convert_helper.py` & `komodo_sdk-0.0.93/komodo/shared/documents/text_convert_helper.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/documents/text_extract.py` & `komodo_sdk-0.0.93/komodo/shared/documents/text_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     result = chardet.detect(raw_data)
     encoding = result['encoding']
 
     # Now that you know the encoding, you can decode the content
     with open(path, 'rb') as file:
         content = file.read().decode(encoding).strip()
 
-    print(f"Detected encoding: {encoding}")
+    # print(f"Detected encoding: {encoding}")
     return content
 
 
 def extract_text_from_pdf(path):
     try:
         return extract_text_from_pdf_textract(path)
     except Exception as e:
```

### Comparing `komodo_sdk-0.0.92/komodo/shared/documents/text_extract_helper.py` & `komodo_sdk-0.0.93/komodo/shared/documents/text_extract_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,21 @@
         if cache_path:
             digest = get_file_digest_short(path)
             self.cache_folder = Path(cache_path) / digest
             os.makedirs(self.cache_folder, exist_ok=True)
 
     def extract_text(self):
         if self.cache_path:
+            # ensure cache is up-to-date
+            updated_at = os.path.getmtime(self.path)
+            extracted_at = os.path.getmtime(self.extracted_path()) if os.path.exists(self.extracted_path()) else 0
+            if updated_at > extracted_at:
+                print("File was created or updated recently. Will extract and cache: " + str(self.path))
+                self.recache = True
+
             if not self.recache:
                 if cached_text := self.get_cached_extracted_text():
                     print("Using cached text for: " + str(self.path))
                     return cached_text
 
             text = self.extract_and_cache()
             return text
@@ -41,20 +48,20 @@
         text = extract_text_from_path(self.path)
         if text:
             with open(self.extracted_path(), "w") as f:
                 f.write(text)
         return text
 
     def get_cached_extracted_text(self):
-        try:
-            if os.path.exists(self.cache_folder):
+        if os.path.exists(self.cache_folder) and os.path.exists(self.extracted_path()):
+            try:
                 with open(self.extracted_path()) as f:
                     return f.read()
-        except Exception as e:
-            print(f"Error reading cached text from {self.cache_folder}: {e}")
+            except Exception as e:
+                print(f"Error reading cached text from {self.cache_folder}: {e}")
         return None
 
 
 if __name__ == "__main__":
     # Example usage:
     # helper = TextExtractHelper(path="/path/to/your/file", cache_path="/path/to/your/cache")
     # text = helper.extract_text()
```

### Comparing `komodo_sdk-0.0.92/komodo/shared/documents/text_html.py` & `komodo_sdk-0.0.93/komodo/shared/documents/text_html.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/embeddings/faiss_store.py` & `komodo_sdk-0.0.93/komodo/shared/embeddings/faiss_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/embeddings/pinecone_store.py` & `komodo_sdk-0.0.93/komodo/shared/embeddings/pinecone_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/mssql/mssql.py` & `komodo_sdk-0.0.93/komodo/shared/mssql/mssql.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/api_query.py` & `komodo_sdk-0.0.93/komodo/shared/utils/api_query.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/digest.py` & `komodo_sdk-0.0.93/komodo/shared/utils/digest.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/filestats.py` & `komodo_sdk-0.0.93/komodo/shared/utils/filestats.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/globber.py` & `komodo_sdk-0.0.93/komodo/shared/utils/globber.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/lambda_entry.py` & `komodo_sdk-0.0.93/komodo/shared/utils/lambda_entry.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/lambda_utils.py` & `komodo_sdk-0.0.93/komodo/shared/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/logconfig.py` & `komodo_sdk-0.0.93/komodo/shared/utils/logconfig.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/s3_file_utils.py` & `komodo_sdk-0.0.93/komodo/shared/utils/s3_file_utils.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/tags.py` & `komodo_sdk-0.0.93/komodo/shared/utils/tags.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/term_colors.py` & `komodo_sdk-0.0.93/komodo/shared/utils/term_colors.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/timebox.py` & `komodo_sdk-0.0.93/komodo/shared/utils/timebox.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/shared/utils/watcher.py` & `komodo_sdk-0.0.93/komodo/shared/utils/watcher.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/store/agent_store.py` & `komodo_sdk-0.0.93/komodo/store/agent_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/store/appliance_store.py` & `komodo_sdk-0.0.93/komodo/store/appliance_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/store/collection_store.py` & `komodo_sdk-0.0.93/komodo/store/collection_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/store/conversations_store.py` & `komodo_sdk-0.0.93/komodo/store/conversations_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/store/logo_store.py` & `komodo_sdk-0.0.93/komodo/store/logo_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/store/redis_database.py` & `komodo_sdk-0.0.93/komodo/store/redis_database.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/store/tool_store.py` & `komodo_sdk-0.0.93/komodo/store/tool_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/store/user_store.py` & `komodo_sdk-0.0.93/komodo/store/user_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/core/test_elastic_agent.py` & `komodo_sdk-0.0.93/komodo/tests/core/test_elastic_agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/core/test_elastic_sample.py` & `komodo_sdk-0.0.93/komodo/tests/core/test_elastic_sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/core/test_elastic_tools.py` & `komodo_sdk-0.0.93/komodo/tests/core/test_elastic_tools.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/core/test_mongo_sample.py` & `komodo_sdk-0.0.93/komodo/tests/core/test_mongo_sample.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/core/test_mongo_tools.py` & `komodo_sdk-0.0.93/komodo/tests/core/test_mongo_tools.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/core/test_serpapi_search.py` & `komodo_sdk-0.0.93/komodo/tests/core/test_serpapi_search.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/models/test_bedrock.py` & `komodo_sdk-0.0.93/komodo/tests/models/test_bedrock.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/models/test_workflow_runner.py` & `komodo_sdk-0.0.93/komodo/tests/models/test_workflow_runner.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/shared/test_mssql.py` & `komodo_sdk-0.0.93/komodo/tests/shared/test_mssql.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/komodo/tests/store/test_conversation_store.py` & `komodo_sdk-0.0.93/komodo/tests/store/test_conversation_store.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/pdf2html/Dockerfile` & `komodo_sdk-0.0.93/pdf2html/Dockerfile`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/pdf2html/server.py` & `komodo_sdk-0.0.93/pdf2html/server.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/pdf2html/data/sample.html` & `komodo_sdk-0.0.93/pdf2html/data/sample.html`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/pdf2html/data/sample.pdf` & `komodo_sdk-0.0.93/pdf2html/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/Dockerfile` & `komodo_sdk-0.0.93/sample/Dockerfile`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/docker-compose.yml` & `komodo_sdk-0.0.93/sample/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/docker-production.yml` & `komodo_sdk-0.0.93/sample/docker-production.yml`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/appliance/appliance.py` & `komodo_sdk-0.0.93/sample/appliance/appliance.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/appliance/config.py` & `komodo_sdk-0.0.93/sample/appliance/config.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/appliance/seed.py` & `komodo_sdk-0.0.93/sample/appliance/seed.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/appliance/server.py` & `komodo_sdk-0.0.93/sample/appliance/server.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/appliance/workflow.py` & `komodo_sdk-0.0.93/sample/appliance/workflow.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/definitions/agents/dasher_v1/instructions.txt` & `komodo_sdk-0.0.93/sample/definitions/agents/dasher_v1/instructions.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/definitions/agents/dasher_v2/instructions.txt` & `komodo_sdk-0.0.93/sample/definitions/agents/dasher_v2/instructions.txt`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/app.py` & `komodo_sdk-0.0.93/sample/widgets/app.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/globals.py` & `komodo_sdk-0.0.93/sample/widgets/globals.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/themes.py` & `komodo_sdk-0.0.93/sample/widgets/themes.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/assets/custom.css` & `komodo_sdk-0.0.93/sample/widgets/assets/custom.css`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/agent.py` & `komodo_sdk-0.0.93/sample/widgets/pages/agent.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/analytics.py` & `komodo_sdk-0.0.93/sample/widgets/pages/analytics.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/appliance.py` & `komodo_sdk-0.0.93/sample/widgets/pages/appliance.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/dasher_v1.py` & `komodo_sdk-0.0.93/sample/widgets/pages/dasher_v1.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/dasher_v2.py` & `komodo_sdk-0.0.93/sample/widgets/pages/dasher_v2.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/department.py` & `komodo_sdk-0.0.93/sample/widgets/pages/department.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/present.py` & `komodo_sdk-0.0.93/sample/widgets/pages/present.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/report.py` & `komodo_sdk-0.0.93/sample/widgets/pages/report.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/side_bar.py` & `komodo_sdk-0.0.93/sample/widgets/pages/side_bar.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/reports/bar_chart.py` & `komodo_sdk-0.0.93/sample/widgets/pages/reports/bar_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/reports/line_chart.py` & `komodo_sdk-0.0.93/sample/widgets/pages/reports/line_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/sample/widgets/pages/reports/pie_chart.py` & `komodo_sdk-0.0.93/sample/widgets/pages/reports/pie_chart.py`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/README.md` & `komodo_sdk-0.0.93/website/README.md`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/package-lock.json` & `komodo_sdk-0.0.93/website/package-lock.json`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/package.json` & `komodo_sdk-0.0.93/website/package.json`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/tailwind.config.js` & `komodo_sdk-0.0.93/website/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/deployment/nginx.default.conf` & `komodo_sdk-0.0.93/website/deployment/nginx.default.conf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/chaticon.png` & `komodo_sdk-0.0.93/website/public/chaticon.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/faqbg.png` & `komodo_sdk-0.0.93/website/public/faqbg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/favicon.ico` & `komodo_sdk-0.0.93/website/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/footer.png` & `komodo_sdk-0.0.93/website/public/footer.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/home.png` & `komodo_sdk-0.0.93/website/public/home.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/index.html` & `komodo_sdk-0.0.93/website/public/index.html`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/logo192.png` & `komodo_sdk-0.0.93/website/public/logo192.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/logo512.png` & `komodo_sdk-0.0.93/website/public/logo512.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/pricingBg.png` & `komodo_sdk-0.0.93/website/public/pricingBg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/pricingBg1.png` & `komodo_sdk-0.0.93/website/public/pricingBg1.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Heavy.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-HeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-Thin.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.otf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf` & `komodo_sdk-0.0.93/website/public/Cerebri.Sans.Pro-www.Dfonts.org/Cerebri.Sans.Pro/CerebriSansPro-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/App.css` & `komodo_sdk-0.0.93/website/src/App.css`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/RouterMain.js` & `komodo_sdk-0.0.93/website/src/RouterMain.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/index.css` & `komodo_sdk-0.0.93/website/src/index.css`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/index.js` & `komodo_sdk-0.0.93/website/src/index.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/logo.svg` & `komodo_sdk-0.0.93/website/src/logo.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/API/API_data.js` & `komodo_sdk-0.0.93/website/src/API/API_data.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/API/ApiComment.js` & `komodo_sdk-0.0.93/website/src/API/ApiComment.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -18,13 +18,18 @@
     collectionsGetUrl: Url + "/collections",
     collectionsAddUrl: Url + "/collections",
     collectionsGetCollectionUrl: (shortcode) => Url + "/collections/" + shortcode,
     collectionsDeleteCollectionUrl: (shortcode) =>
         Url + "/collections/" + shortcode,
     collectionsUploadFilesUrl: (shortcode) =>
         Url + "/collections/upload_files/" + shortcode,
-    collectionsDownloadFileUrl: (shortcode, file_guid) =>
+    collectionsDownloadFileUrl: (shortcode, file_guid, isText) =>
         // Url + "/collections/" + shortcode + "/" + file_guid + "/text",
-        Url + "/collections/" + shortcode + "/" + file_guid,
+        Url +
+        "/collections/" +
+        shortcode +
+        "/" +
+        file_guid +
+        `${isText ? "/text" : ""}`,
     collectionsChatDeleteCollectionUrl: (shortcode, fileId) =>
         Url + "/collections/" + shortcode + "/" + fileId,
 };
```

### Comparing `komodo_sdk-0.0.92/website/src/assets/Frame.svg` & `komodo_sdk-0.0.93/website/src/assets/Frame.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/ai.png` & `komodo_sdk-0.0.93/website/src/assets/ai.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/blue.svg` & `komodo_sdk-0.0.93/website/src/assets/blue.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/botAvatar.svg` & `komodo_sdk-0.0.93/website/src/assets/botAvatar.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/chatListIcon.svg` & `komodo_sdk-0.0.93/website/src/assets/chatListIcon.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/docs.svg` & `komodo_sdk-0.0.93/website/src/assets/docs.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/docx.png` & `komodo_sdk-0.0.93/website/src/assets/docx.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/folder.svg` & `komodo_sdk-0.0.93/website/src/assets/folder.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/gallery.svg` & `komodo_sdk-0.0.93/website/src/assets/gallery.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/headphone.svg` & `komodo_sdk-0.0.93/website/src/assets/headphone.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/magicpen-1.svg` & `komodo_sdk-0.0.93/website/src/assets/magicpen-1.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/magicpen.svg` & `komodo_sdk-0.0.93/website/src/assets/magicpen.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/message.svg` & `komodo_sdk-0.0.93/website/src/assets/message.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/multi.png` & `komodo_sdk-0.0.93/website/src/assets/multi.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/odt.png` & `komodo_sdk-0.0.93/website/src/assets/odt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/pdf.png` & `komodo_sdk-0.0.93/website/src/assets/pdf.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/pdf.svg` & `komodo_sdk-0.0.93/website/src/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/pricingBg.png` & `komodo_sdk-0.0.93/website/src/assets/pricingBg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/profile.png` & `komodo_sdk-0.0.93/website/src/assets/profile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/send.png` & `komodo_sdk-0.0.93/website/src/assets/send.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/setting-1.svg` & `komodo_sdk-0.0.93/website/src/assets/setting-1.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/setting.svg` & `komodo_sdk-0.0.93/website/src/assets/setting.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/text.png` & `komodo_sdk-0.0.93/website/src/assets/text.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/text.svg` & `komodo_sdk-0.0.93/website/src/assets/text.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/trash.svg` & `komodo_sdk-0.0.93/website/src/assets/trash.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/assets/userProfile.svg` & `komodo_sdk-0.0.93/website/src/assets/userProfile.svg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/auth/Login.js` & `komodo_sdk-0.0.93/website/src/auth/Login.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/auth/Signup.js` & `komodo_sdk-0.0.93/website/src/auth/Signup.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/Dashboard.js` & `komodo_sdk-0.0.93/website/src/components/Dashboard.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/DocumentView.js` & `komodo_sdk-0.0.93/website/src/components/DocumentView.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,94 +1,113 @@
 import React, {
-    memo,
+    useState,
     useContext,
     useEffect,
-    useState
+    useMemo,
+    memo
 } from "react";
 import roleContext from "../contexts/roleContext";
 import DocViewer, {
     DocViewerRenderers
 } from "@cyntler/react-doc-viewer";
 import {
     OutTable
 } from "react-excel-renderer";
 
 const DocumentView = ({
     foo
 }) => {
     const contextFiles = useContext(roleContext);
     const [pdfURL, setPdfURL] = useState();
-
+    console.log("pdfURL :>> ", pdfURL);
     useEffect(() => {
         setPdfURL(contextFiles?.pdfURL);
     }, [contextFiles?.pdfURL]);
 
+    const memoizedComponent = useMemo(() => {
+        return pdfURL ? (
+            pdfURL?.rows && pdfURL?.cols ? ( <
+                OutTable key = "OutTable"
+                data = {
+                    pdfURL?.rows || []
+                }
+                columns = {
+                    pdfURL?.cols || []
+                }
+                tableClassName = "ExcelTable2007 border"
+                tableHeaderRowClass = "font-bold bg-blue-100" /
+                >
+            ) : contextFiles?.fileType === "text/plain" ? ( <
+                pre className = "text-wrap font-cerebriregular" > {
+                    pdfURL
+                } < /pre>
+            ) : contextFiles?.fileType === "application/vnd.openxmlformats-officedocument.wordprocessingml.document" ? ( <
+                pre className = "text-wrap font-cerebriregular" > {
+                    pdfURL
+                } < /pre>
+            ) : contextFiles?.fileType === "application/vnd.openxmlformats-officedocument.presentationml.presentation" ? ( <
+                pre className = "text-wrap font-cerebriregular" > {
+                    pdfURL
+                } < /pre>
+            ) : ( <
+                DocViewer key = "DocViewer"
+                pluginRenderers = {
+                    DocViewerRenderers
+                }
+                documents = {
+                    [{
+                        uri: pdfURL
+                    }]
+                }
+                config = {
+                    {
+                        header: {
+                            disableHeader: true,
+                            disableFileName: false,
+                            retainURLParams: false,
+                        },
+                        pdfVerticalScrollByDefault: true,
+                        loadingRenderer: {
+                            overrideComponent: () => {
+                                console.log("Loading...");
+                                return < div > Loading Custom < /div>;
+                            },
+                            showLoadingTimeout: true,
+                        },
+                        noRenderer: {
+                            overrideComponent: ({
+                                document
+                            }) => {
+                                return ( <
+                                    div className = "flex justify-center items-center w-full" >
+                                    Error: {
+                                        " "
+                                    } {
+                                        document?.fileType?.includes("webp") ?
+                                            "Webp file not supported" :
+                                            "Something went wrong"
+                                    } <
+                                    /div>
+                                );
+                            },
+                        },
+                    }
+                }
+                />
+            )
+        ) : null;
+    }, [pdfURL]);
+
     return ( <
         div className = {
             `bg-[#FFFFFF] h-[calc(100vh-93px)] overflow-auto scrollbarCustom px-3 `
         }
         // scrollbar - remove scrollbar
         >
         {
-            pdfURL ? (
-                pdfURL?.rows && pdfURL?.cols ? ( <
-                    OutTable data = {
-                        pdfURL?.rows || []
-                    }
-                    columns = {
-                        pdfURL?.cols || []
-                    }
-                    tableClassName = "ExcelTable2007 border"
-                    tableHeaderRowClass = "font-bold bg-blue-100" /
-                    >
-                ) : ( <
-                    DocViewer pluginRenderers = {
-                        DocViewerRenderers
-                    }
-                    documents = {
-                        [{
-                            uri: pdfURL
-                        }]
-                    }
-                    config = {
-                        {
-                            header: {
-                                disableHeader: true,
-                                disableFileName: false,
-                                retainURLParams: false,
-                            },
-                            pdfVerticalScrollByDefault: true,
-                            loadingRenderer: {
-                                overrideComponent: () => {
-                                    console.log("Loading...");
-                                    return < div > Loading Custom < /div>;
-                                },
-                                showLoadingTimeout: true,
-                            },
-                            noRenderer: {
-                                overrideComponent: ({
-                                    document
-                                }) => {
-                                    return ( <
-                                        div className = "flex justify-center items-center w-full" >
-                                        Error: {
-                                            " "
-                                        } {
-                                            document?.fileType?.includes("webp") ?
-                                                "Webp file not supported" :
-                                                "Something went wrong"
-                                        } <
-                                        /div>
-                                    );
-                                },
-                            },
-                        }
-                    }
-                    />
-                )
-            ) : null
+            memoizedComponent
         } <
         /div>
     );
 };
 
 export default memo(DocumentView);
```

### Comparing `komodo_sdk-0.0.92/website/src/components/Header.js` & `komodo_sdk-0.0.93/website/src/components/Header.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -11,15 +11,15 @@
 
 const Header = () => {
     const navigate = useNavigate();
     const path = window?.location?.hash;
     const selectContext = useContext(roleContext);
     const location = useLocation();
     const searchParams = new URLSearchParams(location.search).get("feature");
-    // console.log(searchParams, "searchParams");
+    console.log(searchParams, "searchParams");
     // console.log("location :>> ", location);
     function handleChange(val) {
         const user = JSON.parse(localStorage.getItem("komodoUser"));
         localStorage.setItem(
             "komodoUser",
             JSON.stringify({
                 ...user,
@@ -27,15 +27,15 @@
             })
         );
         selectContext?.setReactSelect(val);
         selectContext?.setChatGuid("");
         selectContext?.setChatHistory(false);
         selectContext?.setList([]);
         // navigate(path);
-        navigate("/chat");
+        navigate(`/chat${location?.search}`);
     }
 
     const style = {
         control: (base) => ({
             ...base,
             cursor: "pointer",
             border: "0",
@@ -73,40 +73,48 @@
         div className = "w-full xl:flex xl:justify-center xl:items-center xl:flex-col sm:ms-20" > {
             selectContext?.agentList?.length &&
             selectContext?.agentList[searchParams ?? 0]?.agents?.length > 0 ? (
                 // {selectContext?.reactSelect?.purpose !== undefined ? (
                 <
                 >
                 <
-                div className = "min-w-[200px] max-w-fit" >
-                <
-                Select className = "font-cerebriregular selectstyle"
-                // value={selectContext?.agentList[searchParams ?? 0]?.agents?.[0]}
-                value = {
-                    selectContext?.reactSelect
-                }
-                onChange = {
-                    handleChange
-                }
-                // options={location?.state?.agent}
-                options = {
-                    selectContext?.agentList?.length &&
-                    selectContext?.agentList[searchParams ?? 0]?.agents
-                }
-                // options={selectContext?.agentList?.agents}
-                styles = {
-                    style
-                }
-                getOptionLabel = {
-                    (agent) => agent["name"]
-                }
-                getOptionValue = {
-                    (agent) => agent["email"]
-                }
-                /> <
+                div className = "min-w-[200px] max-w-fit" > {
+                    selectContext?.agentList[searchParams ?? 0]?.agents?.length >
+                    1 ? ( <
+                        Select className = "font-cerebriregular selectstyle"
+                        // value={selectContext?.agentList[searchParams ?? 0]?.agents?.[0]}
+                        value = {
+                            selectContext?.reactSelect
+                        }
+                        onChange = {
+                            handleChange
+                        }
+                        // options={location?.state?.agent}
+                        options = {
+                            selectContext?.agentList?.length &&
+                            selectContext?.agentList[searchParams ?? 0]?.agents
+                        }
+                        // options={selectContext?.agentList?.agents}
+                        styles = {
+                            style
+                        }
+                        getOptionLabel = {
+                            (agent) => agent["name"]
+                        }
+                        getOptionValue = {
+                            (agent) => agent["email"]
+                        }
+                        />
+                    ) : ( <
+                        div className = "font-cerebri selectstyle text-[21px] " > {
+                            selectContext?.agentList[searchParams ?? 0]?.agents[0]?.name
+                        } <
+                        /div>
+                    )
+                } <
                 /div> <
                 p className = "m-[2px] font-cerebriregular xl:-ms-4 xs:ms-0 xs:text-center sm:text-[15px] subtitle cursor-pointer"
                 title = {
                     selectContext?.reactSelect?.purpose || ""
                 } >
                 {
                     selectContext?.reactSelect?.purpose || ""
```

### Comparing `komodo_sdk-0.0.92/website/src/components/HeaderSideBar.js` & `komodo_sdk-0.0.93/website/src/components/HeaderSideBar.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/Home.jsx` & `komodo_sdk-0.0.93/website/src/components/Home.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/LayoutHeader.js` & `komodo_sdk-0.0.93/website/src/components/LayoutHeader.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/NavigateBack.js` & `komodo_sdk-0.0.93/website/src/components/NavigateBack.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/Sidebar.js` & `komodo_sdk-0.0.93/website/src/components/Sidebar.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -84,43 +84,43 @@
         localStorage?.removeItem("react-resizable-panels:example");
         navigate(`/${val.feature}?feature=${i}`);
     };
 
     const customIcon = (index) => {};
 
     const icon = {
-        0: ( <
+        chat: ( <
             svg xmlns = "http://www.w3.org/2000/svg"
             width = "26"
             height = "26"
             viewBox = "0 0 24 18"
             fill = "none" >
             <
             path d = "M18.5546 0.817871H7.58507C4.95304 0.817871 2.81163 2.78037 2.81163 5.19287V12.8835L0.822569 15.8194C0.733591 15.9506 0.682026 16.1036 0.67341 16.2618C0.664793 16.4201 0.699451 16.5778 0.773662 16.7178C0.847872 16.8579 0.958833 16.9751 1.09463 17.0569C1.23043 17.1386 1.38593 17.1819 1.54444 17.1819H18.5546C21.1866 17.1819 23.328 15.2194 23.328 12.8069V5.19287C23.328 2.78037 21.1866 0.817871 18.5546 0.817871ZM14.1241 12.3108H8.13507C8.01822 12.3143 7.90186 12.2943 7.79288 12.252C7.68391 12.2097 7.58453 12.146 7.50064 12.0646C7.41675 11.9832 7.35006 11.8857 7.30452 11.7781C7.25898 11.6704 7.23551 11.5547 7.23551 11.4378C7.23551 11.3209 7.25898 11.2052 7.30452 11.0975C7.35006 10.9899 7.41675 10.8924 7.50064 10.811C7.58453 10.7296 7.68391 10.6658 7.79288 10.6235C7.90186 10.5812 8.01822 10.5612 8.13507 10.5647H14.1241C14.3512 10.5715 14.5666 10.6665 14.7248 10.8295C14.883 10.9925 14.9714 11.2107 14.9714 11.4378C14.9714 11.6649 14.883 11.8831 14.7248 12.0461C14.5666 12.2091 14.3512 12.304 14.1241 12.3108ZM18.0476 7.4374H8.13507C8.01822 7.4409 7.90186 7.4209 7.79288 7.3786C7.68391 7.3363 7.58453 7.27255 7.50064 7.19113C7.41675 7.10972 7.35006 7.01229 7.30452 6.90463C7.25898 6.79697 7.23551 6.68125 7.23551 6.56435C7.23551 6.44745 7.25898 6.33174 7.30452 6.22408C7.35006 6.11642 7.41675 6.01899 7.50064 5.93758C7.58453 5.85616 7.68391 5.79241 7.79288 5.75011C7.90186 5.70781 8.01822 5.68781 8.13507 5.69131H18.0476C18.2746 5.6981 18.49 5.79306 18.6482 5.95605C18.8064 6.11903 18.8949 6.33723 18.8949 6.56435C18.8949 6.79148 18.8064 7.00968 18.6482 7.17266C18.49 7.33565 18.2746 7.43061 18.0476 7.4374Z"
             fill = "white" /
             >
             <
             /svg>
         ),
-        1: ( <
+        chatdoc: ( <
             svg xmlns = "http://www.w3.org/2000/svg"
             width = "26"
             height = "26"
             viewBox = "0 0 29 28"
             fill = "none" >
             <
             path fill - rule = "evenodd"
             clip - rule = "evenodd"
             d = "M0.5 5.60002C0.5 2.50741 3.00741 0 6.10002 0H22.9001C25.9927 0 28.5001 2.50741 28.5001 5.60002V18.6667C28.5001 21.7593 25.9927 24.2667 22.9001 24.2667H18.1905L15.2024 27.6814C15.1148 27.7814 15.0068 27.8617 14.8857 27.9166C14.7645 27.9716 14.6331 28 14.5 28C14.367 28 14.2356 27.9716 14.1144 27.9166C13.9933 27.8617 13.8853 27.7814 13.7977 27.6814L10.8101 24.2667H6.10002C3.00741 24.2667 0.5 21.7593 0.5 18.6667V5.60002ZM14.5 5.60002C14.7116 5.60003 14.9168 5.67188 15.0821 5.80381C15.2475 5.93574 15.3631 6.11991 15.41 6.32615L15.9266 8.59743C16.0437 9.11208 16.3038 9.58317 16.677 9.95638C17.0502 10.3296 17.5213 10.5897 18.036 10.7068L20.3073 11.2234C20.5135 11.2704 20.6976 11.386 20.8295 11.5513C20.9614 11.7167 21.0332 11.9219 21.0332 12.1334C21.0332 12.3449 20.9614 12.5501 20.8295 12.7154C20.6976 12.8807 20.5135 12.9964 20.3073 13.0434L18.036 13.56C17.5213 13.677 17.0502 13.9371 16.677 14.3104C16.3038 14.6836 16.0437 15.1547 15.9266 15.6693L15.41 17.9401C15.3631 18.1463 15.2474 18.3305 15.0821 18.4623C14.9168 18.5942 14.7115 18.6661 14.5 18.6661C14.2886 18.6661 14.0833 18.5942 13.918 18.4623C13.7527 18.3305 13.637 18.1463 13.59 17.9401L13.0734 15.6693C12.9564 15.1547 12.6963 14.6836 12.3231 14.3104C11.9498 13.9371 11.4788 13.677 10.9641 13.56L8.69329 13.0434C8.48709 12.9964 8.30296 12.8807 8.17107 12.7154C8.03918 12.5501 7.96735 12.3449 7.96735 12.1334C7.96735 11.9219 8.03918 11.7167 8.17107 11.5513C8.30296 11.386 8.48709 11.2704 8.69329 11.2234L10.9641 10.7068C11.4788 10.5897 11.9498 10.3296 12.3231 9.95638C12.6963 9.58317 12.9564 9.11208 13.0734 8.59743L13.59 6.32662C13.6369 6.12029 13.7525 5.93601 13.9178 5.80399C14.0832 5.67197 14.2885 5.60005 14.5 5.60002Z"
             fill = "white" /
             >
             <
             /svg>
         ),
-        2: ( <
+        reportbuilder: ( <
             svg xmlns = "http://www.w3.org/2000/svg"
             width = "26"
             height = "26"
             viewBox = "0 0 26 26"
             fill = "none" >
             <
             path d = "M9.47913 3.79199V2.16699C9.47913 1.72283 9.11079 1.35449 8.66663 1.35449C8.22246 1.35449 7.85413 1.72283 7.85413 2.16699V3.85699C8.12496 3.82449 8.37413 3.79199 8.66663 3.79199H9.47913Z"
@@ -133,15 +133,15 @@
             <
             path d = "M18.1458 3.85699V5.41699C18.1458 5.86116 17.7775 6.22949 17.3333 6.22949C16.8892 6.22949 16.5208 5.86116 16.5208 5.41699V3.79199H9.47917V5.41699C9.47917 5.86116 9.11083 6.22949 8.66667 6.22949C8.2225 6.22949 7.85417 5.86116 7.85417 5.41699V3.85699C4.65833 4.14949 3.25 6.20783 3.25 9.20866V18.417C3.25 21.667 4.875 23.8337 8.66667 23.8337H17.3333C21.125 23.8337 22.75 21.667 22.75 18.417V9.20866C22.75 6.20783 21.3417 4.14949 18.1458 3.85699ZM13 18.1462H8.66667C8.2225 18.1462 7.85417 17.7778 7.85417 17.3337C7.85417 16.8895 8.2225 16.5212 8.66667 16.5212H13C13.4442 16.5212 13.8125 16.8895 13.8125 17.3337C13.8125 17.7778 13.4442 18.1462 13 18.1462ZM17.3333 12.7295H8.66667C8.2225 12.7295 7.85417 12.3612 7.85417 11.917C7.85417 11.4728 8.2225 11.1045 8.66667 11.1045H17.3333C17.7775 11.1045 18.1458 11.4728 18.1458 11.917C18.1458 12.3612 17.7775 12.7295 17.3333 12.7295Z"
             fill = "white" /
             >
             <
             /svg>
         ),
-        3: ( <
+        dashboard: ( <
             svg xmlns = "http://www.w3.org/2000/svg"
             width = "26"
             height = "26"
             viewBox = "0 0 26 26"
             fill = "none" >
             <
             path d = "M22.2084 11.0395H19.0775C16.51 11.0395 14.4192 8.94866 14.4192 6.38116V3.25033C14.4192 2.65449 13.9317 2.16699 13.3359 2.16699H8.74254C5.40587 2.16699 2.70837 4.33366 2.70837 8.20116V17.7995C2.70837 21.667 5.40587 23.8337 8.74254 23.8337H17.2575C20.5942 23.8337 23.2917 21.667 23.2917 17.7995V12.1228C23.2917 11.527 22.8042 11.0395 22.2084 11.0395Z"
@@ -150,128 +150,136 @@
             <
             path d = "M17.1167 2.39371C16.6725 1.94954 15.9033 2.25288 15.9033 2.87038V6.65121C15.9033 8.23288 17.2467 9.54371 18.8825 9.54371C19.9117 9.55455 21.3417 9.55454 22.5658 9.55454C23.1833 9.55454 23.5083 8.82871 23.075 8.39538C21.515 6.82454 18.72 3.99704 17.1167 2.39371Z"
             fill = "white" /
             >
             <
             /svg>
         ),
-        4: ( <
-            svg xmlns = "http://www.w3.org/2000/svg"
-            width = "26"
-            height = "26"
-            viewBox = "0 0 26 26"
-            fill = "none" >
-            <
-            path d = "M14.2891 6.5H7.35579C7.07413 6.5 6.80329 6.51083 6.54329 6.54333C3.62913 6.7925 2.16663 8.515 2.16663 11.6892V16.0225C2.16663 20.3558 3.89996 21.2117 7.35579 21.2117H7.78913C8.02746 21.2117 8.34163 21.3742 8.48246 21.5583L9.78246 23.2917C10.3566 24.0608 11.2883 24.0608 11.8625 23.2917L13.1625 21.5583C13.325 21.3417 13.585 21.2117 13.8558 21.2117H14.2891C17.4633 21.2117 19.1858 19.76 19.435 16.835C19.4675 16.575 19.4783 16.3042 19.4783 16.0225V11.6892C19.4783 8.23333 17.745 6.5 14.2891 6.5ZM7.04163 15.1667C6.43496 15.1667 5.95829 14.6792 5.95829 14.0833C5.95829 13.4875 6.44579 13 7.04163 13C7.63746 13 8.12496 13.4875 8.12496 14.0833C8.12496 14.6792 7.63746 15.1667 7.04163 15.1667ZM10.8225 15.1667C10.2158 15.1667 9.73913 14.6792 9.73913 14.0833C9.73913 13.4875 10.2266 13 10.8225 13C11.4183 13 11.9058 13.4875 11.9058 14.0833C11.9058 14.6792 11.4291 15.1667 10.8225 15.1667ZM14.6141 15.1667C14.0075 15.1667 13.5308 14.6792 13.5308 14.0833C13.5308 13.4875 14.0183 13 14.6141 13C15.21 13 15.6975 13.4875 15.6975 14.0833C15.6975 14.6792 15.21 15.1667 14.6141 15.1667Z"
-            fill = "white" /
-            >
-            <
-            path d = "M23.8116 7.35616V11.6895C23.8116 13.8562 23.14 15.3295 21.7966 16.142C21.4716 16.337 21.0925 16.077 21.0925 15.6978L21.1033 11.6895C21.1033 7.35616 18.6225 4.87533 14.2891 4.87533L7.69165 4.88616C7.31248 4.88616 7.05248 4.50699 7.24748 4.18199C8.05998 2.83866 9.53331 2.16699 11.6891 2.16699H18.6225C22.0783 2.16699 23.8116 3.90033 23.8116 7.35616Z"
-            fill = "white" /
-            >
-            <
-            /svg>
-        ),
-        5: ( <
-            svg xmlns = "http://www.w3.org/2000/svg"
-            width = "26"
-            height = "26"
-            viewBox = "0 0 31 27"
-            fill = "none" >
-            <
-            path fill - rule = "evenodd"
-            clip - rule = "evenodd"
-            d = "M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
-            fill = "white" /
-            >
-            <
-            /svg>
-        ),
-        6: ( <
-            svg xmlns = "http://www.w3.org/2000/svg"
-            width = "26"
-            height = "26"
-            viewBox = "0 0 26 26"
-            fill = "none" >
-            <
-            path d = "M22.4359 8.79666V18.9908C22.4359 21.6558 20.2584 23.8333 17.5934 23.8333H8.40671C5.74171 23.8333 3.56421 21.6558 3.56421 18.9908V8.79666C3.56421 6.94416 4.60421 5.32999 6.13171 4.51749C6.66254 4.23583 7.32338 4.61499 7.32338 5.22166C7.32338 6.94416 8.73171 8.35249 10.4542 8.35249H15.5459C17.2684 8.35249 18.6767 6.94416 18.6767 5.22166C18.6767 4.61499 19.3267 4.23583 19.8684 4.51749C21.3959 5.32999 22.4359 6.94416 22.4359 8.79666Z"
-            fill = "white" /
-            >
-            <
-            path d = "M15.5459 2.16667H10.4542C9.32757 2.16667 8.40674 3.07667 8.40674 4.20334V5.22167C8.40674 6.34834 9.31674 7.25834 10.4434 7.25834H15.5459C16.6726 7.25834 17.5826 6.34834 17.5826 5.22167V4.20334C17.5934 3.07667 16.6726 2.16667 15.5459 2.16667Z"
-            fill = "white" /
-            >
-            <
-            /svg>
-        ),
-        7: ( <
-            svg xmlns = "http://www.w3.org/2000/svg"
-            width = "26"
-            height = "26"
-            viewBox = "0 0 26 26"
-            fill = "none" >
-            <
-            path d = "M17.5391 2.16667H8.46079C4.51746 2.16667 2.16663 4.5175 2.16663 8.46084V17.5283C2.16663 21.4825 4.51746 23.8333 8.46079 23.8333H17.5283C21.4716 23.8333 23.8225 21.4825 23.8225 17.5392V8.46084C23.8333 4.5175 21.4825 2.16667 17.5391 2.16667ZM7.04163 13.6175H10.0425C10.4866 13.6175 10.855 13.9858 10.855 14.43C10.855 14.8742 10.4866 15.2425 10.0425 15.2425H7.04163C6.59746 15.2425 6.22913 14.8742 6.22913 14.43C6.22913 13.9858 6.59746 13.6175 7.04163 13.6175ZM14.0508 19.3158H7.04163C6.59746 19.3158 6.22913 18.9475 6.22913 18.5033C6.22913 18.0592 6.59746 17.6908 7.04163 17.6908H14.0508C14.495 17.6908 14.8633 18.0592 14.8633 18.5033C14.8633 18.9475 14.5058 19.3158 14.0508 19.3158ZM18.9583 19.3158H16.9541C16.51 19.3158 16.1416 18.9475 16.1416 18.5033C16.1416 18.0592 16.51 17.6908 16.9541 17.6908H18.9583C19.4025 17.6908 19.7708 18.0592 19.7708 18.5033C19.7708 18.9475 19.4025 19.3158 18.9583 19.3158ZM18.9583 15.2425H12.9675C12.5233 15.2425 12.155 14.8742 12.155 14.43C12.155 13.9858 12.5233 13.6175 12.9675 13.6175H18.9583C19.4025 13.6175 19.7708 13.9858 19.7708 14.43C19.7708 14.8742 19.4025 15.2425 18.9583 15.2425Z"
-            fill = "white" /
-            >
-            <
-            /svg>
-        ),
-        8: ( <
-            svg xmlns = "http://www.w3.org/2000/svg"
-            width = "26"
-            height = "26"
-            viewBox = "0 0 26 26"
-            fill = "none" >
-            <
-            path d = "M17.5391 2.16667H8.46079C4.51746 2.16667 2.16663 4.5175 2.16663 8.46084V17.5283C2.16663 21.4825 4.51746 23.8333 8.46079 23.8333H17.5283C21.4716 23.8333 23.8225 21.4825 23.8225 17.5392V8.46084C23.8333 4.5175 21.4825 2.16667 17.5391 2.16667ZM20.0416 17.7667C20.0416 19.3917 19.3916 20.0417 17.7666 20.0417H13.65C12.025 20.0417 11.375 19.3917 11.375 17.7667V15.8167C11.375 14.1917 12.025 13.5417 13.65 13.5417H17.7666C19.3916 13.5417 20.0416 14.1917 20.0416 15.8167V17.7667Z"
-            fill = "white" /
-            >
-            <
-            /svg>
-        ),
-        9: ( <
-            svg xmlns = "http://www.w3.org/2000/svg"
-            width = "26"
-            height = "26"
-            viewBox = "0 0 31 27"
-            fill = "none" >
-            <
-            path fill - rule = "evenodd"
-            clip - rule = "evenodd"
-            d = "M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
-            fill = "white" /
-            >
-            <
-            /svg>
-        ),
-        10: ( <
-            svg xmlns = "http://www.w3.org/2000/svg"
-            width = "26"
-            height = "26"
-            viewBox = "0 0 31 27"
-            fill = "none" >
-            <
-            path fill - rule = "evenodd"
-            clip - rule = "evenodd"
-            d = "M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
-            fill = "white" /
-            >
-            <
-            /svg>
-        ),
+        // 4: (
+        //   <svg
+        //     xmlns="http://www.w3.org/2000/svg"
+        //     width="26"
+        //     height="26"
+        //     viewBox="0 0 26 26"
+        //     fill="none"
+        //   >
+        //     <path
+        //       d="M14.2891 6.5H7.35579C7.07413 6.5 6.80329 6.51083 6.54329 6.54333C3.62913 6.7925 2.16663 8.515 2.16663 11.6892V16.0225C2.16663 20.3558 3.89996 21.2117 7.35579 21.2117H7.78913C8.02746 21.2117 8.34163 21.3742 8.48246 21.5583L9.78246 23.2917C10.3566 24.0608 11.2883 24.0608 11.8625 23.2917L13.1625 21.5583C13.325 21.3417 13.585 21.2117 13.8558 21.2117H14.2891C17.4633 21.2117 19.1858 19.76 19.435 16.835C19.4675 16.575 19.4783 16.3042 19.4783 16.0225V11.6892C19.4783 8.23333 17.745 6.5 14.2891 6.5ZM7.04163 15.1667C6.43496 15.1667 5.95829 14.6792 5.95829 14.0833C5.95829 13.4875 6.44579 13 7.04163 13C7.63746 13 8.12496 13.4875 8.12496 14.0833C8.12496 14.6792 7.63746 15.1667 7.04163 15.1667ZM10.8225 15.1667C10.2158 15.1667 9.73913 14.6792 9.73913 14.0833C9.73913 13.4875 10.2266 13 10.8225 13C11.4183 13 11.9058 13.4875 11.9058 14.0833C11.9058 14.6792 11.4291 15.1667 10.8225 15.1667ZM14.6141 15.1667C14.0075 15.1667 13.5308 14.6792 13.5308 14.0833C13.5308 13.4875 14.0183 13 14.6141 13C15.21 13 15.6975 13.4875 15.6975 14.0833C15.6975 14.6792 15.21 15.1667 14.6141 15.1667Z"
+        //       fill="white"
+        //     />
+        //     <path
+        //       d="M23.8116 7.35616V11.6895C23.8116 13.8562 23.14 15.3295 21.7966 16.142C21.4716 16.337 21.0925 16.077 21.0925 15.6978L21.1033 11.6895C21.1033 7.35616 18.6225 4.87533 14.2891 4.87533L7.69165 4.88616C7.31248 4.88616 7.05248 4.50699 7.24748 4.18199C8.05998 2.83866 9.53331 2.16699 11.6891 2.16699H18.6225C22.0783 2.16699 23.8116 3.90033 23.8116 7.35616Z"
+        //       fill="white"
+        //     />
+        //   </svg>
+        // ),
+        // 5: (
+        //   <svg
+        //     xmlns="http://www.w3.org/2000/svg"
+        //     width="26"
+        //     height="26"
+        //     viewBox="0 0 31 27"
+        //     fill="none"
+        //   >
+        //     <path
+        //       fill-rule="evenodd"
+        //       clip-rule="evenodd"
+        //       d="M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
+        //       fill="white"
+        //     />
+        //   </svg>
+        // ),
+        // 6: (
+        //   <svg
+        //     xmlns="http://www.w3.org/2000/svg"
+        //     width="26"
+        //     height="26"
+        //     viewBox="0 0 26 26"
+        //     fill="none"
+        //   >
+        //     <path
+        //       d="M22.4359 8.79666V18.9908C22.4359 21.6558 20.2584 23.8333 17.5934 23.8333H8.40671C5.74171 23.8333 3.56421 21.6558 3.56421 18.9908V8.79666C3.56421 6.94416 4.60421 5.32999 6.13171 4.51749C6.66254 4.23583 7.32338 4.61499 7.32338 5.22166C7.32338 6.94416 8.73171 8.35249 10.4542 8.35249H15.5459C17.2684 8.35249 18.6767 6.94416 18.6767 5.22166C18.6767 4.61499 19.3267 4.23583 19.8684 4.51749C21.3959 5.32999 22.4359 6.94416 22.4359 8.79666Z"
+        //       fill="white"
+        //     />
+        //     <path
+        //       d="M15.5459 2.16667H10.4542C9.32757 2.16667 8.40674 3.07667 8.40674 4.20334V5.22167C8.40674 6.34834 9.31674 7.25834 10.4434 7.25834H15.5459C16.6726 7.25834 17.5826 6.34834 17.5826 5.22167V4.20334C17.5934 3.07667 16.6726 2.16667 15.5459 2.16667Z"
+        //       fill="white"
+        //     />
+        //   </svg>
+        // ),
+        // 7: (
+        //   <svg
+        //     xmlns="http://www.w3.org/2000/svg"
+        //     width="26"
+        //     height="26"
+        //     viewBox="0 0 26 26"
+        //     fill="none"
+        //   >
+        //     <path
+        //       d="M17.5391 2.16667H8.46079C4.51746 2.16667 2.16663 4.5175 2.16663 8.46084V17.5283C2.16663 21.4825 4.51746 23.8333 8.46079 23.8333H17.5283C21.4716 23.8333 23.8225 21.4825 23.8225 17.5392V8.46084C23.8333 4.5175 21.4825 2.16667 17.5391 2.16667ZM7.04163 13.6175H10.0425C10.4866 13.6175 10.855 13.9858 10.855 14.43C10.855 14.8742 10.4866 15.2425 10.0425 15.2425H7.04163C6.59746 15.2425 6.22913 14.8742 6.22913 14.43C6.22913 13.9858 6.59746 13.6175 7.04163 13.6175ZM14.0508 19.3158H7.04163C6.59746 19.3158 6.22913 18.9475 6.22913 18.5033C6.22913 18.0592 6.59746 17.6908 7.04163 17.6908H14.0508C14.495 17.6908 14.8633 18.0592 14.8633 18.5033C14.8633 18.9475 14.5058 19.3158 14.0508 19.3158ZM18.9583 19.3158H16.9541C16.51 19.3158 16.1416 18.9475 16.1416 18.5033C16.1416 18.0592 16.51 17.6908 16.9541 17.6908H18.9583C19.4025 17.6908 19.7708 18.0592 19.7708 18.5033C19.7708 18.9475 19.4025 19.3158 18.9583 19.3158ZM18.9583 15.2425H12.9675C12.5233 15.2425 12.155 14.8742 12.155 14.43C12.155 13.9858 12.5233 13.6175 12.9675 13.6175H18.9583C19.4025 13.6175 19.7708 13.9858 19.7708 14.43C19.7708 14.8742 19.4025 15.2425 18.9583 15.2425Z"
+        //       fill="white"
+        //     />
+        //   </svg>
+        // ),
+        // 8: (
+        //   <svg
+        //     xmlns="http://www.w3.org/2000/svg"
+        //     width="26"
+        //     height="26"
+        //     viewBox="0 0 26 26"
+        //     fill="none"
+        //   >
+        //     <path
+        //       d="M17.5391 2.16667H8.46079C4.51746 2.16667 2.16663 4.5175 2.16663 8.46084V17.5283C2.16663 21.4825 4.51746 23.8333 8.46079 23.8333H17.5283C21.4716 23.8333 23.8225 21.4825 23.8225 17.5392V8.46084C23.8333 4.5175 21.4825 2.16667 17.5391 2.16667ZM20.0416 17.7667C20.0416 19.3917 19.3916 20.0417 17.7666 20.0417H13.65C12.025 20.0417 11.375 19.3917 11.375 17.7667V15.8167C11.375 14.1917 12.025 13.5417 13.65 13.5417H17.7666C19.3916 13.5417 20.0416 14.1917 20.0416 15.8167V17.7667Z"
+        //       fill="white"
+        //     />
+        //   </svg>
+        // ),
+        // 9: (
+        //   <svg
+        //     xmlns="http://www.w3.org/2000/svg"
+        //     width="26"
+        //     height="26"
+        //     viewBox="0 0 31 27"
+        //     fill="none"
+        //   >
+        //     <path
+        //       fill-rule="evenodd"
+        //       clip-rule="evenodd"
+        //       d="M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
+        //       fill="white"
+        //     />
+        //   </svg>
+        // ),
+        // 10: (
+        //   <svg
+        //     xmlns="http://www.w3.org/2000/svg"
+        //     width="26"
+        //     height="26"
+        //     viewBox="0 0 31 27"
+        //     fill="none"
+        //   >
+        //     <path
+        //       fill-rule="evenodd"
+        //       clip-rule="evenodd"
+        //       d="M6.83325 3C6.83325 2.20435 7.14932 1.44129 7.71193 0.87868C8.27454 0.31607 9.0376 0 9.83325 0H21.8333C22.6289 0 23.392 0.31607 23.9546 0.87868C24.5172 1.44129 24.8333 2.20435 24.8333 3V4.5H6.83325V3ZM3.83325 9.75C3.83325 8.95435 4.14932 8.19129 4.71193 7.62868C5.27454 7.06607 6.0376 6.75 6.83325 6.75H24.8333C25.6289 6.75 26.392 7.06607 26.9546 7.62868C27.5172 8.19129 27.8333 8.95435 27.8333 9.75V11.25H3.83325V9.75ZM0.833252 16.5C0.833252 15.7044 1.14932 14.9413 1.71193 14.3787C2.27454 13.8161 3.0376 13.5 3.83325 13.5H27.8333C28.6289 13.5 29.392 13.8161 29.9546 14.3787C30.5172 14.9413 30.8333 15.7044 30.8333 16.5V21C30.8333 22.5913 30.2011 24.1174 29.0759 25.2426C27.9507 26.3679 26.4246 27 24.8333 27H6.83325C5.24195 27 3.71583 26.3679 2.59061 25.2426C1.46539 24.1174 0.833252 22.5913 0.833252 21V16.5ZM11.7083 18C11.7083 17.7016 11.8268 17.4155 12.0378 17.2045C12.2487 16.9935 12.5349 16.875 12.8333 16.875H18.8333C19.1316 16.875 19.4178 16.9935 19.6287 17.2045C19.8397 17.4155 19.9583 17.7016 19.9583 18C19.9583 18.2984 19.8397 18.5845 19.6287 18.7955C19.4178 19.0065 19.1316 19.125 18.8333 19.125H12.8333C12.5349 19.125 12.2487 19.0065 12.0378 18.7955C11.8268 18.5845 11.7083 18.2984 11.7083 18Z"
+        //       fill="white"
+        //     />
+        //   </svg>
+        // ),
     };
 
     return ( <
         div className = " bg-darkBg px-5 pt-5 max-w-[68px] min-w-[68px] xl:w-[60px] h-screen flex flex-col justify-between items-center" >
         <
         div className = "flex flex-col justify-center items-center gap-6" > {
             pathname !== "/" ? ( <
                 > {
                     configData?.map((v, i) => {
+                        console.log("v?.feature :>> ", v?.feature);
                         return ( <
                             div title = {
                                 v?.description
                             }
                             className = {
                                 path === `#/${v?.feature}?feature=${i}` ?
                                 "bg-customColor p-2 rounded-full" :
@@ -282,15 +290,15 @@
                             // <div to={`/${v.feature}?feature=${i}`} className="text-white cursor-pointer"
                             onClick = {
                                 () => handleConfig(v, i)
                             } >
                             {
                                 " "
                             } {
-                                icon[i]
+                                icon[v?.feature]
                             } {
                                 /* {v?.feature} */ } <
                             /div> <
                             /div>
                         );
                     })
                 }
```

### Comparing `komodo_sdk-0.0.92/website/src/components/DocumentBox/Table.js` & `komodo_sdk-0.0.93/website/src/components/DocumentBox/Table.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/chat/Chat.js` & `komodo_sdk-0.0.93/website/src/components/chat/Chat.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/chat/Details.js` & `komodo_sdk-0.0.93/website/src/components/chat/Details.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/chat/EnhancedPrompt.js` & `komodo_sdk-0.0.93/website/src/components/chat/EnhancedPrompt.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/chatBot/Chat.js` & `komodo_sdk-0.0.93/website/src/components/chatBot/Chat.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -191,21 +191,21 @@
             setApiActive(true);
         }
         setPrompt("");
         scrollToBottom();
     };
 
     const handleKeyPress = (e) => {
-        if (e.key === "Enter") {
-            sendPrompt();
-        }
-        // if (e.key === "Enter" && !e.shiftKey) {
+        // if (e.key === "Enter") {
         //   sendPrompt();
-        //   e.preventDefault();
         // }
+        if (e.key === "Enter" && !e.shiftKey) {
+            sendPrompt();
+            e.preventDefault();
+        }
     };
 
     const fileInputRef = useRef(null);
 
     const uploadFile = async () => {
         fileInputRef.current.value = null;
         fileInputRef.current.click();
@@ -267,23 +267,25 @@
                         <div className="text-customColor font-normal text-[14px] font-cerebri">
                           Export saved
                         </div>
                       </div>
                     </div>
                   </div> */
         } <
+        div className = "h-[calc(100vh-93px)]" >
+        <
         div className = "h-[calc(100vh-177px)] pt-1 flex items-center flex-col" > {
             /* <div className="h-[calc(100vh-239px)] px-5 pt-1"> */ } <
         div className = {
             `chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-8 ${
-            // location?.state?.openChat === true
-            chatContext?.isDoc === true
-              ? "w-full px-5"
-              : "mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
-          }`
+              // location?.state?.openChat === true
+              chatContext?.isDoc === true
+                ? "w-full px-5"
+                : "mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
+              }`
         }
         // className="chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-10 mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
         ref = {
             chatContainerRef
         } >
         {
             allChatData && allChatData.length > 0 ?
@@ -455,37 +457,42 @@
         div className = "w-[14px] sm:w-[40px]" >
         <
         img src = {
             dots
         }
         alt = "send" / >
         <
-        /div> <
-        input type = "text"
-        className = "w-[892px] xl:w-[700px] border border-[#CFD4D8] rounded-md px-4 pt-[13px] pb-[10px] outline-none text-[14px] font-cerebriregular leading-[17.78px]"
+        /div> {
+            /* <input
+                      type="text"
+                      className="w-[892px] xl:w-[700px] border border-[#CFD4D8] rounded-md px-4 pt-[13px] pb-[10px] outline-none text-[14px] font-cerebriregular leading-[17.78px]"
+                      placeholder="Ask or generate anything..."
+                      value={prompt}
+                      onChange={(e) => setPrompt(e.target.value)}
+                      onKeyDown={handleKeyPress}
+                    /> */
+        } <
+        TextareaAutosize minRows = {
+            1
+        }
+        maxRows = {
+            3
+        }
         placeholder = "Ask or generate anything..."
         value = {
             prompt
         }
         onChange = {
             (e) => setPrompt(e.target.value)
         }
         onKeyDown = {
             handleKeyPress
         }
-        /> {
-            /* <TextareaAutosize
-                      minRows={1}
-                      placeholder="Ask or generate anything..."
-                      value={prompt}
-                      onChange={(e) => setPrompt(e.target.value)}
-                      onKeyDown={handleKeyPress}
-                      className="w-[892px] xl:w-[700px] border rounded-lg bg-senderBG border-borderSky  py-3.5 px-4 outline-none text-[14px] font-cerebriregular leading-[17.78px]"
-                    /> */
-        } {
+        className = "w-[892px] xl:w-[700px] border border-[#CFD4D8] rounded-md px-4 pt-[13px] pb-[10px] outline-none text-[14px] font-cerebriregular leading-[17.78px]" /
+        > {
             /* <span className="cursor-pointer " onClick={sendPrompt}>
                       <img src={send} alt="" />
                     </span> */
         }
 
         {
             /* <div
@@ -494,19 +501,18 @@
                     >
                       <RiSendPlaneFill className="text-[21px] rotate-45" />
                     </div> */
         } <
         div > {
             !send ? ( <
                 div className = {
-                    `${
-                prompt.trim() !== ""
+                    `${prompt.trim() !== ""
                   ? "bg-customBgDark cursor-pointer"
                   : "bg-slate-400"
-              }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4`
+                  }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4`
                 }
                 // className="cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4"
                 onClick = {
                     sendPrompt
                 } >
                 <
                 RiSendPlaneFill className = "text-[21px] rotate-45" / >
@@ -521,10 +527,11 @@
                 FaRegCircleStop className = "text-[21px]" / >
                 <
                 /div>
             )
         } <
         /div> <
         /div> <
+        /div> <
         />
     );
 };
```

### Comparing `komodo_sdk-0.0.92/website/src/components/chatBot/ChatBotById.js` & `komodo_sdk-0.0.93/website/src/components/chatBot/ChatBotById.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -44,14 +44,15 @@
 import {
     Box,
     Modal
 } from "@mui/material";
 import {
     IoClose
 } from "react-icons/io5";
+import TextareaAutosize from "react-textarea-autosize";
 
 const style = {
     position: "absolute",
     top: "50%",
     left: "50%",
     transform: "translate(-50%, -50%)",
     width: "80%",
@@ -187,27 +188,24 @@
         <
         Panel defaultSize = {
             50
         }
         id = "sources-explorer-panel"
         // className="min-w-[30%]"
         className = {
-            `xl:border-l xl:border-[#E8E9EA] ${chatContext?.isDoc === true
-              ? // location?.state?.openChat === true
-              "min-w-[30%] xl:w-full"
-              : "min-w-full"
-              }`
+            `xl:border-l xl:border-[#E8E9EA] ${
+              chatContext?.isDoc === true
+                ? // location?.state?.openChat === true
+                  "min-w-[30%] xl:w-full"
+                : "min-w-full"
+            }`
         } >
         <
         div className = {
-            `${chatContext?.isDoc === true
-              ?
-              "block"
-              : "hidden"
-              }`
+            `${chatContext?.isDoc === true ? "block" : "hidden"}`
         } >
         <
         div className = "hidden lg:block absolute top-6 right-7 z-10 text-[40px] cursor-pointer bg-customColor p-2 rounded-full"
         onClick = {
             handleOpen
         } >
         {
@@ -240,19 +238,20 @@
         >
         <
         div className = "h-[calc(100vh-177px)] pt-1 flex items-center flex-col" >
         <
         div
         // className={`chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-8 mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4`}
         className = {
-            `chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-8 ${chatContext?.isDoc === true
-                      ? // location?.state?.openChat === true
-                      "w-full px-5"
-                      : "mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
-                      }`
+            `chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-8 ${
+                      chatContext?.isDoc === true
+                        ? // location?.state?.openChat === true
+                          "w-full px-5"
+                        : "mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
+                    }`
         }
         // className={`chatscreen h-[calc(100vh-140px)] overflow-auto scrollbar mt-8 ${location?.state?.openChat === true
         //     ? "w-full px-5"
         //     : "mx-8 w-[1017px] xl:w-[800px] lg:w-full md:mx-4 lg:px-4"
         //     }`}
         ref = {
             chatContainerRef
@@ -378,37 +377,52 @@
         div className = "w-[14px] sm:w-[40px]" >
         <
         img src = {
             dots
         }
         alt = "send" / >
         <
-        /div> <
-        input type = "text"
-        className = "w-[892px] xl:w-[700px] border border-[#CFD4D8] rounded-md px-4 pt-[13px] pb-[10px] outline-none text-[14px] font-cerebriregular leading-[17.78px]"
+        /div> {
+            /* <input
+                                type="text"
+                                className="w-[892px] xl:w-[700px] border border-[#CFD4D8] rounded-md px-4 pt-[13px] pb-[10px] outline-none text-[14px] font-cerebriregular leading-[17.78px]"
+                                placeholder="Ask or generate anything..."
+                                value={prompt}
+                                onChange={(e) => setPrompt(e.target.value)}
+                                onKeyDown={handleKeyPress}
+                              /> */
+        } <
+        TextareaAutosize minRows = {
+            1
+        }
+        maxRows = {
+            3
+        }
         placeholder = "Ask or generate anything..."
         value = {
             prompt
         }
         onChange = {
             (e) => setPrompt(e.target.value)
         }
         onKeyDown = {
             handleKeyPress
         }
-        />
+        className = "w-[892px] xl:w-[700px] border border-[#CFD4D8] rounded-md px-4 pt-[13px] pb-[10px] outline-none text-[14px] font-cerebriregular leading-[17.78px]" /
+        >
 
         <
         div > {
             !send ? ( <
                 div className = {
-                    `${prompt.trim() !== ""
-                          ? "bg-customBgDark cursor-pointer"
-                          : "bg-slate-400"
-                          }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4`
+                    `${
+                          prompt.trim() !== ""
+                            ? "bg-customBgDark cursor-pointer"
+                            : "bg-slate-400"
+                        }   text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4`
                 }
                 // className="cursor-pointer bg-customBgDark text-white flex items-center justify-center rounded-lg h-[43px] pl-2.5 pr-4"
                 onClick = {
                     sendPrompt
                 } >
                 <
                 RiSendPlaneFill className = "text-[21px] rotate-45" / >
@@ -454,19 +468,20 @@
         PanelResizeHandle / >
         <
         Panel defaultSize = {
             50
         }
         id = "console-panel"
         className = {
-            `border-l border-[#E8E9EA] ${chatContext?.isDoc === true
-              ? // location?.state?.openChat === true
-              "w-[50%] block xl:w-full"
-              : "hidden"
-              }`
+            `border-l border-[#E8E9EA] ${
+              chatContext?.isDoc === true
+                ? // location?.state?.openChat === true
+                  "w-[50%] block xl:w-full"
+                : "hidden"
+            }`
         } >
         <
         DocumentView foo = "bar" / >
         <
         /Panel> <
         /PanelGroup>
 
@@ -478,21 +493,20 @@
             handleClose
         }
         aria - labelledby = "modal-modal-title"
         aria - describedby = "modal-modal-description" >
         <
         Box sx = {
             style
-        } >
-        <
+        } > {
+            console.log("dsad")
+        } <
         div className = "flex justify-between items-center font-cerebri text-[18px] text-[#3C3C3C] mb-2 p-5" >
         <
-        div >
-        File Preview <
-        /div> <
+        div > File Preview < /div> <
         div onClick = {
             handleClose
         }
         className = "text-[25px]" >
         <
         IoClose / >
         <
```

### Comparing `komodo_sdk-0.0.92/website/src/components/chatBot/ChatBotSideBar.js` & `komodo_sdk-0.0.93/website/src/components/chatBot/ChatBotSideBar.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -532,15 +532,17 @@
     const renderChatItem = (val, i) => ( <
         div key = {
             val?.guid
         }
         // onClick={() => handleDetails(val)}
         onClick = {
             () => {
-                navigate(`/chatdoc/${contextFiles?.oldChatId}/${val?.guid}`);
+                navigate(
+                    `/chatdoc/${contextFiles?.oldChatId}/${val?.guid}${location?.search}`
+                );
                 localStorage?.removeItem("react-resizable-panels:example");
                 setIsCollections(false);
             }
         }
         className = {
             `px-5 border-b-[0.5px] border-[#F6F6F9] py-5 text-[#5A636C] text-[14px] leading-[17.78px] flex justify-between items-center font-cerebriregular cursor-pointer ${
         id === val?.guid ? "bg-[#F6F6F9]" : ""
@@ -893,15 +895,15 @@
                             onClick = {
                                 () => {
                                     handleSelectItem(item?.name);
                                     setCollectName(item?.name);
                                     localStorage?.setItem("collectName", item?.name);
                                     contextFiles?.getUserFiles(item?.guid);
                                     contextFiles?.setOldChatId(item?.guid);
-                                    navigate(`/chatdoc/${item?.guid}`, {
+                                    navigate(`/chatdoc/${item?.guid}${location?.search}`, {
                                         state: {
                                             collectionName: item?.name,
                                             // openChat: true,
                                             chatId: item?.guid,
                                         },
                                     });
                                 }
@@ -1016,15 +1018,15 @@
                 div className = "py-3 flex flex-col gap-4 border-b border-customGray" >
                 <
                 div className = "text-blackText px-5 flex items-center text-[18px] gap-2 -ml-2 font-cerebriMedium cursor-pointer "
                 onClick = {
                     () => {
                         setIsCollections(true);
                         setSelectedFileName("");
-                        navigate(`/chatdoc`);
+                        navigate(`/chatdoc${location?.search}`);
                         listData?.setOldChatId("");
                         contextFiles?.setIsdoc(false);
                         contextFiles?.setResFileId("");
                     }
                 } >
                 <
                 img src = {
@@ -1232,15 +1234,17 @@
                         } <
                         div className = "text-center my-1.5 px-3" >
                         <
                         button onClick = {
                             () => {
                                 // listData?.setChatHistory(false);
                                 listData?.setChatGuid("");
-                                navigate(`/chatdoc/${contextFiles?.oldChatId}`);
+                                navigate(
+                                    `/chatdoc/${contextFiles?.oldChatId}${location?.search}`
+                                );
                                 setIsDrawerOpen(false);
                             }
                         }
                         className = "bg-customBgDark text-[#fff] rounded-md w-full px-24 pb-2 pt-3 text-[15px] font-cerebriregular xxl:px-10" >
                         New Chat <
                         /button> <
                         /div> {
```

### Comparing `komodo_sdk-0.0.92/website/src/components/chatBot/EnhancedBot.js` & `komodo_sdk-0.0.93/website/src/components/chatBot/EnhancedBot.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/components/document/DocumentSidebar.js` & `komodo_sdk-0.0.93/website/src/components/document/DocumentSidebar.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/contexts/roleContext.js` & `komodo_sdk-0.0.93/website/src/contexts/roleContext.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -22,29 +22,30 @@
 
 export function RoleStore(props) {
     const [reactSelect, setReactSelect] = useState();
     const [configSelect, setConfigSelect] = useState();
     const [user, setUser] = useState("");
     const [agentList, setAgentList] = useState();
     const [configure, setConfigure] = useState();
+    console.log("configure :>> ", configure);
     const [list, setList] = useState([]);
-    console.log("list :>> ", list);
     const [chatHistory, setChatHistory] = useState(false);
     const [chatGuid, setChatGuid] = useState("");
     const [chatRes, setChatRes] = useState("");
     const [company, setCompany] = useState("");
     const [agentType, setAgentType] = useState("");
     const [filesData, setFilesData] = useState({});
     const [pdfData, setPdfData] = useState("");
     const [pdfURL, setPdfURL] = useState("");
     const [oldChatId, setOldChatId] = useState("");
     const [isCollections, setIsCollections] = useState(true);
     const [activeTab, setActiveTab] = useState(1);
     const [isDoc, setIsdoc] = useState(false);
     const [resFileId, setResFileId] = useState("");
+    const [fileType, setFileType] = useState("")
 
     // console.log("pdfData :>> ", pdfData);
     // const [firstPdfData, setFirstPdfData] = useState("");
 
     useEffect(() => {
         if (user === "") {
             set_user_login_data();
@@ -135,14 +136,15 @@
             console.log("user details get ::error", error);
             setList([]);
             ErrorToast(error?.data?.detail || "Something went wrong");
         }
     };
 
     const getUserFiles = async (shortcode) => {
+        setFilesData()
         try {
             const files = await ApiGet(
                 API_Path.collectionsGetCollectionUrl(shortcode)
             );
             // const dataA = await files?.data?.files?.map((v) => {
             //   return v?.name?.replace(/[_-]/g, " ");
             // });
@@ -150,15 +152,14 @@
             // setFilesData(files?.data);
             const dataA = await files?.data?.files?.map((v) => {
                 return {
                     ...v,
                     name: v?.name?.replace(/[_-]/g, " ")
                 };
             });
-            console.log("dataA :>> ", dataA);
             setFilesData({
                 ...files?.data,
                 files: dataA
             });
             // setFirstPdfData(files?.data?.files[0]);
         } catch (error) {
             console.log("error", error);
@@ -177,14 +178,15 @@
 
     useEffect(() => {
         companyData();
     }, []);
 
     const handleFileData = async (id, guid, type) => {
         console.log("typeasds", type);
+        setFileType(type)
         setPdfURL("");
         try {
             // if (type === "application/pdf") {
             //   const file = await ApiGet(
             //     API_Path.collectionsDownloadFileUrl(id, guid)
             //   );
             //   // console.log("file?.data :>> ", file?.data);
@@ -201,25 +203,42 @@
             // const file = await ApiGet(API_Path.collectionsDownloadFileUrl(id, guid));
             // console.log('file', file);
             // setPdfURL(window.location.origin + API_Path.collectionsDownloadFileUrl(id, guid))
             // setPdfData(file?.data);
 
             // with blob URL
             const authUser = JSON.parse(localStorage.getItem("komodoUser"));
+            console.log("qweqwe", type === "application/vnd.openxmlformats-officedocument.wordprocessingml.document")
+            let config = {
+                headers: {
+                    "Content-Type": "application/json",
+                    "X-User-Email": authUser?.email,
+                    "X-User-Email": authUser?.email,
+                },
+            }
+            if (
+                type !== "text/plain" &&
+                type !== "application/vnd.openxmlformats-officedocument.wordprocessingml.document" &&
+                type !== "application/vnd.openxmlformats-officedocument.presentationml.presentation") {
+                config.responseType = "blob"
+            }
             const response = await axios.get(
-                API_Path.collectionsDownloadFileUrl(id, guid), {
-                    headers: {
-                        "Content-Type": "application/json",
-                        "X-User-Email": authUser?.email,
-                        "X-User-Email": authUser?.email,
-                    },
-                    responseType: "blob", // Important
-                }
+                API_Path.collectionsDownloadFileUrl(id, guid,
+                    type === "application/vnd.openxmlformats-officedocument.wordprocessingml.document" ||
+                    type === "application/vnd.openxmlformats-officedocument.presentationml.presentation"),
+                config
             );
-            console.log("responseasd", response);
+            console.log(response, 'response')
+            if (
+                type === "text/plain" ||
+                type === "application/vnd.openxmlformats-officedocument.wordprocessingml.document" ||
+                type === "application/vnd.openxmlformats-officedocument.presentationml.presentation") {
+                return setPdfURL(response.data)
+            }
+            console.log("responseasd", response.data);
             if (type.includes("sheet")) {
                 return ExcelRenderer(response?.data, (err, resp) => {
                     if (err) {
                         console.log(err);
                     } else {
                         setPdfURL({
                             cols: resp.cols,
@@ -262,14 +281,15 @@
                 configure,
                 configSelect,
                 isCollections,
                 activeTab,
                 oldChatId,
                 isDoc,
                 resFileId,
+                fileType,
                 ...{
                     setReactSelect,
                     setUser,
                     setList,
                     setChatHistory,
                     conversations,
                     setChatGuid,
```

### Comparing `komodo_sdk-0.0.92/website/src/images/Ellipsis.gif` & `komodo_sdk-0.0.93/website/src/images/Ellipsis.gif`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/chat.png` & `komodo_sdk-0.0.93/website/src/images/chat.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/chatgpt.png` & `komodo_sdk-0.0.93/website/src/images/chatgpt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/chatimg.png` & `komodo_sdk-0.0.93/website/src/images/chatimg.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/chattick.png` & `komodo_sdk-0.0.93/website/src/images/chattick.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/content.png` & `komodo_sdk-0.0.93/website/src/images/content.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/copy.png` & `komodo_sdk-0.0.93/website/src/images/copy.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/doc.png` & `komodo_sdk-0.0.93/website/src/images/doc.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/docprofile.png` & `komodo_sdk-0.0.93/website/src/images/docprofile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/docwave.png` & `komodo_sdk-0.0.93/website/src/images/docwave.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/first.png` & `komodo_sdk-0.0.93/website/src/images/first.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/imgLogo.jpg` & `komodo_sdk-0.0.93/website/src/images/imgLogo.jpg`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/login.png` & `komodo_sdk-0.0.93/website/src/images/login.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/pdf.png` & `komodo_sdk-0.0.93/website/src/images/pdf.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/person.png` & `komodo_sdk-0.0.93/website/src/images/person.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/portfolio.png` & `komodo_sdk-0.0.93/website/src/images/portfolio.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/pptLogo.png` & `komodo_sdk-0.0.93/website/src/images/pptLogo.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/profile.png` & `komodo_sdk-0.0.93/website/src/images/profile.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/robot.png` & `komodo_sdk-0.0.93/website/src/images/robot.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/sample.pdf` & `komodo_sdk-0.0.93/website/src/images/sample.pdf`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/second.png` & `komodo_sdk-0.0.93/website/src/images/second.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/send.png` & `komodo_sdk-0.0.93/website/src/images/send.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/setting.png` & `komodo_sdk-0.0.93/website/src/images/setting.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/summary.png` & `komodo_sdk-0.0.93/website/src/images/summary.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/tik.png` & `komodo_sdk-0.0.93/website/src/images/tik.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/txt.png` & `komodo_sdk-0.0.93/website/src/images/txt.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/user.png` & `komodo_sdk-0.0.93/website/src/images/user.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/wave.png` & `komodo_sdk-0.0.93/website/src/images/wave.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/wave1.png` & `komodo_sdk-0.0.93/website/src/images/wave1.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/word.png` & `komodo_sdk-0.0.93/website/src/images/word.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/images/xlsxLogo.png` & `komodo_sdk-0.0.93/website/src/images/xlsxLogo.png`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/layout/CollectionLayout.js` & `komodo_sdk-0.0.93/website/src/layout/CollectionLayout.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/layout/PrimaryLayout.js` & `komodo_sdk-0.0.93/website/src/layout/PrimaryLayout.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/Document.js` & `komodo_sdk-0.0.93/website/src/pages/Document.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/chatBot.js` & `komodo_sdk-0.0.93/website/src/pages/chatBot.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/chat/Chat.js` & `komodo_sdk-0.0.93/website/src/pages/chat/Chat.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/chat/Details.js` & `komodo_sdk-0.0.93/website/src/pages/chat/Details.js`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/pricing/Pricing.jsx` & `komodo_sdk-0.0.93/website/src/pages/pricing/Pricing.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/privacy/Privacy.jsx` & `komodo_sdk-0.0.93/website/src/pages/privacy/Privacy.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/privacy/Terms.jsx` & `komodo_sdk-0.0.93/website/src/pages/privacy/Terms.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/profile/Profile.jsx` & `komodo_sdk-0.0.93/website/src/pages/profile/Profile.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/website/src/pages/settings/Settings.jsx` & `komodo_sdk-0.0.93/website/src/pages/settings/Settings.jsx`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/.gitignore` & `komodo_sdk-0.0.93/.gitignore`

 * *Files identical despite different names*

### Comparing `komodo_sdk-0.0.92/pyproject.toml` & `komodo_sdk-0.0.93/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "komodo-sdk"
-version = "0.0.92"
+version = "0.0.93"
 authors = [
     { name = "Ryan Oberoi", email = "ryan.oberoi@komodoapp.ai" },
 ]
 description = "Komodo SDK"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `komodo_sdk-0.0.92/PKG-INFO` & `komodo_sdk-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: komodo-sdk
-Version: 0.0.92
+Version: 0.0.93
 Summary: Komodo SDK
 Project-URL: Homepage, https://github.com/Komodo-AI/komodo-sdk.git
 Author-email: Ryan Oberoi <ryan.oberoi@komodoapp.ai>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: aiofiles~=23.2.1
```

