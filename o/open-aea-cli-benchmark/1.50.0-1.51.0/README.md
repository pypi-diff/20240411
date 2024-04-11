# Comparing `tmp/open-aea-cli-benchmark-1.50.0.tar.gz` & `tmp/open-aea-cli-benchmark-1.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-cli-benchmark-1.50.0.tar", last modified: Fri Mar 15 09:35:29 2024, max compression
+gzip compressed data, was "open-aea-cli-benchmark-1.51.0.tar", last modified: Thu Apr 11 03:16:25 2024, max compression
```

## Comparing `open-aea-cli-benchmark-1.50.0.tar` & `open-aea-cli-benchmark-1.51.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.904973 open-aea-cli-benchmark-1.50.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-15 09:35:29.904973 open-aea-cli-benchmark-1.50.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.896973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.896973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6564 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.896973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3467 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.896973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_agent_construction_time/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_agent_construction_time/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3159 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_agent_construction_time/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_agent_construction_time/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_decision_maker/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_decision_maker/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7767 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_decision_maker/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_decision_maker/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_dialogues_memory_usage/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_dialogues_memory_usage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3624 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_dialogues_memory_usage/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_dialogues_memory_usage/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_mem_usage/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_mem_usage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2825 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_mem_usage/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_mem_usage/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_messages_memory_usage/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_messages_memory_usage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1939 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_messages_memory_usage/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_messages_memory_usage/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6659 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent_http_dialogues/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent_http_dialogues/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7992 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent_http_dialogues/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent_http_dialogues/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_proactive/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_proactive/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2932 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_proactive/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_proactive/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_reactive/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_reactive/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4459 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_reactive/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_reactive/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.900973 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18604 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/dialogues.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/ledger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.904973 open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-15 09:35:29.000000 open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-15 09:35:29.000000 open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 09:35:29.000000 open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-15 09:35:29.000000 open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-15 09:35:29.000000 open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 09:35:29.000000 open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 09:35:29.904973 open-aea-cli-benchmark-1.50.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2316 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:29.904973 open-aea-cli-benchmark-1.50.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-15 09:35:01.000000 open-aea-cli-benchmark-1.50.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6564 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3467 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_agent_construction_time/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_agent_construction_time/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3159 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_agent_construction_time/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_agent_construction_time/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_decision_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_decision_maker/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7767 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_decision_maker/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_decision_maker/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_dialogues_memory_usage/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_dialogues_memory_usage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3624 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_dialogues_memory_usage/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_dialogues_memory_usage/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_mem_usage/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_mem_usage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2825 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_mem_usage/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_mem_usage/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_messages_memory_usage/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_messages_memory_usage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1939 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_messages_memory_usage/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_messages_memory_usage/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.661471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6659 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent_http_dialogues/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent_http_dialogues/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7992 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent_http_dialogues/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent_http_dialogues/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_proactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_proactive/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2932 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_proactive/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_proactive/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_reactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_reactive/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4459 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_reactive/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_reactive/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18604 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/dialogues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/ledger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 03:16:25.000000 open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-11 03:16:25.000000 open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:16:25.000000 open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 03:16:25.000000 open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 03:16:25.000000 open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 03:16:25.000000 open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2316 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:25.665471 open-aea-cli-benchmark-1.51.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-11 03:15:53.000000 open-aea-cli-benchmark-1.51.0/tests/__init__.py
```

### Comparing `open-aea-cli-benchmark-1.50.0/LICENSE` & `open-aea-cli-benchmark-1.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/PKG-INFO` & `open-aea-cli-benchmark-1.51.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-cli-benchmark
-Version: 1.50.0
+Version: 1.51.0
 Summary: CLI extension for AEA framework benchmarking.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-cli-benchmark-1.50.0/README.md` & `open-aea-cli-benchmark-1.51.0/README.md`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_communication/utils.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_communication/utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_acn_startup/utils.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_acn_startup/utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_agent_construction_time/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_agent_construction_time/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_agent_construction_time/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_agent_construction_time/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_agent_construction_time/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_agent_construction_time/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_decision_maker/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_decision_maker/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_decision_maker/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_decision_maker/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_decision_maker/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_decision_maker/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_dialogues_memory_usage/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_dialogues_memory_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_dialogues_memory_usage/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_dialogues_memory_usage/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_dialogues_memory_usage/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_dialogues_memory_usage/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_mem_usage/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_mem_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_mem_usage/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_mem_usage/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_mem_usage/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_mem_usage/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_messages_memory_usage/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_messages_memory_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_messages_memory_usage/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_messages_memory_usage/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_messages_memory_usage/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_messages_memory_usage/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent_http_dialogues/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent_http_dialogues/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent_http_dialogues/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent_http_dialogues/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_multiagent_http_dialogues/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_multiagent_http_dialogues/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_proactive/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_proactive/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_proactive/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_proactive/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_proactive/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_proactive/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_reactive/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_reactive/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_reactive/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_reactive/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_reactive/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_reactive/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/__init__.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/case.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/case.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/command.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/command.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/core.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/core.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/dialogues.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/dialogues.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/docker_image.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/docker_image.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/case_tx_generate/ledger_utils.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/case_tx_generate/ledger_utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/core.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/core.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/aea_cli_benchmark/utils.py` & `open-aea-cli-benchmark-1.51.0/aea_cli_benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/PKG-INFO` & `open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-cli-benchmark
-Version: 1.50.0
+Version: 1.51.0
 Summary: CLI extension for AEA framework benchmarking.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-cli-benchmark-1.50.0/open_aea_cli_benchmark.egg-info/SOURCES.txt` & `open-aea-cli-benchmark-1.51.0/open_aea_cli_benchmark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-cli-benchmark-1.50.0/setup.py` & `open-aea-cli-benchmark-1.51.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from setuptools import find_packages  # type: ignore
 from setuptools import setup  # type: ignore
 
 
 setup(
     name="open-aea-cli-benchmark",
-    version="1.50.0",
+    version="1.51.0",
     author="Valory AG",
     license="Apache-2.0",
     description="CLI extension for AEA framework benchmarking.",
     long_description="CLI extension for AEA framework benchmarking.",
     long_description_content_type="text/markdown",
     packages=find_packages(
         where=".", include=["aea_cli_benchmark", "aea_cli_benchmark.*"]
```

### Comparing `open-aea-cli-benchmark-1.50.0/tests/__init__.py` & `open-aea-cli-benchmark-1.51.0/tests/__init__.py`

 * *Files identical despite different names*

