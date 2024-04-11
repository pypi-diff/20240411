# Comparing `tmp/spin-sdk-3.0.0.tar.gz` & `tmp/spin-sdk-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin-sdk-3.0.0.tar", last modified: Wed Apr  3 21:43:43 2024, max compression
+gzip compressed data, was "spin-sdk-3.1.0.tar", last modified: Thu Apr 11 16:43:18 2024, max compression
```

## Comparing `spin-sdk-3.0.0.tar` & `spin-sdk-3.1.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.637630 spin-sdk-3.0.0/
--rw-r--r--   0 dicej      (501) staff       (20)    11602 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/LICENSE
--rw-r--r--   0 dicej      (501) staff       (20)       53 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/MANIFEST.in
--rw-r--r--   0 dicej      (501) staff       (20)    16202 2024-04-03 21:43:43.637439 spin-sdk-3.0.0/PKG-INFO
--rw-r--r--   0 dicej      (501) staff       (20)     2380 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/README.md
--rw-r--r--   0 dicej      (501) staff       (20)      657 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/pyproject.toml
--rw-r--r--   0 dicej      (501) staff       (20)       38 2024-04-03 21:43:43.637662 spin-sdk-3.0.0/setup.cfg
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.624387 spin-sdk-3.0.0/src/
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.627451 spin-sdk-3.0.0/src/spin_sdk/
--rw-r--r--   0 dicej      (501) staff       (20)      282 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/__init__.py
--rw-r--r--   0 dicej      (501) staff       (20)       39 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/componentize-py.toml
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.628326 spin-sdk-3.0.0/src/spin_sdk/http/
--rw-r--r--   0 dicej      (501) staff       (20)     7459 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/http/__init__.py
--rw-r--r--   0 dicej      (501) staff       (20)    12299 2024-04-03 21:21:04.000000 spin-sdk-3.0.0/src/spin_sdk/http/poll_loop.py
--rw-r--r--   0 dicej      (501) staff       (20)     1816 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/key_value.py
--rw-r--r--   0 dicej      (501) staff       (20)     2222 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/llm.py
--rw-r--r--   0 dicej      (501) staff       (20)      989 2024-04-03 21:41:05.000000 spin-sdk-3.0.0/src/spin_sdk/mqtt.py
--rw-r--r--   0 dicej      (501) staff       (20)      561 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/mysql.py
--rw-r--r--   0 dicej      (501) staff       (20)      573 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/postgres.py
--rw-r--r--   0 dicej      (501) staff       (20)        0 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/py.typed
--rw-r--r--   0 dicej      (501) staff       (20)      795 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/redis.py
--rw-r--r--   0 dicej      (501) staff       (20)     1416 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/sqlite.py
--rw-r--r--   0 dicej      (501) staff       (20)      195 2024-02-28 16:52:28.000000 spin-sdk-3.0.0/src/spin_sdk/variables.py
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.630327 spin-sdk-3.0.0/src/spin_sdk/wit/
--rw-r--r--   0 dicej      (501) staff       (20)      356 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/__init__.py
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.625069 spin-sdk-3.0.0/src/spin_sdk/wit/deps/
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.631348 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/
--rw-r--r--   0 dicej      (501) staff       (20)       77 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/command.wit
--rw-r--r--   0 dicej      (501) staff       (20)      709 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/environment.wit
--rw-r--r--   0 dicej      (501) staff       (20)      107 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/exit.wit
--rw-r--r--   0 dicej      (501) staff       (20)      445 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/imports.wit
--rw-r--r--   0 dicej      (501) staff       (20)       66 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/run.wit
--rw-r--r--   0 dicej      (501) staff       (20)      316 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/stdio.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1677 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/terminal.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.631710 spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/
--rw-r--r--   0 dicej      (501) staff       (20)     1525 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/monotonic-clock.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1674 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/wall-clock.wit
--rw-r--r--   0 dicej      (501) staff       (20)       97 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/world.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.632108 spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/
--rw-r--r--   0 dicej      (501) staff       (20)      213 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/preopens.wit
--rw-r--r--   0 dicej      (501) staff       (20)    27621 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/types.wit
--rw-r--r--   0 dicej      (501) staff       (20)       89 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/world.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.632469 spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/
--rw-r--r--   0 dicej      (501) staff       (20)     1807 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/handler.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1439 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/proxy.wit
--rw-r--r--   0 dicej      (501) staff       (20)    24187 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/types.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.633232 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/
--rw-r--r--   0 dicej      (501) staff       (20)     1444 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/error.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1590 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/poll.wit
--rw-r--r--   0 dicej      (501) staff       (20)    12096 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/streams.wit
--rw-r--r--   0 dicej      (501) staff       (20)       79 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/world.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.633717 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/
--rw-r--r--   0 dicej      (501) staff       (20)     1104 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/insecure-seed.wit
--rw-r--r--   0 dicej      (501) staff       (20)      863 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/insecure.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1149 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/random.wit
--rw-r--r--   0 dicej      (501) staff       (20)      112 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/world.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.634743 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/
--rw-r--r--   0 dicej      (501) staff       (20)      222 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/instance-network.wit
--rw-r--r--   0 dicej      (501) staff       (20)     2603 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/ip-name-lookup.wit
--rw-r--r--   0 dicej      (501) staff       (20)     4175 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/network.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1487 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/tcp-create-socket.wit
--rw-r--r--   0 dicej      (501) staff       (20)    20199 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/tcp.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1477 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/udp-create-socket.wit
--rw-r--r--   0 dicej      (501) staff       (20)    15189 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/udp.wit
--rw-r--r--   0 dicej      (501) staff       (20)      215 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/world.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.635021 spin-sdk-3.0.0/src/spin_sdk/wit/deps/spin@unversioned/
--rw-r--r--   0 dicej      (501) staff       (20)      191 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/spin@unversioned/inbound-redis.wit
--rw-r--r--   0 dicej      (501) staff       (20)      462 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/spin@unversioned/redis-types.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.635337 spin-sdk-3.0.0/src/spin_sdk/wit/exports/
--rw-r--r--   0 dicej      (501) staff       (20)     1395 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/exports/__init__.py
--rw-r--r--   0 dicej      (501) staff       (20)      246 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/exports/inbound_redis.py
--rw-r--r--   0 dicej      (501) staff       (20)      386 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/exports/incoming_handler.py
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.637075 spin-sdk-3.0.0/src/spin_sdk/wit/imports/
--rw-r--r--   0 dicej      (501) staff       (20)        0 2024-04-02 19:59:36.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/__init__.py
--rw-r--r--   0 dicej      (501) staff       (20)     1871 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/error.py
--rw-r--r--   0 dicej      (501) staff       (20)     2751 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/key_value.py
--rw-r--r--   0 dicej      (501) staff       (20)     2010 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/llm.py
--rw-r--r--   0 dicej      (501) staff       (20)     1472 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/monotonic_clock.py
--rw-r--r--   0 dicej      (501) staff       (20)     1621 2024-04-03 21:41:05.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/mqtt.py
--rw-r--r--   0 dicej      (501) staff       (20)     1476 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/mysql.py
--rw-r--r--   0 dicej      (501) staff       (20)     1143 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/outgoing_handler.py
--rw-r--r--   0 dicej      (501) staff       (20)     2135 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/poll.py
--rw-r--r--   0 dicej      (501) staff       (20)     1451 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/postgres.py
--rw-r--r--   0 dicej      (501) staff       (20)     3447 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/rdbms_types.py
--rw-r--r--   0 dicej      (501) staff       (20)     4488 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/redis.py
--rw-r--r--   0 dicej      (501) staff       (20)      968 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/redis_types.py
--rw-r--r--   0 dicej      (501) staff       (20)     2354 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/sqlite.py
--rw-r--r--   0 dicej      (501) staff       (20)    12935 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/streams.py
--rw-r--r--   0 dicej      (501) staff       (20)    33255 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/types.py
--rw-r--r--   0 dicej      (501) staff       (20)      898 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/variables.py
--rw-r--r--   0 dicej      (501) staff       (20)     1644 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/key-value.wit
--rw-r--r--   0 dicej      (501) staff       (20)     2313 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/llm.wit
--rw-r--r--   0 dicej      (501) staff       (20)      916 2024-04-03 21:41:05.000000 spin-sdk-3.0.0/src/spin_sdk/wit/mqtt.wit
--rw-r--r--   0 dicej      (501) staff       (20)      556 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/mysql.wit
--rw-r--r--   0 dicej      (501) staff       (20)      537 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/postgres.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1462 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/rdbms-types.wit
--rw-r--r--   0 dicej      (501) staff       (20)     2452 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/redis.wit
--rw-r--r--   0 dicej      (501) staff       (20)      466 2024-04-03 21:41:05.000000 spin-sdk-3.0.0/src/spin_sdk/wit/spin.wit
--rw-r--r--   0 dicej      (501) staff       (20)     1600 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/sqlite.wit
--rw-r--r--   0 dicej      (501) staff       (20)      452 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/types.py
--rw-r--r--   0 dicej      (501) staff       (20)      658 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/variables.wit
-drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.637240 spin-sdk-3.0.0/src/spin_sdk.egg-info/
--rw-r--r--   0 dicej      (501) staff       (20)    16202 2024-04-03 21:43:43.000000 spin-sdk-3.0.0/src/spin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dicej      (501) staff       (20)     3024 2024-04-03 21:43:43.000000 spin-sdk-3.0.0/src/spin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dicej      (501) staff       (20)        1 2024-04-03 21:43:43.000000 spin-sdk-3.0.0/src/spin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dicej      (501) staff       (20)        9 2024-04-03 21:43:43.000000 spin-sdk-3.0.0/src/spin_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.897050 spin-sdk-3.1.0/
+-rw-r--r--   0 dicej      (501) staff       (20)    11602 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/LICENSE
+-rw-r--r--   0 dicej      (501) staff       (20)       53 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/MANIFEST.in
+-rw-r--r--   0 dicej      (501) staff       (20)    16205 2024-04-11 16:43:18.896885 spin-sdk-3.1.0/PKG-INFO
+-rw-r--r--   0 dicej      (501) staff       (20)     2383 2024-04-11 16:11:56.000000 spin-sdk-3.1.0/README.md
+-rw-r--r--   0 dicej      (501) staff       (20)      657 2024-04-11 16:12:02.000000 spin-sdk-3.1.0/pyproject.toml
+-rw-r--r--   0 dicej      (501) staff       (20)       38 2024-04-11 16:43:18.897081 spin-sdk-3.1.0/setup.cfg
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.886520 spin-sdk-3.1.0/src/
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.888871 spin-sdk-3.1.0/src/spin_sdk/
+-rw-r--r--   0 dicej      (501) staff       (20)      282 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/__init__.py
+-rw-r--r--   0 dicej      (501) staff       (20)       39 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/componentize-py.toml
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.889540 spin-sdk-3.1.0/src/spin_sdk/http/
+-rw-r--r--   0 dicej      (501) staff       (20)     7208 2024-04-11 16:09:17.000000 spin-sdk-3.1.0/src/spin_sdk/http/__init__.py
+-rw-r--r--   0 dicej      (501) staff       (20)    12326 2024-04-11 16:09:17.000000 spin-sdk-3.1.0/src/spin_sdk/http/poll_loop.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1816 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/key_value.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2222 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/llm.py
+-rw-r--r--   0 dicej      (501) staff       (20)      989 2024-04-03 21:41:05.000000 spin-sdk-3.1.0/src/spin_sdk/mqtt.py
+-rw-r--r--   0 dicej      (501) staff       (20)      561 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/mysql.py
+-rw-r--r--   0 dicej      (501) staff       (20)      573 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/postgres.py
+-rw-r--r--   0 dicej      (501) staff       (20)        0 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/py.typed
+-rw-r--r--   0 dicej      (501) staff       (20)      795 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/redis.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1416 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/sqlite.py
+-rw-r--r--   0 dicej      (501) staff       (20)      195 2024-02-28 16:52:28.000000 spin-sdk-3.1.0/src/spin_sdk/variables.py
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.890776 spin-sdk-3.1.0/src/spin_sdk/wit/
+-rw-r--r--   0 dicej      (501) staff       (20)      356 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/__init__.py
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.887131 spin-sdk-3.1.0/src/spin_sdk/wit/deps/
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.891438 spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/
+-rw-r--r--   0 dicej      (501) staff       (20)       77 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/command.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      709 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/environment.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      107 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/exit.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      445 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/imports.wit
+-rw-r--r--   0 dicej      (501) staff       (20)       66 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/run.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      316 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/stdio.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1677 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/terminal.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.891754 spin-sdk-3.1.0/src/spin_sdk/wit/deps/clocks/
+-rw-r--r--   0 dicej      (501) staff       (20)     1525 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/clocks/monotonic-clock.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1674 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/clocks/wall-clock.wit
+-rw-r--r--   0 dicej      (501) staff       (20)       97 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/clocks/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.892094 spin-sdk-3.1.0/src/spin_sdk/wit/deps/filesystem/
+-rw-r--r--   0 dicej      (501) staff       (20)      213 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/filesystem/preopens.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    27621 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/filesystem/types.wit
+-rw-r--r--   0 dicej      (501) staff       (20)       89 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/filesystem/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.892424 spin-sdk-3.1.0/src/spin_sdk/wit/deps/http/
+-rw-r--r--   0 dicej      (501) staff       (20)     1807 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/http/handler.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1439 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/http/proxy.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    24187 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/http/types.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.892836 spin-sdk-3.1.0/src/spin_sdk/wit/deps/io/
+-rw-r--r--   0 dicej      (501) staff       (20)     1444 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/io/error.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1590 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/io/poll.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    12096 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/io/streams.wit
+-rw-r--r--   0 dicej      (501) staff       (20)       79 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/io/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.893287 spin-sdk-3.1.0/src/spin_sdk/wit/deps/random/
+-rw-r--r--   0 dicej      (501) staff       (20)     1104 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/random/insecure-seed.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      863 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/random/insecure.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1149 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/random/random.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      112 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/random/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.894123 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/
+-rw-r--r--   0 dicej      (501) staff       (20)      222 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/instance-network.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     2603 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/ip-name-lookup.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     4175 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/network.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1487 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/tcp-create-socket.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    20199 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/tcp.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1477 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/udp-create-socket.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    15189 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/udp.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      215 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.894335 spin-sdk-3.1.0/src/spin_sdk/wit/deps/spin@unversioned/
+-rw-r--r--   0 dicej      (501) staff       (20)      191 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/spin@unversioned/inbound-redis.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      462 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/deps/spin@unversioned/redis-types.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.894652 spin-sdk-3.1.0/src/spin_sdk/wit/exports/
+-rw-r--r--   0 dicej      (501) staff       (20)     1395 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/exports/__init__.py
+-rw-r--r--   0 dicej      (501) staff       (20)      246 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/exports/inbound_redis.py
+-rw-r--r--   0 dicej      (501) staff       (20)      386 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/exports/incoming_handler.py
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.896486 spin-sdk-3.1.0/src/spin_sdk/wit/imports/
+-rw-r--r--   0 dicej      (501) staff       (20)        0 2024-04-02 19:59:36.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/__init__.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1871 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/error.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2751 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/key_value.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2010 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/llm.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1472 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/monotonic_clock.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1621 2024-04-03 21:41:05.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/mqtt.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1476 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/mysql.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1143 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/outgoing_handler.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2135 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/poll.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1451 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/postgres.py
+-rw-r--r--   0 dicej      (501) staff       (20)     3447 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/rdbms_types.py
+-rw-r--r--   0 dicej      (501) staff       (20)     4488 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/redis.py
+-rw-r--r--   0 dicej      (501) staff       (20)      968 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/redis_types.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2354 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/sqlite.py
+-rw-r--r--   0 dicej      (501) staff       (20)    12935 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/streams.py
+-rw-r--r--   0 dicej      (501) staff       (20)    33255 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/types.py
+-rw-r--r--   0 dicej      (501) staff       (20)      898 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/imports/variables.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1644 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/key-value.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     2313 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/llm.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      916 2024-04-03 21:41:05.000000 spin-sdk-3.1.0/src/spin_sdk/wit/mqtt.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      556 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/mysql.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      537 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/postgres.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1462 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/rdbms-types.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     2452 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/redis.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      466 2024-04-03 21:41:05.000000 spin-sdk-3.1.0/src/spin_sdk/wit/spin.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1600 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/sqlite.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      452 2024-04-03 21:20:56.000000 spin-sdk-3.1.0/src/spin_sdk/wit/types.py
+-rw-r--r--   0 dicej      (501) staff       (20)      658 2024-02-16 14:45:39.000000 spin-sdk-3.1.0/src/spin_sdk/wit/variables.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-11 16:43:18.896697 spin-sdk-3.1.0/src/spin_sdk.egg-info/
+-rw-r--r--   0 dicej      (501) staff       (20)    16205 2024-04-11 16:43:18.000000 spin-sdk-3.1.0/src/spin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dicej      (501) staff       (20)     3024 2024-04-11 16:43:18.000000 spin-sdk-3.1.0/src/spin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dicej      (501) staff       (20)        1 2024-04-11 16:43:18.000000 spin-sdk-3.1.0/src/spin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dicej      (501) staff       (20)        9 2024-04-11 16:43:18.000000 spin-sdk-3.1.0/src/spin_sdk.egg-info/top_level.txt
```

### Comparing `spin-sdk-3.0.0/LICENSE` & `spin-sdk-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/PKG-INFO` & `spin-sdk-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-sdk
-Version: 3.0.0
+Version: 3.1.0
 Summary: Experimental SDK for Spin and Componentize-Py
 Author-email: Fermyon Engineering <engineering@fermyon.com>
 Maintainer-email: Fermyon Engineering <engineering@fermyon.com>
 License:                               Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
@@ -232,15 +232,15 @@
 
 This is an SDK for creating [Spin](https://github.com/fermyon/spin) apps using Python.
 
 Note that this SDK supersedes an earlier, experimental version, which may be
 found in the [old-sdk](https://github.com/fermyon/spin-python-sdk/tree/old-sdk)
 branch.
 
-## [API Documentation](https://fermyon.github.io/spin-python-sdk/index.html)
+## [API Documentation](https://fermyon.github.io/spin-python-sdk/v3/index.html)
 
 ## Example
 
 ### Prerequisites
 
 - [Python 3.10 or later and pip](https://www.python.org/downloads/)
 - [componentize-py](https://pypi.org/project/componentize-py/)
@@ -250,15 +250,15 @@
 
 Once you have Python and pip installed, you can use the latter to create and
 enter a virtual environment and then install the desired packages
 
 ```shell
 python -m venv .venv
 source .venv/bin/activate
-pip install componentize-py==0.13.1 spin-sdk==3.0.0 mypy==1.8.0
+pip install componentize-py==0.13.2 spin-sdk==3.1.0 mypy==1.8.0
 ```
 
 ### Hello, World
 
 A minimal app requires two files: a `spin.toml` and a Python script, which we'll
 name `app.py`:
```

### Comparing `spin-sdk-3.0.0/README.md` & `spin-sdk-3.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This is an SDK for creating [Spin](https://github.com/fermyon/spin) apps using Python.
 
 Note that this SDK supersedes an earlier, experimental version, which may be
 found in the [old-sdk](https://github.com/fermyon/spin-python-sdk/tree/old-sdk)
 branch.
 
-## [API Documentation](https://fermyon.github.io/spin-python-sdk/index.html)
+## [API Documentation](https://fermyon.github.io/spin-python-sdk/v3/index.html)
 
 ## Example
 
 ### Prerequisites
 
 - [Python 3.10 or later and pip](https://www.python.org/downloads/)
 - [componentize-py](https://pypi.org/project/componentize-py/)
@@ -20,15 +20,15 @@
 
 Once you have Python and pip installed, you can use the latter to create and
 enter a virtual environment and then install the desired packages
 
 ```shell
 python -m venv .venv
 source .venv/bin/activate
-pip install componentize-py==0.13.1 spin-sdk==3.0.0 mypy==1.8.0
+pip install componentize-py==0.13.2 spin-sdk==3.1.0 mypy==1.8.0
 ```
 
 ### Hello, World
 
 A minimal app requires two files: a `spin.toml` and a Python script, which we'll
 name `app.py`:
```

### Comparing `spin-sdk-3.0.0/pyproject.toml` & `spin-sdk-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spin-sdk"
-version = "3.0.0"
+version = "3.1.0"
 description = "Experimental SDK for Spin and Componentize-Py"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [ { name = "Fermyon Engineering", email = "engineering@fermyon.com" } ]
 maintainers = [ { name = "Fermyon Engineering", email = "engineering@fermyon.com" } ]
 keywords = [ "webassembly", "wasm", "component", "spin" ]
```

### Comparing `spin-sdk-3.0.0/src/spin_sdk/http/__init__.py` & `spin-sdk-3.1.0/src/spin_sdk/http/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 """Module with helpers for wasi http"""
 
+import asyncio
 import traceback
-
+from spin_sdk.http import poll_loop
+from spin_sdk.http.poll_loop import PollLoop, Sink, Stream
 from spin_sdk.wit import exports
 from spin_sdk.wit.types import Ok, Err
-from spin_sdk.wit.imports import types, outgoing_handler
 from spin_sdk.wit.imports.types import (
-    Method, Method_Get, Method_Head, Method_Post, Method_Put, Method_Delete, Method_Connect, Method_Options,
+    IncomingResponse, Method, Method_Get, Method_Head, Method_Post, Method_Put, Method_Delete, Method_Connect, Method_Options,
     Method_Trace, Method_Patch, Method_Other, IncomingRequest, IncomingBody, ResponseOutparam, OutgoingResponse,
     Fields, Scheme, Scheme_Http, Scheme_Https, Scheme_Other, OutgoingRequest, OutgoingBody
 )
 from spin_sdk.wit.imports.streams import StreamError_Closed
 from dataclasses import dataclass
-from collections.abc import Mapping
+from collections.abc import MutableMapping
 from typing import Optional
 from urllib import parse
 
 @dataclass
 class Request:
     """An HTTP request"""
     method: str
     uri: str
-    headers: Mapping[str, str]
+    headers: MutableMapping[str, str]
     body: Optional[bytes]
 
 @dataclass
 class Response:
     """An HTTP response"""
     status: int
-    headers: Mapping[str, str]
+    headers: MutableMapping[str, str]
     body: Optional[bytes]
 
 class IncomingHandler(exports.IncomingHandler):
     """Simplified handler for incoming HTTP requests using blocking, buffered I/O."""
     
     def handle_request(self, request: Request) -> Response:
         """Handle an incoming HTTP request and return a response or raise an error"""
@@ -95,14 +96,18 @@
             traceback.print_exc()
 
             response = OutgoingResponse(Fields())
             response.set_status_code(500)
             ResponseOutparam.set(response_out, Ok(response))
             return
 
+        if simple_response.headers.get('content-length') is None:
+            content_length = len(simple_response.body) if simple_response.body is not None else 0
+            simple_response.headers['content-length'] = str(content_length)
+
         response = OutgoingResponse(Fields.from_list(list(map(
             lambda pair: (pair[0], bytes(pair[1], "utf-8")),
             simple_response.headers.items()
         ))))
         response_body = response.body()
         response.set_status_code(simple_response.status)
         ResponseOutparam.set(response_out, Ok(response))
@@ -115,15 +120,20 @@
                 response_stream.blocking_write_and_flush(simple_response.body[offset:offset+count])
                 offset += count
         response_stream.__exit__()
         OutgoingBody.finish(response_body, None)
     
 def send(request: Request) -> Response:
     """Send an HTTP request and return a response or raise an error"""
+    loop = PollLoop()
+    asyncio.set_event_loop(loop)
+    return loop.run_until_complete(send_async(request))
+    
 
+async def send_async(request: Request) -> Response:
     match request.method:
         case "GET":
             method: Method = Method_Get()
         case "HEAD":
             method = Method_Head()
         case "POST":
             method = Method_Post()
@@ -148,59 +158,49 @@
         case "http":
             scheme: Scheme = Scheme_Http()
         case "https":
             scheme = Scheme_Https()
         case _:
             scheme = Scheme_Other(url_parsed.scheme)
 
-    outgoing_request = OutgoingRequest(Fields.from_list(list(map(
+    if request.headers.get('content-length') is None:
+        content_length = len(request.body) if request.body is not None else 0
+        request.headers['content-length'] = str(content_length)
+
+    headers = list(map(
         lambda pair: (pair[0], bytes(pair[1], "utf-8")),
         request.headers.items()
-    ))))
+    ))
+
+    outgoing_request = OutgoingRequest(Fields.from_list(headers))
     outgoing_request.set_method(method)
     outgoing_request.set_scheme(scheme)
     outgoing_request.set_authority(url_parsed.netloc)
     outgoing_request.set_path_with_query(url_parsed.path)
 
-    if request.body is not None:
-        raise NotImplementedError("todo: handle outgoing request bodies")
+    outgoing_body = request.body if request.body is not None else bytearray()
+    sink = Sink(outgoing_request.body())
+    incoming_response: IncomingResponse = (await asyncio.gather(
+        poll_loop.send(outgoing_request),
+        sink.send(outgoing_body)
+    ))[0]
 
-    future = outgoing_handler.handle(outgoing_request, None)
-    pollable = future.subscribe()
+    sink.close()
 
+    response_body = Stream(incoming_response.consume())
+    body = bytearray()
     while True:
-        response = future.get()
-        if response is None:
-            pollable.block()
+        chunk = await response_body.next()
+        if chunk is None:
+            simple_response = Response(
+                incoming_response.status(),
+                dict(map(
+                    lambda pair: (pair[0], str(pair[1], "utf-8")),
+                    incoming_response.headers().entries()
+                )),
+                bytes(body)
+            )
+            incoming_response.__exit__()
+            return simple_response
         else:
-            pollable.__exit__()
-            future.__exit__()
-            
-            if isinstance(response, Ok):
-                if isinstance(response.value, Ok):
-                    response_value = response.value.value
-                    response_body = response_value.consume()
-                    response_stream = response_body.stream()
-                    body = bytearray()
-                    while True:
-                        try:
-                            body += response_stream.blocking_read(16 * 1024)
-                        except Err as e:
-                            if isinstance(e.value, StreamError_Closed):
-                                response_stream.__exit__()
-                                IncomingBody.finish(response_body)
-                                simple_response = Response(
-                                    response_value.status(),
-                                    dict(map(
-                                        lambda pair: (pair[0], str(pair[1], "utf-8")),
-                                        response_value.headers().entries()
-                                    )),
-                                    bytes(body)
-                                )
-                                response_value.__exit__()
-                                return simple_response
-                            else:
-                                raise e
-                else:
-                    raise response.value
-            else:
-                raise response
+            body += chunk
+
```

### Comparing `spin-sdk-3.0.0/src/spin_sdk/http/poll_loop.py` & `spin-sdk-3.1.0/src/spin_sdk/http/poll_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,18 +123,19 @@
 
     def run_until_complete(self, future):
         future = asyncio.ensure_future(future, loop=self)
 
         self.running = True
         asyncio.events._set_running_loop(self)
         while self.running and not future.done():
-            handle = self.handles[0]
-            self.handles = self.handles[1:]
-            if not handle._cancelled:
-                handle._run()
+            handles = self.handles
+            self.handles = []
+            for handle in handles:
+                if not handle._cancelled:
+                    handle._run()
                 
             if self.wakers:
                 [pollables, wakers] = list(map(list, zip(*self.wakers)))
                 
                 new_wakers = []
                 ready = [False] * len(pollables)
                 for index in poll.poll(pollables):
```

### Comparing `spin-sdk-3.0.0/src/spin_sdk/key_value.py` & `spin-sdk-3.1.0/src/spin_sdk/key_value.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/llm.py` & `spin-sdk-3.1.0/src/spin_sdk/llm.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/mqtt.py` & `spin-sdk-3.1.0/src/spin_sdk/mqtt.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/mysql.py` & `spin-sdk-3.1.0/src/spin_sdk/mysql.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/postgres.py` & `spin-sdk-3.1.0/src/spin_sdk/postgres.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/redis.py` & `spin-sdk-3.1.0/src/spin_sdk/redis.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/sqlite.py` & `spin-sdk-3.1.0/src/spin_sdk/sqlite.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/environment.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/environment.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/terminal.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/cli/terminal.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/monotonic-clock.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/clocks/monotonic-clock.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/wall-clock.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/clocks/wall-clock.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/types.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/filesystem/types.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/handler.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/http/handler.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/proxy.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/http/proxy.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/types.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/http/types.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/error.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/io/error.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/poll.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/io/poll.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/streams.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/io/streams.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/insecure-seed.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/random/insecure-seed.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/insecure.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/random/insecure.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/random.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/random/random.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/ip-name-lookup.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/ip-name-lookup.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/network.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/network.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/tcp-create-socket.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/tcp-create-socket.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/tcp.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/tcp.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/udp-create-socket.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/udp-create-socket.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/udp.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/deps/sockets/udp.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/exports/__init__.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/error.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/error.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/key_value.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/key_value.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/llm.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/llm.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/monotonic_clock.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/monotonic_clock.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/mqtt.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/mqtt.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/mysql.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/mysql.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/outgoing_handler.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/outgoing_handler.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/poll.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/poll.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/postgres.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/postgres.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/rdbms_types.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/rdbms_types.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/redis.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/redis.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/redis_types.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/redis_types.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/sqlite.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/sqlite.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/streams.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/streams.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/types.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/types.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/imports/variables.py` & `spin-sdk-3.1.0/src/spin_sdk/wit/imports/variables.py`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/key-value.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/key-value.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/llm.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/llm.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/mqtt.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/mqtt.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/mysql.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/mysql.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/postgres.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/postgres.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/rdbms-types.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/rdbms-types.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/redis.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/redis.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/sqlite.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/sqlite.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk/wit/variables.wit` & `spin-sdk-3.1.0/src/spin_sdk/wit/variables.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-3.0.0/src/spin_sdk.egg-info/PKG-INFO` & `spin-sdk-3.1.0/src/spin_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-sdk
-Version: 3.0.0
+Version: 3.1.0
 Summary: Experimental SDK for Spin and Componentize-Py
 Author-email: Fermyon Engineering <engineering@fermyon.com>
 Maintainer-email: Fermyon Engineering <engineering@fermyon.com>
 License:                               Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
@@ -232,15 +232,15 @@
 
 This is an SDK for creating [Spin](https://github.com/fermyon/spin) apps using Python.
 
 Note that this SDK supersedes an earlier, experimental version, which may be
 found in the [old-sdk](https://github.com/fermyon/spin-python-sdk/tree/old-sdk)
 branch.
 
-## [API Documentation](https://fermyon.github.io/spin-python-sdk/index.html)
+## [API Documentation](https://fermyon.github.io/spin-python-sdk/v3/index.html)
 
 ## Example
 
 ### Prerequisites
 
 - [Python 3.10 or later and pip](https://www.python.org/downloads/)
 - [componentize-py](https://pypi.org/project/componentize-py/)
@@ -250,15 +250,15 @@
 
 Once you have Python and pip installed, you can use the latter to create and
 enter a virtual environment and then install the desired packages
 
 ```shell
 python -m venv .venv
 source .venv/bin/activate
-pip install componentize-py==0.13.1 spin-sdk==3.0.0 mypy==1.8.0
+pip install componentize-py==0.13.2 spin-sdk==3.1.0 mypy==1.8.0
 ```
 
 ### Hello, World
 
 A minimal app requires two files: a `spin.toml` and a Python script, which we'll
 name `app.py`:
```

### Comparing `spin-sdk-3.0.0/src/spin_sdk.egg-info/SOURCES.txt` & `spin-sdk-3.1.0/src/spin_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

