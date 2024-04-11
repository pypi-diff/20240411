# Comparing `tmp/beer-garden-3.8.1.tar.gz` & `tmp/beer-garden-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/beer-garden-3.8.1.tar", last modified: Tue Dec  7 15:18:41 2021, max compression
+gzip compressed data, was "dist/beer-garden-3.9.0.tar", last modified: Wed Dec  8 18:50:01 2021, max compression
```

## Comparing `beer-garden-3.8.1.tar` & `beer-garden-3.9.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     3118 2021-12-07 15:18:41.000000 beer-garden-3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-12-07 15:18:22.000000 beer-garden-3.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2120 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/authorization.py
--rw-r--r--   0 runner    (1001) docker     (121)     9340 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/http/
--rw-r--r--   0 runner    (1001) docker     (121)    14348 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/http/authentication/
--rw-r--r--   0 runner    (1001) docker     (121)     5916 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/authentication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/http/authentication/login_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/authentication/login_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/authentication/login_handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/authentication/login_handlers/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/authentication/login_handlers/certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)     9833 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8318 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/authorization_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/
--rw-r--r--   0 runner    (1001) docker     (121)      674 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/forward.py
--rw-r--r--   0 runner    (1001) docker     (121)     7888 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/garden.py
--rw-r--r--   0 runner    (1001) docker     (121)     9917 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)    11993 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)    25052 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/request.py
--rw-r--r--   0 runner    (1001) docker     (121)    13001 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/system.py
--rw-r--r--   0 runner    (1001) docker     (121)     4382 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     4522 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/v1/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8203 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/chunk.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)    10439 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/publishers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/http/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/http/schemas/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/schemas/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/http/schemas/v1/token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/api/stomp/
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/stomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7181 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/stomp/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7468 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/api/stomp/transport.py
--rw-r--r--   0 runner    (1001) docker     (121)    15042 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     9668 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/authorization.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)    48930 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/db/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/db/mongo/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12932 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     5006 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/jobstore.py
--rw-r--r--   0 runner    (1001) docker     (121)    35977 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/motor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4257 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/pruner.py
--rw-r--r--   0 runner    (1001) docker     (121)    13937 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      449 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/db/mongo/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/events/
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/events/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/events/parent_procesors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/events/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)    17909 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/files.py
--rw-r--r--   0 runner    (1001) docker     (121)    10383 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/garden.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/local_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/local_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/local_plugins/env_help.py
--rw-r--r--   0 runner    (1001) docker     (121)    31544 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/local_plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7842 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/local_plugins/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     8377 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/namespace.py
--rw-r--r--   0 runner    (1001) docker     (121)    15461 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden/queue/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/queue/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    13399 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/queue/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3325 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/queues.py
--rw-r--r--   0 runner    (1001) docker     (121)    34999 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/role.py
--rw-r--r--   0 runner    (1001) docker     (121)    26090 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/router.py
--rw-r--r--   0 runner    (1001) docker     (121)    22757 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)    12807 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/systems.py
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-12-07 15:18:22.000000 beer-garden-3.8.1/beer_garden/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3118 2021-12-07 15:18:40.000000 beer-garden-3.8.1/beer_garden.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3334 2021-12-07 15:18:41.000000 beer-garden-3.8.1/beer_garden.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 15:18:40.000000 beer-garden-3.8.1/beer_garden.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      576 2021-12-07 15:18:40.000000 beer-garden-3.8.1/beer_garden.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      219 2021-12-07 15:18:40.000000 beer-garden-3.8.1/beer_garden.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-07 15:18:40.000000 beer-garden-3.8.1/beer_garden.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-12-07 15:18:41.000000 beer-garden-3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2021-12-07 15:18:22.000000 beer-garden-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     3118 2021-12-08 18:50:01.000000 beer-garden-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2021-12-08 18:49:46.000000 beer-garden-3.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2120 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9340 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/http/
+-rw-r--r--   0 runner    (1001) docker     (121)    14348 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/http/authentication/
+-rw-r--r--   0 runner    (1001) docker     (121)     5934 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/authentication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/http/authentication/login_handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/authentication/login_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/authentication/login_handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/authentication/login_handlers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7064 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/authentication/login_handlers/trusted_header.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9833 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1807 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8814 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/authorization_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2397 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3318 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1530 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2274 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/forward.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7888 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/garden.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9917 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12340 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3955 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25261 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13001 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4382 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4522 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/v1/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8203 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      983 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2655 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10439 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/publishers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/http/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/http/schemas/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/schemas/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/http/schemas/v1/token.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/api/stomp/
+-rw-r--r--   0 runner    (1001) docker     (121)     2448 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/stomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7181 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/stomp/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7468 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/api/stomp/transport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15042 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9668 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50682 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/db/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/db/mongo/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12932 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5006 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/jobstore.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36062 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/motor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4257 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13937 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      449 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/db/mongo/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/events/
+-rw-r--r--   0 runner    (1001) docker     (121)     3829 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/events/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/events/parent_procesors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2987 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/events/processors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17909 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/files.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10383 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/garden.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/local_plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/local_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/local_plugins/env_help.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31544 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/local_plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7842 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/local_plugins/runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8377 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4538 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2566 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15461 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden/queue/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/queue/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13399 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/queue/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3325 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/queues.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34999 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26090 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/router.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23309 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12807 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/systems.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-12-08 18:49:46.000000 beer-garden-3.9.0/beer_garden/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 18:50:01.000000 beer-garden-3.9.0/beer_garden.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3118 2021-12-08 18:50:00.000000 beer-garden-3.9.0/beer_garden.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3337 2021-12-08 18:50:00.000000 beer-garden-3.9.0/beer_garden.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-08 18:50:00.000000 beer-garden-3.9.0/beer_garden.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-12-08 18:50:00.000000 beer-garden-3.9.0/beer_garden.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-12-08 18:50:00.000000 beer-garden-3.9.0/beer_garden.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-08 18:50:00.000000 beer-garden-3.9.0/beer_garden.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-12-08 18:50:01.000000 beer-garden-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2021-12-08 18:49:46.000000 beer-garden-3.9.0/setup.py
```

### Comparing `beer-garden-3.8.1/PKG-INFO` & `beer-garden-3.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: beer-garden
-Version: 3.8.1
+Version: 3.9.0
 Summary: Beergarden Application
 Home-page: https://beer-garden.io
 Author: The Beer Garden Team
 Author-email: beer@beer-garden.io
 License: MIT
 Description: 
         ===========================
```

### Comparing `beer-garden-3.8.1/README.rst` & `beer-garden-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/__main__.py` & `beer-garden-3.9.0/beer_garden/__main__.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/authorization.py` & `beer-garden-3.9.0/beer_garden/api/authorization.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 
 class Permissions(Enum):
     """Defines the list of valid permission strings, mostly used for validation
     that the permissions assigned to roles are ones that beer garden recognizes.
     """
 
+    EVENT_FORWARD = "event:forward"
+
     JOB_CREATE = "job:create"
     JOB_READ = "job:read"
     JOB_UPDATE = "job:update"
     JOB_DELETE = "job:delete"
 
     GARDEN_CREATE = "garden:create"
     GARDEN_READ = "garden:read"
```

### Comparing `beer-garden-3.8.1/beer_garden/api/entry_point.py` & `beer-garden-3.9.0/beer_garden/api/entry_point.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/__init__.py` & `beer-garden-3.9.0/beer_garden/api/http/__init__.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/authentication/__init__.py` & `beer-garden-3.9.0/beer_garden/api/http/authentication/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 from uuid import UUID, uuid4
 
 import jwt
 from tornado.httputil import HTTPServerRequest
 
 from beer_garden import config
-from beer_garden.api.http.authentication.login_handlers import LOGIN_HANDLERS
+from beer_garden.api.http.authentication.login_handlers import enabled_login_handlers
 from beer_garden.authorization import permissions_for_user
 from beer_garden.db.mongo.models import User, UserToken
 from beer_garden.errors import ExpiredTokenException, InvalidTokenException
 
 
 def user_login(request: HTTPServerRequest) -> Optional[User]:
     """Attempt to authenticate a user based on the information supplied in the request.
@@ -24,15 +24,15 @@
 
     Returns:
         User: The User object for the successfully authenticated user
         None: If unable to authenticate a user based on the request
     """
     user = None
 
-    for handler in LOGIN_HANDLERS:
+    for handler in enabled_login_handlers():
         user = handler().get_user(request)
 
         if user:
             break
 
     return user
```

### Comparing `beer-garden-3.8.1/beer_garden/api/http/authentication/login_handlers/base.py` & `beer-garden-3.9.0/beer_garden/api/http/authentication/login_handlers/base.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/authentication/login_handlers/basic.py` & `beer-garden-3.9.0/beer_garden/api/http/authentication/login_handlers/basic.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/base_handler.py` & `beer-garden-3.9.0/beer_garden/api/http/base_handler.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/client.py` & `beer-garden-3.9.0/beer_garden/api/http/client.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/exceptions.py` & `beer-garden-3.9.0/beer_garden/api/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/authorization_handler.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/authorization_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,14 +116,30 @@
 
         # This call forces the authorization check on every request because it calls
         # get_current_user(). The result is cached, so subsequent calls to
         # self.current_user within the life of the request will not result in a
         # duplication of the work required to identify and retrieve the User object.
         _ = self.current_user
 
+    def verify_user_global_permission(self, permission: str) -> None:
+        """Verifies that the requesting use has the specified permission for the Global
+        scope.
+
+        Args:
+            permission: The permission to check against
+
+        Raises:
+            RequestForbidden: The user does not have the required object permissions
+
+        Returns:
+            None
+        """
+        if permission not in self.current_user.global_permissions:
+            raise RequestForbidden
+
     def verify_user_permission_for_object(
         self, permission: str, obj: Union[Document, BrewtilsModel]
     ) -> None:
         """Verifies that the requesting user has the specified permission for the
         given object.
 
         Args:
```

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/misc.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/misc.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/__init__.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/admin.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/admin.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/command.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/command.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/event.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/event.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/forward.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/forward.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 import asyncio
 
 from brewtils.errors import TimeoutExceededError
 from brewtils.schema_parser import SchemaParser
 
-from beer_garden.api.http.base_handler import BaseHandler
+from beer_garden.api.authorization import Permissions
+from beer_garden.api.http.handlers import AuthorizationHandler
 
+EVENT_FORWARD = Permissions.EVENT_FORWARD.value
 
-class ForwardAPI(BaseHandler):
 
-    # @Todo Create new Persmission
+class ForwardAPI(AuthorizationHandler):
     async def post(self):
         """
         ---
         summary: Forward a request from a parent or child BG instance
         description: |
             When a Beer Garden needs to forward a request, this API will support routing
             to all CRUD actions exposed by the entry points.
@@ -33,23 +34,25 @@
           - name: forward
             in: body
             required: true
             description: The Forward Object
             schema:
                 $ref: '#/definitions/Forward'
         responses:
-          200:
+          204:
             description: Forward Request Accepted
           400:
             $ref: '#/definitions/400Error'
           50x:
             $ref: '#/definitions/50xError'
         tags:
           - Forward
         """
+        self.verify_user_global_permission(EVENT_FORWARD)
+
         operation = SchemaParser.parse_operation(
             self.request.decoded_body, from_string=True
         )
 
         task = asyncio.create_task(self.client(operation))
 
         # Deal with blocking
```

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/garden.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/garden.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/instance.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/instance.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/job.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from brewtils.errors import ModelValidationError, NotFoundError
 from brewtils.models import Operation
 from brewtils.schema_parser import SchemaParser
 from brewtils.schemas import JobExportInputSchema, JobSchema
 from mongoengine.errors import ValidationError
 
 from beer_garden.api.authorization import Permissions
+from beer_garden.api.http.exceptions import BadRequest
 from beer_garden.api.http.handlers import AuthorizationHandler
 from beer_garden.db.mongo.models import Job
 from beer_garden.scheduler import create_jobs
 
 JOB_CREATE = Permissions.JOB_CREATE.value
 JOB_READ = Permissions.JOB_READ.value
 JOB_UPDATE = Permissions.JOB_UPDATE.value
@@ -361,15 +362,25 @@
           50x:
             $ref: '#/definitions/50xError'
         tags:
           - Jobs
         """
         _ = self.get_or_raise(Job, JOB_CREATE, id=job_id)
 
+        reset_interval = (
+            True
+            if self.get_argument("reset_interval", "False").lower() == "true"
+            else False
+        )
+
         try:
-            await self.client(Operation(operation_type="JOB_EXECUTE", args=[job_id]))
+            await self.client(
+                Operation(operation_type="JOB_EXECUTE", args=[job_id, reset_interval])
+            )
         except ValidationError:
             raise NotFoundError
+        except ModelValidationError as exc:
+            raise BadRequest(reason=f"{exc}")
 
         self.set_status(202)
         self.set_header("Content-Type", "application/json; charset=UTF-8")
         self.write("")
```

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/logging.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/logging.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/namespace.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/queue.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/queue.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/request.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
           50x:
             $ref: '#/definitions/50xError'
         tags:
           - Requests
         """
         request = self.get_or_raise(Request, REQUEST_READ, id=request_id)
 
+        # brewtils dependencies make universal handling of children overly cumbersome,
+        # so just manually populate them here for now.
+        request.children = Request.objects.filter(parent=request)
+
         response = MongoParser.serialize(request)
 
         self.set_header("Content-Type", "application/json; charset=UTF-8")
         self.write(response)
 
     async def patch(self, request_id):
         """
```

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/system.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/system.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/token.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/token.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/v1/user.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/v1/user.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/chunk.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/chunk.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/event.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/event.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/file.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/file.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/handlers/vbeta/runner.py` & `beer-garden-3.9.0/beer_garden/api/http/handlers/vbeta/runner.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/processors.py` & `beer-garden-3.9.0/beer_garden/api/http/processors.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/publishers.py` & `beer-garden-3.9.0/beer_garden/api/http/publishers.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/http/schemas/v1/token.py` & `beer-garden-3.9.0/beer_garden/api/http/schemas/v1/token.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/stomp/__init__.py` & `beer-garden-3.9.0/beer_garden/api/stomp/__init__.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/stomp/manager.py` & `beer-garden-3.9.0/beer_garden/api/stomp/manager.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/api/stomp/transport.py` & `beer-garden-3.9.0/beer_garden/api/stomp/transport.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/app.py` & `beer-garden-3.9.0/beer_garden/app.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/authorization.py` & `beer-garden-3.9.0/beer_garden/authorization.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/commands.py` & `beer-garden-3.9.0/beer_garden/commands.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/config.py` & `beer-garden-3.9.0/beer_garden/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,14 +592,57 @@
             "default": "Beer Garden",
             "description": "The title to display on the GUI",
             "previous_names": ["application_name"],
         },
     },
 }
 
+_AUTHENTICATION_HANDLERS_SPEC = {
+    "type": "dict",
+    "items": {
+        "basic": {
+            "type": "dict",
+            "items": {
+                "enabled": {
+                    "type": "bool",
+                    "default": True,
+                    "description": "Enable authentication via username and" "password",
+                }
+            },
+        },
+        "trusted_header": {
+            "type": "dict",
+            "items": {
+                "enabled": {
+                    "type": "bool",
+                    "default": False,
+                    "description": "Enable authentication via trusted headers",
+                },
+                "username_header": {
+                    "type": "str",
+                    "default": "bg-username",
+                    "description": "The http header containing the username",
+                },
+                "user_groups_header": {
+                    "type": "str",
+                    "default": "bg-user-groups",
+                    "description": "The http header containing the comma separated "
+                    "list of the user's groups.",
+                },
+                "create_users": {
+                    "type": "bool",
+                    "default": True,
+                    "description": "Create an account for the user specified by"
+                    "username_header if one does not already exist",
+                },
+            },
+        },
+    },
+}
+
 _AUTH_SPEC = {
     "type": "dict",
     "items": {
         "enabled": {
             "type": "bool",
             "default": False,
             "description": "Use role-based authentication / authorization",
@@ -621,14 +664,21 @@
         "role_definition_file": {
             "type": "str",
             "description": (
                 "Path to the yaml file that defines roles used for authorization"
             ),
             "required": False,
         },
+        "group_definition_file": {
+            "type": "str",
+            "description": "Path to the file containg a mapping of "
+            "groups to beer garden role assignments",
+            "required": False,
+        },
+        "authentication_handlers": _AUTHENTICATION_HANDLERS_SPEC,
     },
 }
 
 _DB_SPEC = {
     "type": "dict",
     "items": {
         "name": {
```

### Comparing `beer-garden-3.8.1/beer_garden/db/api.py` & `beer-garden-3.9.0/beer_garden/db/api.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/db/mongo/api.py` & `beer-garden-3.9.0/beer_garden/db/mongo/api.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/db/mongo/jobstore.py` & `beer-garden-3.9.0/beer_garden/db/mongo/jobstore.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/db/mongo/models.py` & `beer-garden-3.9.0/beer_garden/db/mongo/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,18 @@
     def pre_serialize(self):
         pass
 
     @property
     def changed_fields(self):
         return getattr(self, "_changed_fields", [])
 
+    @property
+    def created(self):
+        return getattr(self, "_created", False)
+
 
 # MongoEngine needs all EmbeddedDocuments to be defined before any Documents that
 # reference them. So Parameter must be defined before Command, and choices should be
 # defined before Parameter
 
 
 class Choices(MongoModel, EmbeddedDocument):
@@ -312,15 +316,15 @@
     output = StringField()
     output_gridfs = FileField()
     output_type = StringField(choices=BrewtilsCommand.OUTPUT_TYPES)
     status = StringField(choices=BrewtilsRequest.STATUS_LIST, default="CREATED")
     command_type = StringField(choices=BrewtilsCommand.COMMAND_TYPES)
     created_at = DateTimeField(default=datetime.datetime.utcnow, required=True)
     updated_at = DateTimeField(default=None, required=True)
-    status_updated_at = DateTimeField(default=datetime.datetime.utcnow, required=True)
+    status_updated_at = DateTimeField()
     error_class = StringField(required=False)
     has_parent = BooleanField(required=False)
     hidden = BooleanField(required=False)
     requester = StringField(required=False)
     parameters_gridfs = FileField()
 
     meta = {
@@ -476,15 +480,15 @@
             self.has_parent = bool(self.parent)
         elif self.has_parent != bool(self.parent):
             raise ModelValidationError(
                 f"Cannot save Request {self}: parent value of {self.parent!r} is not "
                 f"consistent with has_parent value of {self.has_parent}"
             )
 
-        if "status" in self.changed_fields:
+        if "status" in self.changed_fields or self.created:
             self.status_updated_at = datetime.datetime.utcnow()
 
     def clean_update(self):
         """Ensure that the update would not result in an illegal status transition"""
         # Get the original status
         old_status = Request.objects.get(id=self.id).status
 
@@ -867,16 +871,16 @@
         if self.identifiers == {} and self.scope != "Global":
             raise ValidationError(
                 "identifiers field is required for all scopes other than Global"
             )
 
 
 class RoleAssignment(EmbeddedDocument):
-    domain = EmbeddedDocumentField(RoleAssignmentDomain)
-    role = ReferenceField("Role")
+    domain = EmbeddedDocumentField(RoleAssignmentDomain, required=True)
+    role = ReferenceField("Role", required=True)
 
 
 class User(Document):
     username = StringField(required=True)
     password = StringField()
     role_assignments = EmbeddedDocumentListField("RoleAssignment")
```

### Comparing `beer-garden-3.8.1/beer_garden/db/mongo/motor.py` & `beer-garden-3.9.0/beer_garden/db/mongo/motor.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/db/mongo/parser.py` & `beer-garden-3.9.0/beer_garden/db/mongo/parser.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/db/mongo/pruner.py` & `beer-garden-3.9.0/beer_garden/db/mongo/pruner.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/db/mongo/util.py` & `beer-garden-3.9.0/beer_garden/db/mongo/util.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/errors.py` & `beer-garden-3.9.0/beer_garden/errors.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/events/__init__.py` & `beer-garden-3.9.0/beer_garden/events/__init__.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/events/handlers.py` & `beer-garden-3.9.0/beer_garden/events/handlers.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/events/parent_procesors.py` & `beer-garden-3.9.0/beer_garden/events/parent_procesors.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/events/processors.py` & `beer-garden-3.9.0/beer_garden/events/processors.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/files.py` & `beer-garden-3.9.0/beer_garden/files.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/garden.py` & `beer-garden-3.9.0/beer_garden/garden.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/local_plugins/env_help.py` & `beer-garden-3.9.0/beer_garden/local_plugins/env_help.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/local_plugins/manager.py` & `beer-garden-3.9.0/beer_garden/local_plugins/manager.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/local_plugins/runner.py` & `beer-garden-3.9.0/beer_garden/local_plugins/runner.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/log.py` & `beer-garden-3.9.0/beer_garden/log.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/metrics.py` & `beer-garden-3.9.0/beer_garden/metrics.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/monitor.py` & `beer-garden-3.9.0/beer_garden/monitor.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/namespace.py` & `beer-garden-3.9.0/beer_garden/namespace.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/plugin.py` & `beer-garden-3.9.0/beer_garden/plugin.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/queue/rabbit.py` & `beer-garden-3.9.0/beer_garden/queue/rabbit.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/queues.py` & `beer-garden-3.9.0/beer_garden/queues.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/requests.py` & `beer-garden-3.9.0/beer_garden/requests.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/role.py` & `beer-garden-3.9.0/beer_garden/role.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/router.py` & `beer-garden-3.9.0/beer_garden/router.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/scheduler.py` & `beer-garden-3.9.0/beer_garden/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,14 +360,20 @@
             trigger=DateTrigger(datetime.utcnow(), timezone="UTC"),
             trigger_type="date",
             coalesce=job.coalesce,
             kwargs={"job_id": job.id, "request_template": job.request_template},
             id="ad-hoc",
         )
 
+        if reset_interval:
+            job = beer_garden.application.scheduler.get_job(job_id)
+            beer_garden.application.scheduler.reschedule_job(
+                job_id, trigger=job.trigger
+            )
+
     def _add_triggers(self, handler, triggers, func):
         """Attaches the function to the handler callback
 
         Args:
             handler: The event handler
             triggers: A dictionary of triggers that maps callback method
                 names to boolean values (e.g. on_moved -> True)
@@ -632,26 +638,34 @@
         The Job ID
     """
     # The scheduler takes care of removing the Job from the database
     return db.query_unique(Job, id=job_id)
 
 
 @publish_event(Events.JOB_EXECUTED)
-def execute_job(job_id: str) -> Job:
+def execute_job(job_id: str, reset_interval=False) -> Job:
     """Execute a Job ad-hoc
 
     Creates a new job with a trigger for now.
 
     Args:
         job_id: The Job ID
 
     Returns:
         The spawned Request
     """
-    return db.query_unique(Job, id=job_id, raise_missing=True)
+    job = db.query_unique(Job, id=job_id, raise_missing=True)
+    job.reset_interval = reset_interval
+
+    if reset_interval and job.trigger_type != "interval":
+        raise ModelValidationError(
+            "reset_interval can only be used with trigger type of interval"
+        )
+
+    return job
 
 
 def handle_event(event: Event) -> None:
     """Handle JOB events
 
     When creating or updating a job, make sure to mark as local first.
 
@@ -696,9 +710,11 @@
             )
         elif event.name == Events.JOB_DELETED.name:
             beer_garden.application.scheduler.remove_job(
                 event.payload.id, jobstore="beer_garden"
             )
         elif event.name == Events.JOB_EXECUTED.name:
             beer_garden.application.scheduler.execute_job(
-                event.payload.id, jobstore="beer_garden"
+                event.payload.id,
+                jobstore="beer_garden",
+                reset_interval=event.payload.reset_interval,
             )
```

### Comparing `beer-garden-3.8.1/beer_garden/systems.py` & `beer-garden-3.9.0/beer_garden/systems.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden/user.py` & `beer-garden-3.9.0/beer_garden/user.py`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/beer_garden.egg-info/PKG-INFO` & `beer-garden-3.9.0/beer_garden.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: beer-garden
-Version: 3.8.1
+Version: 3.9.0
 Summary: Beergarden Application
 Home-page: https://beer-garden.io
 Author: The Beer Garden Team
 Author-email: beer@beer-garden.io
 License: MIT
 Description: 
         ===========================
```

### Comparing `beer-garden-3.8.1/beer_garden.egg-info/SOURCES.txt` & `beer-garden-3.9.0/beer_garden.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 beer_garden/api/http/metrics.py
 beer_garden/api/http/processors.py
 beer_garden/api/http/publishers.py
 beer_garden/api/http/authentication/__init__.py
 beer_garden/api/http/authentication/login_handlers/__init__.py
 beer_garden/api/http/authentication/login_handlers/base.py
 beer_garden/api/http/authentication/login_handlers/basic.py
-beer_garden/api/http/authentication/login_handlers/certificate.py
+beer_garden/api/http/authentication/login_handlers/trusted_header.py
 beer_garden/api/http/handlers/__init__.py
 beer_garden/api/http/handlers/authorization_handler.py
 beer_garden/api/http/handlers/misc.py
 beer_garden/api/http/handlers/v1/__init__.py
 beer_garden/api/http/handlers/v1/admin.py
 beer_garden/api/http/handlers/v1/command.py
 beer_garden/api/http/handlers/v1/event.py
```

### Comparing `beer-garden-3.8.1/beer_garden.egg-info/entry_points.txt` & `beer-garden-3.9.0/beer_garden.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `beer-garden-3.8.1/setup.py` & `beer-garden-3.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url="https://beer-garden.io",
     packages=(find_packages(exclude=["test", "test.*"])),
     license="MIT",
     keywords="beer beer-garden beergarden",
     install_requires=[
         "apispec<0.39",
         "apscheduler<4",
-        "brewtils>=3.8.0",
+        "brewtils>=3.9.0",
         "marshmallow<3",
         "mongoengine<0.21",
         "more-itertools<9",
         "motor<3",
         "passlib<1.8",
         "prometheus-client<1",
         "pyyaml<6",
```

