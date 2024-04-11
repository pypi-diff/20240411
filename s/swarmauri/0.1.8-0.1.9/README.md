# Comparing `tmp/swarmauri-0.1.8.tar.gz` & `tmp/swarmauri-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarmauri-0.1.8.tar", last modified: Wed Mar  6 12:26:28 2024, max compression
+gzip compressed data, was "swarmauri-0.1.9.tar", last modified: Thu Mar  7 03:38:55 2024, max compression
```

## Comparing `swarmauri-0.1.8.tar` & `swarmauri-0.1.9.tar`

### file list

```diff
@@ -1,379 +1,405 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.290000 swarmauri-0.1.8/
--rw-rw-rw-   0        0        0     3496 2024-03-06 12:26:30.000000 swarmauri-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      952 2024-03-03 14:10:52.000000 swarmauri-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-06 12:26:30.000000 swarmauri-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2170 2024-03-04 21:18:48.000000 swarmauri-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.290000 swarmauri-0.1.8/swarmauri/
--rw-rw-rw-   0        0        0       21 2024-03-06 10:50:20.000000 swarmauri-0.1.8/swarmauri/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.300000 swarmauri-0.1.8/swarmauri/community/
--rw-rw-rw-   0        0        0        0 2024-03-01 11:37:30.000000 swarmauri-0.1.8/swarmauri/community/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.300000 swarmauri-0.1.8/swarmauri/community/document_stores/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/community/document_stores/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.300000 swarmauri-0.1.8/swarmauri/community/document_stores/base/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/community/document_stores/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.310000 swarmauri-0.1.8/swarmauri/community/document_stores/concrete/
--rw-rw-rw-   0        0        0     2873 2024-02-27 22:23:48.000000 swarmauri-0.1.8/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/community/document_stores/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.310000 swarmauri-0.1.8/swarmauri/community/retrievers/
--rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.8/swarmauri/community/retrievers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.310000 swarmauri-0.1.8/swarmauri/community/retrievers/base/
--rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.8/swarmauri/community/retrievers/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.320000 swarmauri-0.1.8/swarmauri/community/retrievers/concrete/
--rw-rw-rw-   0        0        0     2087 2024-02-27 19:40:22.000000 swarmauri-0.1.8/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
--rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.8/swarmauri/community/retrievers/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.320000 swarmauri-0.1.8/swarmauri/community/tools/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/community/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.320000 swarmauri-0.1.8/swarmauri/community/tools/base/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/community/tools/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.320000 swarmauri-0.1.8/swarmauri/community/tools/concrete/
--rw-rw-rw-   0        0        0     2477 2024-02-26 12:20:58.000000 swarmauri-0.1.8/swarmauri/community/tools/concrete/DownloadPdfTool.py
--rw-rw-rw-   0        0        0     1159 2024-02-25 00:17:10.000000 swarmauri-0.1.8/swarmauri/community/tools/concrete/EntityRecognitionTool.py
--rw-rw-rw-   0        0        0     4073 2024-02-25 00:17:14.000000 swarmauri-0.1.8/swarmauri/community/tools/concrete/GmailReadTool.py
--rw-rw-rw-   0        0        0     4081 2024-03-03 17:06:56.000000 swarmauri-0.1.8/swarmauri/community/tools/concrete/GmailSendTool.py
--rw-rw-rw-   0        0        0     2491 2024-02-27 06:54:54.000000 swarmauri-0.1.8/swarmauri/community/tools/concrete/PaCMAP.py
--rw-rw-rw-   0        0        0      888 2024-02-25 00:17:56.000000 swarmauri-0.1.8/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
--rw-rw-rw-   0        0        0     2098 2024-02-26 10:14:00.000000 swarmauri-0.1.8/swarmauri/community/tools/concrete/WebScrapingTool.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/community/tools/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.330000 swarmauri-0.1.8/swarmauri/core/
--rw-rw-rw-   0        0        0        0 2024-03-03 23:23:40.000000 swarmauri-0.1.8/swarmauri/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.330000 swarmauri-0.1.8/swarmauri/core/agent_apis/
--rw-rw-rw-   0        0        0     2067 2024-02-29 07:10:06.000000 swarmauri-0.1.8/swarmauri/core/agent_apis/IAgentCommands.py
--rw-rw-rw-   0        0        0     1786 2024-02-29 07:10:32.000000 swarmauri-0.1.8/swarmauri/core/agent_apis/IAgentRouterCRUD.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/agent_apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.330000 swarmauri-0.1.8/swarmauri/core/agents/
--rw-rw-rw-   0        0        0     1869 2024-02-24 21:26:04.000000 swarmauri-0.1.8/swarmauri/core/agents/ISwarmAgent.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.340000 swarmauri-0.1.8/swarmauri/core/chains/
--rw-rw-rw-   0        0        0      511 2024-03-06 07:13:14.000000 swarmauri-0.1.8/swarmauri/core/chains/ICallableChain.py
--rw-rw-rw-   0        0        0       63 2024-03-06 07:46:14.000000 swarmauri-0.1.8/swarmauri/core/chains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.340000 swarmauri-0.1.8/swarmauri/core/chunkers/
--rw-rw-rw-   0        0        0     1134 2024-03-06 09:41:16.000000 swarmauri-0.1.8/swarmauri/core/chunkers/IChunker.py
--rw-rw-rw-   0        0        0       93 2024-02-29 02:35:28.000000 swarmauri-0.1.8/swarmauri/core/chunkers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.340000 swarmauri-0.1.8/swarmauri/core/conversations/
--rw-rw-rw-   0        0        0     1165 2024-02-24 21:26:54.000000 swarmauri-0.1.8/swarmauri/core/conversations/IConversation.py
--rw-rw-rw-   0        0        0      307 2024-02-24 19:48:48.000000 swarmauri-0.1.8/swarmauri/core/conversations/IMaxSize.py
--rw-rw-rw-   0        0        0      871 2024-02-24 21:28:08.000000 swarmauri-0.1.8/swarmauri/core/conversations/ISystemContext.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/conversations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.340000 swarmauri-0.1.8/swarmauri/core/document_stores/
--rw-rw-rw-   0        0        0     2179 2024-02-25 01:07:04.000000 swarmauri-0.1.8/swarmauri/core/document_stores/IDocumentStore.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/document_stores/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.350000 swarmauri-0.1.8/swarmauri/core/documents/
--rw-rw-rw-   0        0        0     1597 2024-02-29 23:27:20.000000 swarmauri-0.1.8/swarmauri/core/documents/IDocument.py
--rw-rw-rw-   0        0        0      486 2024-03-04 22:09:54.000000 swarmauri-0.1.8/swarmauri/core/documents/IEmbed.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/documents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.350000 swarmauri-0.1.8/swarmauri/core/messages/
--rw-rw-rw-   0        0        0      722 2024-02-22 03:01:56.000000 swarmauri-0.1.8/swarmauri/core/messages/IMessage.py
--rw-rw-rw-   0        0        0       30 2024-02-24 21:26:46.000000 swarmauri-0.1.8/swarmauri/core/messages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.350000 swarmauri-0.1.8/swarmauri/core/models/
--rw-rw-rw-   0        0        0      298 2024-02-29 03:14:00.000000 swarmauri-0.1.8/swarmauri/core/models/IFit.py
--rw-rw-rw-   0        0        0      485 2024-02-29 03:15:00.000000 swarmauri-0.1.8/swarmauri/core/models/IModel.py
--rw-rw-rw-   0        0        0      311 2024-02-29 03:13:40.000000 swarmauri-0.1.8/swarmauri/core/models/IPredict.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.360000 swarmauri-0.1.8/swarmauri/core/parsers/
--rw-rw-rw-   0        0        0      778 2024-02-24 21:26:38.000000 swarmauri-0.1.8/swarmauri/core/parsers/IParser.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.360000 swarmauri-0.1.8/swarmauri/core/prompts/
--rw-rw-rw-   0        0        0      556 2024-02-24 19:59:22.000000 swarmauri-0.1.8/swarmauri/core/prompts/IPrompt.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/prompts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.360000 swarmauri-0.1.8/swarmauri/core/retrievers/
--rw-rw-rw-   0        0        0      904 2024-02-24 21:27:04.000000 swarmauri-0.1.8/swarmauri/core/retrievers/IRetriever.py
--rw-rw-rw-   0        0        0        0 2024-03-03 23:23:58.000000 swarmauri-0.1.8/swarmauri/core/retrievers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.360000 swarmauri-0.1.8/swarmauri/core/swarm_apis/
--rw-rw-rw-   0        0        0     2306 2024-02-29 07:15:38.000000 swarmauri-0.1.8/swarmauri/core/swarm_apis/IAgentRegistration.py
--rw-rw-rw-   0        0        0     1140 2024-03-03 14:20:54.000000 swarmauri-0.1.8/swarmauri/core/swarm_apis/ISwarmAPI.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/swarm_apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.370000 swarmauri-0.1.8/swarmauri/core/swarms/
--rw-rw-rw-   0        0        0        0 2024-02-23 03:51:40.000000 swarmauri-0.1.8/swarmauri/core/swarms/ISwarm.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/swarms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.370000 swarmauri-0.1.8/swarmauri/core/toolkits/
--rw-rw-rw-   0        0        0     1635 2024-02-24 21:26:30.000000 swarmauri-0.1.8/swarmauri/core/toolkits/IToolkit.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/toolkits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.370000 swarmauri-0.1.8/swarmauri/core/tools/
--rw-rw-rw-   0        0        0     2042 2024-02-24 20:06:46.000000 swarmauri-0.1.8/swarmauri/core/tools/IParameter.py
--rw-rw-rw-   0        0        0      516 2024-03-03 17:27:50.000000 swarmauri-0.1.8/swarmauri/core/tools/ITool.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.380000 swarmauri-0.1.8/swarmauri/core/tracing/
--rw-rw-rw-   0        0        0     1058 2024-03-06 05:25:36.000000 swarmauri-0.1.8/swarmauri/core/tracing/IChainTracer.py
--rw-rw-rw-   0        0        0      804 2024-03-02 05:02:52.000000 swarmauri-0.1.8/swarmauri/core/tracing/ITraceContext.py
--rw-rw-rw-   0        0        0     1606 2024-03-06 00:14:54.000000 swarmauri-0.1.8/swarmauri/core/tracing/ITracer.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/tracing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.380000 swarmauri-0.1.8/swarmauri/core/utils/
--rw-rw-rw-   0        0        0      637 2024-02-27 19:34:00.000000 swarmauri-0.1.8/swarmauri/core/utils/ITransactional.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/core/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.380000 swarmauri-0.1.8/swarmauri/core/vector_stores/
--rw-rw-rw-   0        0        0      800 2024-02-29 05:59:20.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IAngleBetweenVectors.py
--rw-rw-rw-   0        0        0     1054 2024-02-29 06:51:34.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IDecompose.py
--rw-rw-rw-   0        0        0     1676 2024-03-01 22:46:34.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IDistanceSimilarity.py
--rw-rw-rw-   0        0        0      702 2024-02-29 06:17:22.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IDivergence.py
--rw-rw-rw-   0        0        0      828 2024-02-29 06:15:56.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IGradient.py
--rw-rw-rw-   0        0        0      721 2024-02-29 05:46:12.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IOrthogonalProject.py
--rw-rw-rw-   0        0        0      619 2024-02-29 05:46:38.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IProject.py
--rw-rw-rw-   0        0        0      661 2024-02-29 06:12:02.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IReflect.py
--rw-rw-rw-   0        0        0      939 2024-02-29 04:08:20.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/ISimilarity.py
--rw-rw-rw-   0        0        0      848 2024-02-27 19:35:06.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/ISimiliarityQuery.py
--rw-rw-rw-   0        0        0      888 2024-02-29 05:28:14.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorArithmetic.py
--rw-rw-rw-   0        0        0      588 2024-02-29 06:55:40.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorBasisCheck.py
--rw-rw-rw-   0        0        0      711 2024-02-29 06:44:38.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorLinearCombination.py
--rw-rw-rw-   0        0        0     1362 2024-02-29 04:54:00.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorNorm.py
--rw-rw-rw-   0        0        0     2108 2024-02-29 05:40:54.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorProduct.py
--rw-rw-rw-   0        0        0      757 2024-02-29 06:25:06.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorRotate.py
--rw-rw-rw-   0        0        0      672 2024-02-29 06:40:18.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorSpan.py
--rw-rw-rw-   0        0        0     1924 2024-02-29 22:26:24.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorStore.py
--rw-rw-rw-   0        0        0        0 2024-03-03 23:24:08.000000 swarmauri-0.1.8/swarmauri/core/vector_stores/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.380000 swarmauri-0.1.8/swarmauri/core/vectorizers/
--rw-rw-rw-   0        0        0      624 2024-03-01 10:44:28.000000 swarmauri-0.1.8/swarmauri/core/vectorizers/IVectorize.py
--rw-rw-rw-   0        0        0        1 2024-02-29 23:57:16.000000 swarmauri-0.1.8/swarmauri/core/vectorizers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.390000 swarmauri-0.1.8/swarmauri/core/vectors/
--rw-rw-rw-   0        0        0      578 2024-03-01 23:23:06.000000 swarmauri-0.1.8/swarmauri/core/vectors/IVector.py
--rw-rw-rw-   0        0        0      900 2024-02-29 04:09:42.000000 swarmauri-0.1.8/swarmauri/core/vectors/IVectorMeta.py
--rw-rw-rw-   0        0        0     1312 2024-02-29 22:50:46.000000 swarmauri-0.1.8/swarmauri/core/vectors/IVectorTransform.py
--rw-rw-rw-   0        0        0        0 2024-03-03 23:24:16.000000 swarmauri-0.1.8/swarmauri/core/vectors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.390000 swarmauri-0.1.8/swarmauri/experimental/
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/experimental/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.390000 swarmauri-0.1.8/swarmauri/experimental/conversations/
--rw-rw-rw-   0        0        0     3471 2024-03-04 00:27:10.000000 swarmauri-0.1.8/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
--rw-rw-rw-   0        0        0     2219 2024-02-24 23:03:58.000000 swarmauri-0.1.8/swarmauri/experimental/conversations/SemanticConversation.py
--rw-rw-rw-   0        0        0        0 2024-02-23 04:51:08.000000 swarmauri-0.1.8/swarmauri/experimental/conversations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.400000 swarmauri-0.1.8/swarmauri/experimental/models/
--rw-rw-rw-   0        0        0     3556 2024-03-03 14:27:12.000000 swarmauri-0.1.8/swarmauri/experimental/models/HierarchicalAttentionModel.py
--rw-rw-rw-   0        0        0     1846 2024-02-24 23:05:02.000000 swarmauri-0.1.8/swarmauri/experimental/models/SageMaker.py
--rw-rw-rw-   0        0        0        0 2024-02-23 05:01:34.000000 swarmauri-0.1.8/swarmauri/experimental/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.400000 swarmauri-0.1.8/swarmauri/experimental/parsers/
--rw-rw-rw-   0        0        0     1508 2024-02-29 02:42:10.000000 swarmauri-0.1.8/swarmauri/experimental/parsers/PDFToTextParser.py
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/experimental/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.400000 swarmauri-0.1.8/swarmauri/experimental/tools/
--rw-rw-rw-   0        0        0     1414 2024-02-29 02:47:28.000000 swarmauri-0.1.8/swarmauri/experimental/tools/CypherQueryTool.py
--rw-rw-rw-   0        0        0     1237 2024-02-29 02:49:12.000000 swarmauri-0.1.8/swarmauri/experimental/tools/FileDownloaderTool.py
--rw-rw-rw-   0        0        0     3466 2024-02-24 23:06:28.000000 swarmauri-0.1.8/swarmauri/experimental/tools/LinkedInArticleTool.py
--rw-rw-rw-   0        0        0     2918 2024-02-27 18:57:56.000000 swarmauri-0.1.8/swarmauri/experimental/tools/OutlookSendMailTool.py
--rw-rw-rw-   0        0        0     1357 2024-02-29 02:51:04.000000 swarmauri-0.1.8/swarmauri/experimental/tools/SQLite3QueryTool.py
--rw-rw-rw-   0        0        0     1511 2024-02-24 23:06:52.000000 swarmauri-0.1.8/swarmauri/experimental/tools/TwitterPostTool.py
--rw-rw-rw-   0        0        0       27 2024-02-27 18:55:30.000000 swarmauri-0.1.8/swarmauri/experimental/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.410000 swarmauri-0.1.8/swarmauri/experimental/utils/
--rw-rw-rw-   0        0        0      973 2024-02-27 19:36:04.000000 swarmauri-0.1.8/swarmauri/experimental/utils/ISerializable.py
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/experimental/utils/__init__.py
--rw-rw-rw-   0        0        0      655 2024-02-23 08:24:16.000000 swarmauri-0.1.8/swarmauri/experimental/utils/get_last_frame.py
--rw-rw-rw-   0        0        0     2141 2024-02-23 08:34:46.000000 swarmauri-0.1.8/swarmauri/experimental/utils/save_schema.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.410000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/
--rw-rw-rw-   0        0        0     2854 2024-03-03 14:29:14.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/CanberraDistance.py
--rw-rw-rw-   0        0        0     1875 2024-03-03 14:30:48.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/ChebyshevDistance.py
--rw-rw-rw-   0        0        0     2024 2024-03-03 14:31:04.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/HaversineDistance.py
--rw-rw-rw-   0        0        0     2347 2024-03-03 14:31:12.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/ManhattanDistance.py
--rw-rw-rw-   0        0        0     2866 2024-03-03 14:35:10.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/MinkowskiDistance.py
--rw-rw-rw-   0        0        0     2057 2024-02-29 09:06:24.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/SSASimilarity.py
--rw-rw-rw-   0        0        0     2643 2024-02-29 09:07:00.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/SSIVSimilarity.py
--rw-rw-rw-   0        0        0     7058 2024-03-03 09:40:08.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/ScannVectorStore.py
--rw-rw-rw-   0        0        0     2213 2024-03-03 14:31:54.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/SorensenDiceDistance.py
--rw-rw-rw-   0        0        0     1989 2024-03-03 14:31:30.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/experimental/vector_stores/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.410000 swarmauri-0.1.8/swarmauri/standard/
--rw-rw-rw-   0        0        0        0 2024-03-06 07:33:08.000000 swarmauri-0.1.8/swarmauri/standard/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.420000 swarmauri-0.1.8/swarmauri/standard/agents/
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.420000 swarmauri-0.1.8/swarmauri/standard/agents/base/
--rw-rw-rw-   0        0        0     3398 2024-02-26 09:36:04.000000 swarmauri-0.1.8/swarmauri/standard/agents/base/SwarmAgentBase.py
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/agents/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.430000 swarmauri-0.1.8/swarmauri/standard/agents/concrete/
--rw-rw-rw-   0        0        0     2169 2024-02-26 14:24:34.000000 swarmauri-0.1.8/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
--rw-rw-rw-   0        0        0     2404 2024-02-27 03:25:22.000000 swarmauri-0.1.8/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
--rw-rw-rw-   0        0        0     4086 2024-02-27 03:25:24.000000 swarmauri-0.1.8/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
--rw-rw-rw-   0        0        0     1428 2024-02-24 22:41:54.000000 swarmauri-0.1.8/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
--rw-rw-rw-   0        0        0     1135 2024-02-24 22:42:02.000000 swarmauri-0.1.8/swarmauri/standard/agents/concrete/SingleCommandAgent.py
--rw-rw-rw-   0        0        0     3804 2024-03-03 19:50:24.000000 swarmauri-0.1.8/swarmauri/standard/agents/concrete/ToolAgent.py
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/agents/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.430000 swarmauri-0.1.8/swarmauri/standard/apis/
--rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.8/swarmauri/standard/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.430000 swarmauri-0.1.8/swarmauri/standard/apis/base/
--rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.8/swarmauri/standard/apis/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.430000 swarmauri-0.1.8/swarmauri/standard/apis/concrete/
--rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.8/swarmauri/standard/apis/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.440000 swarmauri-0.1.8/swarmauri/standard/chains/
--rw-rw-rw-   0        0        0        0 2024-03-06 07:46:30.000000 swarmauri-0.1.8/swarmauri/standard/chains/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.440000 swarmauri-0.1.8/swarmauri/standard/chains/base/
--rw-rw-rw-   0        0        0        1 2024-03-06 07:27:50.000000 swarmauri-0.1.8/swarmauri/standard/chains/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.440000 swarmauri-0.1.8/swarmauri/standard/chains/concrete/
--rw-rw-rw-   0        0        0     1262 2024-03-06 10:26:28.000000 swarmauri-0.1.8/swarmauri/standard/chains/concrete/CallableChain.py
--rw-rw-rw-   0        0        0     4481 2024-03-06 12:26:20.000000 swarmauri-0.1.8/swarmauri/standard/chains/concrete/TypeAgnosticCallableChain.py
--rw-rw-rw-   0        0        0        0 2024-03-06 07:46:36.000000 swarmauri-0.1.8/swarmauri/standard/chains/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.440000 swarmauri-0.1.8/swarmauri/standard/chunkers/
--rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.8/swarmauri/standard/chunkers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.460000 swarmauri-0.1.8/swarmauri/standard/chunkers/base/
--rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.8/swarmauri/standard/chunkers/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.470000 swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/
--rw-rw-rw-   0        0        0     1935 2024-03-03 14:28:00.000000 swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
--rw-rw-rw-   0        0        0     1477 2024-03-03 14:27:50.000000 swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
--rw-rw-rw-   0        0        0     2164 2024-03-06 09:27:14.000000 swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
--rw-rw-rw-   0        0        0     1198 2024-03-05 00:05:40.000000 swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
--rw-rw-rw-   0        0        0     1605 2024-03-03 14:27:52.000000 swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
--rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.470000 swarmauri-0.1.8/swarmauri/standard/conversations/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/conversations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.480000 swarmauri-0.1.8/swarmauri/standard/conversations/base/
--rw-rw-rw-   0        0        0     1129 2024-02-26 07:54:40.000000 swarmauri-0.1.8/swarmauri/standard/conversations/base/ConversationBase.py
--rw-rw-rw-   0        0        0     1615 2024-02-26 08:46:46.000000 swarmauri-0.1.8/swarmauri/standard/conversations/base/SystemContextBase.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/conversations/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.490000 swarmauri-0.1.8/swarmauri/standard/conversations/concrete/
--rw-rw-rw-   0        0        0     1355 2024-02-24 22:46:46.000000 swarmauri-0.1.8/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
--rw-rw-rw-   0        0        0     3621 2024-02-26 07:48:40.000000 swarmauri-0.1.8/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
--rw-rw-rw-   0        0        0     4703 2024-03-03 21:57:50.000000 swarmauri-0.1.8/swarmauri/standard/conversations/concrete/SharedConversation.py
--rw-rw-rw-   0        0        0      349 2024-02-25 00:13:18.000000 swarmauri-0.1.8/swarmauri/standard/conversations/concrete/SimpleConversation.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/conversations/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.490000 swarmauri-0.1.8/swarmauri/standard/document_stores/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/document_stores/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.500000 swarmauri-0.1.8/swarmauri/standard/document_stores/base/
--rw-rw-rw-   0        0        0     2465 2024-02-27 13:13:34.000000 swarmauri-0.1.8/swarmauri/standard/document_stores/base/DocumentStoreBase.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/document_stores/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.510000 swarmauri-0.1.8/swarmauri/standard/document_stores/concrete/
--rw-rw-rw-   0        0        0     2598 2024-03-05 01:36:40.000000 swarmauri-0.1.8/swarmauri/standard/document_stores/concrete/Doc2VecDocumentStore.py
--rw-rw-rw-   0        0        0     2781 2024-03-05 03:23:04.000000 swarmauri-0.1.8/swarmauri/standard/document_stores/concrete/TFIDFDocumentStore.py
--rw-rw-rw-   0        0        0     3898 2024-03-04 23:55:32.000000 swarmauri-0.1.8/swarmauri/standard/document_stores/concrete/Word2VecDocumentStore.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/document_stores/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.510000 swarmauri-0.1.8/swarmauri/standard/documents/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/documents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.520000 swarmauri-0.1.8/swarmauri/standard/documents/base/
--rw-rw-rw-   0        0        0     1615 2024-03-05 00:27:00.000000 swarmauri-0.1.8/swarmauri/standard/documents/base/DocumentBase.py
--rw-rw-rw-   0        0        0      538 2024-03-04 23:27:36.000000 swarmauri-0.1.8/swarmauri/standard/documents/base/EmbeddedBase.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/documents/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.530000 swarmauri-0.1.8/swarmauri/standard/documents/concrete/
--rw-rw-rw-   0        0        0      132 2024-03-05 01:42:48.000000 swarmauri-0.1.8/swarmauri/standard/documents/concrete/Document.py
--rw-rw-rw-   0        0        0      469 2024-03-04 23:01:20.000000 swarmauri-0.1.8/swarmauri/standard/documents/concrete/EmbeddedDocument.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/documents/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.530000 swarmauri-0.1.8/swarmauri/standard/messages/
--rw-rw-rw-   0        0        0        0 2024-02-24 22:27:04.000000 swarmauri-0.1.8/swarmauri/standard/messages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.530000 swarmauri-0.1.8/swarmauri/standard/messages/base/
--rw-rw-rw-   0        0        0     1628 2024-02-26 05:35:02.000000 swarmauri-0.1.8/swarmauri/standard/messages/base/MessageBase.py
--rw-rw-rw-   0        0        0        0 2024-02-24 22:28:22.000000 swarmauri-0.1.8/swarmauri/standard/messages/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.540000 swarmauri-0.1.8/swarmauri/standard/messages/concrete/
--rw-rw-rw-   0        0        0      309 2024-02-24 23:56:56.000000 swarmauri-0.1.8/swarmauri/standard/messages/concrete/AgentMessage.py
--rw-rw-rw-   0        0        0      836 2024-02-24 23:57:04.000000 swarmauri-0.1.8/swarmauri/standard/messages/concrete/FunctionMessage.py
--rw-rw-rw-   0        0        0      761 2024-02-24 23:57:02.000000 swarmauri-0.1.8/swarmauri/standard/messages/concrete/HumanMessage.py
--rw-rw-rw-   0        0        0      536 2024-02-24 23:57:08.000000 swarmauri-0.1.8/swarmauri/standard/messages/concrete/SystemMessage.py
--rw-rw-rw-   0        0        0      166 2024-02-24 22:27:54.000000 swarmauri-0.1.8/swarmauri/standard/messages/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.550000 swarmauri-0.1.8/swarmauri/standard/models/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.570000 swarmauri-0.1.8/swarmauri/standard/models/base/
--rw-rw-rw-   0        0        0      770 2024-02-29 03:23:18.000000 swarmauri-0.1.8/swarmauri/standard/models/base/ModelBase.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/models/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.580000 swarmauri-0.1.8/swarmauri/standard/models/concrete/
--rw-rw-rw-   0        0        0     2387 2024-02-29 03:27:06.000000 swarmauri-0.1.8/swarmauri/standard/models/concrete/AzureGPT.py
--rw-rw-rw-   0        0        0     1565 2024-02-29 03:27:20.000000 swarmauri-0.1.8/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
--rw-rw-rw-   0        0        0     2105 2024-02-29 03:25:52.000000 swarmauri-0.1.8/swarmauri/standard/models/concrete/OpenAIModel.py
--rw-rw-rw-   0        0        0      825 2024-03-03 21:05:02.000000 swarmauri-0.1.8/swarmauri/standard/models/concrete/OpenAIToolModel.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/models/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.580000 swarmauri-0.1.8/swarmauri/standard/parsers/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.590000 swarmauri-0.1.8/swarmauri/standard/parsers/base/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/parsers/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.600000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/
--rw-rw-rw-   0        0        0     2357 2024-03-01 04:56:04.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
--rw-rw-rw-   0        0        0     1785 2024-02-29 23:28:16.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/CSVParser.py
--rw-rw-rw-   0        0        0     1670 2024-02-29 23:28:30.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
--rw-rw-rw-   0        0        0     1275 2024-02-29 23:28:38.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
--rw-rw-rw-   0        0        0     1925 2024-02-29 23:28:44.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
--rw-rw-rw-   0        0        0     1723 2024-02-29 23:28:50.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/MarkdownParser.py
--rw-rw-rw-   0        0        0     1938 2024-02-29 23:28:54.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
--rw-rw-rw-   0        0        0     1576 2024-02-29 23:28:58.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
--rw-rw-rw-   0        0        0     2118 2024-02-29 23:29:02.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/PythonParser.py
--rw-rw-rw-   0        0        0     1645 2024-02-29 23:29:10.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/RegExParser.py
--rw-rw-rw-   0        0        0     1857 2024-02-29 23:29:14.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
--rw-rw-rw-   0        0        0     1386 2024-02-29 23:29:36.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
--rw-rw-rw-   0        0        0      829 2024-02-29 23:29:42.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/TfidfParser.py
--rw-rw-rw-   0        0        0     1661 2024-02-29 23:29:48.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/URLExtractorParser.py
--rw-rw-rw-   0        0        0     1952 2024-02-29 23:29:54.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/XMLParser.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/parsers/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.600000 swarmauri-0.1.8/swarmauri/standard/prompts/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/prompts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.610000 swarmauri-0.1.8/swarmauri/standard/prompts/base/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/prompts/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.630000 swarmauri-0.1.8/swarmauri/standard/prompts/concrete/
--rw-rw-rw-   0        0        0     1522 2024-02-24 22:55:06.000000 swarmauri-0.1.8/swarmauri/standard/prompts/concrete/Prompt.py
--rw-rw-rw-   0        0        0     2082 2024-02-24 22:55:20.000000 swarmauri-0.1.8/swarmauri/standard/prompts/concrete/PromptTemplate.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/prompts/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.630000 swarmauri-0.1.8/swarmauri/standard/retrievers/
--rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.8/swarmauri/standard/retrievers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.640000 swarmauri-0.1.8/swarmauri/standard/retrievers/base/
--rw-rw-rw-   0        0        0     1525 2024-02-27 13:25:48.000000 swarmauri-0.1.8/swarmauri/standard/retrievers/base/DocumentRetrieverBase.py
--rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.8/swarmauri/standard/retrievers/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.640000 swarmauri-0.1.8/swarmauri/standard/retrievers/concrete/
--rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.8/swarmauri/standard/retrievers/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.650000 swarmauri-0.1.8/swarmauri/standard/states/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/states/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.650000 swarmauri-0.1.8/swarmauri/standard/states/base/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/states/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.660000 swarmauri-0.1.8/swarmauri/standard/states/concrete/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/states/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.660000 swarmauri-0.1.8/swarmauri/standard/swarms/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/swarms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.670000 swarmauri-0.1.8/swarmauri/standard/swarms/base/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/swarms/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.680000 swarmauri-0.1.8/swarmauri/standard/swarms/concrete/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/swarms/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.680000 swarmauri-0.1.8/swarmauri/standard/toolkits/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/toolkits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.690000 swarmauri-0.1.8/swarmauri/standard/toolkits/base/
--rw-rw-rw-   0        0        0     2430 2024-02-25 00:14:18.000000 swarmauri-0.1.8/swarmauri/standard/toolkits/base/ToolkitBase.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/toolkits/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.700000 swarmauri-0.1.8/swarmauri/standard/toolkits/concrete/
--rw-rw-rw-   0        0        0      510 2024-02-25 00:14:40.000000 swarmauri-0.1.8/swarmauri/standard/toolkits/concrete/Toolkit.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/toolkits/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.700000 swarmauri-0.1.8/swarmauri/standard/tools/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.710000 swarmauri-0.1.8/swarmauri/standard/tools/base/
--rw-rw-rw-   0        0        0     2351 2024-03-03 17:48:26.000000 swarmauri-0.1.8/swarmauri/standard/tools/base/ToolBase.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/tools/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.720000 swarmauri-0.1.8/swarmauri/standard/tools/concrete/
--rw-rw-rw-   0        0        0     1021 2024-02-29 03:53:26.000000 swarmauri-0.1.8/swarmauri/standard/tools/concrete/AdditionTool.py
--rw-rw-rw-   0        0        0     3181 2024-02-25 00:22:04.000000 swarmauri-0.1.8/swarmauri/standard/tools/concrete/Parameter.py
--rw-rw-rw-   0        0        0      981 2024-02-24 22:57:00.000000 swarmauri-0.1.8/swarmauri/standard/tools/concrete/TestTool.py
--rw-rw-rw-   0        0        0     1121 2024-02-24 22:57:12.000000 swarmauri-0.1.8/swarmauri/standard/tools/concrete/WeatherTool.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/tools/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.720000 swarmauri-0.1.8/swarmauri/standard/tracing/
--rw-rw-rw-   0        0        0        1 2024-03-02 03:57:38.000000 swarmauri-0.1.8/swarmauri/standard/tracing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.720000 swarmauri-0.1.8/swarmauri/standard/tracing/base/
--rw-rw-rw-   0        0        0        1 2024-03-02 03:57:44.000000 swarmauri-0.1.8/swarmauri/standard/tracing/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.730000 swarmauri-0.1.8/swarmauri/standard/tracing/concrete/
--rw-rw-rw-   0        0        0     1424 2024-03-06 07:31:36.000000 swarmauri-0.1.8/swarmauri/standard/tracing/concrete/CallableTracer.py
--rw-rw-rw-   0        0        0     2115 2024-03-06 05:51:12.000000 swarmauri-0.1.8/swarmauri/standard/tracing/concrete/ChainTracer.py
--rw-rw-rw-   0        0        0      715 2024-03-06 07:30:20.000000 swarmauri-0.1.8/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
--rw-rw-rw-   0        0        0     1660 2024-03-06 00:24:10.000000 swarmauri-0.1.8/swarmauri/standard/tracing/concrete/SimpleTracer.py
--rw-rw-rw-   0        0        0     1126 2024-03-06 00:57:18.000000 swarmauri-0.1.8/swarmauri/standard/tracing/concrete/TracedVariable.py
--rw-rw-rw-   0        0        0     1042 2024-03-06 07:31:20.000000 swarmauri-0.1.8/swarmauri/standard/tracing/concrete/VariableTracer.py
--rw-rw-rw-   0        0        0        0 2024-03-06 07:46:20.000000 swarmauri-0.1.8/swarmauri/standard/tracing/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.740000 swarmauri-0.1.8/swarmauri/standard/utils/
--rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.8/swarmauri/standard/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.740000 swarmauri-0.1.8/swarmauri/standard/vector_stores/
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.750000 swarmauri-0.1.8/swarmauri/standard/vector_stores/base/
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.760000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/
--rw-rw-rw-   0        0        0     1504 2024-03-03 14:30:54.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/ChiSquaredDistance.py
--rw-rw-rw-   0        0        0     2682 2024-03-04 23:27:58.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/CosineDistance.py
--rw-rw-rw-   0        0        0     1998 2024-03-03 14:29:58.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/EuclideanDistance.py
--rw-rw-rw-   0        0        0     3527 2024-03-01 03:38:10.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/FaissVectorStore.py
--rw-rw-rw-   0        0        0     2769 2024-03-03 14:31:06.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/JaccardIndexDistance.py
--rw-rw-rw-   0        0        0     3242 2024-03-03 14:30:12.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/LevenshteinDistance.py
--rw-rw-rw-   0        0        0     1429 2024-03-01 10:02:22.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/VectorProduct.py
--rw-rw-rw-   0        0        0     1542 2024-03-03 14:31:34.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/WeaviateVectorStore.py
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.760000 swarmauri-0.1.8/swarmauri/standard/vectorizers/
--rw-rw-rw-   0        0        0        1 2024-03-01 00:01:54.000000 swarmauri-0.1.8/swarmauri/standard/vectorizers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.770000 swarmauri-0.1.8/swarmauri/standard/vectorizers/base/
--rw-rw-rw-   0        0        0        1 2024-03-01 00:02:00.000000 swarmauri-0.1.8/swarmauri/standard/vectorizers/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.780000 swarmauri-0.1.8/swarmauri/standard/vectorizers/concrete/
--rw-rw-rw-   0        0        0     2285 2024-03-01 10:45:14.000000 swarmauri-0.1.8/swarmauri/standard/vectorizers/concrete/BERTEmbeddingVectorizer.py
--rw-rw-rw-   0        0        0     2369 2024-03-01 10:43:42.000000 swarmauri-0.1.8/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
--rw-rw-rw-   0        0        0        1 2024-03-01 00:01:54.000000 swarmauri-0.1.8/swarmauri/standard/vectorizers/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.790000 swarmauri-0.1.8/swarmauri/standard/vectors/
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/vectors/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.800000 swarmauri-0.1.8/swarmauri/standard/vectors/base/
--rw-rw-rw-   0        0        0      751 2024-03-01 23:28:40.000000 swarmauri-0.1.8/swarmauri/standard/vectors/base/VectorBase.py
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/vectors/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.810000 swarmauri-0.1.8/swarmauri/standard/vectors/concrete/
--rw-rw-rw-   0        0        0      211 2024-03-01 04:52:48.000000 swarmauri-0.1.8/swarmauri/standard/vectors/concrete/SimpleVector.py
--rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.8/swarmauri/standard/vectors/concrete/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-06 12:26:20.290000 swarmauri-0.1.8/swarmauri.egg-info/
--rw-rw-rw-   0        0        0     3496 2024-03-06 12:26:30.000000 swarmauri-0.1.8/swarmauri.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12966 2024-03-06 12:26:30.000000 swarmauri-0.1.8/swarmauri.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 12:26:30.000000 swarmauri-0.1.8/swarmauri.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      576 2024-03-06 12:26:30.000000 swarmauri-0.1.8/swarmauri.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-06 12:26:30.000000 swarmauri-0.1.8/swarmauri.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.960000 swarmauri-0.1.9/
+-rw-rw-rw-   0        0        0     3496 2024-03-07 03:38:56.000000 swarmauri-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2024-03-03 14:10:52.000000 swarmauri-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-07 03:38:56.000000 swarmauri-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2170 2024-03-04 21:18:48.000000 swarmauri-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.970000 swarmauri-0.1.9/swarmauri/
+-rw-rw-rw-   0        0        0       21 2024-03-06 12:54:10.000000 swarmauri-0.1.9/swarmauri/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.970000 swarmauri-0.1.9/swarmauri/community/
+-rw-rw-rw-   0        0        0        0 2024-03-01 11:37:30.000000 swarmauri-0.1.9/swarmauri/community/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.980000 swarmauri-0.1.9/swarmauri/community/document_stores/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/document_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.980000 swarmauri-0.1.9/swarmauri/community/document_stores/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/document_stores/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.980000 swarmauri-0.1.9/swarmauri/community/document_stores/concrete/
+-rw-rw-rw-   0        0        0     2873 2024-02-27 22:23:48.000000 swarmauri-0.1.9/swarmauri/community/document_stores/concrete/RedisDocumentStore.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/document_stores/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.980000 swarmauri-0.1.9/swarmauri/community/retrievers/
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/community/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.990000 swarmauri-0.1.9/swarmauri/community/retrievers/base/
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/community/retrievers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.990000 swarmauri-0.1.9/swarmauri/community/retrievers/concrete/
+-rw-rw-rw-   0        0        0     2087 2024-02-27 19:40:22.000000 swarmauri-0.1.9/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/community/retrievers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.990000 swarmauri-0.1.9/swarmauri/community/tools/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.000000 swarmauri-0.1.9/swarmauri/community/tools/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/tools/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/
+-rw-rw-rw-   0        0        0     2477 2024-02-26 12:20:58.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/DownloadPdfTool.py
+-rw-rw-rw-   0        0        0     1159 2024-02-25 00:17:10.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/EntityRecognitionTool.py
+-rw-rw-rw-   0        0        0     4073 2024-02-25 00:17:14.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/GmailReadTool.py
+-rw-rw-rw-   0        0        0     4081 2024-03-03 17:06:56.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/GmailSendTool.py
+-rw-rw-rw-   0        0        0     2491 2024-02-27 06:54:54.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/PaCMAP.py
+-rw-rw-rw-   0        0        0      888 2024-02-25 00:17:56.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/SentimentAnalysisTool.py
+-rw-rw-rw-   0        0        0     2098 2024-02-26 10:14:00.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/WebScrapingTool.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/community/tools/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.000000 swarmauri-0.1.9/swarmauri/core/
+-rw-rw-rw-   0        0        0        0 2024-03-03 23:23:40.000000 swarmauri-0.1.9/swarmauri/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.010000 swarmauri-0.1.9/swarmauri/core/agent_apis/
+-rw-rw-rw-   0        0        0     2067 2024-02-29 07:10:06.000000 swarmauri-0.1.9/swarmauri/core/agent_apis/IAgentCommands.py
+-rw-rw-rw-   0        0        0     1786 2024-02-29 07:10:32.000000 swarmauri-0.1.9/swarmauri/core/agent_apis/IAgentRouterCRUD.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/agent_apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.010000 swarmauri-0.1.9/swarmauri/core/agents/
+-rw-rw-rw-   0        0        0      477 2024-03-06 13:34:16.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentConversation.py
+-rw-rw-rw-   0        0        0      317 2024-03-06 13:37:18.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentDocument.py
+-rw-rw-rw-   0        0        0      355 2024-03-06 14:06:14.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentName.py
+-rw-rw-rw-   0        0        0      303 2024-03-06 13:37:54.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentParser.py
+-rw-rw-rw-   0        0        0      327 2024-03-06 13:37:14.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentRetriever.py
+-rw-rw-rw-   0        0        0      317 2024-03-06 13:33:32.000000 swarmauri-0.1.9/swarmauri/core/agents/IAgentToolkit.py
+-rw-rw-rw-   0        0        0      638 2024-03-06 13:34:38.000000 swarmauri-0.1.9/swarmauri/core/agents/ISwarmAgent.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.010000 swarmauri-0.1.9/swarmauri/core/chains/
+-rw-rw-rw-   0        0        0      511 2024-03-06 07:13:14.000000 swarmauri-0.1.9/swarmauri/core/chains/ICallableChain.py
+-rw-rw-rw-   0        0        0     1228 2024-03-07 03:38:28.000000 swarmauri-0.1.9/swarmauri/core/chains/IChain.py
+-rw-rw-rw-   0        0        0      960 2024-03-06 22:31:24.000000 swarmauri-0.1.9/swarmauri/core/chains/IChainStep.py
+-rw-rw-rw-   0        0        0       63 2024-03-06 07:46:14.000000 swarmauri-0.1.9/swarmauri/core/chains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.020000 swarmauri-0.1.9/swarmauri/core/chunkers/
+-rw-rw-rw-   0        0        0     1134 2024-03-06 09:41:16.000000 swarmauri-0.1.9/swarmauri/core/chunkers/IChunker.py
+-rw-rw-rw-   0        0        0       93 2024-02-29 02:35:28.000000 swarmauri-0.1.9/swarmauri/core/chunkers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.020000 swarmauri-0.1.9/swarmauri/core/conversations/
+-rw-rw-rw-   0        0        0     1165 2024-02-24 21:26:54.000000 swarmauri-0.1.9/swarmauri/core/conversations/IConversation.py
+-rw-rw-rw-   0        0        0      307 2024-02-24 19:48:48.000000 swarmauri-0.1.9/swarmauri/core/conversations/IMaxSize.py
+-rw-rw-rw-   0        0        0      871 2024-02-24 21:28:08.000000 swarmauri-0.1.9/swarmauri/core/conversations/ISystemContext.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/conversations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.020000 swarmauri-0.1.9/swarmauri/core/document_stores/
+-rw-rw-rw-   0        0        0     2179 2024-02-25 01:07:04.000000 swarmauri-0.1.9/swarmauri/core/document_stores/IDocumentStore.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/document_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.030000 swarmauri-0.1.9/swarmauri/core/documents/
+-rw-rw-rw-   0        0        0     1597 2024-02-29 23:27:20.000000 swarmauri-0.1.9/swarmauri/core/documents/IDocument.py
+-rw-rw-rw-   0        0        0      486 2024-03-04 22:09:54.000000 swarmauri-0.1.9/swarmauri/core/documents/IEmbed.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/documents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.030000 swarmauri-0.1.9/swarmauri/core/messages/
+-rw-rw-rw-   0        0        0      722 2024-02-22 03:01:56.000000 swarmauri-0.1.9/swarmauri/core/messages/IMessage.py
+-rw-rw-rw-   0        0        0       30 2024-02-24 21:26:46.000000 swarmauri-0.1.9/swarmauri/core/messages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.030000 swarmauri-0.1.9/swarmauri/core/models/
+-rw-rw-rw-   0        0        0      298 2024-02-29 03:14:00.000000 swarmauri-0.1.9/swarmauri/core/models/IFit.py
+-rw-rw-rw-   0        0        0      485 2024-02-29 03:15:00.000000 swarmauri-0.1.9/swarmauri/core/models/IModel.py
+-rw-rw-rw-   0        0        0      311 2024-02-29 03:13:40.000000 swarmauri-0.1.9/swarmauri/core/models/IPredict.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.030000 swarmauri-0.1.9/swarmauri/core/parsers/
+-rw-rw-rw-   0        0        0      778 2024-02-24 21:26:38.000000 swarmauri-0.1.9/swarmauri/core/parsers/IParser.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.040000 swarmauri-0.1.9/swarmauri/core/prompts/
+-rw-rw-rw-   0        0        0      556 2024-02-24 19:59:22.000000 swarmauri-0.1.9/swarmauri/core/prompts/IPrompt.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/prompts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.040000 swarmauri-0.1.9/swarmauri/core/retrievers/
+-rw-rw-rw-   0        0        0      904 2024-02-24 21:27:04.000000 swarmauri-0.1.9/swarmauri/core/retrievers/IRetriever.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 23:23:58.000000 swarmauri-0.1.9/swarmauri/core/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.040000 swarmauri-0.1.9/swarmauri/core/swarm_apis/
+-rw-rw-rw-   0        0        0     2306 2024-02-29 07:15:38.000000 swarmauri-0.1.9/swarmauri/core/swarm_apis/IAgentRegistration.py
+-rw-rw-rw-   0        0        0     1140 2024-03-03 14:20:54.000000 swarmauri-0.1.9/swarmauri/core/swarm_apis/ISwarmAPI.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/swarm_apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.050000 swarmauri-0.1.9/swarmauri/core/swarms/
+-rw-rw-rw-   0        0        0        0 2024-02-23 03:51:40.000000 swarmauri-0.1.9/swarmauri/core/swarms/ISwarm.py
+-rw-rw-rw-   0        0        0      331 2024-03-06 22:32:50.000000 swarmauri-0.1.9/swarmauri/core/swarms/ISwarmComponent.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/swarms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.050000 swarmauri-0.1.9/swarmauri/core/toolkits/
+-rw-rw-rw-   0        0        0     1635 2024-02-24 21:26:30.000000 swarmauri-0.1.9/swarmauri/core/toolkits/IToolkit.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/toolkits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.060000 swarmauri-0.1.9/swarmauri/core/tools/
+-rw-rw-rw-   0        0        0     2042 2024-02-24 20:06:46.000000 swarmauri-0.1.9/swarmauri/core/tools/IParameter.py
+-rw-rw-rw-   0        0        0      516 2024-03-03 17:27:50.000000 swarmauri-0.1.9/swarmauri/core/tools/ITool.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.060000 swarmauri-0.1.9/swarmauri/core/tracing/
+-rw-rw-rw-   0        0        0     1058 2024-03-06 05:25:36.000000 swarmauri-0.1.9/swarmauri/core/tracing/IChainTracer.py
+-rw-rw-rw-   0        0        0      804 2024-03-02 05:02:52.000000 swarmauri-0.1.9/swarmauri/core/tracing/ITraceContext.py
+-rw-rw-rw-   0        0        0     1606 2024-03-06 00:14:54.000000 swarmauri-0.1.9/swarmauri/core/tracing/ITracer.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/tracing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.060000 swarmauri-0.1.9/swarmauri/core/utils/
+-rw-rw-rw-   0        0        0      637 2024-02-27 19:34:00.000000 swarmauri-0.1.9/swarmauri/core/utils/ITransactional.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/core/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.070000 swarmauri-0.1.9/swarmauri/core/vector_stores/
+-rw-rw-rw-   0        0        0      800 2024-02-29 05:59:20.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IAngleBetweenVectors.py
+-rw-rw-rw-   0        0        0     1054 2024-02-29 06:51:34.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IDecompose.py
+-rw-rw-rw-   0        0        0     1676 2024-03-01 22:46:34.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IDistanceSimilarity.py
+-rw-rw-rw-   0        0        0      702 2024-02-29 06:17:22.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IDivergence.py
+-rw-rw-rw-   0        0        0      828 2024-02-29 06:15:56.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IGradient.py
+-rw-rw-rw-   0        0        0      721 2024-02-29 05:46:12.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IOrthogonalProject.py
+-rw-rw-rw-   0        0        0      619 2024-02-29 05:46:38.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IProject.py
+-rw-rw-rw-   0        0        0      661 2024-02-29 06:12:02.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IReflect.py
+-rw-rw-rw-   0        0        0      939 2024-02-29 04:08:20.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/ISimilarity.py
+-rw-rw-rw-   0        0        0      848 2024-02-27 19:35:06.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/ISimiliarityQuery.py
+-rw-rw-rw-   0        0        0      888 2024-02-29 05:28:14.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorArithmetic.py
+-rw-rw-rw-   0        0        0      588 2024-02-29 06:55:40.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorBasisCheck.py
+-rw-rw-rw-   0        0        0      711 2024-02-29 06:44:38.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorLinearCombination.py
+-rw-rw-rw-   0        0        0     1362 2024-02-29 04:54:00.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorNorm.py
+-rw-rw-rw-   0        0        0     2108 2024-02-29 05:40:54.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorProduct.py
+-rw-rw-rw-   0        0        0      757 2024-02-29 06:25:06.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorRotate.py
+-rw-rw-rw-   0        0        0      672 2024-02-29 06:40:18.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorSpan.py
+-rw-rw-rw-   0        0        0     1924 2024-02-29 22:26:24.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorStore.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 23:24:08.000000 swarmauri-0.1.9/swarmauri/core/vector_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.080000 swarmauri-0.1.9/swarmauri/core/vectorizers/
+-rw-rw-rw-   0        0        0      624 2024-03-01 10:44:28.000000 swarmauri-0.1.9/swarmauri/core/vectorizers/IVectorize.py
+-rw-rw-rw-   0        0        0        1 2024-02-29 23:57:16.000000 swarmauri-0.1.9/swarmauri/core/vectorizers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.080000 swarmauri-0.1.9/swarmauri/core/vectors/
+-rw-rw-rw-   0        0        0      578 2024-03-01 23:23:06.000000 swarmauri-0.1.9/swarmauri/core/vectors/IVector.py
+-rw-rw-rw-   0        0        0      900 2024-02-29 04:09:42.000000 swarmauri-0.1.9/swarmauri/core/vectors/IVectorMeta.py
+-rw-rw-rw-   0        0        0     1312 2024-02-29 22:50:46.000000 swarmauri-0.1.9/swarmauri/core/vectors/IVectorTransform.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 23:24:16.000000 swarmauri-0.1.9/swarmauri/core/vectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.080000 swarmauri-0.1.9/swarmauri/experimental/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/experimental/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.080000 swarmauri-0.1.9/swarmauri/experimental/chains/
+-rw-rw-rw-   0        0        0      628 2024-03-06 23:57:40.000000 swarmauri-0.1.9/swarmauri/experimental/chains/ChainOrderStrategy.py
+-rw-rw-rw-   0        0        0      516 2024-03-06 22:36:46.000000 swarmauri-0.1.9/swarmauri/experimental/chains/ChainOrderStrategyBase.py
+-rw-rw-rw-   0        0        0      842 2024-03-06 23:53:50.000000 swarmauri-0.1.9/swarmauri/experimental/chains/ChainProcessingStrategy.py
+-rw-rw-rw-   0        0        0      603 2024-03-06 23:48:40.000000 swarmauri-0.1.9/swarmauri/experimental/chains/ChainProcessingStrategyBase.py
+-rw-rw-rw-   0        0        0      299 2024-03-06 22:32:20.000000 swarmauri-0.1.9/swarmauri/experimental/chains/IChainOrderStrategy.py
+-rw-rw-rw-   0        0        0      585 2024-03-06 22:32:10.000000 swarmauri-0.1.9/swarmauri/experimental/chains/IChainProcessingStrategy.py
+-rw-rw-rw-   0        0        0      725 2024-03-07 01:54:34.000000 swarmauri-0.1.9/swarmauri/experimental/chains/MatrixOrderStrategy.py
+-rw-rw-rw-   0        0        0     1073 2024-03-07 00:47:16.000000 swarmauri-0.1.9/swarmauri/experimental/chains/MatrixProcessingStrategy.py
+-rw-rw-rw-   0        0        0     4481 2024-03-06 12:26:20.000000 swarmauri-0.1.9/swarmauri/experimental/chains/TypeAgnosticCallableChain.py
+-rw-rw-rw-   0        0        0        1 2024-03-07 03:35:10.000000 swarmauri-0.1.9/swarmauri/experimental/chains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.090000 swarmauri-0.1.9/swarmauri/experimental/conversations/
+-rw-rw-rw-   0        0        0     3471 2024-03-04 00:27:10.000000 swarmauri-0.1.9/swarmauri/experimental/conversations/ConsensusBuildingConversation.py
+-rw-rw-rw-   0        0        0     2219 2024-02-24 23:03:58.000000 swarmauri-0.1.9/swarmauri/experimental/conversations/SemanticConversation.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:51:08.000000 swarmauri-0.1.9/swarmauri/experimental/conversations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.090000 swarmauri-0.1.9/swarmauri/experimental/models/
+-rw-rw-rw-   0        0        0     3556 2024-03-03 14:27:12.000000 swarmauri-0.1.9/swarmauri/experimental/models/HierarchicalAttentionModel.py
+-rw-rw-rw-   0        0        0     1846 2024-02-24 23:05:02.000000 swarmauri-0.1.9/swarmauri/experimental/models/SageMaker.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 05:01:34.000000 swarmauri-0.1.9/swarmauri/experimental/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.090000 swarmauri-0.1.9/swarmauri/experimental/parsers/
+-rw-rw-rw-   0        0        0     1508 2024-02-29 02:42:10.000000 swarmauri-0.1.9/swarmauri/experimental/parsers/PDFToTextParser.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/experimental/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.100000 swarmauri-0.1.9/swarmauri/experimental/tools/
+-rw-rw-rw-   0        0        0     1414 2024-02-29 02:47:28.000000 swarmauri-0.1.9/swarmauri/experimental/tools/CypherQueryTool.py
+-rw-rw-rw-   0        0        0     1237 2024-02-29 02:49:12.000000 swarmauri-0.1.9/swarmauri/experimental/tools/FileDownloaderTool.py
+-rw-rw-rw-   0        0        0     3466 2024-02-24 23:06:28.000000 swarmauri-0.1.9/swarmauri/experimental/tools/LinkedInArticleTool.py
+-rw-rw-rw-   0        0        0     2918 2024-02-27 18:57:56.000000 swarmauri-0.1.9/swarmauri/experimental/tools/OutlookSendMailTool.py
+-rw-rw-rw-   0        0        0     1357 2024-02-29 02:51:04.000000 swarmauri-0.1.9/swarmauri/experimental/tools/SQLite3QueryTool.py
+-rw-rw-rw-   0        0        0     1511 2024-02-24 23:06:52.000000 swarmauri-0.1.9/swarmauri/experimental/tools/TwitterPostTool.py
+-rw-rw-rw-   0        0        0       27 2024-02-27 18:55:30.000000 swarmauri-0.1.9/swarmauri/experimental/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.110000 swarmauri-0.1.9/swarmauri/experimental/utils/
+-rw-rw-rw-   0        0        0      973 2024-02-27 19:36:04.000000 swarmauri-0.1.9/swarmauri/experimental/utils/ISerializable.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/experimental/utils/__init__.py
+-rw-rw-rw-   0        0        0      655 2024-02-23 08:24:16.000000 swarmauri-0.1.9/swarmauri/experimental/utils/get_last_frame.py
+-rw-rw-rw-   0        0        0     2141 2024-02-23 08:34:46.000000 swarmauri-0.1.9/swarmauri/experimental/utils/save_schema.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.110000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/
+-rw-rw-rw-   0        0        0     2854 2024-03-03 14:29:14.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/CanberraDistance.py
+-rw-rw-rw-   0        0        0     1875 2024-03-03 14:30:48.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/ChebyshevDistance.py
+-rw-rw-rw-   0        0        0     2024 2024-03-03 14:31:04.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/HaversineDistance.py
+-rw-rw-rw-   0        0        0     2347 2024-03-03 14:31:12.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/ManhattanDistance.py
+-rw-rw-rw-   0        0        0     2866 2024-03-03 14:35:10.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/MinkowskiDistance.py
+-rw-rw-rw-   0        0        0     2057 2024-02-29 09:06:24.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/SSASimilarity.py
+-rw-rw-rw-   0        0        0     2643 2024-02-29 09:07:00.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/SSIVSimilarity.py
+-rw-rw-rw-   0        0        0     7058 2024-03-03 09:40:08.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/ScannVectorStore.py
+-rw-rw-rw-   0        0        0     2213 2024-03-03 14:31:54.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/SorensenDiceDistance.py
+-rw-rw-rw-   0        0        0     1989 2024-03-03 14:31:30.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/experimental/vector_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.110000 swarmauri-0.1.9/swarmauri/standard/
+-rw-rw-rw-   0        0        0        0 2024-03-06 07:33:08.000000 swarmauri-0.1.9/swarmauri/standard/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.120000 swarmauri-0.1.9/swarmauri/standard/agents/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.120000 swarmauri-0.1.9/swarmauri/standard/agents/base/
+-rw-rw-rw-   0        0        0     1650 2024-03-06 14:58:36.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/AgentBase.py
+-rw-rw-rw-   0        0        0      913 2024-03-06 15:05:42.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/ConversationAgentBase.py
+-rw-rw-rw-   0        0        0      546 2024-03-06 14:31:00.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/NamedAgentBase.py
+-rw-rw-rw-   0        0        0     1061 2024-03-06 15:05:50.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/ToolAgentBase.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/agents/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.120000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/
+-rw-rw-rw-   0        0        0     1688 2024-03-06 14:42:14.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/ChatSwarmAgent.py
+-rw-rw-rw-   0        0        0     2101 2024-03-06 15:05:58.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
+-rw-rw-rw-   0        0        0     3847 2024-03-06 15:06:02.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
+-rw-rw-rw-   0        0        0      925 2024-03-06 14:55:40.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
+-rw-rw-rw-   0        0        0      569 2024-03-06 14:55:32.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/SingleCommandAgent.py
+-rw-rw-rw-   0        0        0     3451 2024-03-06 14:00:52.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/ToolAgent.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/agents/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.130000 swarmauri-0.1.9/swarmauri/standard/apis/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.130000 swarmauri-0.1.9/swarmauri/standard/apis/base/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/apis/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.130000 swarmauri-0.1.9/swarmauri/standard/apis/concrete/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/apis/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.150000 swarmauri-0.1.9/swarmauri/standard/chains/
+-rw-rw-rw-   0        0        0        0 2024-03-06 07:46:30.000000 swarmauri-0.1.9/swarmauri/standard/chains/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.150000 swarmauri-0.1.9/swarmauri/standard/chains/base/
+-rw-rw-rw-   0        0        0     2007 2024-03-07 03:22:46.000000 swarmauri-0.1.9/swarmauri/standard/chains/base/ChainBase.py
+-rw-rw-rw-   0        0        0     1050 2024-03-06 23:41:32.000000 swarmauri-0.1.9/swarmauri/standard/chains/base/ChainStepBase.py
+-rw-rw-rw-   0        0        0        1 2024-03-06 07:27:50.000000 swarmauri-0.1.9/swarmauri/standard/chains/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.150000 swarmauri-0.1.9/swarmauri/standard/chains/concrete/
+-rw-rw-rw-   0        0        0     1262 2024-03-06 10:26:28.000000 swarmauri-0.1.9/swarmauri/standard/chains/concrete/CallableChain.py
+-rw-rw-rw-   0        0        0     1594 2024-03-06 23:53:24.000000 swarmauri-0.1.9/swarmauri/standard/chains/concrete/Chain.py
+-rw-rw-rw-   0        0        0        0 2024-03-06 07:46:36.000000 swarmauri-0.1.9/swarmauri/standard/chains/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.160000 swarmauri-0.1.9/swarmauri/standard/chunkers/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.160000 swarmauri-0.1.9/swarmauri/standard/chunkers/base/
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.160000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/
+-rw-rw-rw-   0        0        0     1935 2024-03-03 14:28:00.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
+-rw-rw-rw-   0        0        0     1477 2024-03-03 14:27:50.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
+-rw-rw-rw-   0        0        0     2164 2024-03-06 09:27:14.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
+-rw-rw-rw-   0        0        0     1198 2024-03-05 00:05:40.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
+-rw-rw-rw-   0        0        0     1605 2024-03-03 14:27:52.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 04:36:46.000000 swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.170000 swarmauri-0.1.9/swarmauri/standard/conversations/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.180000 swarmauri-0.1.9/swarmauri/standard/conversations/base/
+-rw-rw-rw-   0        0        0     1129 2024-02-26 07:54:40.000000 swarmauri-0.1.9/swarmauri/standard/conversations/base/ConversationBase.py
+-rw-rw-rw-   0        0        0     1615 2024-02-26 08:46:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/base/SystemContextBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.180000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/
+-rw-rw-rw-   0        0        0     1355 2024-02-24 22:46:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py
+-rw-rw-rw-   0        0        0     3621 2024-02-26 07:48:40.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py
+-rw-rw-rw-   0        0        0     4703 2024-03-03 21:57:50.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/SharedConversation.py
+-rw-rw-rw-   0        0        0      349 2024-02-25 00:13:18.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/SimpleConversation.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/conversations/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.190000 swarmauri-0.1.9/swarmauri/standard/document_stores/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.190000 swarmauri-0.1.9/swarmauri/standard/document_stores/base/
+-rw-rw-rw-   0        0        0     2465 2024-02-27 13:13:34.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/base/DocumentStoreBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.200000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/
+-rw-rw-rw-   0        0        0     2598 2024-03-05 01:36:40.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/Doc2VecDocumentStore.py
+-rw-rw-rw-   0        0        0     2781 2024-03-05 03:23:04.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/TFIDFDocumentStore.py
+-rw-rw-rw-   0        0        0     3898 2024-03-04 23:55:32.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/Word2VecDocumentStore.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.200000 swarmauri-0.1.9/swarmauri/standard/documents/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/documents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.200000 swarmauri-0.1.9/swarmauri/standard/documents/base/
+-rw-rw-rw-   0        0        0     1615 2024-03-05 00:27:00.000000 swarmauri-0.1.9/swarmauri/standard/documents/base/DocumentBase.py
+-rw-rw-rw-   0        0        0      538 2024-03-04 23:27:36.000000 swarmauri-0.1.9/swarmauri/standard/documents/base/EmbeddedBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/documents/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.210000 swarmauri-0.1.9/swarmauri/standard/documents/concrete/
+-rw-rw-rw-   0        0        0      132 2024-03-05 01:42:48.000000 swarmauri-0.1.9/swarmauri/standard/documents/concrete/Document.py
+-rw-rw-rw-   0        0        0      469 2024-03-04 23:01:20.000000 swarmauri-0.1.9/swarmauri/standard/documents/concrete/EmbeddedDocument.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/documents/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.220000 swarmauri-0.1.9/swarmauri/standard/messages/
+-rw-rw-rw-   0        0        0        0 2024-02-24 22:27:04.000000 swarmauri-0.1.9/swarmauri/standard/messages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.220000 swarmauri-0.1.9/swarmauri/standard/messages/base/
+-rw-rw-rw-   0        0        0     1628 2024-02-26 05:35:02.000000 swarmauri-0.1.9/swarmauri/standard/messages/base/MessageBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-24 22:28:22.000000 swarmauri-0.1.9/swarmauri/standard/messages/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.230000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/
+-rw-rw-rw-   0        0        0      309 2024-02-24 23:56:56.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/AgentMessage.py
+-rw-rw-rw-   0        0        0      836 2024-02-24 23:57:04.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/FunctionMessage.py
+-rw-rw-rw-   0        0        0      761 2024-02-24 23:57:02.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/HumanMessage.py
+-rw-rw-rw-   0        0        0      536 2024-02-24 23:57:08.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/SystemMessage.py
+-rw-rw-rw-   0        0        0      166 2024-02-24 22:27:54.000000 swarmauri-0.1.9/swarmauri/standard/messages/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.230000 swarmauri-0.1.9/swarmauri/standard/models/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.240000 swarmauri-0.1.9/swarmauri/standard/models/base/
+-rw-rw-rw-   0        0        0      770 2024-02-29 03:23:18.000000 swarmauri-0.1.9/swarmauri/standard/models/base/ModelBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/models/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.240000 swarmauri-0.1.9/swarmauri/standard/models/concrete/
+-rw-rw-rw-   0        0        0     2387 2024-02-29 03:27:06.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/AzureGPT.py
+-rw-rw-rw-   0        0        0     1565 2024-02-29 03:27:20.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIImageGenerator.py
+-rw-rw-rw-   0        0        0     2105 2024-02-29 03:25:52.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIModel.py
+-rw-rw-rw-   0        0        0      825 2024-03-03 21:05:02.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIToolModel.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/models/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.240000 swarmauri-0.1.9/swarmauri/standard/parsers/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.250000 swarmauri-0.1.9/swarmauri/standard/parsers/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/parsers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.250000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/
+-rw-rw-rw-   0        0        0     2357 2024-03-01 04:56:04.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py
+-rw-rw-rw-   0        0        0     1785 2024-02-29 23:28:16.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/CSVParser.py
+-rw-rw-rw-   0        0        0     1670 2024-02-29 23:28:30.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py
+-rw-rw-rw-   0        0        0     1275 2024-02-29 23:28:38.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py
+-rw-rw-rw-   0        0        0     1925 2024-02-29 23:28:44.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py
+-rw-rw-rw-   0        0        0     1723 2024-02-29 23:28:50.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/MarkdownParser.py
+-rw-rw-rw-   0        0        0     1938 2024-02-29 23:28:54.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py
+-rw-rw-rw-   0        0        0     1576 2024-02-29 23:28:58.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py
+-rw-rw-rw-   0        0        0     2118 2024-02-29 23:29:02.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/PythonParser.py
+-rw-rw-rw-   0        0        0     1645 2024-02-29 23:29:10.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/RegExParser.py
+-rw-rw-rw-   0        0        0     1857 2024-02-29 23:29:14.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TextBlobNounParser.py
+-rw-rw-rw-   0        0        0     1386 2024-02-29 23:29:36.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py
+-rw-rw-rw-   0        0        0      829 2024-02-29 23:29:42.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TfidfParser.py
+-rw-rw-rw-   0        0        0     1661 2024-02-29 23:29:48.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/URLExtractorParser.py
+-rw-rw-rw-   0        0        0     1952 2024-02-29 23:29:54.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/XMLParser.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/parsers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.260000 swarmauri-0.1.9/swarmauri/standard/prompts/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/prompts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.260000 swarmauri-0.1.9/swarmauri/standard/prompts/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/prompts/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.270000 swarmauri-0.1.9/swarmauri/standard/prompts/concrete/
+-rw-rw-rw-   0        0        0     1522 2024-02-24 22:55:06.000000 swarmauri-0.1.9/swarmauri/standard/prompts/concrete/Prompt.py
+-rw-rw-rw-   0        0        0     2082 2024-02-24 22:55:20.000000 swarmauri-0.1.9/swarmauri/standard/prompts/concrete/PromptTemplate.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/prompts/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.270000 swarmauri-0.1.9/swarmauri/standard/retrievers/
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/standard/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.280000 swarmauri-0.1.9/swarmauri/standard/retrievers/base/
+-rw-rw-rw-   0        0        0     1525 2024-02-27 13:25:48.000000 swarmauri-0.1.9/swarmauri/standard/retrievers/base/DocumentRetrieverBase.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/standard/retrievers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.280000 swarmauri-0.1.9/swarmauri/standard/retrievers/concrete/
+-rw-rw-rw-   0        0        0       27 2024-02-20 00:24:10.000000 swarmauri-0.1.9/swarmauri/standard/retrievers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.290000 swarmauri-0.1.9/swarmauri/standard/states/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/states/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.290000 swarmauri-0.1.9/swarmauri/standard/states/base/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/states/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.300000 swarmauri-0.1.9/swarmauri/standard/states/concrete/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/states/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.300000 swarmauri-0.1.9/swarmauri/standard/swarms/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/swarms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.300000 swarmauri-0.1.9/swarmauri/standard/swarms/base/
+-rw-rw-rw-   0        0        0      553 2024-03-06 22:40:40.000000 swarmauri-0.1.9/swarmauri/standard/swarms/base/SwarmComponentBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/swarms/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.310000 swarmauri-0.1.9/swarmauri/standard/swarms/concrete/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/swarms/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.320000 swarmauri-0.1.9/swarmauri/standard/toolkits/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.320000 swarmauri-0.1.9/swarmauri/standard/toolkits/base/
+-rw-rw-rw-   0        0        0     2430 2024-02-25 00:14:18.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/base/ToolkitBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.320000 swarmauri-0.1.9/swarmauri/standard/toolkits/concrete/
+-rw-rw-rw-   0        0        0      510 2024-02-25 00:14:40.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/concrete/Toolkit.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/toolkits/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.330000 swarmauri-0.1.9/swarmauri/standard/tools/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.330000 swarmauri-0.1.9/swarmauri/standard/tools/base/
+-rw-rw-rw-   0        0        0     2351 2024-03-03 17:48:26.000000 swarmauri-0.1.9/swarmauri/standard/tools/base/ToolBase.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/tools/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.330000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/
+-rw-rw-rw-   0        0        0     1021 2024-02-29 03:53:26.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/AdditionTool.py
+-rw-rw-rw-   0        0        0     3181 2024-02-25 00:22:04.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/Parameter.py
+-rw-rw-rw-   0        0        0      981 2024-02-24 22:57:00.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/TestTool.py
+-rw-rw-rw-   0        0        0     1121 2024-02-24 22:57:12.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/WeatherTool.py
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/tools/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.330000 swarmauri-0.1.9/swarmauri/standard/tracing/
+-rw-rw-rw-   0        0        0        1 2024-03-02 03:57:38.000000 swarmauri-0.1.9/swarmauri/standard/tracing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.340000 swarmauri-0.1.9/swarmauri/standard/tracing/base/
+-rw-rw-rw-   0        0        0        1 2024-03-02 03:57:44.000000 swarmauri-0.1.9/swarmauri/standard/tracing/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.340000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/
+-rw-rw-rw-   0        0        0     1424 2024-03-06 07:31:36.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/CallableTracer.py
+-rw-rw-rw-   0        0        0     2115 2024-03-06 05:51:12.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/ChainTracer.py
+-rw-rw-rw-   0        0        0      715 2024-03-06 07:30:20.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/SimpleTraceContext.py
+-rw-rw-rw-   0        0        0     1660 2024-03-06 00:24:10.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/SimpleTracer.py
+-rw-rw-rw-   0        0        0     1126 2024-03-06 00:57:18.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/TracedVariable.py
+-rw-rw-rw-   0        0        0     1042 2024-03-06 07:31:20.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/VariableTracer.py
+-rw-rw-rw-   0        0        0        0 2024-03-06 07:46:20.000000 swarmauri-0.1.9/swarmauri/standard/tracing/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.360000 swarmauri-0.1.9/swarmauri/standard/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-19 02:42:46.000000 swarmauri-0.1.9/swarmauri/standard/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.360000 swarmauri-0.1.9/swarmauri/standard/vector_stores/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.370000 swarmauri-0.1.9/swarmauri/standard/vector_stores/base/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.380000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/
+-rw-rw-rw-   0        0        0     1504 2024-03-03 14:30:54.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/ChiSquaredDistance.py
+-rw-rw-rw-   0        0        0     2682 2024-03-04 23:27:58.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/CosineDistance.py
+-rw-rw-rw-   0        0        0     1998 2024-03-03 14:29:58.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/EuclideanDistance.py
+-rw-rw-rw-   0        0        0     3527 2024-03-01 03:38:10.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/FaissVectorStore.py
+-rw-rw-rw-   0        0        0     2769 2024-03-03 14:31:06.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/JaccardIndexDistance.py
+-rw-rw-rw-   0        0        0     3242 2024-03-03 14:30:12.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/LevenshteinDistance.py
+-rw-rw-rw-   0        0        0     1429 2024-03-01 10:02:22.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/VectorProduct.py
+-rw-rw-rw-   0        0        0     1542 2024-03-03 14:31:34.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/WeaviateVectorStore.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.380000 swarmauri-0.1.9/swarmauri/standard/vectorizers/
+-rw-rw-rw-   0        0        0        1 2024-03-01 00:01:54.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.400000 swarmauri-0.1.9/swarmauri/standard/vectorizers/base/
+-rw-rw-rw-   0        0        0        1 2024-03-01 00:02:00.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.410000 swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/
+-rw-rw-rw-   0        0        0     2285 2024-03-01 10:45:14.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/BERTEmbeddingVectorizer.py
+-rw-rw-rw-   0        0        0     2369 2024-03-01 10:43:42.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
+-rw-rw-rw-   0        0        0        1 2024-03-01 00:01:54.000000 swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.420000 swarmauri-0.1.9/swarmauri/standard/vectors/
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vectors/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.420000 swarmauri-0.1.9/swarmauri/standard/vectors/base/
+-rw-rw-rw-   0        0        0      751 2024-03-01 23:28:40.000000 swarmauri-0.1.9/swarmauri/standard/vectors/base/VectorBase.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vectors/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:55.430000 swarmauri-0.1.9/swarmauri/standard/vectors/concrete/
+-rw-rw-rw-   0        0        0      211 2024-03-01 04:52:48.000000 swarmauri-0.1.9/swarmauri/standard/vectors/concrete/SimpleVector.py
+-rw-rw-rw-   0        0        0       27 2024-02-20 05:28:32.000000 swarmauri-0.1.9/swarmauri/standard/vectors/concrete/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-07 03:38:54.970000 swarmauri-0.1.9/swarmauri.egg-info/
+-rw-rw-rw-   0        0        0     3496 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14135 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      576 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-03-07 03:38:56.000000 swarmauri-0.1.9/swarmauri.egg-info/top_level.txt
```

### Comparing `swarmauri-0.1.8/PKG-INFO` & `swarmauri-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.1.8
+Version: 0.1.9
 Summary: A short description of your package
 Home-page: http://github.com/yourusername/your_package_name
 Author: Jacob Stewart
 Author-email: your_email@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri-0.1.8/README.md` & `swarmauri-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/setup.py` & `swarmauri-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/document_stores/concrete/RedisDocumentStore.py` & `swarmauri-0.1.9/swarmauri/community/document_stores/concrete/RedisDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py` & `swarmauri-0.1.9/swarmauri/community/retrievers/concrete/RedisDocumentRetriever.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/tools/concrete/DownloadPdfTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/DownloadPdfTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/tools/concrete/EntityRecognitionTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/EntityRecognitionTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/tools/concrete/GmailReadTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/GmailReadTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/tools/concrete/GmailSendTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/GmailSendTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/tools/concrete/PaCMAP.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/PaCMAP.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/tools/concrete/SentimentAnalysisTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/SentimentAnalysisTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/community/tools/concrete/WebScrapingTool.py` & `swarmauri-0.1.9/swarmauri/community/tools/concrete/WebScrapingTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/agent_apis/IAgentCommands.py` & `swarmauri-0.1.9/swarmauri/core/agent_apis/IAgentCommands.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/agent_apis/IAgentRouterCRUD.py` & `swarmauri-0.1.9/swarmauri/core/agent_apis/IAgentRouterCRUD.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/chunkers/IChunker.py` & `swarmauri-0.1.9/swarmauri/core/chunkers/IChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/conversations/IConversation.py` & `swarmauri-0.1.9/swarmauri/core/conversations/IConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/conversations/ISystemContext.py` & `swarmauri-0.1.9/swarmauri/core/conversations/ISystemContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/document_stores/IDocumentStore.py` & `swarmauri-0.1.9/swarmauri/core/document_stores/IDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/documents/IDocument.py` & `swarmauri-0.1.9/swarmauri/core/documents/IDocument.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/messages/IMessage.py` & `swarmauri-0.1.9/swarmauri/core/messages/IMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/parsers/IParser.py` & `swarmauri-0.1.9/swarmauri/core/parsers/IParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/prompts/IPrompt.py` & `swarmauri-0.1.9/swarmauri/core/prompts/IPrompt.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/retrievers/IRetriever.py` & `swarmauri-0.1.9/swarmauri/core/retrievers/IRetriever.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/swarm_apis/IAgentRegistration.py` & `swarmauri-0.1.9/swarmauri/core/swarm_apis/IAgentRegistration.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/swarm_apis/ISwarmAPI.py` & `swarmauri-0.1.9/swarmauri/core/swarm_apis/ISwarmAPI.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/toolkits/IToolkit.py` & `swarmauri-0.1.9/swarmauri/core/toolkits/IToolkit.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/tools/IParameter.py` & `swarmauri-0.1.9/swarmauri/core/tools/IParameter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/tools/ITool.py` & `swarmauri-0.1.9/swarmauri/core/tools/ITool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/tracing/IChainTracer.py` & `swarmauri-0.1.9/swarmauri/core/tracing/IChainTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/tracing/ITraceContext.py` & `swarmauri-0.1.9/swarmauri/core/tracing/ITraceContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/tracing/ITracer.py` & `swarmauri-0.1.9/swarmauri/core/tracing/ITracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/utils/ITransactional.py` & `swarmauri-0.1.9/swarmauri/core/utils/ITransactional.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IAngleBetweenVectors.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IAngleBetweenVectors.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IDecompose.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IDecompose.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IDistanceSimilarity.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IDistanceSimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IDivergence.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IDivergence.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IGradient.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IGradient.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IOrthogonalProject.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IOrthogonalProject.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IProject.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IProject.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IReflect.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IReflect.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/ISimilarity.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/ISimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/ISimiliarityQuery.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/ISimiliarityQuery.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorArithmetic.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorArithmetic.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorBasisCheck.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorBasisCheck.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorLinearCombination.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorLinearCombination.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorNorm.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorNorm.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorProduct.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorProduct.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorRotate.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorRotate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorSpan.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorSpan.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vector_stores/IVectorStore.py` & `swarmauri-0.1.9/swarmauri/core/vector_stores/IVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vectorizers/IVectorize.py` & `swarmauri-0.1.9/swarmauri/core/vectorizers/IVectorize.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vectors/IVector.py` & `swarmauri-0.1.9/swarmauri/core/vectors/IVector.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vectors/IVectorMeta.py` & `swarmauri-0.1.9/swarmauri/core/vectors/IVectorMeta.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/core/vectors/IVectorTransform.py` & `swarmauri-0.1.9/swarmauri/core/vectors/IVectorTransform.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/conversations/ConsensusBuildingConversation.py` & `swarmauri-0.1.9/swarmauri/experimental/conversations/ConsensusBuildingConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/conversations/SemanticConversation.py` & `swarmauri-0.1.9/swarmauri/experimental/conversations/SemanticConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/models/HierarchicalAttentionModel.py` & `swarmauri-0.1.9/swarmauri/experimental/models/HierarchicalAttentionModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/models/SageMaker.py` & `swarmauri-0.1.9/swarmauri/experimental/models/SageMaker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/parsers/PDFToTextParser.py` & `swarmauri-0.1.9/swarmauri/experimental/parsers/PDFToTextParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/tools/CypherQueryTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/CypherQueryTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/tools/FileDownloaderTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/FileDownloaderTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/tools/LinkedInArticleTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/LinkedInArticleTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/tools/OutlookSendMailTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/OutlookSendMailTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/tools/SQLite3QueryTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/SQLite3QueryTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/tools/TwitterPostTool.py` & `swarmauri-0.1.9/swarmauri/experimental/tools/TwitterPostTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/utils/ISerializable.py` & `swarmauri-0.1.9/swarmauri/experimental/utils/ISerializable.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/utils/get_last_frame.py` & `swarmauri-0.1.9/swarmauri/experimental/utils/get_last_frame.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/utils/save_schema.py` & `swarmauri-0.1.9/swarmauri/experimental/utils/save_schema.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/CanberraDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/CanberraDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/ChebyshevDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/ChebyshevDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/HaversineDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/HaversineDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/ManhattanDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/ManhattanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/MinkowskiDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/MinkowskiDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/SSASimilarity.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/SSASimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/SSIVSimilarity.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/SSIVSimilarity.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/ScannVectorStore.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/ScannVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/SorensenDiceDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/SorensenDiceDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py` & `swarmauri-0.1.9/swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/agents/base/SwarmAgentBase.py` & `swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/Doc2VecDocumentStore.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,57 @@
-from typing import Any, Optional, List
-from abc import ABC, abstractmethod
-from ....core.agents.ISwarmAgent import ISwarmAgent
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....core.conversations.IConversation import IConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ...messages.concrete.HumanMessage import HumanMessage
-
-class SwarmAgentBase(ISwarmAgent, ABC):
-    @abstractmethod
-    def __init__(self, 
-                 model: IModel, 
-                 conversation: Optional[IConversation] = None,
-                 toolkit: Optional[IToolkit] = None, parser: Optional[IParser] = None, 
-                 documents: Optional[List[IDocument]] = [], retriever: Optional[IRetriever] = None):
-
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
-        self._model = model
-        self._toolkit = toolkit
-        self._parser = parser
-        self._conversation = conversation
-        self._documents = documents 
-        self._retriever = retriever
-
-    def exec(self, input_str: Optional[Any]) -> Any:
-        pass
-    
-    @property
-    def model(self) -> IModel:
-        return self._model
-    
-    @model.setter
-    def model(self, value) -> IModel:
-        self._model = value        
-
-    def get_model(self) -> IModel:
-        return self._model
-    
-    def get_toolkit(self) -> Optional[IToolkit]:
-        return self._toolkit
-    
-    @property
-    def parser(self) -> IModel:
-        return self._parser
-    
-    @model.setter
-    def parser(self, value) -> IModel:
-        self._parser = value
-    
-    
-    def get_parser(self) -> Optional[IParser]:
-        return self._parser
-
-    @property
-    def conversation(self) -> Optional[IConversation]:
-        return self._conversation
-
-    @conversation.setter
-    def conversation(self, value) -> Optional[IConversation]:
-        self._conversation = value
-
-    def get_conversation(self) -> Optional[IConversation]:
-        return self._conversation
-    
-    def get_documents(self) -> List[IDocument]:
-        return self._documents
-    
-    def get_retriever(self) -> Optional[IRetriever]:
-        return self._retriever 
-    
-    def __getattr__(self, name):
-        # Example of transforming attribute name from simplified to internal naming convention
-        internal_name = f"_{name}"
-        if internal_name in self.__dict__:
-            return self.__dict__[internal_name]
-        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
-    
-    def __setattr__(self, name, value):
-        # Direct assignment to the __dict__ to bypass any potential infinite recursion
-        # from setting attributes that do not explicitly exist.
-        object.__setattr__(self, name, value) 
+from typing import List, Union, Optional
+import numpy as np
+from gensim.models.doc2vec import TaggedDocument, Doc2Vec
+from swarmauri.core.document_stores.IDocumentStore import IDocumentStore
+from swarmauri.core.retrievers.IRetriever import IRetriever
+from swarmauri.core.documents.IDocument import IDocument
+from swarmauri.standard.vector_stores.concrete.CosineDistance import CosineDistance
+from swarmauri.standard.vectors.concrete.SimpleVector import SimpleVector
+import gensim.downloader as api
+
+class Doc2VecDocumentStore(IDocumentStore, IRetriever):
+    def __init__(self):
+        self.model = Doc2Vec(vector_size=2000, window=10, min_count=1, workers=5)  # Example parameters; adjust as needed
+        self.documents = []
+        self.metric = CosineDistance()
+
+    def add_document(self, document: IDocument) -> None:
+        self.documents.append(document)
+        self._train()
         
+    def add_documents(self, documents: List[IDocument]) -> None:
+        self.documents.extend(documents)
+        self._train()
         
-    def __str__(self):
-        class_name = self.__class__.__name__
-        variables_str = ", ".join(f"{k}={v}" for k, v in self.__dict__.items())
-        return f"<{class_name} {variables_str}>"
+    def get_document(self, doc_id: str) -> Union[IDocument, None]:
+        for document in self.documents:
+            if document.id == doc_id:
+                return document
+        return None
         
-    def __repr__(self):
-        class_name = self.__class__.__name__
-        variables_str = ", ".join(f"{k}={v}" for k, v in self.__dict__.items())
-        return f"{class_name} ({variables_str})"
+    def get_all_documents(self) -> List[IDocument]:
+        return self.documents
+        
+    def delete_document(self, doc_id: str) -> None:
+        self.documents = [doc for doc in self.documents if doc.id != doc_id]
+
+    def update_document(self, doc_id: str, updated_document: IDocument) -> None:
+        for i, document in enumerate(self.documents):
+            if document.id == doc_id:
+                self.documents[i] = updated_document
+                break
+        self._train()
+
+    def retrieve(self, query: str, top_k: int = 5) -> List[IDocument]:
+        """
+        Retrieve documents similar to the query string based on Word2Vec embeddings.
+        """
+        query_vector = self.model.infer_vector(query.split())
+
+        similarities = self.model.dv.most_similar([query_vector], topn=self.model.corpus_count)
+        top_k_indices = sorted(range(len(similarities)), key=lambda i: similarities[i], reverse=True)[:top_k]
+        return [self.documents[i] for i in top_k_indices]
+
+    def _train(self):
+        tagged_data = [TaggedDocument(words=_d.content.split(), tags=[str(i)]) for i, _d in enumerate(self.documents) if _d.content]
+        self.model.build_vocab(tagged_data)
+        self.model.train(tagged_data, total_examples=self.model.corpus_count, epochs=self.model.epochs)
```

### Comparing `swarmauri-0.1.8/swarmauri/standard/agents/concrete/ChatSwarmAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/ChatSwarmAgent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-from typing import Any, Optional, List, Union, Dict
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....core.conversations.IConversation import IConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from typing import Any, Optional, Union, Dict
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.messages import IMessage
+from swarmauri.core.conversations import IConversation
+from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage, AgentMessage
-
-class ChatSwarmAgent(SwarmAgentBase):
-    def __init__(self, 
-                 model: IModel, 
-                 conversation: Optional[IConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None,
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IRetriever] = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
+class ChatSwarmAgent(ConversationAgentBase):
+    def __init__(self, model: IModel, conversation: IConversation):
+        super().__init__(model, conversation)
 
     def exec(self, input_data: Union[str, IMessage], model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.get_conversation()
-        model = self.get_model()
+        conversation = self.conversation
+        model = self.model
 
         # Check if the input is a string, then wrap it in a HumanMessage
         if isinstance(input_data, str):
             human_message = HumanMessage(input_data)
         elif isinstance(input_data, IMessage):
             human_message = input_data
         else:
```

### Comparing `swarmauri-0.1.8/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,28 @@
-from typing import Any, Optional, List, Union, Dict
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....standard.conversations.concrete.SharedConversation import SharedConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from typing import Any, Optional, Union, Dict
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage, AgentMessage
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.messages import IMessage
 
-class MultiPartyChatSwarmAgent(SwarmAgentBase):
+from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
+from swarmauri.standard.agents.base.NamedAgentBase import NamedAgentBase
+from swarmauri.standard.conversations.concrete.SharedConversation import SharedConversation
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage
+
+class MultiPartyChatSwarmAgent(ConversationAgentBase, NamedAgentBase):
     def __init__(self, 
                  model: IModel, 
-                 conversation: Optional[SharedConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None,
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IRetriever] = None,
-                 name: str = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
-        self.name = name
+                 conversation: SharedConversation,
+                 name: str):
+        ConversationAgentBase.__init__(self, model, conversation)
+        NamedAgentBase.__init__(self, name)
 
     def exec(self, input_data: Union[str, IMessage] = "", model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.get_conversation()
-        model = self.get_model()
+        conversation = self.conversation
+        model = self.model
 
         # Check if the input is a string, then wrap it in a HumanMessage
         if isinstance(input_data, str):
             human_message = HumanMessage(input_data)
         elif isinstance(input_data, IMessage):
             human_message = input_data
         else:
```

### Comparing `swarmauri-0.1.8/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py` & `swarmauri-0.1.9/swarmauri/standard/agents/concrete/SimpleSwarmAgent.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-from typing import Any, Optional, List
+from typing import Any, Optional
 
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....core.conversations.IConversation import IConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.conversations.IConversation import IConversation
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage
 
-class SimpleSwarmAgent(SwarmAgentBase):
+from swarmauri.standard.agents.base.SwarmAgentBase import AgentBase
+from swarmauri.standard.messages.concrete import HumanMessage
+
+class SimpleSwarmAgent(AgentBase):
     def __init__(self, model: IModel, 
-                 conversation: Optional[IConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None, 
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IRetriever] = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
+                 conversation: IConversation):
+        super().__init__(model, conversation)
 
     def exec(self, input_str: Optional[str] = None) -> Any:
-        conversation = self.get_conversation()
-        model = self.get_model()
+        conversation = self.conversation
+        model = self.model
 
         # Construct a new human message (for example purposes)
         if input_str:
             human_message = HumanMessage(input_str)
             conversation.add_message(human_message)
         
         messages = conversation.as_dict()
```

### Comparing `swarmauri-0.1.8/swarmauri/standard/chains/concrete/CallableChain.py` & `swarmauri-0.1.9/swarmauri/standard/chains/concrete/CallableChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/chains/concrete/TypeAgnosticCallableChain.py` & `swarmauri-0.1.9/swarmauri/experimental/chains/TypeAgnosticCallableChain.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py` & `swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py` & `swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/FixedLengthChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py` & `swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/MdSnippetChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py` & `swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py` & `swarmauri-0.1.9/swarmauri/standard/chunkers/concrete/SlidingWindowChunker.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/conversations/base/ConversationBase.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/base/ConversationBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/conversations/base/SystemContextBase.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/base/SystemContextBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/concrete/LimitedSizeConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/concrete/LimitedSystemContextConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/conversations/concrete/SharedConversation.py` & `swarmauri-0.1.9/swarmauri/standard/conversations/concrete/SharedConversation.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/document_stores/base/DocumentStoreBase.py` & `swarmauri-0.1.9/swarmauri/standard/document_stores/base/DocumentStoreBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/document_stores/concrete/TFIDFDocumentStore.py` & `swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/TFIDFDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/document_stores/concrete/Word2VecDocumentStore.py` & `swarmauri-0.1.9/swarmauri/standard/document_stores/concrete/Word2VecDocumentStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/documents/base/DocumentBase.py` & `swarmauri-0.1.9/swarmauri/standard/documents/base/DocumentBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/documents/base/EmbeddedBase.py` & `swarmauri-0.1.9/swarmauri/standard/documents/base/EmbeddedBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/messages/base/MessageBase.py` & `swarmauri-0.1.9/swarmauri/standard/messages/base/MessageBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/messages/concrete/FunctionMessage.py` & `swarmauri-0.1.9/swarmauri/standard/messages/concrete/FunctionMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/messages/concrete/HumanMessage.py` & `swarmauri-0.1.9/swarmauri/standard/messages/concrete/HumanMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/messages/concrete/SystemMessage.py` & `swarmauri-0.1.9/swarmauri/standard/messages/concrete/SystemMessage.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/models/base/ModelBase.py` & `swarmauri-0.1.9/swarmauri/standard/models/base/ModelBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/models/concrete/AzureGPT.py` & `swarmauri-0.1.9/swarmauri/standard/models/concrete/AzureGPT.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/models/concrete/OpenAIImageGenerator.py` & `swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIImageGenerator.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/models/concrete/OpenAIModel.py` & `swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/models/concrete/OpenAIToolModel.py` & `swarmauri-0.1.9/swarmauri/standard/models/concrete/OpenAIToolModel.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/BERTEmbeddingParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/CSVParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/CSVParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/EntityRecognitionParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/HtmlTagStripParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/KeywordExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/MarkdownParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/MarkdownParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/OpenAPISpecParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/PhoneNumberExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/PythonParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/PythonParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/RegExParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/RegExParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/TextBlobNounParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TextBlobNounParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TextBlobSentenceParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/TfidfParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/TfidfParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/URLExtractorParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/URLExtractorParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/parsers/concrete/XMLParser.py` & `swarmauri-0.1.9/swarmauri/standard/parsers/concrete/XMLParser.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/prompts/concrete/Prompt.py` & `swarmauri-0.1.9/swarmauri/standard/prompts/concrete/Prompt.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/prompts/concrete/PromptTemplate.py` & `swarmauri-0.1.9/swarmauri/standard/prompts/concrete/PromptTemplate.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/retrievers/base/DocumentRetrieverBase.py` & `swarmauri-0.1.9/swarmauri/standard/retrievers/base/DocumentRetrieverBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/toolkits/base/ToolkitBase.py` & `swarmauri-0.1.9/swarmauri/standard/toolkits/base/ToolkitBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tools/base/ToolBase.py` & `swarmauri-0.1.9/swarmauri/standard/tools/base/ToolBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tools/concrete/AdditionTool.py` & `swarmauri-0.1.9/swarmauri/standard/tools/concrete/AdditionTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tools/concrete/Parameter.py` & `swarmauri-0.1.9/swarmauri/standard/tools/concrete/Parameter.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tools/concrete/TestTool.py` & `swarmauri-0.1.9/swarmauri/standard/tools/concrete/TestTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tools/concrete/WeatherTool.py` & `swarmauri-0.1.9/swarmauri/standard/tools/concrete/WeatherTool.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tracing/concrete/CallableTracer.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/CallableTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tracing/concrete/ChainTracer.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/ChainTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tracing/concrete/SimpleTraceContext.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/SimpleTraceContext.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tracing/concrete/SimpleTracer.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/SimpleTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tracing/concrete/TracedVariable.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/TracedVariable.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/tracing/concrete/VariableTracer.py` & `swarmauri-0.1.9/swarmauri/standard/tracing/concrete/VariableTracer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/ChiSquaredDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/ChiSquaredDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/CosineDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/CosineDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/EuclideanDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/EuclideanDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/FaissVectorStore.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/FaissVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/JaccardIndexDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/JaccardIndexDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/LevenshteinDistance.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/LevenshteinDistance.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/VectorProduct.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/VectorProduct.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vector_stores/concrete/WeaviateVectorStore.py` & `swarmauri-0.1.9/swarmauri/standard/vector_stores/concrete/WeaviateVectorStore.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vectorizers/concrete/BERTEmbeddingVectorizer.py` & `swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/BERTEmbeddingVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py` & `swarmauri-0.1.9/swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri/standard/vectors/base/VectorBase.py` & `swarmauri-0.1.9/swarmauri/standard/vectors/base/VectorBase.py`

 * *Files identical despite different names*

### Comparing `swarmauri-0.1.8/swarmauri.egg-info/PKG-INFO` & `swarmauri-0.1.9/swarmauri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.1.8
+Version: 0.1.9
 Summary: A short description of your package
 Home-page: http://github.com/yourusername/your_package_name
 Author: Jacob Stewart
 Author-email: your_email@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `swarmauri-0.1.8/swarmauri.egg-info/SOURCES.txt` & `swarmauri-0.1.9/swarmauri.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,25 @@
 swarmauri/community/tools/concrete/SentimentAnalysisTool.py
 swarmauri/community/tools/concrete/WebScrapingTool.py
 swarmauri/community/tools/concrete/__init__.py
 swarmauri/core/__init__.py
 swarmauri/core/agent_apis/IAgentCommands.py
 swarmauri/core/agent_apis/IAgentRouterCRUD.py
 swarmauri/core/agent_apis/__init__.py
+swarmauri/core/agents/IAgentConversation.py
+swarmauri/core/agents/IAgentDocument.py
+swarmauri/core/agents/IAgentName.py
+swarmauri/core/agents/IAgentParser.py
+swarmauri/core/agents/IAgentRetriever.py
+swarmauri/core/agents/IAgentToolkit.py
 swarmauri/core/agents/ISwarmAgent.py
 swarmauri/core/agents/__init__.py
 swarmauri/core/chains/ICallableChain.py
+swarmauri/core/chains/IChain.py
+swarmauri/core/chains/IChainStep.py
 swarmauri/core/chains/__init__.py
 swarmauri/core/chunkers/IChunker.py
 swarmauri/core/chunkers/__init__.py
 swarmauri/core/conversations/IConversation.py
 swarmauri/core/conversations/IMaxSize.py
 swarmauri/core/conversations/ISystemContext.py
 swarmauri/core/conversations/__init__.py
@@ -56,14 +64,15 @@
 swarmauri/core/prompts/__init__.py
 swarmauri/core/retrievers/IRetriever.py
 swarmauri/core/retrievers/__init__.py
 swarmauri/core/swarm_apis/IAgentRegistration.py
 swarmauri/core/swarm_apis/ISwarmAPI.py
 swarmauri/core/swarm_apis/__init__.py
 swarmauri/core/swarms/ISwarm.py
+swarmauri/core/swarms/ISwarmComponent.py
 swarmauri/core/swarms/__init__.py
 swarmauri/core/toolkits/IToolkit.py
 swarmauri/core/toolkits/__init__.py
 swarmauri/core/tools/IParameter.py
 swarmauri/core/tools/ITool.py
 swarmauri/core/tools/__init__.py
 swarmauri/core/tracing/IChainTracer.py
@@ -94,14 +103,24 @@
 swarmauri/core/vectorizers/IVectorize.py
 swarmauri/core/vectorizers/__init__.py
 swarmauri/core/vectors/IVector.py
 swarmauri/core/vectors/IVectorMeta.py
 swarmauri/core/vectors/IVectorTransform.py
 swarmauri/core/vectors/__init__.py
 swarmauri/experimental/__init__.py
+swarmauri/experimental/chains/ChainOrderStrategy.py
+swarmauri/experimental/chains/ChainOrderStrategyBase.py
+swarmauri/experimental/chains/ChainProcessingStrategy.py
+swarmauri/experimental/chains/ChainProcessingStrategyBase.py
+swarmauri/experimental/chains/IChainOrderStrategy.py
+swarmauri/experimental/chains/IChainProcessingStrategy.py
+swarmauri/experimental/chains/MatrixOrderStrategy.py
+swarmauri/experimental/chains/MatrixProcessingStrategy.py
+swarmauri/experimental/chains/TypeAgnosticCallableChain.py
+swarmauri/experimental/chains/__init__.py
 swarmauri/experimental/conversations/ConsensusBuildingConversation.py
 swarmauri/experimental/conversations/SemanticConversation.py
 swarmauri/experimental/conversations/__init__.py
 swarmauri/experimental/models/HierarchicalAttentionModel.py
 swarmauri/experimental/models/SageMaker.py
 swarmauri/experimental/models/__init__.py
 swarmauri/experimental/parsers/PDFToTextParser.py
@@ -126,30 +145,35 @@
 swarmauri/experimental/vector_stores/SSIVSimilarity.py
 swarmauri/experimental/vector_stores/ScannVectorStore.py
 swarmauri/experimental/vector_stores/SorensenDiceDistance.py
 swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py
 swarmauri/experimental/vector_stores/__init__.py
 swarmauri/standard/__init__.py
 swarmauri/standard/agents/__init__.py
-swarmauri/standard/agents/base/SwarmAgentBase.py
+swarmauri/standard/agents/base/AgentBase.py
+swarmauri/standard/agents/base/ConversationAgentBase.py
+swarmauri/standard/agents/base/NamedAgentBase.py
+swarmauri/standard/agents/base/ToolAgentBase.py
 swarmauri/standard/agents/base/__init__.py
 swarmauri/standard/agents/concrete/ChatSwarmAgent.py
 swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
 swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
 swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
 swarmauri/standard/agents/concrete/SingleCommandAgent.py
 swarmauri/standard/agents/concrete/ToolAgent.py
 swarmauri/standard/agents/concrete/__init__.py
 swarmauri/standard/apis/__init__.py
 swarmauri/standard/apis/base/__init__.py
 swarmauri/standard/apis/concrete/__init__.py
 swarmauri/standard/chains/__init__.py
+swarmauri/standard/chains/base/ChainBase.py
+swarmauri/standard/chains/base/ChainStepBase.py
 swarmauri/standard/chains/base/__init__.py
 swarmauri/standard/chains/concrete/CallableChain.py
-swarmauri/standard/chains/concrete/TypeAgnosticCallableChain.py
+swarmauri/standard/chains/concrete/Chain.py
 swarmauri/standard/chains/concrete/__init__.py
 swarmauri/standard/chunkers/__init__.py
 swarmauri/standard/chunkers/base/__init__.py
 swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
 swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
 swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
 swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
@@ -221,14 +245,15 @@
 swarmauri/standard/retrievers/base/DocumentRetrieverBase.py
 swarmauri/standard/retrievers/base/__init__.py
 swarmauri/standard/retrievers/concrete/__init__.py
 swarmauri/standard/states/__init__.py
 swarmauri/standard/states/base/__init__.py
 swarmauri/standard/states/concrete/__init__.py
 swarmauri/standard/swarms/__init__.py
+swarmauri/standard/swarms/base/SwarmComponentBase.py
 swarmauri/standard/swarms/base/__init__.py
 swarmauri/standard/swarms/concrete/__init__.py
 swarmauri/standard/toolkits/__init__.py
 swarmauri/standard/toolkits/base/ToolkitBase.py
 swarmauri/standard/toolkits/base/__init__.py
 swarmauri/standard/toolkits/concrete/Toolkit.py
 swarmauri/standard/toolkits/concrete/__init__.py
```

### Comparing `swarmauri-0.1.8/swarmauri.egg-info/requires.txt` & `swarmauri-0.1.9/swarmauri.egg-info/requires.txt`

 * *Files identical despite different names*

