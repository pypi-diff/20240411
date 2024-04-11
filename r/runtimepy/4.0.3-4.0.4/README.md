# Comparing `tmp/runtimepy-4.0.3.tar.gz` & `tmp/runtimepy-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-4.0.3.tar", last modified: Tue Apr  9 18:20:49 2024, max compression
+gzip compressed data, was "runtimepy-4.0.4.tar", last modified: Wed Apr 10 23:19:43 2024, max compression
```

## Comparing `runtimepy-4.0.3.tar` & `runtimepy-4.0.4.tar`

### file list

```diff
@@ -1,291 +1,291 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.367071 runtimepy-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 18:18:49.000000 runtimepy-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-09 18:20:49.367071 runtimepy-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-09 18:18:49.000000 runtimepy-4.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-09 18:18:49.000000 runtimepy-4.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.331072 runtimepy-4.0.3/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.335072 runtimepy-4.0.3/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.335072 runtimepy-4.0.3/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.335072 runtimepy-4.0.3/runtimepy/channel/environment/command/
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/command/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/command/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/environment/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.335072 runtimepy-4.0.3/runtimepy/channel/event/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/event/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.335072 runtimepy-4.0.3/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.335072 runtimepy-4.0.3/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.335072 runtimepy-4.0.3/runtimepy/codec/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/codec/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.339072 runtimepy-4.0.3/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/commands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.339072 runtimepy-4.0.3/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.339072 runtimepy-4.0.3/runtimepy/data/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/css/bootstrap_extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/dummy_load.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/factories.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.339072 runtimepy-4.0.3/runtimepy/data/js/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/audio.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.343072 runtimepy-4.0.3/runtimepy/data/js/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/App.js
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/ChannelTable.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/Plot.js
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/PlotManager.js
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/TabFilter.js
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/TabInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/WindowHashManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/classes/WorkerInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/init.js
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.343072 runtimepy-4.0.3/runtimepy/data/js/tab/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/tab/env.js
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/tab/sound.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.343072 runtimepy-4.0.3/runtimepy/data/js/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/unused/pyodide.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/js/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.343072 runtimepy-4.0.3/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/ChannelCommand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/FindFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/StructConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/schemas/has_request_flag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/server_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/data/server_dev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.343072 runtimepy-4.0.3/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/enum/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.347072 runtimepy-4.0.3/runtimepy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/metrics/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/metrics/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/metrics/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.347072 runtimepy-4.0.3/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/mixins/async_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/mixins/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/mixins/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.347072 runtimepy-4.0.3/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.347072 runtimepy-4.0.3/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.347072 runtimepy-4.0.3/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.347072 runtimepy-4.0.3/runtimepy/net/arbiter/config/
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/config/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/housekeeping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/arbiter/imports/
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/imports/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/arbiter/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/arbiter/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/tcp/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/http/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/http/request_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/http/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/http/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.351072 runtimepy-4.0.3/runtimepy/net/server/app/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/server/app/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/bootstrap/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/bootstrap/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/server/app/env/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/env/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/server/app/env/tab/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/env/tab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/env/tab/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/env/tab/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/env/tab/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/env/tab/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/env/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/app/tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/server/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/server/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/server/websocket/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/stream/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/stream/json/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/stream/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/stream/json/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/stream/json/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/stream/json/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/stream/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/tcp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/tcp/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/tcp/http/
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/tcp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/tcp/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.355072 runtimepy-4.0.3/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.359072 runtimepy-4.0.3/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/udp/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.359072 runtimepy-4.0.3/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.359072 runtimepy-4.0.3/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.359072 runtimepy-4.0.3/runtimepy/primitives/array/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.359072 runtimepy-4.0.3/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.359072 runtimepy-4.0.3/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.359072 runtimepy-4.0.3/runtimepy/primitives/serializable/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/serializable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/serializable/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/serializable/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/serializable/prefixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/primitives/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/types/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/types/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/primitives/types/int.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/task/basic/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/task/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/task/trig/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/task/trig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/tui/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/tui/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/tui/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/tui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 18:18:49.000000 runtimepy-4.0.3/runtimepy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-09 18:20:49.000000 runtimepy-4.0.3/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-09 18:20:49.000000 runtimepy-4.0.3/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:20:49.000000 runtimepy-4.0.3/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 18:20:49.000000 runtimepy-4.0.3/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 18:20:49.000000 runtimepy-4.0.3/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 18:20:49.000000 runtimepy-4.0.3/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:20:49.367071 runtimepy-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 18:18:49.000000 runtimepy-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:20:49.363072 runtimepy-4.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 18:18:49.000000 runtimepy-4.0.3/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-09 18:18:49.000000 runtimepy-4.0.3/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 18:18:49.000000 runtimepy-4.0.3/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.458404 runtimepy-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-10 23:17:35.000000 runtimepy-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-10 23:19:43.458404 runtimepy-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-10 23:17:35.000000 runtimepy-4.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-10 23:17:35.000000 runtimepy-4.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.418404 runtimepy-4.0.4/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.422404 runtimepy-4.0.4/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.422404 runtimepy-4.0.4/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.422404 runtimepy-4.0.4/runtimepy/channel/environment/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/command/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/command/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/environment/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.422404 runtimepy-4.0.4/runtimepy/channel/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/event/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.422404 runtimepy-4.0.4/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.422404 runtimepy-4.0.4/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.422404 runtimepy-4.0.4/runtimepy/codec/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/codec/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.426404 runtimepy-4.0.4/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.426404 runtimepy-4.0.4/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.426404 runtimepy-4.0.4/runtimepy/data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/css/bootstrap_extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/dummy_load.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/factories.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.426404 runtimepy-4.0.4/runtimepy/data/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/audio.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.430404 runtimepy-4.0.4/runtimepy/data/js/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/App.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/ChannelTable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/Plot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/PlotManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/TabFilter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/TabInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/WindowHashManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/classes/WorkerInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.430404 runtimepy-4.0.4/runtimepy/data/js/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/tab/env.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/tab/sound.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.430404 runtimepy-4.0.4/runtimepy/data/js/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/unused/pyodide.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/js/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.434404 runtimepy-4.0.4/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/ChannelCommand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/FindFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/StructConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/schemas/has_request_flag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/server_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/data/server_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.434404 runtimepy-4.0.4/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/enum/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.434404 runtimepy-4.0.4/runtimepy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/metrics/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/metrics/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/metrics/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.434404 runtimepy-4.0.4/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/mixins/async_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/mixins/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/mixins/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/arbiter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/config/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/housekeeping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/arbiter/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/imports/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/arbiter/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/arbiter/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/tcp/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.438404 runtimepy-4.0.4/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.442404 runtimepy-4.0.4/runtimepy/net/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/http/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/http/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/http/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/http/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.442404 runtimepy-4.0.4/runtimepy/net/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.442404 runtimepy-4.0.4/runtimepy/net/server/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.442404 runtimepy-4.0.4/runtimepy/net/server/app/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/bootstrap/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/bootstrap/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.442404 runtimepy-4.0.4/runtimepy/net/server/app/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/env/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.446404 runtimepy-4.0.4/runtimepy/net/server/app/env/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/env/tab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/env/tab/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/env/tab/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/env/tab/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/env/tab/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/env/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/app/tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.446404 runtimepy-4.0.4/runtimepy/net/server/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.446404 runtimepy-4.0.4/runtimepy/net/server/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/server/websocket/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.446404 runtimepy-4.0.4/runtimepy/net/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/stream/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.446404 runtimepy-4.0.4/runtimepy/net/stream/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/stream/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/stream/json/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/stream/json/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/stream/json/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/stream/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.446404 runtimepy-4.0.4/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/tcp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/tcp/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.446404 runtimepy-4.0.4/runtimepy/net/tcp/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/tcp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/tcp/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.446404 runtimepy-4.0.4/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.450404 runtimepy-4.0.4/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/udp/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.450404 runtimepy-4.0.4/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.450404 runtimepy-4.0.4/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.450404 runtimepy-4.0.4/runtimepy/primitives/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.450404 runtimepy-4.0.4/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.450404 runtimepy-4.0.4/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.450404 runtimepy-4.0.4/runtimepy/primitives/serializable/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/serializable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/serializable/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/serializable/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/serializable/prefixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/primitives/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/types/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/types/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/primitives/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/task/basic/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/task/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/task/trig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/task/trig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/tui/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/tui/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/tui/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/tui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 23:17:35.000000 runtimepy-4.0.4/runtimepy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.458404 runtimepy-4.0.4/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-10 23:19:43.000000 runtimepy-4.0.4/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-10 23:19:43.000000 runtimepy-4.0.4/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:19:43.000000 runtimepy-4.0.4/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 23:19:43.000000 runtimepy-4.0.4/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 23:19:43.000000 runtimepy-4.0.4/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 23:19:43.000000 runtimepy-4.0.4/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:19:43.458404 runtimepy-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-10 23:17:35.000000 runtimepy-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:19:43.454404 runtimepy-4.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-10 23:17:35.000000 runtimepy-4.0.4/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-10 23:17:35.000000 runtimepy-4.0.4/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-10 23:17:35.000000 runtimepy-4.0.4/tests/test_resources.py
```

### Comparing `runtimepy-4.0.3/LICENSE` & `runtimepy-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/PKG-INFO` & `runtimepy-4.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.0.3
+Version: 4.0.4
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psutil
-Requires-Dist: svgen>=0.6.5
 Requires-Dist: vcorelib>=3.2.2
+Requires-Dist: svgen>=0.6.5
 Requires-Dist: websockets
+Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=b46d92eb818e462d978d8fcf87af04ed
+    hash=901fe42416b14697d7706086dcd4e0a4
     =====================================
 -->
 
-# runtimepy ([4.0.3](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.0.4](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.0.3/README.md` & `runtimepy-4.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=b46d92eb818e462d978d8fcf87af04ed
+    hash=901fe42416b14697d7706086dcd4e0a4
     =====================================
 -->
 
-# runtimepy ([4.0.3](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.0.4](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.0.3/pyproject.toml` & `runtimepy-4.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "4.0.3"
+version = "4.0.4"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-4.0.3/runtimepy/app.py` & `runtimepy-4.0.4/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/__init__.py` & `runtimepy-4.0.4/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/__init__.py` & `runtimepy-4.0.4/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/array.py` & `runtimepy-4.0.4/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/base.py` & `runtimepy-4.0.4/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/command/__init__.py` & `runtimepy-4.0.4/runtimepy/channel/environment/command/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/command/parser.py` & `runtimepy-4.0.4/runtimepy/channel/environment/command/parser.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/command/processor.py` & `runtimepy-4.0.4/runtimepy/channel/environment/command/processor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/command/result.py` & `runtimepy-4.0.4/runtimepy/channel/environment/command/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/create.py` & `runtimepy-4.0.4/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/file.py` & `runtimepy-4.0.4/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/environment/sample.py` & `runtimepy-4.0.4/runtimepy/channel/environment/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/event/__init__.py` & `runtimepy-4.0.4/runtimepy/channel/event/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/event/header.py` & `runtimepy-4.0.4/runtimepy/channel/event/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/channel/registry.py` & `runtimepy-4.0.4/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/codec/protocol/__init__.py` & `runtimepy-4.0.4/runtimepy/codec/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/codec/protocol/base.py` & `runtimepy-4.0.4/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/codec/protocol/json.py` & `runtimepy-4.0.4/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/codec/system/__init__.py` & `runtimepy-4.0.4/runtimepy/codec/system/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/commands/all.py` & `runtimepy-4.0.4/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/commands/arbiter.py` & `runtimepy-4.0.4/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/commands/common.py` & `runtimepy-4.0.4/runtimepy/commands/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/commands/server.py` & `runtimepy-4.0.4/runtimepy/commands/server.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/commands/task.py` & `runtimepy-4.0.4/runtimepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/commands/tui.py` & `runtimepy-4.0.4/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/css/bootstrap_extra.css` & `runtimepy-4.0.4/runtimepy/data/css/bootstrap_extra.css`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/dummy_load.yaml` & `runtimepy-4.0.4/runtimepy/data/dummy_load.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/factories.yaml` & `runtimepy-4.0.4/runtimepy/data/factories.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/favicon.ico` & `runtimepy-4.0.4/runtimepy/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/JsonConnection.js` & `runtimepy-4.0.4/runtimepy/data/js/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/audio.js` & `runtimepy-4.0.4/runtimepy/data/js/audio.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/classes/App.js` & `runtimepy-4.0.4/runtimepy/data/js/classes/App.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/classes/ChannelTable.js` & `runtimepy-4.0.4/runtimepy/data/js/classes/ChannelTable.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/classes/JsonConnection.js` & `runtimepy-4.0.4/runtimepy/data/js/classes/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/classes/Plot.js` & `runtimepy-4.0.4/runtimepy/data/js/classes/Plot.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/classes/PlotManager.js` & `runtimepy-4.0.4/runtimepy/data/js/classes/PlotManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/classes/TabFilter.js` & `runtimepy-4.0.4/runtimepy/data/js/classes/TabFilter.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/classes/TabInterface.js` & `runtimepy-4.0.4/runtimepy/data/js/classes/TabInterface.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/classes/WindowHashManager.js` & `runtimepy-4.0.4/runtimepy/data/js/classes/WindowHashManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/tab/sound.js` & `runtimepy-4.0.4/runtimepy/data/js/tab/sound.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/unused/pyodide.js` & `runtimepy-4.0.4/runtimepy/data/js/unused/pyodide.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/util.js` & `runtimepy-4.0.4/runtimepy/data/js/util.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/js/worker.js` & `runtimepy-4.0.4/runtimepy/data/js/worker.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-4.0.4/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-4.0.4/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/schemas/FindFile.yaml` & `runtimepy-4.0.4/runtimepy/data/schemas/FindFile.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/data/server_base.yaml` & `runtimepy-4.0.4/runtimepy/data/server_base.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/entry.py` & `runtimepy-4.0.4/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/enum/__init__.py` & `runtimepy-4.0.4/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/enum/registry.py` & `runtimepy-4.0.4/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/enum/types.py` & `runtimepy-4.0.4/runtimepy/enum/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/mapping.py` & `runtimepy-4.0.4/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/metrics/channel.py` & `runtimepy-4.0.4/runtimepy/metrics/channel.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/metrics/connection.py` & `runtimepy-4.0.4/runtimepy/metrics/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/metrics/task.py` & `runtimepy-4.0.4/runtimepy/metrics/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/mixins/async_command.py` & `runtimepy-4.0.4/runtimepy/mixins/async_command.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/mixins/enum.py` & `runtimepy-4.0.4/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/mixins/environment.py` & `runtimepy-4.0.4/runtimepy/mixins/environment.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/mixins/finalize.py` & `runtimepy-4.0.4/runtimepy/mixins/finalize.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/mixins/logging.py` & `runtimepy-4.0.4/runtimepy/mixins/logging.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/mixins/regex.py` & `runtimepy-4.0.4/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/__init__.py` & `runtimepy-4.0.4/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/apps/__init__.py` & `runtimepy-4.0.4/runtimepy/net/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/__init__.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/base.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,16 +242,14 @@
 
             # Run application, but only if all the registered connections are
             # still alive after initialization.
             if not check_connections or not any(
                 x.disabled for x in self._connections.values()
             ):
                 async with _AsyncExitStack() as stack:
-                    self.logger.info("Application starting.")
-
                     info = AppInfo(
                         self.logger,
                         stack,
                         self._connections,
                         self.manager,
                         self._namespace,
                         self.stop_sig,
@@ -332,21 +330,21 @@
 
         pairs = [(app, info.with_new_logger(app.__name__)) for app in apps]
 
         # Pre-populate stage results with "not run" placeholders.
         stage_results = [AppResult(app.__name__) for app in apps]
 
         for _, inf in pairs:
-            inf.logger.info("Starting.")
+            inf.logger.debug("Starting.")
 
         total = 0
         try:
             results = await _asyncio.gather(*(app(inf) for app, inf in pairs))
             for idx, result in enumerate(results):
-                pairs[idx][1].logger.info("Returned %d.", result)
+                pairs[idx][1].logger.debug("Returned %d.", result)
                 total += result
 
                 # Capture a normal result.
                 stage_results[idx] = AppResult(
                     apps[idx].__name__, ResultState.from_int(result), result
                 )
```

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/config/__init__.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/config/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/config/codec.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/config/codec.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/config/util.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/config/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/factory/task.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/imports/__init__.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/imports/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/imports/util.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/imports/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/info.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/result.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/struct/__init__.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/task.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/tcp/__init__.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/tcp/json.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/tcp/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/udp.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/arbiter/websocket.py` & `runtimepy-4.0.4/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/backoff.py` & `runtimepy-4.0.4/runtimepy/net/backoff.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/connection.py` & `runtimepy-4.0.4/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/factories/__init__.py` & `runtimepy-4.0.4/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/http/__init__.py` & `runtimepy-4.0.4/runtimepy/net/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/http/common.py` & `runtimepy-4.0.4/runtimepy/net/http/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/http/header.py` & `runtimepy-4.0.4/runtimepy/net/http/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/http/request_target.py` & `runtimepy-4.0.4/runtimepy/net/http/request_target.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/http/response.py` & `runtimepy-4.0.4/runtimepy/net/http/response.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/http/state.py` & `runtimepy-4.0.4/runtimepy/net/http/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/http/version.py` & `runtimepy-4.0.4/runtimepy/net/http/version.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/manager.py` & `runtimepy-4.0.4/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/mixin.py` & `runtimepy-4.0.4/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/__init__.py` & `runtimepy-4.0.4/runtimepy/net/server/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/__init__.py` & `runtimepy-4.0.4/runtimepy/net/server/app/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/base.py` & `runtimepy-4.0.4/runtimepy/net/server/app/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/bootstrap/__init__.py` & `runtimepy-4.0.4/runtimepy/net/server/app/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/bootstrap/elements.py` & `runtimepy-4.0.4/runtimepy/net/server/app/bootstrap/elements.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/bootstrap/tabs.py` & `runtimepy-4.0.4/runtimepy/net/server/app/bootstrap/tabs.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/create.py` & `runtimepy-4.0.4/runtimepy/net/server/app/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/elements.py` & `runtimepy-4.0.4/runtimepy/net/server/app/elements.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/env/__init__.py` & `runtimepy-4.0.4/runtimepy/net/server/app/env/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/env/modal.py` & `runtimepy-4.0.4/runtimepy/net/server/app/env/modal.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/env/tab/__init__.py` & `runtimepy-4.0.4/runtimepy/net/server/app/env/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/env/tab/base.py` & `runtimepy-4.0.4/runtimepy/net/server/app/env/tab/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/env/tab/html.py` & `runtimepy-4.0.4/runtimepy/net/server/app/env/tab/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/env/tab/message.py` & `runtimepy-4.0.4/runtimepy/net/server/app/env/tab/message.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/env/widgets.py` & `runtimepy-4.0.4/runtimepy/net/server/app/env/widgets.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/files.py` & `runtimepy-4.0.4/runtimepy/net/server/app/files.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/placeholder.py` & `runtimepy-4.0.4/runtimepy/net/server/app/placeholder.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/sound.py` & `runtimepy-4.0.4/runtimepy/net/server/app/sound.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/app/tab.py` & `runtimepy-4.0.4/runtimepy/net/server/app/tab.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/html.py` & `runtimepy-4.0.4/runtimepy/net/server/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/json.py` & `runtimepy-4.0.4/runtimepy/net/server/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/struct/__init__.py` & `runtimepy-4.0.4/runtimepy/net/server/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/websocket/__init__.py` & `runtimepy-4.0.4/runtimepy/net/server/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/server/websocket/state.py` & `runtimepy-4.0.4/runtimepy/net/server/websocket/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/stream/__init__.py` & `runtimepy-4.0.4/runtimepy/net/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/stream/base.py` & `runtimepy-4.0.4/runtimepy/net/stream/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/stream/json/base.py` & `runtimepy-4.0.4/runtimepy/net/stream/json/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/stream/json/handlers.py` & `runtimepy-4.0.4/runtimepy/net/stream/json/handlers.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/stream/json/types.py` & `runtimepy-4.0.4/runtimepy/net/stream/json/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/stream/string.py` & `runtimepy-4.0.4/runtimepy/net/stream/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/tcp/connection.py` & `runtimepy-4.0.4/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/tcp/create.py` & `runtimepy-4.0.4/runtimepy/net/tcp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/tcp/http/__init__.py` & `runtimepy-4.0.4/runtimepy/net/tcp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/tcp/protocol.py` & `runtimepy-4.0.4/runtimepy/net/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-4.0.4/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-4.0.4/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/udp/connection.py` & `runtimepy-4.0.4/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/udp/create.py` & `runtimepy-4.0.4/runtimepy/net/udp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/udp/protocol.py` & `runtimepy-4.0.4/runtimepy/net/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/util.py` & `runtimepy-4.0.4/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/net/websocket/connection.py` & `runtimepy-4.0.4/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/__init__.py` & `runtimepy-4.0.4/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/array/__init__.py` & `runtimepy-4.0.4/runtimepy/primitives/array/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/base.py` & `runtimepy-4.0.4/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/bool.py` & `runtimepy-4.0.4/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/byte_order.py` & `runtimepy-4.0.4/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/field/__init__.py` & `runtimepy-4.0.4/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/field/fields.py` & `runtimepy-4.0.4/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-4.0.4/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/field/manager/base.py` & `runtimepy-4.0.4/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/float.py` & `runtimepy-4.0.4/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/int.py` & `runtimepy-4.0.4/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/scaling.py` & `runtimepy-4.0.4/runtimepy/primitives/scaling.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/serializable/base.py` & `runtimepy-4.0.4/runtimepy/primitives/serializable/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/serializable/fixed.py` & `runtimepy-4.0.4/runtimepy/primitives/serializable/fixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/serializable/prefixed.py` & `runtimepy-4.0.4/runtimepy/primitives/serializable/prefixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/string.py` & `runtimepy-4.0.4/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/types/__init__.py` & `runtimepy-4.0.4/runtimepy/primitives/types/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/types/base.py` & `runtimepy-4.0.4/runtimepy/primitives/types/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/types/bool.py` & `runtimepy-4.0.4/runtimepy/primitives/types/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/types/bounds.py` & `runtimepy-4.0.4/runtimepy/primitives/types/bounds.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/types/float.py` & `runtimepy-4.0.4/runtimepy/primitives/types/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/primitives/types/int.py` & `runtimepy-4.0.4/runtimepy/primitives/types/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/registry/__init__.py` & `runtimepy-4.0.4/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/registry/bool.py` & `runtimepy-4.0.4/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/registry/item.py` & `runtimepy-4.0.4/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/registry/name.py` & `runtimepy-4.0.4/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/schemas.py` & `runtimepy-4.0.4/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/struct/__init__.py` & `runtimepy-4.0.4/runtimepy/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/task/asynchronous.py` & `runtimepy-4.0.4/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/task/basic/manager.py` & `runtimepy-4.0.4/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/task/basic/periodic.py` & `runtimepy-4.0.4/runtimepy/task/basic/periodic.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def set_period(self, period_s: float = None) -> bool:
         """Attempt to set a new period for this task."""
 
         result = False
 
         if period_s is not None and self.period_s != period_s:
             self.period_s.value = period_s
-            self.logger.info(
+            self.logger.debug(
                 "Task rate set to %s.", _rate_str(self.period_s.value)
             )
             result = True
 
         return result
 
     @_abstractmethod
@@ -156,18 +156,18 @@
 
             if self._enabled:
                 try:
                     await _asyncio.sleep(
                         max(self.period_s.value - iter_time.value, 0)
                     )
                 except _asyncio.CancelledError:
-                    self.logger.info("Task was cancelled.")
+                    self.logger.debug("Task was cancelled.")
                     self.disable()
 
-        self.logger.info("Task completed.")
+        self.logger.debug("Task completed.")
 
     async def stop_extra(self) -> None:
         """Extra actions to perform when this task is stopping."""
 
     async def stop(self) -> bool:
         """Wait for this task to stop running (if it is)."""
```

### Comparing `runtimepy-4.0.3/runtimepy/task/sample.py` & `runtimepy-4.0.4/runtimepy/task/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/task/trig/__init__.py` & `runtimepy-4.0.4/runtimepy/task/trig/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/tui/channels/__init__.py` & `runtimepy-4.0.4/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/tui/cursor.py` & `runtimepy-4.0.4/runtimepy/tui/cursor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/tui/mixin.py` & `runtimepy-4.0.4/runtimepy/tui/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/tui/mock.py` & `runtimepy-4.0.4/runtimepy/tui/mock.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy/tui/task.py` & `runtimepy-4.0.4/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/runtimepy.egg-info/PKG-INFO` & `runtimepy-4.0.4/runtimepy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.0.3
+Version: 4.0.4
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psutil
-Requires-Dist: svgen>=0.6.5
 Requires-Dist: vcorelib>=3.2.2
+Requires-Dist: svgen>=0.6.5
 Requires-Dist: websockets
+Requires-Dist: psutil
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=b46d92eb818e462d978d8fcf87af04ed
+    hash=901fe42416b14697d7706086dcd4e0a4
     =====================================
 -->
 
-# runtimepy ([4.0.3](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.0.4](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.0.3/runtimepy.egg-info/SOURCES.txt` & `runtimepy-4.0.4/runtimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/setup.py` & `runtimepy-4.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/tests/test_entry.py` & `runtimepy-4.0.4/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.0.3/tests/test_mapping.py` & `runtimepy-4.0.4/tests/test_mapping.py`

 * *Files identical despite different names*
