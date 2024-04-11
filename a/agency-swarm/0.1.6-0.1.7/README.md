# Comparing `tmp/agency-swarm-0.1.6.tar.gz` & `tmp/agency-swarm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agency-swarm-0.1.6.tar", last modified: Tue Mar 26 14:59:09 2024, max compression
+gzip compressed data, was "agency-swarm-0.1.7.tar", last modified: Thu Apr 11 10:16:07 2024, max compression
```

## Comparing `agency-swarm-0.1.6.tar` & `agency-swarm-0.1.7.tar`

### file list

```diff
@@ -1,176 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.320582 agency-swarm-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.324582 agency-swarm-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.324582 agency-swarm-0.1.6/agency_swarm/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.328582 agency-swarm-0.1.6/agency_swarm/agency/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38376 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/agency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.328582 agency-swarm-0.1.6/agency_swarm/agency/genesis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.328582 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.328582 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/GetAvailableAgents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.328582 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisAgency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.328582 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.332582 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.332582 agency-swarm-0.1.6/agency_swarm/agency/genesis/OpenAPICreator/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/OpenAPICreator/OpenAPICreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/OpenAPICreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/OpenAPICreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.332582 agency-swarm-0.1.6/agency_swarm/agency/genesis/OpenAPICreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.332582 agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/instructions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.332582 agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/manifesto.md
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agency/genesis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.332582 agency-swarm-0.1.6/agency_swarm/agents/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22460 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.332582 agency-swarm-0.1.6/agency_swarm/agents/browsing/
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/BrowsingAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.336582 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/AnalyzeContent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/ClickElement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/ExportFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/GoBack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/ReadURL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/Scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/SelectDropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/SendKeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/SolveCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.336582 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/util/get_b64_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/util/highlights.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/util/selenium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.336582 agency-swarm-0.1.6/agency_swarm/agents/coding/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.336582 agency-swarm-0.1.6/agency_swarm/agents/coding/CodingAgent/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/coding/CodingAgent/CodingAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/coding/CodingAgent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/coding/CodingAgent/instructions.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/agents/coding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.336582 agency-swarm-0.1.6/agency_swarm/messages/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/messages/message_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.336582 agency-swarm-0.1.6/agency_swarm/threads/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/threads/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/threads/thread_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.336582 agency-swarm-0.1.6/agency_swarm/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/BaseTool.py
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/ToolFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.336582 agency-swarm-0.1.6/agency_swarm/tools/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/coding/ChangeDir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/coding/ChangeLines.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/coding/CreateFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/coding/ListDir.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/coding/ReadFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/coding/WriteFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.340582 agency-swarm-0.1.6/agency_swarm/tools/oai/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/oai/CodeInterpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/oai/Retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/tools/oai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.340582 agency-swarm-0.1.6/agency_swarm/user/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/user/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.340582 agency-swarm-0.1.6/agency_swarm/util/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/util/create_agent_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/util/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/util/oai.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/util/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/agency_swarm/util/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/agency_swarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11322 2024-03-26 14:59:09.000000 agency-swarm-0.1.6/agency_swarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-03-26 14:59:09.000000 agency-swarm-0.1.6/agency_swarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 14:59:09.000000 agency-swarm-0.1.6/agency_swarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-26 14:59:09.000000 agency-swarm-0.1.6/agency_swarm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-26 14:59:09.000000 agency-swarm-0.1.6/agency_swarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-26 14:59:09.000000 agency-swarm-0.1.6/agency_swarm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.340582 agency-swarm-0.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.340582 agency-swarm-0.1.6/docs/advanced-usage/
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/advanced-usage/agencies.md
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/advanced-usage/agents.md
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/advanced-usage/azure-openai.md
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/advanced-usage/tools.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.340582 agency-swarm-0.1.6/docs/introduction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/introduction/showcase.md
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/notebooks/agency_async.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/notebooks/azure.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/notebooks/genesis_agency.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/notebooks/web_browser_agent.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.324582 agency-swarm-0.1.6/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/tests/data/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/files/csv-test.csv
--rw-r--r--   0 runner    (1001) docker     (127)   102408 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/files/generated_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/files/test-docx.docx
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/files/test-html.html
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/files/test-md.md
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/files/test-pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/files/test-txt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/files/test-xml.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/tests/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/schemas/ga4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/schemas/get-headers-params.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/schemas/get-weather.json
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/schemas/relevance.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/tests/data/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/data/tools/ExampleTool1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:59:09.344582 agency-swarm-0.1.6/tests/demos/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/demos/demo_gradio.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/demos/streaming_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/demos/term_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    15677 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/test_agency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-03-26 14:59:04.000000 agency-swarm-0.1.6/tests/test_tool_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.317707 agency-swarm-0.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.325707 agency-swarm-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.325707 agency-swarm-0.1.7/agency_swarm/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.325707 agency-swarm-0.1.7/agency_swarm/agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42253 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/agency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.325707 agency-swarm-0.1.7/agency_swarm/agency/genesis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisAgency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/OpenAPICreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.329707 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.333707 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/manifesto.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agency/genesis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.333707 agency-swarm-0.1.7/agency_swarm/agents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.333707 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/BrowsingAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/instructions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.333707 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/GoBack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/Scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/get_b64_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/selenium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/agents/Devid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/Devid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/instructions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/ChangeFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/CheckCurrentDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/CommandExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/DirectoryNavigator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileMover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/FileWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/ListDir.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/util/format_file_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23014 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/agents/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/messages/message_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.337707 agency-swarm-0.1.7/agency_swarm/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/threads/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/threads/thread_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/BaseTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/ToolFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/tools/oai/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/oai/CodeInterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/oai/Retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/tools/oai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/user/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/util/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/cli/create_agent_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/cli/import_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.341707 agency-swarm-0.1.7/agency_swarm/util/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/helpers/get_available_agent_descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/helpers/list_available_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/oai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/agency_swarm/util/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/agency_swarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 10:16:07.000000 agency-swarm-0.1.7/agency_swarm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/docs/advanced-usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/advanced-usage/agencies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/advanced-usage/agents.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/advanced-usage/azure-openai.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/advanced-usage/tools.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/docs/introduction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/introduction/showcase.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/docs/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/notebooks/agency_async.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/notebooks/azure.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20289 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/notebooks/genesis_agency.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/notebooks/web_browser_agent.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.345707 agency-swarm-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.321707 agency-swarm-0.1.7/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/tests/data/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/csv-test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   102408 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/generated_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-docx.docx
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-html.html
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-md.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-txt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/files/test-xml.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/tests/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/schemas/ga4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/schemas/get-headers-params.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/schemas/get-weather.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/schemas/relevance.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/tests/data/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/data/tools/ExampleTool1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:16:07.349707 agency-swarm-0.1.7/tests/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/demos/demo_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/demos/streaming_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/demos/term_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/test_agency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-11 10:16:03.000000 agency-swarm-0.1.7/tests/test_tool_factory.py
```

### Comparing `agency-swarm-0.1.6/.github/workflows/docs.yml` & `agency-swarm-0.1.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/.github/workflows/publish.yml` & `agency-swarm-0.1.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/.github/workflows/test.yml` & `agency-swarm-0.1.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/.gitignore` & `agency-swarm-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/CONTRIBUTING.md` & `agency-swarm-0.1.7/docs/contributing.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 # Contributing to Agency Swarm
-Each agent or tool you add to Agency Swarm will automatically be available for import by the Genesis Swarm, which will help us create an exponentially larger and smarter system.  
 
-This document provides guidelines for contributing new agents and tools to the framework.
+Each agent or tool you add to Agency Swarm will automatically be available for import by the Genesis Swarm, which will help us create an exponentially larger and smarter system.
 
-## Folder Structure for Tools
+This document provides guidelines for contributing new agents and tools to the framework.
 
-1. Tools should be added in the `agency_swarm/tools/{category}/` directory like below.
-2. Each tool should be in its specific category folder like `coding`, `browsing`, `investing` etc.
-3. Your tool file should be named `YourNewTool.py`.
-4. Tests should be added in `agency_swarm/tests/test_tools.py`.
+!!! warning "Will be updated soon"
+    The way we contribute agents and tools will be updated soon to load source files directly from the repository, rather than import them into the framework. This will allow you to have full control over all your agents and tools.
 
+### Folder Structure for Tools
+Tools should be added in the agency_swarm/tools/{category}/ directory like below.
+Each tool should be in its specific category folder like coding, browsing, investing etc.
 
+Your tool file should be named YourNewTool.py.
+Tests should be added in agency_swarm/tests/test_tools.py.
 Directory structure for a new tool:
-```
+
+```py
 agency_swarm/tools/your-tool-category/
 │
 ├── YourNewTool.py          # The main agent class file
 └── __init__.py             # Make sure to import your tool here
 ```
-
 ### Adding Tests For Your Tools
-For each tool, please add the following test case in `agency_swarm/tests/test_tools.py`:
-
-```python
+For each tool, please add the following test case in agency_swarm/tests/test_tools.py:
+```py
     def test_my_tool_example(self):
         output = MyCustomTool(query='John Doe').run()
         self.assertFalse("error" in output.lower())
 ```
+### Folder Structure for Agents
 
-## Folder Structure for Agents
-
-1. Agents should be placed in `agency_swarm/agents/{category}/` directory.
-2. Each agent should have its dedicated folder named `AgentName` like below.
-3. Make sure to use **CamelCase** for the agent name and the folder.
-
-```
+Agents should be placed in agency_swarm/agents/{category}/ directory.
+Each agent should have its dedicated folder named AgentName like below.
+Make sure to use CamelCase for the agent name and the folder.
+```python
 agency_swarm/agents/your-agent-category/AgentName/
 │
 ├── agency_manifesto.md or .txt # Agency's guiding principles (created if not exists)
 └── AgentName/                  # Directory for the specific agent
     ├── files/                  # Directory for files that will be uploaded to openai (if any)
     ├── schemas/                # Directory for OpenAPI schemas to be converted into tools (if any)
     ├── AgentName.py            # The main agent class file
     ├── __init__.py             # Initializes the agent folder as a Python package
     └── instructions.md         # Instruction document for the agent
 ```
-
 ### Creating an Agent
 
-1. Follow the structure below in your `AgentName.py` as a guideline. 
-2. All tools (except schemas) should be imported in `AgentName.py` from the `agency_swarm/tools/...` folder.
-
+Follow the structure below in your AgentName.py as a guideline.
+All tools (except schemas) should be imported in AgentName.py from the agency_swarm/tools/... folder.
 ```python
 from agency_swarm import Agent
 from agency_swarm.tools.example import ExampleTool
 
 class AgentName(Agent):
     def __init__(self, **kwargs):
         # Initialize tools in kwargs if not present
@@ -68,10 +65,9 @@
         
         # Add more kwargs as needed
 
         # Initialize the parent class
         super().__init__(**kwargs)
 ```
 
----
 
 Thank you for contributing to Agency Swarm! Your efforts help us build a more robust and versatile framework.
```

### Comparing `agency-swarm-0.1.6/LICENSE` & `agency-swarm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/PKG-INFO` & `agency-swarm-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency-swarm
-Version: 0.1.6
+Version: 0.1.7
 Summary: An open source agent orchestration framework built on top of the latest OpenAI Assistants API.
 Home-page: https://github.com/VRSEN/agency-swarm
 Author: VRSEN
 Author-email: VRSEN <arseny9795@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arsenii Shatokhin
@@ -144,31 +144,35 @@
                 description="Responsible for client communication, task planning and management.",
                 instructions="You must converse with other agents to ensure complete task execution.", # can be a file like ./instructions.md
                 files_folder="./files", # files to be uploaded to OpenAI
                 schemas_folder="./schemas", # OpenAPI schemas to be converted into tools
                 tools=[MyCustomTool, LangchainTool])
     ```
 
-    Import from existing agents (will be deprecated in future versions):
-    
-    ```python
-    from agency_swarm.agents.browsing import BrowsingAgent
-    
-    browsing_agent = BrowsingAgent()
-    
-    browsing_agent.instructions += "\n\nYou can add additional instructions here."
-    ```
+    Import from existing agents:
+
+   ```bash
+   agency-swarm import-agent --name "Devid" --destination "./"
+   ```
+   
+   This will import Devid (Software Developer) Agent locally, including all source code files, so you have full control over your system. Currently, available agents are: `Devid`, `BrowsingAgent`.
 
 
 
 4. **Define Agency Communication Flows**: 
 Establish how your agents will communicate with each other.
 
     ```python
     from agency_swarm import Agency
+    # if importing from local files
+    from Developer import Developer
+    from VirtualAssistant import VirtualAssistant
+   
+    dev = Developer()
+    va = VirtualAssistant()
     
     agency = Agency([
         ceo,  # CEO will be the entry point for communication with the user
         [ceo, dev],  # CEO can initiate communication with Developer
         [ceo, va],   # CEO can initiate communication with Virtual Assistant
         [dev, va]    # Developer can initiate communication with Virtual Assistant
     ], shared_instructions='agency_manifesto.md') # shared instructions for all agents
@@ -210,14 +214,26 @@
 ```
 
 Make sure to include:
 - Your mission and goals.
 - The agents you want to involve and their communication flows.
 - Which tools or APIs each agent should have access to, if any.
 
+## Importing Existing Agents
+
+This CLI command allows you to import existing agents from local files into your agency.
+
+#### **Command Syntax:**
+
+```bash
+agency-swarm import-agent --name "AgentName" --destination "/path/to/directory"
+```
+
+To check available agents, simply run this command without any arguments.
+
 ## Creating Agent Templates Locally
 
 This CLI command simplifies the process of creating a structured environment for each agent.
 
 #### **Command Syntax:**
 
 ```bash
```

### Comparing `agency-swarm-0.1.6/README.md` & `agency-swarm-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -100,31 +100,35 @@
                 description="Responsible for client communication, task planning and management.",
                 instructions="You must converse with other agents to ensure complete task execution.", # can be a file like ./instructions.md
                 files_folder="./files", # files to be uploaded to OpenAI
                 schemas_folder="./schemas", # OpenAPI schemas to be converted into tools
                 tools=[MyCustomTool, LangchainTool])
     ```
 
-    Import from existing agents (will be deprecated in future versions):
-    
-    ```python
-    from agency_swarm.agents.browsing import BrowsingAgent
-    
-    browsing_agent = BrowsingAgent()
-    
-    browsing_agent.instructions += "\n\nYou can add additional instructions here."
-    ```
+    Import from existing agents:
+
+   ```bash
+   agency-swarm import-agent --name "Devid" --destination "./"
+   ```
+   
+   This will import Devid (Software Developer) Agent locally, including all source code files, so you have full control over your system. Currently, available agents are: `Devid`, `BrowsingAgent`.
 
 
 
 4. **Define Agency Communication Flows**: 
 Establish how your agents will communicate with each other.
 
     ```python
     from agency_swarm import Agency
+    # if importing from local files
+    from Developer import Developer
+    from VirtualAssistant import VirtualAssistant
+   
+    dev = Developer()
+    va = VirtualAssistant()
     
     agency = Agency([
         ceo,  # CEO will be the entry point for communication with the user
         [ceo, dev],  # CEO can initiate communication with Developer
         [ceo, va],   # CEO can initiate communication with Virtual Assistant
         [dev, va]    # Developer can initiate communication with Virtual Assistant
     ], shared_instructions='agency_manifesto.md') # shared instructions for all agents
@@ -166,14 +170,26 @@
 ```
 
 Make sure to include:
 - Your mission and goals.
 - The agents you want to involve and their communication flows.
 - Which tools or APIs each agent should have access to, if any.
 
+## Importing Existing Agents
+
+This CLI command allows you to import existing agents from local files into your agency.
+
+#### **Command Syntax:**
+
+```bash
+agency-swarm import-agent --name "AgentName" --destination "/path/to/directory"
+```
+
+To check available agents, simply run this command without any arguments.
+
 ## Creating Agent Templates Locally
 
 This CLI command simplifies the process of creating a structured environment for each agent.
 
 #### **Command Syntax:**
 
 ```bash
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/agency.py` & `agency-swarm-0.1.7/agency_swarm/agency/agency.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import threading
 import uuid
 from enum import Enum
 from typing import List, TypedDict, Callable, Any, Dict, Literal, Union
 
 from openai.types.beta.threads import Message
 from openai.types.beta.threads.runs import RunStep
-from pydantic import Field, field_validator
+from pydantic import Field, field_validator, model_validator
 from rich.console import Console
 from typing_extensions import override
 
 from agency_swarm.agents import Agent
 from agency_swarm.messages import MessageOutput
 from agency_swarm.messages.message_output import MessageOutputLive
 from agency_swarm.threads import Thread
@@ -33,15 +33,15 @@
 class ThreadsCallbacks(TypedDict):
     load: Callable[[], Dict]
     save: Callable[[Dict], Any]
 
 
 class Agency:
     ThreadType = Thread
-    send_message_tool_description = """Use this tool to facilitate direct, synchronous communication between specialized agents within your agency. When you send a message using this tool, you receive a response exclusively from the designated recipient agent. To continue the dialogue, invoke this tool again with the desired recipient agent and your follow-up message. Remember, communication here is synchronous; the recipient agent won't perform any tasks post-response. You are responsible for relaying the recipient agent's responses back to the user, as the user does not have direct access to these replies. Keep engaging with the tool for continuous interaction until the task is fully resolved."""
+    send_message_tool_description = """Use this tool to facilitate direct, synchronous communication between specialized agents within your agency. When you send a message using this tool, you receive a response exclusively from the designated recipient agent. To continue the dialogue, invoke this tool again with the desired recipient agent and your follow-up message. Remember, communication here is synchronous; the recipient agent won't perform any tasks post-response. You are responsible for relaying the recipient agent's responses back to the user, as the user does not have direct access to these replies. Keep engaging with the tool for continuous interaction until the task is fully resolved. Do not send more than 1 message at a time."""
     send_message_tool_description_async = """Use this tool for asynchronous communication with other agents within your agency. Initiate tasks by messaging, and check status and responses later with the 'GetResponse' tool. Relay responses to the user, who instructs on status checks. Continue until task completion."""
 
     def __init__(self,
                  agency_chart: List,
                  shared_instructions: str = "",
                  shared_files: Union[str, List[str]] = None,
                  async_mode: Literal['threading'] = None,
@@ -69,15 +69,15 @@
 
         self.ceo = None
         self.user = User()
         self.agents = []
         self.agents_and_threads = {}
         self.main_recipients = []
         self.main_thread = None
-        self.recipient_agents = None # for autocomplete
+        self.recipient_agents = None  # for autocomplete
         self.shared_files = shared_files if shared_files else []
         self.settings_path = settings_path
         self.settings_callbacks = settings_callbacks
         self.threads_callbacks = threads_callbacks
 
         if os.path.isfile(os.path.join(self._get_class_folder_path(), shared_instructions)):
             self._read_instructions(os.path.join(self._get_class_folder_path(), shared_instructions))
@@ -87,76 +87,80 @@
             self.shared_instructions = shared_instructions
 
         self._parse_agency_chart(agency_chart)
         self._create_special_tools()
         self._init_agents()
         self._init_threads()
 
-    def get_completion(self, message: str, message_files=None, yield_messages=True, recipient_agent=None):
+    def get_completion(self, message: str, message_files=None, yield_messages=True, recipient_agent=None,
+                       additional_instructions=None):
         """
         Retrieves the completion for a given message from the main thread.
 
         Parameters:
             message (str): The message for which completion is to be retrieved.
             message_files (list, optional): A list of file ids to be sent as attachments with the message. Defaults to None.
             yield_messages (bool, optional): Flag to determine if intermediate messages should be yielded. Defaults to True.
             recipient_agent (Agent, optional): The agent to which the message should be sent. Defaults to the first agent in the agency chart.
-
+            additional_instructions (str, optional): Additional instructions to be sent with the message. Defaults to None.
         Returns:
             Generator or final response: Depending on the 'yield_messages' flag, this method returns either a generator yielding intermediate messages or the final response from the main thread.
         """
         gen = self.main_thread.get_completion(message=message, message_files=message_files,
-                                              yield_messages=yield_messages, recipient_agent=recipient_agent)
+                                              yield_messages=yield_messages, recipient_agent=recipient_agent,
+                                              additional_instructions=additional_instructions)
 
         if not yield_messages:
             while True:
                 try:
                     next(gen)
                 except StopIteration as e:
                     return e.value
 
         return gen
 
     def get_completion_stream(self, message: str, event_handler: type(AgencyEventHandler), message_files=None,
-                              recipient_agent=None):
+                              recipient_agent=None, additional_instructions: str = None):
         """
         Generates a stream of completions for a given message from the main thread.
 
         Parameters:
             message (str): The message for which completion is to be retrieved.
             event_handler (type(AgencyEventHandler)): The event handler class to handle the completion stream. https://github.com/openai/openai-python/blob/main/helpers.md
             message_files (list, optional): A list of file ids to be sent as attachments with the message. Defaults to None.
             recipient_agent (Agent, optional): The agent to which the message should be sent. Defaults to the first agent in the agency chart.
+            additional_instructions (str, optional): Additional instructions to be sent with the message. Defaults to None.
         Returns:
             Final response: Final response from the main thread.
         """
         if self.async_mode:
             raise Exception("Streaming is not supported in async mode.")
 
         if not inspect.isclass(event_handler):
             raise Exception("Event handler must not be an instance.")
 
         gen = self.main_thread.get_completion_stream(message=message, event_handler=event_handler,
-                                                     message_files=message_files, recipient_agent=recipient_agent)
+                                                     message_files=message_files, recipient_agent=recipient_agent,
+                                                     additional_instructions=additional_instructions)
 
         while True:
             try:
                 next(gen)
             except StopIteration as e:
                 event_handler.on_all_streams_end()
                 return e.value
 
-    def demo_gradio(self, height=450, dark_mode=True, share=False):
+    def demo_gradio(self, height=450, dark_mode=True, **kwargs):
         """
         Launches a Gradio-based demo interface for the agency chatbot.
 
         Parameters:
             height (int, optional): The height of the chatbot widget in the Gradio interface. Default is 600.
             dark_mode (bool, optional): Flag to determine if the interface should be displayed in dark mode. Default is True.
-            share (bool, optional): Flag to determine if the interface should be shared publicly. Default is False.
+            **kwargs: Additional keyword arguments to be passed to the Gradio interface.
         This method sets up and runs a Gradio interface, allowing users to interact with the agency's chatbot. It includes a text input for the user's messages and a chatbot interface for displaying the conversation. The method handles user input and chatbot responses, updating the interface dynamically.
         """
 
         try:
             import gradio as gr
         except ImportError:
             raise Exception("Please install gradio: pip install gradio")
@@ -239,67 +243,95 @@
             class GradioEventHandler(AgencyEventHandler):
                 message_output = None
 
                 @override
                 def on_message_created(self, message: Message) -> None:
                     if message.role == "user":
                         self.message_output = MessageOutput("text", self.agent_name, self.recipient_agent_name,
-                                                            "")
+                                                            message.content[0].text.value)
+
                     else:
-                        self.message_output = MessageOutput("text", self.recipient_agent_name, self.agent_name, "")
-                        chatbot_queue.put("[new_message]")
+                        self.message_output = MessageOutput("text", self.recipient_agent_name, self.agent_name,
+                                                            "")
 
-                    chatbot_queue.put(self.message_output.get_formatted_header() + "\n")
+                    chatbot_queue.put("[new_message]")
+                    chatbot_queue.put(self.message_output.get_formatted_content())
 
                 @override
                 def on_text_delta(self, delta, snapshot):
                     chatbot_queue.put(delta.value)
 
                 @override
                 def on_tool_call_created(self, tool_call):
-                    chatbot_queue.put("[new_message]")
-                    self.message_output = MessageOutput("function", self.recipient_agent_name, self.agent_name,
-                                                        str(tool_call.function))
-
-                    chatbot_queue.put(self.message_output.get_formatted_header() + "\n")
+                    # TODO: add support for code interpreter and retirieval tools
+                    if tool_call.type == "function":
+                        chatbot_queue.put("[new_message]")
+                        self.message_output = MessageOutput("function", self.recipient_agent_name, self.agent_name,
+                                                            str(tool_call.function))
+                        chatbot_queue.put(self.message_output.get_formatted_header() + "\n")
 
                 @override
                 def on_tool_call_done(self, snapshot):
+                    self.message_output = None
+
+                    # TODO: add support for code interpreter and retirieval tools
+                    if snapshot.type != "function":
+                        return
+
                     chatbot_queue.put(str(snapshot.function))
 
+                    if snapshot.function.name == "SendMessage":
+                        try:
+                            args = eval(snapshot.function.arguments)
+                            recipient = args["recipient"]
+                            self.message_output = MessageOutput("text", self.recipient_agent_name, recipient,
+                                                                    args["message"])
+
+                            chatbot_queue.put("[new_message]")
+                            chatbot_queue.put(self.message_output.get_formatted_content())
+                        except Exception as e:
+                            pass
+
+                    self.message_output = None
+
                 @override
                 def on_run_step_done(self, run_step: RunStep) -> None:
                     if run_step.type == "tool_calls":
                         for tool_call in run_step.step_details.tool_calls:
+                            if tool_call.type != "function":
+                                continue
+
                             if tool_call.function.name == "SendMessage":
                                 continue
 
                             self.message_output = None
                             chatbot_queue.put("[new_message]")
 
                             self.message_output = MessageOutput("function_output", tool_call.function.name,
                                                                 self.recipient_agent_name,
                                                                 tool_call.function.output)
 
                             chatbot_queue.put(self.message_output.get_formatted_header() + "\n")
                             chatbot_queue.put(tool_call.function.output)
+
                 @override
                 @classmethod
                 def on_all_streams_end(cls):
                     self.message_output = None
                     chatbot_queue.put("[end]")
 
             def bot(original_message, history):
                 nonlocal message_file_ids
                 nonlocal message_file_names
                 nonlocal recipient_agent
                 print("Message files: ", message_file_ids)
                 # Replace this with your actual chatbot logic
 
-                completion_thread = threading.Thread(target=self.get_completion_stream, args=(original_message, GradioEventHandler, message_file_ids, recipient_agent))
+                completion_thread = threading.Thread(target=self.get_completion_stream, args=(
+                original_message, GradioEventHandler, message_file_ids, recipient_agent))
                 completion_thread.start()
 
                 message_file_ids = []
                 message_file_names = []
 
                 new_message = True
                 while True:
@@ -337,15 +369,15 @@
                 bot, [msg, chatbot], [msg, chatbot]
             )
 
             # Enable queuing for streaming intermediate outputs
             demo.queue()
 
         # Launch the demo
-        demo.launch(share=share)
+        demo.launch(**kwargs)
         return demo
 
     def _recipient_agent_completer(self, text, state):
         """
         Autocomplete completer for recipient agent names.
         """
         options = [agent for agent in self.recipient_agents if agent.lower().startswith(text.lower())]
@@ -361,15 +393,16 @@
         try:
             import readline
         except ImportError:
             # Attempt to import pyreadline for Windows compatibility
             try:
                 import pyreadline as readline
             except ImportError:
-                print("Module 'readline' not found. Autocomplete will not work. If you are using Windows, try installing 'pyreadline3'.")
+                print(
+                    "Module 'readline' not found. Autocomplete will not work. If you are using Windows, try installing 'pyreadline3'.")
                 return
 
         if not readline:
             return
 
         try:
             readline.set_completer(self._recipient_agent_completer)
@@ -386,42 +419,66 @@
             message_output = None
 
             @override
             def on_message_created(self, message: Message) -> None:
                 if message.role == "user":
                     self.message_output = MessageOutputLive("text", self.agent_name, self.recipient_agent_name,
                                                             "")
+                    self.message_output.cprint_update(message.content[0].text.value)
                 else:
                     self.message_output = MessageOutputLive("text", self.recipient_agent_name, self.agent_name, "")
 
             @override
             def on_message_done(self, message: Message) -> None:
                 self.message_output = None
 
             @override
             def on_text_delta(self, delta, snapshot):
                 self.message_output.cprint_update(snapshot.value)
 
             @override
             def on_tool_call_created(self, tool_call):
-                self.message_output = MessageOutputLive("function", self.recipient_agent_name, self.agent_name,
+                # TODO: add support for code interpreter and retirieval tools
+
+                if tool_call.type == "function":
+                    self.message_output = MessageOutputLive("function", self.recipient_agent_name, self.agent_name,
                                                         str(tool_call.function))
 
             @override
             def on_tool_call_delta(self, delta, snapshot):
                 self.message_output.cprint_update(str(snapshot.function))
 
             @override
             def on_tool_call_done(self, snapshot):
                 self.message_output = None
 
+                # TODO: add support for code interpreter and retrieval tools
+                if snapshot.type != "function":
+                    return
+
+                if snapshot.function.name == "SendMessage":
+                    try:
+                        args = eval(snapshot.function.arguments)
+                        recipient = args["recipient"]
+                        self.message_output = MessageOutputLive("text", self.recipient_agent_name, recipient,
+                                                                "")
+
+                        self.message_output.cprint_update(args["message"])
+                    except Exception as e:
+                        pass
+
+                self.message_output = None
+
             @override
             def on_run_step_done(self, run_step: RunStep) -> None:
                 if run_step.type == "tool_calls":
                     for tool_call in run_step.step_details.tool_calls:
+                        if tool_call.type != "function":
+                            continue
+
                         if tool_call.function.name == "SendMessage":
                             continue
 
                         self.message_output = None
                         self.message_output = MessageOutputLive("function_output", tool_call.function.name,
                                                                 self.recipient_agent_name, tool_call.function.output)
                         self.message_output.cprint_update(tool_call.function.output)
@@ -445,15 +502,15 @@
 
             recipient_agent = None
             if "@" in text:
                 recipient_agent = text.split("@")[1].split(" ")[0]
                 text = text.replace(f"@{recipient_agent}", "").strip()
                 try:
                     recipient_agent = \
-                    [agent for agent in self.recipient_agents if agent.lower() == recipient_agent.lower()][0]
+                        [agent for agent in self.recipient_agents if agent.lower() == recipient_agent.lower()][0]
                     recipient_agent = self._get_agent_by_name(recipient_agent)
                 except Exception as e:
                     print(f"Recipient agent {recipient_agent} not found.")
                     continue
 
             self.get_completion_stream(message=text, event_handler=TermEventHandler, recipient_agent=recipient_agent)
 
@@ -695,50 +752,63 @@
                 continue
             agent_descriptions += recipient_agent.name + ": "
             agent_descriptions += recipient_agent.description + "\n"
 
         outer_self = self
 
         class SendMessage(BaseTool):
-            instructions: str = Field(...,
-                                      description="Please repeat your instructions step-by-step, including both completed "
+            my_primary_instructions: str = Field(...,
+                                      description="Please repeat your primary instructions step-by-step, including both completed "
                                                   "and the following next steps that you need to perfrom. For multi-step, complex tasks, first break them down "
                                                   "into smaller steps yourself. Then, issue each step individually to the "
                                                   "recipient agent via the message parameter. Each identified step should be "
                                                   "sent in separate message. Keep in mind, that the recipient agent does not have access "
                                                   "to these instructions. You must include recipient agent-specific instructions "
-                                                  "in the message parameter.")
+                                                  "in the message or additional_instructions parameters.")
             recipient: recipients = Field(..., description=agent_descriptions)
             message: str = Field(...,
                                  description="Specify the task required for the recipient agent to complete. Focus on "
                                              "clarifying what the task entails, rather than providing exact "
                                              "instructions.")
             message_files: List[str] = Field(default=None,
                                              description="A list of file ids to be sent as attachments to this message. Only use this if you have the file id that starts with 'file-'.",
                                              examples=["file-1234", "file-5678"])
+            additional_instructions: str = Field(default=None,
+                                                 description="Any additional instructions or clarifications that you would like to provide to the recipient agent.")
+            one_call_at_a_time: bool = True
+
+            @model_validator(mode='after')
+            def validate_files(self):
+                if "file-" in self.message or (self.additional_instructions and "file-" in self.additional_instructions):
+                    if not self.message_files:
+                        raise ValueError("You must include file ids in message_files parameter.")
 
             @field_validator('recipient')
             def check_recipient(cls, value):
                 if value.value not in recipient_names:
                     raise ValueError(f"Recipient {value} is not valid. Valid recipients are: {recipient_names}")
                 return value
 
             def run(self):
                 thread = outer_self.agents_and_threads[self.caller_agent.name][self.recipient.value]
 
                 if not outer_self.async_mode:
-                    gen = thread.get_completion(message=self.message, message_files=self.message_files,
-                                                event_handler=self.event_handler)
+                    gen = thread.get_completion(message=self.message,
+                                                message_files=self.message_files,
+                                                event_handler=self.event_handler,
+                                                additional_instructions=self.additional_instructions)
                     try:
                         while True:
                             yield next(gen)
                     except StopIteration as e:
                         message = e.value
                 else:
-                    message = thread.get_completion_async(message=self.message, message_files=self.message_files)
+                    message = thread.get_completion_async(message=self.message,
+                                                          message_files=self.message_files,
+                                                          additional_instructions=self.additional_instructions)
 
                 return message or ""
 
         SendMessage.caller_agent = agent
         if self.async_mode:
             SendMessage.__doc__ = self.send_message_tool_description_async
         else:
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/instructions.md` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/instructions.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,11 +2,12 @@
 
 You are an agent that creates other agents as instructed by the user. 
 
 The user will communicate to you each agent that needs to be created. Below are your instructions that needs to be followed for each agent communicated by the user.
 
 **Primary Instructions:**
 1. First, read the manifesto using `ReadManifesto` tool if you have not already done so. This file contains the agency manifesto that describes the agency's purpose and goals.
-2. Create a new agent using `CreateAgentTemplate` function. 
-3. Tell the ToolCreator or OpenAPICreator agent to create tools or APIs for this agent. Make sure to also communicate the agent description, name and a summary of the processes that it needs to perform. CEO Agents do not need to utilize any tools, so you can skip this and the following steps.
-4. If there are no issues and tools or APIs have been successfully created, notify the user that the agent has been created. Otherwise, try to resolve any issues with other agents before reporting back.
-5. Repeat this process for each agent that needs to be created.
+2. If a similar agent to the requested one is accessible through the `ImportAgent` tool, import this agent and inform the user that the agent has been created. Skip the following steps.
+3. If not, create a new agent using `CreateAgentTemplate` tool. 
+4. Tell the ToolCreator or OpenAPICreator agent to create tools or APIs for this agent. Make sure to also communicate the agent description, name and a summary of the processes that it needs to perform. CEO Agents do not need to utilize any tools, so you can skip this and the following steps.
+5. If there are no issues and tools or APIs have been successfully created, notify the user that the agent has been created. Otherwise, try to resolve any issues with the tool creator before reporting back to the user.
+6. Repeat this process for each agent that needs to be created, as instructed by the user.
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py`

 * *Files 15% similar despite different names*

```diff
@@ -65,14 +65,26 @@
 
         create_agent_template(self.agent_name,
                               self.agent_description,
                               instructions=self.instructions,
                               code_interpreter=True if "CodeInterpreter" in self.default_tools else None,
                               include_example_tool=False)
 
+        # # create or append to init file
+        path = self.shared_state.get("agency_path")
+        folder_name = self.agent_name.lower().replace(" ", "_")
+        class_name = self.agent_name.replace(" ", "").strip()
+        global_init_path = os.path.join(path, "__init__.py")
+        if not os.path.isfile(global_init_path):
+            with open(global_init_path, "w") as f:
+                f.write(f"from .{folder_name} import {class_name}")
+        else:
+            with open(global_init_path, "a") as f:
+                f.write(f"\nfrom .{folder_name} import {class_name}")
+
         # add agent on second line to agency.py
         with open("agency.py", "r") as f:
             lines = f.readlines()
             lines.insert(1, f"from {self.agent_name} import {self.agent_name}\n")
 
         with open("agency.py", "w") as f:
             f.writelines(lines)
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/instructions.md` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/instructions.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GenesisCEO Agent Instructions
 
 As a Genesis CEO Agent within the Agency Swarm framework, your mission is to help users define the structure of their agency and create the initial agents.
 
-1. Pick a name for the agency, determine its goals and mission, Ask the user for any clarification if needed.
-2. Propose an initial structure for the agency, including the roles of the agents, their communication flows and what APIs or Tools each agent can use, if specified by the user. Focus on creating at most 2 agents, plus CEO, unless instructed otherwise by the user. Output the code snippet like below. Adjust it accordingly, based on user's input.
+1. Pick a name for the agency, determine its goals and mission. Ask the user for any clarification if needed.
+2. Propose an initial structure for the agency, including the roles of the agents, their communication flows and what APIs or Tools each agent can use, if specified by the user. Focus on creating at most 2 agents, plus CEO, unless instructed otherwise by the user. Do not name the CEO agent GenesisCEO. It's name must be tailored for the purpose of the agency. Output the code snippet like below. Adjust it accordingly, based on user's input.
 3. Upon confirmation of the agency structure, use `CreateAgencyFolder` tool to create a folder for the agency. If any modifications are required please use this tool again with the same agency name and it will overwrite the existing folder.
 4. Tell AgentCreator to create these agents one by one, starting with the CEO. Each agent should be sent in a separate message using the `SendMessage` tool. Please make sure to include the agent description, summary of the processes it needs to perform and the APIs or Tools that it can use via the message parameter.
 5. Once all agents are created, please use the `FinalizeAgency` tool, and tell the user that he can now navigate to the agency folder and start it with `python agency.py` command.
 
 
 ### Example of communication flows
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/CreateAgencyFolder.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,20 +15,20 @@
     """
     agency_name: str = Field(
         ..., description="Name of the agency to be created. Must not contain spaces or special characters.",
         examples=["AgencyName", "MyAgency", "ExampleAgency"]
     )
     agency_chart: str = Field(
         ..., description="Agency chart to be passed into the Agency class.",
-        examples=["[ceo, [ceo, dev], [ceo, va], [dev, va] ]"]
+        examples=["[ceo, [ceo, dev], [ceo, va], [dev, va]]"]
     )
     manifesto: str = Field(
         ..., description="Manifesto for the agency, describing its goals and additional context shared by all agents "
                          "in markdown format. It must include information about the working environment, the mission "
-                         "and the goals of the agency.",
+                         "and the goals of the agency. Do not add descriptions of the agents themselves or the agency structure.",
     )
 
     def run(self):
         if not self.shared_state.get("default_folder"):
             self.shared_state.set('default_folder', Path.cwd())
 
         if self.shared_state.get("agency_name") is None:
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/FinalizeAgency.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,26 @@
 from agency_swarm.util import create_agent_template
 
 
 class FinalizeAgency(BaseTool):
     """
     This tool finalizes the agency structure and it's imports. Please make sure to use at only at the very end, after all agents have been created.
     """
+    agency_path: str = Field(
+        None, description="Path to the agency folder. Defaults to the agency currently being created."
+    )
 
     def run(self):
-        os.chdir(self.shared_state.get("agency_path"))
+        agency_path = None
+        if self.shared_state.get("agency_path"):
+            os.chdir(self.shared_state.get("agency_path"))
+            agency_path = self.shared_state.get("agency_path")
+        else:
+            os.chdir(self.agency_path)
+            agency_path = self.agency_path
 
         client = get_openai_client()
 
         # read agency.py
         with open("./agency.py", "r") as f:
             agency_py = f.read()
             f.close()
@@ -33,20 +42,20 @@
         message = res.choices[0].message.content
 
         # write agency.py
         with open("./agency.py", "w") as f:
             f.write(message)
             f.close()
 
-        return "Successfully finalized agency structure. You can now instruct the user to run the agency.py file."
+        return f"Successfully finalized {agency_path} structure. You can now instruct the user to run the agency.py file."
 
     @model_validator(mode="after")
     def validate_agency_path(self):
-        if not self.shared_state.get("agency_path"):
-            raise ValueError("Agency path not found. Please use CreateAgencyFolder tool to create the agency folder first.")
+        if not self.shared_state.get("agency_path") and not self.agency_path:
+            raise ValueError("Agency path not found. Please specify the agency_path. Ask user for clarification if needed.")
 
 
 SYSTEM_PROMPT = """"Please read the file provided by the user and fix all the imports and indentation accordingly. 
 
 Only output the full valid python code and nothing else."""
 
 example_input = """
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/GenesisCEO/tools/ReadRequirements.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/OpenAPICreator/instructions.md` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/OpenAPICreator/tools/CreateToolsFromOpenAPISpec.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/instructions.md` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/instructions.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 from agency_swarm.agency.genesis.util import check_agency_path, check_agent_path
 from agency_swarm.tools import BaseTool
 from pydantic import Field, model_validator
 import importlib
 
-from agency_swarm.util.create_agent_template import example_tool_template
+from agency_swarm.util.cli.create_agent_template import example_tool_template
 
 
 class CreateTool(BaseTool):
     """
     This tool creates tools for the agent.
     """
     agent_name: str = Field(
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/manifesto.md` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/manifesto.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agency/genesis/util.py` & `agency-swarm-0.1.7/agency_swarm/agency/genesis/util.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/agent.py` & `agency-swarm-0.1.7/agency_swarm/agents/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import json
 import os
 from typing import Dict, Union, Any, Type
 from typing import List
 
 from deepdiff import DeepDiff
+from openai import NotFoundError
 
 from agency_swarm.tools import BaseTool, ToolFactory
 from agency_swarm.tools import Retrieval, CodeInterpreter
 from agency_swarm.util.oai import get_openai_client
 from agency_swarm.util.openapi import validate_openapi_spec
 
 
@@ -23,29 +24,43 @@
     def assistant(self, value):
         self._assistant = value
 
     @property
     def functions(self):
         return [tool for tool in self.tools if issubclass(tool, BaseTool)]
 
+    def response_validator(self, message: str) -> str:
+        """
+        Validates the response from the agent. If the response is invalid, it must raise an exception with instructions
+        for the caller agent on how to proceed.
+
+        Parameters:
+            message (str): The response from the agent.
+
+        Returns:
+            str: The validated response.
+        """
+        return message
+
     def __init__(
             self,
             id: str = None,
             name: str = None,
             description: str = None,
             instructions: str = "",
             tools: List[Union[Type[BaseTool], Type[Retrieval], Type[CodeInterpreter]]] = None,
             tools_folder: str = None,
             files_folder: Union[List[str], str] = None,
             schemas_folder: Union[List[str], str] = None,
             api_headers: Dict[str, Dict[str, str]] = None,
             api_params: Dict[str, Dict[str, str]] = None,
             file_ids: List[str] = None,
             metadata: Dict[str, str] = None,
-            model: str = "gpt-4-turbo-preview"
+            model: str = "gpt-4-turbo-preview",
+            validation_attempts: int = 1,
     ):
         """
         Initializes an Agent with specified attributes, tools, and OpenAI client.
 
         Parameters:
             id (str, optional): Loads the assistant from OpenAI assistant ID. Assistant will be created or loaded from settings if ID is not provided. Defaults to None.
             name (str, optional): Name of the agent. Defaults to the class name if not provided.
@@ -56,14 +71,15 @@
             files_folder (Union[List[str], str], optional): Path or list of paths to directories containing files associated with the agent. Defaults to None.
             schemas_folder (Union[List[str], str], optional): Path or list of paths to directories containing OpenAPI schemas associated with the agent. Defaults to None.
             api_headers (Dict[str,Dict[str, str]], optional): Headers to be used for the openapi requests. Each key must be a full filename from schemas_folder. Defaults to an empty dictionary.
             api_params (Dict[str, Dict[str, str]], optional): Extra params to be used for the openapi requests. Each key must be a full filename from schemas_folder. Defaults to an empty dictionary.
             file_ids (List[str], optional): List of file IDs for files associated with the agent. Defaults to an empty list.
             metadata (Dict[str, str], optional): Metadata associated with the agent. Defaults to an empty dictionary.
             model (str, optional): The model identifier for the OpenAI API. Defaults to "gpt-4-turbo-preview".
+            validation_attempts (int, optional): Number of attempts to validate the response with response_validator function. Defaults to 1.
 
         This constructor sets up the agent with its unique properties, initializes the OpenAI client, reads instructions if provided, and uploads any associated files.
         """
         # public attributes
         self.id = id
         self.name = name if name else self.__class__.__name__
         self.description = description
@@ -74,34 +90,28 @@
         self.files_folder = files_folder if files_folder else []
         self.schemas_folder = schemas_folder if schemas_folder else []
         self.api_headers = api_headers if api_headers else {}
         self.api_params = api_params if api_params else {}
         self.file_ids = file_ids if file_ids else []
         self.metadata = metadata if metadata else {}
         self.model = model
+        self.validation_attempts = validation_attempts
 
         self.settings_path = './settings.json'
 
         # private attributes
         self._assistant: Any = None
         self._shared_instructions = None
 
         # init methods
         self.client = get_openai_client()
         self._read_instructions()
 
         # upload files
-        prev_timeout = None
-        if isinstance(self.client.timeout, int) or isinstance(self.client.timeout, float):
-            # default timeout is too low for file large file uploads
-            prev_timeout = self.client.timeout
-            self.client.timeout = 120 if prev_timeout < 120 else prev_timeout
         self._upload_files()
-        if prev_timeout:
-            self.client.timeout = prev_timeout
 
         self._parse_schemas()
         self._parse_tools_folder()
 
     # --- OpenAI Assistant Methods ---
 
     def init_oai(self):
@@ -134,22 +144,25 @@
         # load assistant from settings
         if os.path.exists(path):
             with open(path, 'r') as f:
                 settings = json.load(f)
                 # iterate settings and find the assistant with the same name
                 for assistant_settings in settings:
                     if assistant_settings['name'] == self.name:
-                        self.assistant = self.client.beta.assistants.retrieve(assistant_settings['id'])
-                        self.id = assistant_settings['id']
-                        # update assistant if parameters are different
-                        if not self._check_parameters(self.assistant.model_dump()):
-                            print("Updating assistant... " + self.name)
-                            self._update_assistant()
-                        self._update_settings()
-                        return self
+                        try:
+                            self.assistant = self.client.beta.assistants.retrieve(assistant_settings['id'])
+                            self.id = assistant_settings['id']
+                            # update assistant if parameters are different
+                            if not self._check_parameters(self.assistant.model_dump()):
+                                print("Updating assistant... " + self.name)
+                                self._update_assistant()
+                            self._update_settings()
+                            return self
+                        except NotFoundError:
+                            continue
 
         # create assistant if settings.json does not exist or assistant with the same name does not exist
         self.assistant = self.client.beta.assistants.create(
             name=self.name,
             description=self.description,
             instructions=self.instructions,
             tools=self.get_oai_tools(),
@@ -234,20 +247,22 @@
                         file_id = get_id_from_file(f_path)
                         if file_id:
                             print("File already uploaded. Skipping... " + os.path.basename(f_path))
                             self.file_ids.append(file_id)
                         else:
                             print("Uploading new file... " + os.path.basename(f_path))
                             with open(f_path, 'rb') as f:
-                                file_id = self.client.files.create(file=f, purpose="assistants").id
+                                file_id = self.client.with_options(
+                                    timeout=80 * 1000,
+                                ).files.create(file=f, purpose="assistants").id
                                 self.file_ids.append(file_id)
                                 f.close()
                             add_id_to_file(f_path, file_id)
                 else:
-                    print("Files folder path is not a directory. Skipping... ", f_path)
+                    print(f"Files folder '{f_path}' is not a directory. Skipping...", )
             else:
                 print("Files folder path must be a string or list of strings. Skipping... ", files_folder)
 
         if Retrieval not in self.tools and CodeInterpreter not in self.tools and self.file_ids:
             print("Detected files without Retrieval. Adding Retrieval tool...")
             self.add_tool(Retrieval)
 
@@ -341,30 +356,32 @@
                     print("Schemas folder path is not a directory. Skipping... ", f_path)
             else:
                 print("Schemas folder path must be a string or list of strings. Skipping... ", schemas_folder)
 
     def _parse_tools_folder(self):
         if not self.tools_folder:
             return
+
         if not os.path.isdir(self.tools_folder):
             self.tools_folder = os.path.join(self.get_class_folder_path(), self.tools_folder)
             self.tools_folder = os.path.normpath(self.tools_folder)
+
         if os.path.isdir(self.tools_folder):
             f_paths = os.listdir(self.tools_folder)
             f_paths = [f for f in f_paths if not f.startswith(".") and not f.startswith("__")]
             f_paths = [os.path.join(self.tools_folder, f) for f in f_paths]
             for f_path in f_paths:
                 if not f_path.endswith(".py"):
                     continue
                 if os.path.isfile(f_path):
                     try:
                         tool = ToolFactory.from_file(f_path)
                         self.add_tool(tool)
                     except Exception as e:
-                        print("Error parsing tool. Skipping... " + os.path.basename(f_path))
+                        print(f"Error parsing tool file {os.path.basename(f_path)}: {e}. Skipping...")
                 else:
                     print("Items in tools folder must be files. Skipping... ", f_path)
         else:
             print("Tools folder path is not a directory. Skipping... ", self.tools_folder)
 
     def get_openapi_schema(self, url):
         """Get openapi schema that contains all tools from the agent as different api paths. Make sure to call this after agency has been initialized."""
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/AnalyzeContent.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/ClickElement.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ClickElement.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/ExportFile.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ExportFile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import base64
 import os
 
-from agency_swarm import BaseTool, get_openai_client
+from agency_swarm.tools import BaseTool
 from .util import get_web_driver
 
 
 class ExportFile(BaseTool):
     """This tool converts the current full web page into a file and returns its file_id. You can then analyze this file using the myfiles_browser tool."""
 
     def run(self):
         wd = get_web_driver()
-
+        from agency_swarm import get_openai_client
         client = get_openai_client()
 
         # Define the parameters for the PDF
         params = {
             'landscape': False,
             'displayHeaderFooter': False,
             'printBackground': True,
@@ -23,19 +23,33 @@
 
         # Execute the command to print to PDF
         result = wd.execute_cdp_cmd('Page.printToPDF', params)
         pdf = result['data']
 
         pdf_bytes = base64.b64decode(pdf)
 
-        file_id = client.files.create(file=pdf_bytes, purpose="assistants").id
+        # Save the PDF to a file
+        with open("exported_file.pdf", "wb") as f:
+            f.write(pdf_bytes)
+
+        file_id = client.files.create(file=open("exported_file.pdf", "rb"), purpose="assistants",).id
 
         # update caller agent assistant
         self.caller_agent.file_ids.append(file_id)
 
         client.beta.assistants.update(
             assistant_id=self.caller_agent.id,
             file_ids=self.caller_agent.file_ids
         )
 
-        return ("Success. File exported with id: " + file_id +
-                " You can now use myfiles_browser tool to analyze the contents of this webpage.")
+        self.shared_state.set("file_id", file_id)
+
+        return ("Success. File exported with id: `" + file_id +
+                "` You can now use myfiles_browser tool to analyze the contents of this webpage " +
+                "or send this file id back to the user.")
+
+
+if __name__ == "__main__":
+    wd = get_web_driver()
+    wd.get("https://www.google.com")
+    tool = ExportFile()
+    tool.run()
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/ReadURL.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/ReadURL.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,23 @@
     """
 This tool reads a single URL and opens it in your current browser window. For each new source, go to a direct URL
 that you think might contain the answer to the user's question or perform a google search like
 'https://google.com/search?q=search' if applicable. Otherwise, don't try to guess the direct url, use ClickElement tool
 to click on the link that you think might contain the desired information on the current web page.
 Remember, this tool only supports opening 1 URL at a time. Previous URL will be closed when you open a new one.
     """
+    chain_of_thought: str = Field(
+        ..., description="Think step-by-step about where you need to navigate next to find the necessary information.",
+        exclude=True
+    )
     url: str = Field(
         ..., description="URL of the webpage.", examples=["https://google.com/search?q=search"]
     )
+    one_call_at_a_time: bool = True
+
 
     def run(self):
         wd = get_web_driver()
 
         wd.get(self.url)
 
         time.sleep(2)
@@ -39,7 +45,11 @@
 
         wd.execute_script(js_script)
 
         set_web_driver(wd)
 
         return "Current URL is: " + wd.current_url + "\n"
 
+
+if __name__ == "__main__":
+    tool = ReadURL(url="https://google.com")
+    print(tool.run())
```

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/Scroll.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/Scroll.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/SelectDropdown.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/SendKeys.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SendKeys.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/SolveCaptcha.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/agents/browsing/tools/util/highlights.py` & `agency-swarm-0.1.7/agency_swarm/agents/BrowsingAgent/tools/util/highlights.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/cli.py` & `agency-swarm-0.1.7/agency_swarm/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import argparse
 import os
+from dotenv import load_dotenv
+from agency_swarm.util.helpers import list_available_agents
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Create agent template.')
+    parser = argparse.ArgumentParser(description='Agency Swarm CLI.')
 
-    subparsers = parser.add_subparsers(dest='command', help='Create agent template.')
+    subparsers = parser.add_subparsers(dest='command', help='Utility commands to simplify the agent creation process.')
     subparsers.required = True
 
     # create-agent-template
     create_parser = subparsers.add_parser('create-agent-template', help='Create agent template folder locally.')
     create_parser.add_argument('--path', type=str, default="./", help='Path to create agent folder.')
     create_parser.add_argument('--use_txt', action='store_true', default=False,
                                help='Use txt instead of md for instructions and manifesto.')
@@ -18,29 +20,39 @@
 
     # genesis-agency
     genesis_parser = subparsers.add_parser('genesis', help='Start genesis agency.')
     genesis_parser.add_argument('--openai_key', default=None, type=str, help='OpenAI API key.')
     genesis_parser.add_argument('--with_browsing', default=False, action='store_true',
                                 help='Enable browsing agent.')
 
+    # import-agent
+    import_parser = subparsers.add_parser('import-agent', help='Import pre-made agent by name to a local directory.')
+    available_agents = list_available_agents()
+    import_parser.add_argument('--name', type=str, required=True, choices=available_agents, help='Name of the agent to import.')
+    import_parser.add_argument('--destination', type=str, default="./", help='Destination path to copy the agent files.')
+
     args = parser.parse_args()
 
     if args.command == "create-agent-template":
         from agency_swarm.util import create_agent_template
         create_agent_template(args.name, args.description, args.path, args.use_txt)
     elif args.command == "genesis":
+        load_dotenv()
         if not os.getenv('OPENAI_API_KEY') and not args.openai_key:
             print("OpenAI API key not set. "
                   "Please set it with --openai_key argument or by setting OPENAI_API_KEY environment variable.")
             return
 
         if args.openai_key:
             from agency_swarm import set_openai_key
             set_openai_key(args.openai_key)
 
         from agency_swarm.agency.genesis import GenesisAgency
         agency = GenesisAgency(with_browsing=args.with_browsing)
         agency.run_demo()
+    elif args.command == "import-agent":
+        from agency_swarm.util import import_agent
+        import_agent(args.name, args.destination)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `agency-swarm-0.1.6/agency_swarm/messages/message_output.py` & `agency-swarm-0.1.7/agency_swarm/messages/message_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 
     @property
     def formatted_header(self):
         return self.get_formatted_header()
 
     def get_formatted_header(self):
         if self.msg_type == "function":
-            text = f"{self.sender_name} 🛠️ Executing Function"
+            text = f"{self.sender_emoji} {self.sender_name} 🛠️ Executing Function"
             return text
 
         if self.msg_type == "function_output":
             text = f"{self.sender_name} ⚙️ Function Output"
             return text
 
-        text = f"{self.sender_name} 🗣️ @{self.receiver_name}"
+        text = f"{self.sender_emoji} {self.sender_name} 🗣️ @{self.receiver_name}"
 
         return text
 
     def get_formatted_content(self):
         header = self.get_formatted_header()
         content = f"\n{self.content}\n"
         return header + content
@@ -100,30 +100,30 @@
 class MessageOutputLive(MessageOutput):
     live_display = None
 
     def __init__(self, msg_type: Literal["function", "function_output", "text", "system"], sender_name: str,
                  receiver_name: str, content):
         super().__init__(msg_type, sender_name, receiver_name, content)
         # Initialize Live display if not already done
-        self.live_display = Live()
+        self.live_display = Live(vertical_overflow="visible")
         self.live_display.start()
 
         console.rule()
 
     def __del__(self):
         self.live_display.stop()
         self.live_display = None
 
     def cprint_update(self, snapshot):
         """
         Update the display with new snapshot content.
         """
         self.content = snapshot  # Update content with the latest snapshot
 
-        header_text = self.sender_emoji + " " + self.formatted_header
+        header_text = self.formatted_header
         md_content = Markdown(self.content)
 
         # Creating a group of renderables for the live display
         render_group = Group(header_text, md_content)
 
         # Update the Live display
         self.live_display.update(render_group)
```

### Comparing `agency-swarm-0.1.6/agency_swarm/threads/thread_async.py` & `agency-swarm-0.1.7/agency_swarm/threads/thread_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,41 +8,43 @@
 
 class ThreadAsync(Thread):
     def __init__(self, agent: Literal[Agent, User], recipient_agent: Agent):
         super().__init__(agent, recipient_agent)
         self.pythread = None
         self.response = None
 
-    def worker(self, message: str, message_files=None):
-        gen = super().get_completion(message=message, message_files=message_files,
-                                  yield_messages=False) # yielding is not supported in async mode
+    def worker(self, message: str, message_files=None, additional_instructions: str = None):
+        gen = super().get_completion(message=message,
+                                     message_files=message_files,
+                                     yield_messages=False,  # yielding is not supported in async mode
+                                     additional_instructions=additional_instructions)
         while True:
             try:
                 next(gen)
             except StopIteration as e:
                 self.response = f"""{self.recipient_agent.name}'s Response: '{e.value}'"""
                 break
 
         return
 
-    def get_completion_async(self, message: str, message_files=None):
+    def get_completion_async(self, message: str, message_files=None, additional_instructions: str = None):
         if self.pythread and self.pythread.is_alive():
             return "System Notification: 'Agent is busy, so your message was not received. Please always use 'GetResponse' tool to check for status first, before using 'SendMessage' tool again for the same agent.'"
         elif self.pythread and not self.pythread.is_alive():
             self.pythread.join()
             self.pythread = None
             self.response = None
 
         run = self.get_last_run()
 
         if run and run.status in ['queued', 'in_progress', 'requires_action']:
             return "System Notification: 'Agent is busy, so your message was not received. Please always use 'GetResponse' tool to check for status first, before using 'SendMessage' tool again for the same agent.'"
 
         self.pythread = threading.Thread(target=self.worker,
-                                         args=(message, message_files))
+                                         args=(message, message_files, additional_instructions))
 
         self.pythread.start()
 
         return "System Notification: 'Task has started. Please notify the user that they can tell you to check the status later. You can do this with the 'GetResponse' tool, after you have been instructed to do so. Don't mention the tool itself to the user. "
 
     def check_status(self, run=None):
         if not run:
@@ -75,8 +77,8 @@
         )
 
         if len(runs.data) == 0:
             return None
 
         run = runs.data[0]
 
-        return run
+        return run
```

### Comparing `agency-swarm-0.1.6/agency_swarm/tools/BaseTool.py` & `agency-swarm-0.1.7/agency_swarm/tools/BaseTool.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         return self.data.get(key, default)
 
 
 class BaseTool(OpenAISchema, ABC):
     shared_state: ClassVar[SharedState] = SharedState()
     caller_agent: Any = None
     event_handler: Any = None
+    one_call_at_a_time: bool = False
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         # # Exclude 'run' method from Pydantic model fields
         # self.model_fields.pop("run", None)
 
     @classmethod
@@ -36,21 +37,24 @@
         schema = super(BaseTool, cls).openai_schema
 
         properties = schema.get("parameters", {}).get("properties", {})
 
         properties.pop("caller_agent", None)
         properties.pop("shared_state", None)
         properties.pop("event_handler", None)
+        properties.pop("one_call_at_a_time", None)
 
         required = schema.get("parameters", {}).get("required", [])
         if "caller_agent" in required:
             required.remove("caller_agent")
         if "shared_state" in required:
             required.remove("shared_state")
         if "event_handler" in required:
             required.remove("event_handler")
+        if "one_call_at_a_time" in required:
+            required.remove("one_call_at_a_time")
 
         return schema
 
     @abstractmethod
     def run(self, **kwargs):
         pass
```

### Comparing `agency-swarm-0.1.6/agency_swarm/tools/ToolFactory.py` & `agency-swarm-0.1.7/agency_swarm/tools/ToolFactory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib.util
 import inspect
 import json
 import os
 import sys
+from importlib import import_module
 from typing import Any, Dict, List, Type, Union
 
 import jsonref
 from jsonref import requests
 from pydantic import create_model, Field
 
 from .BaseTool import BaseTool
@@ -281,41 +282,40 @@
 
                 tools.append(ToolFactory.from_openai_schema(function, callback))
 
         return tools
 
     @staticmethod
     def from_file(file_path: str) -> Type[BaseTool]:
-        """Dynamically imports a BaseTool from a Python file. The file must be named the same as the class.
+        """Dynamically imports a BaseTool class from a Python file within a package structure.
 
         Parameters:
             file_path: The file path to the Python file containing the BaseTool class.
 
         Returns:
-            The BaseTool class from the given file path.
-
+            The imported BaseTool class.
         """
-        # Extract class name from file path (assuming class name matches file name without .py extension)
-        class_name = os.path.basename(file_path)
-        if class_name.endswith('.py'):
-            class_name = class_name[:-3]  # Remove .py extension
-
-        # Load the module from the given file path
-        spec = importlib.util.spec_from_file_location(class_name, file_path)
-        module = importlib.util.module_from_spec(spec)
-        sys.modules[class_name] = module
-        spec.loader.exec_module(module)
-
-        # Dynamically access the class based on the extracted class name
-        if hasattr(module, class_name):
-            tool = getattr(module, class_name)
-        else:
-            raise AttributeError(f"The class {class_name} was not found in {file_path}")
+        file_path = os.path.relpath(file_path)
+        # Normalize the file path to be absolute and extract components
+        directory, file_name = os.path.split(file_path)
+        import_path = os.path.splitext(file_path)[0].replace(os.sep, ".")
+        class_name = os.path.splitext(file_name)[0]
+
+        exec_globals = globals()
+        exec(f"from {import_path} import {class_name}", exec_globals)
+
+        imported_class = exec_globals.get(class_name)
+        if not imported_class:
+            raise ImportError(f"Could not import {class_name} from {import_path}")
+
+        # Check if the imported class is a subclass of BaseTool
+        if not issubclass(imported_class, BaseTool):
+            raise TypeError(f"Class {class_name} must be a subclass of BaseTool")
 
-        return tool
+        return imported_class
 
     @staticmethod
     def get_openapi_schema(tools: List[Type[BaseTool]], url: str, title="Agent Tools",
                            description="A collection of tools.") -> str:
         """
         Generates an OpenAPI schema from a list of BaseTools.
```

### Comparing `agency-swarm-0.1.6/agency_swarm/tools/coding/ChangeLines.py` & `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/ChangeFile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 import os
+from enum import Enum
 from typing import Literal, Optional, List
 
 from instructor import OpenAISchema
 from pydantic import Field, model_validator, field_validator
 
 from agency_swarm import BaseTool
 
-
 class LineChange(OpenAISchema):
     """
     Line changes to be made.
     """
     line_number: int = Field(
         ..., description="Line number to change.",
         examples=[1, 2, 3]
     )
     new_line: Optional[str] = Field(
-        ..., description="New line to replace the old line. Not required only for delete mode.",
+        None, description="New line to replace the old line. Not required only for delete mode.",
         examples=["This is a new line"]
     )
     mode: Literal["replace", "insert", "delete"] = Field(
-        "replace", description='Mode to use for the line change. "replace" replaces the line with the new line, '
-                               '"insert" inserts the new line at the specified line number, and "delete" deletes the '
-                               "specified line number.",
+        "replace", description='Mode to use for the line change. "replace" replaces the line with the new line. '
+                               '"insert" inserts the new line at the specified line number, moving the previous line down.'
+                               ' "delete" deletes the specified line number.',
     )
 
     @model_validator(mode='after')
     def validate_new_line(self):
-        if self.mode == "delete":
-            if "new_line" in self:
-                raise ValueError("new_line should not be specified for delete mode.")
-        else:
-            if not self.new_line:
-                raise ValueError("new_line should be specified for replace and insert modes.")
-
+        mode, new_line = self.mode, self.new_line
+        if mode == "delete" and new_line is not None:
+            raise ValueError("new_line should not be specified for delete mode.")
+        elif mode in ["replace", "insert"] and new_line is None:
+            raise ValueError("new_line should be specified for replace and insert modes.")
         return self
 
 
-class ChangeLines(BaseTool):
+class ChangeFile(BaseTool):
     """
-    This tool changes specified lines in a file. Returns the new file contents.
+    This tool changes specified lines in a file. Returns the new file contents with line numbers at the start of each line.
     """
+    chain_of_thought: str = Field(
+        ..., description="Please think step-by-step about the required changes to the file in order to construct a fully functioning and correct program according to the requirements.",
+        exclude=True,
+    )
     file_path: str = Field(
         ..., description="Path to the file with extension.",
         examples=["./file.txt", "./file.json", "../../file.py"]
     )
     changes: List[LineChange] = Field(
         ..., description="Line changes to be made to the file.",
-        examples=[LineChange(line_number=1, new_line="This is a new line").model_dump()]
+        examples=[{"line_number": 1, "new_line": "This is a new line", "mode": "replace"}]
     )
 
     def run(self):
         # read file
         with open(self.file_path, "r") as f:
             file_contents = f.readlines()
 
-        # make changes
-        for change in self.changes:
-            if change.mode == "replace":
-                file_contents[change.line_number - 1] = change.new_line
-            elif change.mode == "insert":
-                file_contents.insert(change.line_number - 1, change.new_line)
-            elif change.mode == "delete":
-                file_contents.pop(change.line_number - 1)
+            # Process changes in a way that accounts for modifications affecting line numbers
+            for change in sorted(self.changes, key=lambda x: x.line_number, reverse=True):
+                try:
+                    if change.mode == "replace" and 0 < change.line_number <= len(file_contents):
+                        file_contents[change.line_number - 1] = change.new_line + '\n'
+                    elif change.mode == "insert":
+                        file_contents.insert(change.line_number - 1, change.new_line + '\n')
+                    elif change.mode == "delete" and 0 < change.line_number <= len(file_contents):
+                        file_contents.pop(change.line_number - 1)
+                except IndexError:
+                    return f"Error: Line number {change.line_number} is out of the file's range."
 
         # write file
         with open(self.file_path, "w") as f:
             f.writelines(file_contents)
 
+        with open(self.file_path, "r") as f:
+            file_contents = f.readlines()
+
         # return file contents with line numbers
         return "\n".join([f"{i + 1}. {line}" for i, line in enumerate(file_contents)])
 
     # use field validation to ensure that the file path is valid
     @field_validator("file_path", mode='after')
     @classmethod
     def validate_file_path(cls, v: str):
         if not os.path.exists(v):
             raise ValueError("File path does not exist.")
 
-        return v
+        return v
```

### Comparing `agency-swarm-0.1.6/agency_swarm/tools/coding/WriteFiles.py` & `agency-swarm-0.1.7/agency_swarm/agents/Devid/tools/DirectoryNavigator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import os
-from typing import List
+from pydantic import Field, model_validator, field_validator
 
-from pydantic import Field
+from agency_swarm.tools import BaseTool
 
-from agency_swarm import BaseTool
 
-
-class File(BaseTool):
-    """
-    File to be written to the disk with an appropriate name and file path, containing code that can be saved and executed locally at a later time.
-    """
-    file_name: str = Field(
-        ...,
-        description="The name of the file including the extension and the file path from your current directory if needed."
+class DirectoryNavigator(BaseTool):
+    """Allows you to navigate directories. Do not use this tool more than once at a time.
+    You must finish all tasks in the current directory before navigating into new directory."""
+    path: str = Field(
+        ..., description="The path of the directory to navigate to."
     )
-    body: str = Field(..., description="Correct contents of a file")
-
-    def run(self):
-        # Extract the directory path from the file name
-        directory = os.path.dirname(self.file_name)
-
-        # If the directory is not empty, check if it exists and create it if not
-        if directory and not os.path.exists(directory):
-            os.makedirs(directory)
-
-        # Write the file
-        with open(self.file_name, "w") as f:
-            f.write(self.body)
-
-        return "File written to " + self.file_name
-
-
-class WriteFiles(BaseTool):
-    """
-    Set of files that represent a complete and correct program.
-    """
-    chain_of_thought: str = Field(...,
-                                  description="Think step by step to determine the correct actions that are needed to implement the program.")
-    files: List[File] = Field(..., description="List of files")
+    create: bool = Field(
+        False, description="If True, the directory will be created if it does not exist."
+    )
+    one_call_at_a_time: bool = True
 
     def run(self):
-        outputs = []
-        for file in self.files:
-            outputs.append(file.run())
+        try:
+            os.chdir(self.path)
+            return f'Successfully changed directory to: {self.path}'
+        except Exception as e:
+            return f'Error changing directory: {e}'
+
+    @field_validator("create", mode="before")
+    @classmethod
+    def validate_create(cls, v):
+        if not isinstance(v, bool):
+            if v.lower() == "true":
+                return True
+            elif v.lower() == "false":
+                return False
+        return v
+
+    @model_validator(mode='after')
+    def validate_path(self):
+        if not os.path.isdir(self.path):
+            if "/mnt/data" in self.path:
+                raise ValueError("You tried to access an openai file directory with a local directory reader tool. " +
+                                 "Please use the `myfiles_browser` tool to access openai files instead. " +
+                                 "Your local files are most likely located in your current directory.")
+
+            if self.create:
+                os.makedirs(self.path)
+            else:
+                raise ValueError(f"The path {self.path} does not exist. Please provide a valid directory path. " +
+                                 "If you want to create the directory, set the `create` parameter to True.")
 
-        return str(outputs)
+        return self
```

### Comparing `agency-swarm-0.1.6/agency_swarm/util/event_handler.py` & `agency-swarm-0.1.7/agency_swarm/util/event_handler.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/util/oai.py` & `agency-swarm-0.1.7/agency_swarm/util/oai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import httpx
 import openai
 import threading
 import os
 import instructor
 
 from dotenv import load_dotenv
 
@@ -16,15 +17,15 @@
     with client_lock:
         if client is None:
             # Check if the API key is set
             api_key = openai.api_key or os.getenv('OPENAI_API_KEY')
             if api_key is None:
                 raise ValueError("OpenAI API key is not set. Please set it using set_openai_key.")
             client = instructor.patch(openai.OpenAI(api_key=api_key,
-                                                    timeout=10,
+                                                    timeout=httpx.Timeout(60.0, read=30, connect=5.0),
                                                     max_retries=5))
     return client
 
 
 def set_openai_client(new_client):
     global client
     with client_lock:
```

### Comparing `agency-swarm-0.1.6/agency_swarm/util/openapi.py` & `agency-swarm-0.1.7/agency_swarm/util/openapi.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm/util/schema.py` & `agency-swarm-0.1.7/agency_swarm/util/schema.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/agency_swarm.egg-info/PKG-INFO` & `agency-swarm-0.1.7/agency_swarm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agency-swarm
-Version: 0.1.6
+Version: 0.1.7
 Summary: An open source agent orchestration framework built on top of the latest OpenAI Assistants API.
 Home-page: https://github.com/VRSEN/agency-swarm
 Author: VRSEN
 Author-email: VRSEN <arseny9795@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Arsenii Shatokhin
@@ -144,31 +144,35 @@
                 description="Responsible for client communication, task planning and management.",
                 instructions="You must converse with other agents to ensure complete task execution.", # can be a file like ./instructions.md
                 files_folder="./files", # files to be uploaded to OpenAI
                 schemas_folder="./schemas", # OpenAPI schemas to be converted into tools
                 tools=[MyCustomTool, LangchainTool])
     ```
 
-    Import from existing agents (will be deprecated in future versions):
-    
-    ```python
-    from agency_swarm.agents.browsing import BrowsingAgent
-    
-    browsing_agent = BrowsingAgent()
-    
-    browsing_agent.instructions += "\n\nYou can add additional instructions here."
-    ```
+    Import from existing agents:
+
+   ```bash
+   agency-swarm import-agent --name "Devid" --destination "./"
+   ```
+   
+   This will import Devid (Software Developer) Agent locally, including all source code files, so you have full control over your system. Currently, available agents are: `Devid`, `BrowsingAgent`.
 
 
 
 4. **Define Agency Communication Flows**: 
 Establish how your agents will communicate with each other.
 
     ```python
     from agency_swarm import Agency
+    # if importing from local files
+    from Developer import Developer
+    from VirtualAssistant import VirtualAssistant
+   
+    dev = Developer()
+    va = VirtualAssistant()
     
     agency = Agency([
         ceo,  # CEO will be the entry point for communication with the user
         [ceo, dev],  # CEO can initiate communication with Developer
         [ceo, va],   # CEO can initiate communication with Virtual Assistant
         [dev, va]    # Developer can initiate communication with Virtual Assistant
     ], shared_instructions='agency_manifesto.md') # shared instructions for all agents
@@ -210,14 +214,26 @@
 ```
 
 Make sure to include:
 - Your mission and goals.
 - The agents you want to involve and their communication flows.
 - Which tools or APIs each agent should have access to, if any.
 
+## Importing Existing Agents
+
+This CLI command allows you to import existing agents from local files into your agency.
+
+#### **Command Syntax:**
+
+```bash
+agency-swarm import-agent --name "AgentName" --destination "/path/to/directory"
+```
+
+To check available agents, simply run this command without any arguments.
+
 ## Creating Agent Templates Locally
 
 This CLI command simplifies the process of creating a structured environment for each agent.
 
 #### **Command Syntax:**
 
 ```bash
```

### Comparing `agency-swarm-0.1.6/agency_swarm.egg-info/SOURCES.txt` & `agency-swarm-0.1.7/agency_swarm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 agency_swarm/agency/genesis/__init__.py
 agency_swarm/agency/genesis/manifesto.md
 agency_swarm/agency/genesis/util.py
 agency_swarm/agency/genesis/AgentCreator/AgentCreator.py
 agency_swarm/agency/genesis/AgentCreator/__init__.py
 agency_swarm/agency/genesis/AgentCreator/instructions.md
 agency_swarm/agency/genesis/AgentCreator/tools/CreateAgentTemplate.py
-agency_swarm/agency/genesis/AgentCreator/tools/GetAvailableAgents.py
 agency_swarm/agency/genesis/AgentCreator/tools/ImportAgent.py
 agency_swarm/agency/genesis/AgentCreator/tools/ReadManifesto.py
 agency_swarm/agency/genesis/AgentCreator/tools/util/__init__.py
 agency_swarm/agency/genesis/AgentCreator/tools/util/get_modules.py
 agency_swarm/agency/genesis/GenesisCEO/GenesisCEO.py
 agency_swarm/agency/genesis/GenesisCEO/__init__.py
 agency_swarm/agency/genesis/GenesisCEO/instructions.md
@@ -48,61 +47,72 @@
 agency_swarm/agency/genesis/ToolCreator/ToolCreator.py
 agency_swarm/agency/genesis/ToolCreator/__init__.py
 agency_swarm/agency/genesis/ToolCreator/instructions.md
 agency_swarm/agency/genesis/ToolCreator/tools/CreateTool.py
 agency_swarm/agency/genesis/ToolCreator/tools/TestTool.py
 agency_swarm/agents/__init__.py
 agency_swarm/agents/agent.py
-agency_swarm/agents/browsing/BrowsingAgent.py
-agency_swarm/agents/browsing/__init__.py
-agency_swarm/agents/browsing/tools/AnalyzeContent.py
-agency_swarm/agents/browsing/tools/ClickElement.py
-agency_swarm/agents/browsing/tools/ExportFile.py
-agency_swarm/agents/browsing/tools/GoBack.py
-agency_swarm/agents/browsing/tools/ReadURL.py
-agency_swarm/agents/browsing/tools/Scroll.py
-agency_swarm/agents/browsing/tools/SelectDropdown.py
-agency_swarm/agents/browsing/tools/SendKeys.py
-agency_swarm/agents/browsing/tools/SolveCaptcha.py
-agency_swarm/agents/browsing/tools/__init__.py
-agency_swarm/agents/browsing/tools/util/__init__.py
-agency_swarm/agents/browsing/tools/util/get_b64_screenshot.py
-agency_swarm/agents/browsing/tools/util/highlights.py
-agency_swarm/agents/browsing/tools/util/selenium.py
-agency_swarm/agents/coding/__init__.py
-agency_swarm/agents/coding/CodingAgent/CodingAgent.py
-agency_swarm/agents/coding/CodingAgent/__init__.py
-agency_swarm/agents/coding/CodingAgent/instructions.md
+agency_swarm/agents/BrowsingAgent/BrowsingAgent.py
+agency_swarm/agents/BrowsingAgent/__init__.py
+agency_swarm/agents/BrowsingAgent/instructions.md
+agency_swarm/agents/BrowsingAgent/requirements.txt
+agency_swarm/agents/BrowsingAgent/tools/AnalyzeContent.py
+agency_swarm/agents/BrowsingAgent/tools/ClickElement.py
+agency_swarm/agents/BrowsingAgent/tools/ExportFile.py
+agency_swarm/agents/BrowsingAgent/tools/GoBack.py
+agency_swarm/agents/BrowsingAgent/tools/ReadURL.py
+agency_swarm/agents/BrowsingAgent/tools/Scroll.py
+agency_swarm/agents/BrowsingAgent/tools/SelectDropdown.py
+agency_swarm/agents/BrowsingAgent/tools/SendKeys.py
+agency_swarm/agents/BrowsingAgent/tools/SolveCaptcha.py
+agency_swarm/agents/BrowsingAgent/tools/WebPageSummarizer.py
+agency_swarm/agents/BrowsingAgent/tools/__init__.py
+agency_swarm/agents/BrowsingAgent/tools/util/__init__.py
+agency_swarm/agents/BrowsingAgent/tools/util/get_b64_screenshot.py
+agency_swarm/agents/BrowsingAgent/tools/util/highlights.py
+agency_swarm/agents/BrowsingAgent/tools/util/selenium.py
+agency_swarm/agents/Devid/Devid.py
+agency_swarm/agents/Devid/__init__.py
+agency_swarm/agents/Devid/instructions.md
+agency_swarm/agents/Devid/tools/ChangeFile.py
+agency_swarm/agents/Devid/tools/CheckCurrentDir.py
+agency_swarm/agents/Devid/tools/CommandExecutor.py
+agency_swarm/agents/Devid/tools/DirectoryNavigator.py
+agency_swarm/agents/Devid/tools/FileMover.py
+agency_swarm/agents/Devid/tools/FileReader.py
+agency_swarm/agents/Devid/tools/FileWriter.py
+agency_swarm/agents/Devid/tools/ListDir.py
+agency_swarm/agents/Devid/tools/__init__.py
+agency_swarm/agents/Devid/tools/util/__init__.py
+agency_swarm/agents/Devid/tools/util/format_file_deps.py
 agency_swarm/messages/__init__.py
 agency_swarm/messages/message_output.py
 agency_swarm/threads/__init__.py
 agency_swarm/threads/thread.py
 agency_swarm/threads/thread_async.py
 agency_swarm/tools/BaseTool.py
 agency_swarm/tools/ToolFactory.py
 agency_swarm/tools/__init__.py
-agency_swarm/tools/coding/ChangeDir.py
-agency_swarm/tools/coding/ChangeLines.py
-agency_swarm/tools/coding/CreateFolder.py
-agency_swarm/tools/coding/ListDir.py
-agency_swarm/tools/coding/ReadFile.py
-agency_swarm/tools/coding/WriteFiles.py
-agency_swarm/tools/coding/__init__.py
 agency_swarm/tools/oai/CodeInterpreter.py
 agency_swarm/tools/oai/Retrieval.py
 agency_swarm/tools/oai/__init__.py
 agency_swarm/user/__init__.py
 agency_swarm/user/user.py
 agency_swarm/util/__init__.py
-agency_swarm/util/create_agent_template.py
 agency_swarm/util/event_handler.py
 agency_swarm/util/oai.py
 agency_swarm/util/openapi.py
 agency_swarm/util/schema.py
 agency_swarm/util/streaming.py
+agency_swarm/util/cli/__init__.py
+agency_swarm/util/cli/create_agent_template.py
+agency_swarm/util/cli/import_agent.py
+agency_swarm/util/helpers/__init__.py
+agency_swarm/util/helpers/get_available_agent_descriptions.py
+agency_swarm/util/helpers/list_available_agents.py
 docs/api.md
 docs/contributing.md
 docs/deployment.md
 docs/examples.md
 docs/index.md
 docs/quick_start.md
 docs/advanced-usage/agencies.md
```

### Comparing `agency-swarm-0.1.6/docs/advanced-usage/agencies.md` & `agency-swarm-0.1.7/docs/advanced-usage/agencies.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/docs/advanced-usage/agents.md` & `agency-swarm-0.1.7/docs/advanced-usage/agents.md`

 * *Files 8% similar despite different names*

```diff
@@ -71,29 +71,33 @@
             name="agent_name",
             description="agent_description",
             instructions="./instructions.md",
             files_folder="./files",
             schemas_folder="./schemas",
             tools_folder="./tools"
         )
+
+    def response_validator(self, message: str) -> str:
+        """This function is used to validate the response before sending it to the user or another agent."""
+        if "bad word" in message:
+            return "Please don't use bad words."
+        
+        return message
 ```
 
 To initialize the agent, you can simply import the agent and instantiate it:
 
 ```python
 from AgentName import AgentName
 
 agent = AgentName()
 ```
 
 ### Importing existing agents
 
-For the most complex and requested use cases, we will be creating premade agents that you can import and reuse in your own projects. 
+For the most complex and requested use cases, we will be creating premade agents that you can import and reuse in your own projects. To import an existing agent, you can run the following CLI command:
 
-!!! warning "Will be deprecated in future versions."
-    We are planning to deprecate agent imports in future versions, as this takes away the flexibility of the framework. Instead, we are planning to add a functionality to download agent source files locally from github, which will allow you to modify the inner logic and tools as you see fit.
+```bash
+agency-swarm import-agent --name "AgentName" --destination "/path/to/directory"
+```
 
-```py
-from agency_swarm.agents.browsing import BrowsingAgent
-browsing_agent = BrowsingAgent()
-browsing_agent.instructions += "\n\nYou can add additional instructions here."
-```
+This will copy all your agent source files locally. You can then import the agent as shown above. To check available agents, simply run this command without any arguments.
```

### Comparing `agency-swarm-0.1.6/docs/advanced-usage/azure-openai.md` & `agency-swarm-0.1.7/docs/advanced-usage/azure-openai.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/docs/advanced-usage/tools.md` & `agency-swarm-0.1.7/docs/advanced-usage/tools.md`

 * *Files 2% similar despite different names*

```diff
@@ -242,7 +242,17 @@
    
         def run(self):
             if self.shared_state.get("action_1_result", None) is "failure":
                 raise ValueError("Please proceed with the Action1 tool first.")
             else:
                 return "Success. The action has been taken."
     ```
+4. Consider `one_call_at_a_time` class attribute to prevent multiple instances of the same tool from running at the same time. This is useful when you want your agents to see the results of the previous action before proceeding with the next one.
+
+    ```python
+    class Action1(BaseTool):
+        input: str = Field(...)
+        one_call_at_a_time: bool = True
+   
+        def run(self):
+            # your code here
+    ```
```

### Comparing `agency-swarm-0.1.6/docs/deployment.md` & `agency-swarm-0.1.7/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/docs/examples.md` & `agency-swarm-0.1.7/docs/examples.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/docs/index.md` & `agency-swarm-0.1.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/docs/quick_start.md` & `agency-swarm-0.1.7/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/mkdocs.yml` & `agency-swarm-0.1.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/notebooks/agency_async.ipynb` & `agency-swarm-0.1.7/notebooks/agency_async.ipynb`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/notebooks/azure.ipynb` & `agency-swarm-0.1.7/notebooks/azure.ipynb`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/notebooks/genesis_agency.ipynb` & `agency-swarm-0.1.7/notebooks/genesis_agency.ipynb`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/notebooks/web_browser_agent.ipynb` & `agency-swarm-0.1.7/notebooks/web_browser_agent.ipynb`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/pyproject.toml` & `agency-swarm-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/run_tests.py` & `agency-swarm-0.1.7/run_tests.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/setup.py` & `agency-swarm-0.1.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='agency-swarm',
-    version='0.1.6',
+    version='0.1.7',
     author='VRSEN',
     author_email='arseny9795@gmail.com',
     description='An opensource agent orchestration framework built on top of the latest OpenAI Assistants API.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VRSEN/agency-swarm',
-    packages=find_packages(),
+    packages=find_packages(exclude=['tests', 'tests.*']),
     install_requires=requirements,
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
     ],
     entry_points = {
```

### Comparing `agency-swarm-0.1.6/tests/data/files/csv-test.csv` & `agency-swarm-0.1.7/tests/data/files/csv-test.csv`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/data/files/generated_data.json` & `agency-swarm-0.1.7/tests/data/files/generated_data.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/data/files/test-docx.docx` & `agency-swarm-0.1.7/tests/data/files/test-docx.docx`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/data/files/test-html.html` & `agency-swarm-0.1.7/tests/data/files/test-html.html`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/data/files/test-pdf.pdf` & `agency-swarm-0.1.7/tests/data/files/test-pdf.pdf`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/data/schemas/ga4.json` & `agency-swarm-0.1.7/tests/data/schemas/ga4.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/data/schemas/get-headers-params.json` & `agency-swarm-0.1.7/tests/data/schemas/get-headers-params.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/data/schemas/get-weather.json` & `agency-swarm-0.1.7/tests/data/schemas/get-weather.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/data/schemas/relevance.json` & `agency-swarm-0.1.7/tests/data/schemas/relevance.json`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/demos/demo_gradio.py` & `agency-swarm-0.1.7/tests/demos/demo_gradio.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/demos/streaming_demo.py` & `agency-swarm-0.1.7/tests/demos/streaming_demo.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/demos/term_demo.py` & `agency-swarm-0.1.7/tests/demos/term_demo.py`

 * *Files identical despite different names*

### Comparing `agency-swarm-0.1.6/tests/test_agency.py` & `agency-swarm-0.1.7/tests/test_agency.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,15 +112,17 @@
                 """
                 self.shared_state.set("test_tool_used", True)
 
                 return "Test Successful"
 
         cls.TestTool = TestTool
 
-        from test_agents import CEO, TestAgent1, TestAgent2
+        from test_agents.CEO import CEO
+        from test_agents.TestAgent1 import TestAgent1
+        from test_agents.TestAgent2 import TestAgent2
         cls.ceo = CEO()
         cls.agent1 = TestAgent1()
         cls.agent1.add_tool(Retrieval)
         cls.agent2 = TestAgent2()
         cls.agent2.add_tool(cls.TestTool)
 
     def test_1_init_agency(self):
@@ -134,15 +136,15 @@
             threads_callbacks=self.__class__.threads_callbacks,
         )
 
         self.check_all_agents_settings()
 
     def test_2_load_agent(self):
         """it should load existing assistant from settings"""
-        from test_agents import TestAgent1
+        from test_agents.TestAgent1 import TestAgent1
         agent3 = TestAgent1()
         agent3.add_shared_instructions(self.__class__.agency.shared_instructions)
         agent3.tools = self.__class__.agent1.tools
         agent3 = agent3.init_oai()
 
         print("agent3", agent3.assistant.model_dump())
         print("agent1", self.__class__.agent1.assistant.model_dump())
@@ -201,16 +203,19 @@
                     test_agent2_used = True
 
             def on_tool_call_done(self, tool_call: ToolCall) -> None:
                 if tool_call.function.name == "TestTool":
                     nonlocal test_tool_used
                     test_tool_used = True
 
-        message = self.__class__.agency.get_completion_stream("Please tell TestAgent1 to tell TestAgent 2 to use test tool.",
-                                                              event_handler=EventHandler)
+        message = self.__class__.agency.get_completion_stream(
+            "Please tell TestAgent1 to tell TestAgent 2 to use test tool.",
+            event_handler=EventHandler,
+            additional_instructions="Your message to TestAgent1 should be exactly as follows: "
+                                    "'Please tell TestAgent2 to use test tool.'",)
 
         # self.assertFalse('error' in message.lower())
 
         self.assertTrue(test_tool_used)
         self.assertTrue(test_agent2_used)
 
         self.assertTrue(self.__class__.TestTool.shared_state.get("test_tool_used"))
@@ -225,15 +230,17 @@
     def test_6_load_from_db(self):
         """it should load agents from db"""
         # os.rename("settings.json", "settings2.json")
 
         previous_loaded_thread_ids = self.__class__.loaded_thread_ids
         previous_loaded_agents_settings = self.__class__.loaded_agents_settings
 
-        from test_agents import CEO, TestAgent1, TestAgent2
+        from test_agents.CEO import CEO
+        from test_agents.TestAgent1 import TestAgent1
+        from test_agents.TestAgent2 import TestAgent2
         agent1 = TestAgent1()
         agent1.add_tool(Retrieval)
         agent2 = TestAgent2()
         agent2.add_tool(self.__class__.TestTool)
 
         ceo = CEO()
```

### Comparing `agency-swarm-0.1.6/tests/test_tool_factory.py` & `agency-swarm-0.1.7/tests/test_tool_factory.py`

 * *Files identical despite different names*

