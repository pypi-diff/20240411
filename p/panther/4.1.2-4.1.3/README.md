# Comparing `tmp/panther-4.1.2.tar.gz` & `tmp/panther-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-4.1.2.tar", last modified: Mon Apr  8 02:19:14 2024, max compression
+gzip compressed data, was "panther-4.1.3.tar", last modified: Thu Apr 11 01:05:43 2024, max compression
```

## Comparing `panther-4.1.2.tar` & `panther-4.1.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.852240 panther-4.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-08 02:19:01.000000 panther-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-08 02:19:14.852240 panther-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-08 02:19:01.000000 panther-4.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.840240 panther-4.1.2/panther/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 02:19:01.000000 panther-4.1.2/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-08 02:19:01.000000 panther-4.1.2/panther/_load_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-08 02:19:01.000000 panther-4.1.2/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-08 02:19:01.000000 panther-4.1.2/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-08 02:19:01.000000 panther-4.1.2/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-08 02:19:01.000000 panther-4.1.2/panther/background_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-08 02:19:01.000000 panther-4.1.2/panther/base_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-08 02:19:01.000000 panther-4.1.2/panther/base_websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-08 02:19:01.000000 panther-4.1.2/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.844240 panther-4.1.2/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:01.000000 panther-4.1.2/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-08 02:19:01.000000 panther-4.1.2/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-08 02:19:01.000000 panther-4.1.2/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-08 02:19:01.000000 panther-4.1.2/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-08 02:19:01.000000 panther-4.1.2/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-08 02:19:01.000000 panther-4.1.2/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-08 02:19:01.000000 panther-4.1.2/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-08 02:19:01.000000 panther-4.1.2/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.844240 panther-4.1.2/panther/db/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.844240 panther-4.1.2/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/queries/base_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11462 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-08 02:19:01.000000 panther-4.1.2/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-08 02:19:01.000000 panther-4.1.2/panther/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-08 02:19:01.000000 panther-4.1.2/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-08 02:19:01.000000 panther-4.1.2/panther/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-08 02:19:01.000000 panther-4.1.2/panther/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-08 02:19:01.000000 panther-4.1.2/panther/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-08 02:19:01.000000 panther-4.1.2/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.848240 panther-4.1.2/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 02:19:01.000000 panther-4.1.2/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-08 02:19:01.000000 panther-4.1.2/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-08 02:19:01.000000 panther-4.1.2/panther/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-08 02:19:01.000000 panther-4.1.2/panther/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.848240 panther-4.1.2/panther/panel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:01.000000 panther-4.1.2/panther/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-08 02:19:01.000000 panther-4.1.2/panther/panel/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-08 02:19:01.000000 panther-4.1.2/panther/panel/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 02:19:01.000000 panther-4.1.2/panther/panel/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-08 02:19:01.000000 panther-4.1.2/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-08 02:19:01.000000 panther-4.1.2/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-08 02:19:01.000000 panther-4.1.2/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-08 02:19:01.000000 panther-4.1.2/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-08 02:19:01.000000 panther-4.1.2/panther/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-08 02:19:01.000000 panther-4.1.2/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-08 02:19:01.000000 panther-4.1.2/panther/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-08 02:19:01.000000 panther-4.1.2/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-08 02:19:01.000000 panther-4.1.2/panther/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-08 02:19:01.000000 panther-4.1.2/panther/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.848240 panther-4.1.2/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-08 02:19:14.000000 panther-4.1.2/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-08 02:19:14.000000 panther-4.1.2/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 02:19:14.000000 panther-4.1.2/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 02:19:14.000000 panther-4.1.2/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-08 02:19:14.000000 panther-4.1.2/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 02:19:14.000000 panther-4.1.2/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-08 02:19:01.000000 panther-4.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 02:19:14.852240 panther-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-08 02:19:01.000000 panther-4.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 02:19:14.848240 panther-4.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_background_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15572 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_multipart.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_panel_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-08 02:19:01.000000 panther-4.1.2/tests/test_websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.828752 panther-4.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-11 01:05:31.000000 panther-4.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-11 01:05:43.828752 panther-4.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-11 01:05:31.000000 panther-4.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.816752 panther-4.1.3/panther/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 01:05:31.000000 panther-4.1.3/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-11 01:05:31.000000 panther-4.1.3/panther/_load_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-11 01:05:31.000000 panther-4.1.3/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-11 01:05:31.000000 panther-4.1.3/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-11 01:05:31.000000 panther-4.1.3/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-11 01:05:31.000000 panther-4.1.3/panther/background_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-11 01:05:31.000000 panther-4.1.3/panther/base_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-11 01:05:31.000000 panther-4.1.3/panther/base_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-11 01:05:31.000000 panther-4.1.3/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.820752 panther-4.1.3/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-11 01:05:31.000000 panther-4.1.3/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.820752 panther-4.1.3/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.820752 panther-4.1.3/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/base_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-11 01:05:31.000000 panther-4.1.3/panther/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-11 01:05:31.000000 panther-4.1.3/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-11 01:05:31.000000 panther-4.1.3/panther/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-11 01:05:31.000000 panther-4.1.3/panther/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-11 01:05:31.000000 panther-4.1.3/panther/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-11 01:05:31.000000 panther-4.1.3/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.824752 panther-4.1.3/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 01:05:31.000000 panther-4.1.3/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-11 01:05:31.000000 panther-4.1.3/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-11 01:05:31.000000 panther-4.1.3/panther/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-11 01:05:31.000000 panther-4.1.3/panther/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.824752 panther-4.1.3/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:31.000000 panther-4.1.3/panther/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-11 01:05:31.000000 panther-4.1.3/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-11 01:05:31.000000 panther-4.1.3/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 01:05:31.000000 panther-4.1.3/panther/panel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-11 01:05:31.000000 panther-4.1.3/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-11 01:05:31.000000 panther-4.1.3/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-11 01:05:31.000000 panther-4.1.3/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-11 01:05:31.000000 panther-4.1.3/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9096 2024-04-11 01:05:31.000000 panther-4.1.3/panther/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-11 01:05:31.000000 panther-4.1.3/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-11 01:05:31.000000 panther-4.1.3/panther/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 01:05:31.000000 panther-4.1.3/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-11 01:05:31.000000 panther-4.1.3/panther/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-11 01:05:31.000000 panther-4.1.3/panther/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.828752 panther-4.1.3/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 01:05:31.000000 panther-4.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:05:43.828752 panther-4.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-11 01:05:31.000000 panther-4.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.824752 panther-4.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_background_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15572 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_panel_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_websockets.py
```

### Comparing `panther-4.1.2/LICENSE` & `panther-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/PKG-INFO` & `panther-4.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 4.1.2
+Version: 4.1.3
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: BSD-3-Clause license
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `panther-4.1.2/README.md` & `panther-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/_load_configs.py` & `panther-4.1.3/panther/_load_configs.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/_utils.py` & `panther-4.1.3/panther/_utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/app.py` & `panther-4.1.3/panther/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,23 +147,23 @@
             raise BadRequestAPIError(detail='Content-Type is not valid')
         if request.data is None:
             raise BadRequestAPIError(detail='Request body is required')
         try:
             # `request` will be ignored in regular `BaseModel`
             return model(**request.data, request=request)
         except ValidationError as validation_error:
-            error = {'.'.join(loc for loc in e['loc']): e['msg'] for e in validation_error.errors()}
+            error = {'.'.join(str(loc) for loc in e['loc']): e['msg'] for e in validation_error.errors()}
             raise BadRequestAPIError(detail=error)
         except JSONDecodeError:
             raise JSONDecodeAPIError
 
 
 class GenericAPI:
-    input_model: type[ModelSerializer] | type[BaseModel] = None
-    output_model: type[ModelSerializer] | type[BaseModel] = None
+    input_model: type[ModelSerializer] | type[BaseModel] | None = None
+    output_model: type[ModelSerializer] | type[BaseModel] | None = None
     auth: bool = False
     permissions: list | None = None
     throttling: Throttling | None = None
     cache: bool = False
     cache_exp_time: timedelta | int | None = None
 
     async def get(self, *args, **kwargs):
@@ -177,14 +177,20 @@
 
     async def patch(self, *args, **kwargs):
         raise MethodNotAllowedAPIError
 
     async def delete(self, *args, **kwargs):
         raise MethodNotAllowedAPIError
 
+    async def get_input_model(self, request: Request) -> type[ModelSerializer] | type[BaseModel] | None:
+        return None
+
+    async def get_output_model(self, request: Request) -> type[ModelSerializer] | type[BaseModel] | None:
+        return None
+
     async def call_method(self, request: Request):
         match request.method:
             case 'GET':
                 func = self.get
             case 'POST':
                 func = self.post
             case 'PUT':
@@ -193,15 +199,15 @@
                 func = self.patch
             case 'DELETE':
                 func = self.delete
             case _:
                 raise MethodNotAllowedAPIError
 
         return await API(
-            input_model=self.input_model,
-            output_model=self.output_model,
+            input_model=self.input_model or await self.get_input_model(request=request),
+            output_model=self.output_model or await self.get_output_model(request=request),
             auth=self.auth,
             permissions=self.permissions,
             throttling=self.throttling,
             cache=self.cache,
             cache_exp_time=self.cache_exp_time,
         )(func)(request=request)
```

### Comparing `panther-4.1.2/panther/authentications.py` & `panther-4.1.3/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/background_tasks.py` & `panther-4.1.3/panther/background_tasks.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/base_request.py` & `panther-4.1.3/panther/base_request.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/base_websocket.py` & `panther-4.1.3/panther/base_websocket.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/caching.py` & `panther-4.1.3/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/cli/create_command.py` & `panther-4.1.3/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/cli/main.py` & `panther-4.1.3/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/cli/monitor_command.py` & `panther-4.1.3/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/cli/run_command.py` & `panther-4.1.3/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/cli/template.py` & `panther-4.1.3/panther/cli/template.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/cli/utils.py` & `panther-4.1.3/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/configs.py` & `panther-4.1.3/panther/configs.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/db/connections.py` & `panther-4.1.3/panther/db/connections.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/db/cursor.py` & `panther-4.1.3/panther/db/cursor.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/db/models.py` & `panther-4.1.3/panther/db/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def validate_object_id(value, handler):
     if config.DATABASE.__class__.__name__ == 'MongoDBConnection':
         if isinstance(value, bson.ObjectId):
             return value
         else:
             try:
                 return bson.ObjectId(value)
-            except bson.objectid.InvalidId as e:
+            except Exception as e:
                 msg = 'Invalid ObjectId'
                 raise ValueError(msg) from e
     return str(value)
 
 
 ID = Annotated[str, WrapValidator(validate_object_id), PlainSerializer(lambda x: str(x), return_type=str)]
```

### Comparing `panther-4.1.2/panther/db/queries/base_queries.py` & `panther-4.1.3/panther/db/queries/base_queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/db/queries/mongodb_queries.py` & `panther-4.1.3/panther/db/queries/mongodb_queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,29 +98,44 @@
     @classmethod
     async def delete_many(cls, _filter: dict | None = None, /, **kwargs) -> int:
         result = await db.session[cls.__name__].delete_many(cls._merge(_filter, kwargs))
         return result.deleted_count
 
     # # # # # Update # # # # #
     async def update(self, _update: dict | None = None, /, **kwargs) -> None:
-        document = self._merge(_update, kwargs)
-        document.pop('_id', None)
-        self._validate_data(data=document, is_updating=True)
-
-        for field, value in document.items():
-            setattr(self, field, value)
-        update_fields = {'$set': document}
-        await db.session[self.__class__.__name__].update_one({'_id': self._id}, update_fields)
+        merged_update_query = self._merge(_update, kwargs)
+        merged_update_query.pop('_id', None)
+
+        self._validate_data(data=merged_update_query, is_updating=True)
+
+        update_query = {}
+        for field, value in merged_update_query.items():
+            if field.startswith('$'):
+                update_query[field] = value
+            else:
+                update_query['$set'] = update_query.get('$set', {})
+                update_query['$set'][field] = value
+                setattr(self, field, value)
+
+        await db.session[self.__class__.__name__].update_one({'_id': self._id}, update_query)
 
     @classmethod
     async def update_one(cls, _filter: dict, _update: dict | None = None, /, **kwargs) -> bool:
         prepare_id_for_query(_filter, is_mongo=True)
-        update_fields = {'$set': cls._merge(_update, kwargs)}
+        merged_update_query = cls._merge(_update, kwargs)
+
+        update_query = {}
+        for field, value in merged_update_query.items():
+            if field.startswith('$'):
+                update_query[field] = value
+            else:
+                update_query['$set'] = update_query.get('$set', {})
+                update_query['$set'][field] = value
 
-        result = await db.session[cls.__name__].update_one(_filter, update_fields)
+        result = await db.session[cls.__name__].update_one(_filter, update_query)
         return bool(result.matched_count)
 
     @classmethod
     async def update_many(cls, _filter: dict, _update: dict | None = None, /, **kwargs) -> int:
         prepare_id_for_query(_filter, is_mongo=True)
         update_fields = {'$set': cls._merge(_update, kwargs)}
```

### Comparing `panther-4.1.2/panther/db/queries/pantherdb_queries.py` & `panther-4.1.3/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/db/queries/queries.py` & `panther-4.1.3/panther/db/queries/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,16 +360,14 @@
             >>> await User.find_one_or_raise({'age': 18}, name='Ali')
         """
         if obj := await cls.find_one(_filter, **kwargs):
             return obj
 
         raise NotFoundAPIError(detail=f'{cls.__name__} Does Not Exist')
 
-    @check_connection
-    @log_query
     async def save(self) -> None:
         """
         Save the document
             If it has `id` --> Update It
             else --> Insert It
         Example:
         -------
@@ -380,12 +378,18 @@
             >>> user.name = 'Saba'
             >>> await user.save()
             or
             # Insert
             >>> user = User(name='Ali')
             >>> await user.save()
         """
-        document = self.model_dump(exclude=['_id'])
+        document = {field: getattr(self, field) for field in self.model_fields_set if field != 'request'}
+
         if self.id:
             await self.update(document)
         else:
             await self.insert_one(document)
+
+    async def reload(self) -> Self:
+        new_obj = await self.find_one(id=self.id)
+        [setattr(self, f, getattr(new_obj, f)) for f in new_obj.model_fields]
+        return self
```

### Comparing `panther-4.1.2/panther/db/utils.py` & `panther-4.1.3/panther/db/utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/events.py` & `panther-4.1.3/panther/events.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/exceptions.py` & `panther-4.1.3/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/file_handler.py` & `panther-4.1.3/panther/file_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 from functools import cached_property
 
 from panther import status
-from pydantic import BaseModel, field_validator
+from pydantic import BaseModel, field_validator, model_serializer
 
 from panther.exceptions import APIError
 
 
 class File(BaseModel):
     file_name: str
     content_type: str
     file: bytes
 
     @cached_property
     def size(self):
         return len(self.file)
 
+    def save(self) -> str:
+        if hasattr(self, '_file_name'):
+            return self._file_name
+
+        self._file_name = self.file_name
+        # TODO: check for duplication
+        with open(self._file_name, 'wb') as file:
+            file.write(self.file)
+
+        return self.file_name
+
+    @model_serializer(mode='wrap')
+    def _serialize(self, handler):
+        result = handler(self)
+        result['path'] = self.save()
+        return result
+
     def __repr__(self) -> str:
         return f'{self.__repr_name__()}(file_name={self.file_name}, content_type={self.content_type})'
 
     __str__ = __repr__
 
 
 class Image(File):
```

### Comparing `panther-4.1.2/panther/generics.py` & `panther-4.1.3/panther/generics.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     import bson
 
 logger = logging.getLogger('panther')
 
 
 class ObjectRequired:
     def _check_object(self, instance):
-        if issubclass(type(instance), Model) is False:
+        if instance and issubclass(type(instance), Model) is False:
             logger.critical(f'`{self.__class__.__name__}.object()` should return instance of a Model --> `find_one()`')
             raise APIError
 
     async def object(self, request: Request, **kwargs):
         """
         Used in `RetrieveAPI`, `UpdateAPI`, `DeleteAPI`
         """
@@ -125,17 +125,19 @@
             return self.pagination(query_params=query_params, cursor=cursor)
 
 
 class CreateAPI(GenericAPI):
     input_model: type[ModelSerializer]
 
     async def post(self, request: Request, **kwargs):
-        instance = await request.validated_data.create(
-            validated_data=request.validated_data.model_dump()
-        )
+        instance = await request.validated_data.create(validated_data={
+            field: getattr(request.validated_data, field)
+            for field in request.validated_data.model_fields_set
+            if field != 'request'
+        })
         return Response(data=instance, status_code=status.HTTP_201_CREATED)
 
 
 class UpdateAPI(GenericAPI, ObjectRequired):
     input_model: type[ModelSerializer]
 
     async def put(self, request: Request, **kwargs):
@@ -156,17 +158,34 @@
             instance=instance,
             validated_data=request.validated_data.model_dump(exclude_none=True)
         )
         return Response(data=instance, status_code=status.HTTP_200_OK)
 
 
 class DeleteAPI(GenericAPI, ObjectRequired):
+    async def pre_delete(self, instance, request: Request, **kwargs):
+        pass
+
+    async def post_delete(self, instance, request: Request, **kwargs):
+        pass
+
     async def delete(self, request: Request, **kwargs):
         instance = await self.object(request=request, **kwargs)
         self._check_object(instance)
 
+        await self.pre_delete(instance, request=request, **kwargs)
         await instance.delete()
+        await self.post_delete(instance, request=request, **kwargs)
+
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
 class ListCreateAPI(CreateAPI, ListAPI):
     pass
+
+
+class UpdateDeleteAPI(UpdateAPI, DeleteAPI):
+    pass
+
+
+class RetrieveUpdateDeleteAPI(RetrieveAPI, UpdateAPI, DeleteAPI):
+    pass
```

### Comparing `panther-4.1.2/panther/logging.py` & `panther-4.1.3/panther/logging.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/main.py` & `panther-4.1.3/panther/main.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/middlewares/base.py` & `panther-4.1.3/panther/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/monitoring.py` & `panther-4.1.3/panther/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/pagination.py` & `panther-4.1.3/panther/pagination.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/panel/apis.py` & `panther-4.1.3/panther/panel/apis.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/request.py` & `panther-4.1.3/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/response.py` & `panther-4.1.3/panther/response.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/routings.py` & `panther-4.1.3/panther/routings.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/serializer.py` & `panther-4.1.3/panther/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         # Check `model`
         if (model := getattr(config, 'model', None)) is None:
             msg = f'`{cls_name}.Config.model` is required.'
             raise AttributeError(msg) from None
 
         # Check `model` type
         try:
-            if not issubclass(model, Model):
-                msg = f'`{cls_name}.Config.model` is not subclass of `panther.db.Model`.'
+            if not issubclass(model, (Model, BaseModel)):
+                msg = f'`{cls_name}.Config.model` is not subclass of `panther.db.Model` or `pydantic.BaseModel`.'
                 raise AttributeError(msg) from None
         except TypeError:
             msg = f'`{cls_name}.Config.model` is not subclass of `panther.db.Model`.'
             raise AttributeError(msg) from None
 
         # Check `fields`
         if not hasattr(config, 'fields'):
```

### Comparing `panther-4.1.2/panther/status.py` & `panther-4.1.3/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/test.py` & `panther-4.1.3/panther/test.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/utils.py` & `panther-4.1.3/panther/utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther/websocket.py` & `panther-4.1.3/panther/websocket.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/panther.egg-info/PKG-INFO` & `panther-4.1.3/panther.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 4.1.2
+Version: 4.1.3
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: BSD-3-Clause license
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `panther-4.1.2/panther.egg-info/SOURCES.txt` & `panther-4.1.3/panther.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/setup.py` & `panther-4.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_authentication.py` & `panther-4.1.3/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_background_tasks.py` & `panther-4.1.3/tests/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_caching.py` & `panther-4.1.3/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_cli.py` & `panther-4.1.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_database.py` & `panther-4.1.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_events.py` & `panther-4.1.3/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_generics.py` & `panther-4.1.3/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_multipart.py` & `panther-4.1.3/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_panel_apis.py` & `panther-4.1.3/tests/test_panel_apis.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_request.py` & `panther-4.1.3/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_response.py` & `panther-4.1.3/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_routing.py` & `panther-4.1.3/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_run.py` & `panther-4.1.3/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_serializer.py` & `panther-4.1.3/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_status.py` & `panther-4.1.3/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_throttling.py` & `panther-4.1.3/tests/test_throttling.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_utils.py` & `panther-4.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.2/tests/test_websockets.py` & `panther-4.1.3/tests/test_websockets.py`

 * *Files identical despite different names*

