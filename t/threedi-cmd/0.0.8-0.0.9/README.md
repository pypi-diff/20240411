# Comparing `tmp/threedi_cmd-0.0.8.tar.gz` & `tmp/threedi_cmd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi_cmd-0.0.8.tar", last modified: Wed Apr 28 12:34:22 2021, max compression
+gzip compressed data, was "threedi_cmd-0.0.9.tar", last modified: Wed May  5 14:15:02 2021, max compression
```

## Comparing `threedi_cmd-0.0.8.tar` & `threedi_cmd-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 12:34:22.912390 threedi_cmd-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      930 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      236 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9125 2021-04-28 12:34:22.912390 threedi_cmd-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5643 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      486 2021-04-28 12:34:22.912390 threedi_cmd-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 12:34:22.904390 threedi_cmd-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/tests/test_scenario_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 12:34:22.904390 threedi_cmd-0.0.8/threedi_cmd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 12:34:22.908390 threedi_cmd-0.0.8/threedi_cmd/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/active_simulations.py
--rw-r--r--   0 runner    (1001) docker     (121)    13740 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/app_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)      513 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (121)     8665 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/slack_notify.py
--rw-r--r--   0 runner    (1001) docker     (121)    12282 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/suite.py
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/console.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 12:34:22.912390 threedi_cmd-0.0.8/threedi_cmd/models/
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6797 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/boundary_conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/breach.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3956 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/initial_waterlevels.py
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/lateral.py
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/leakage.py
--rw-r--r--   0 runner    (1001) docker     (121)     9469 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4102 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/rain.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/rasteredit.py
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/savedstate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5011 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/scenario.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/simulation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4075 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/sources_sinks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/structure_control.py
--rw-r--r--   0 runner    (1001) docker     (121)     6910 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/waitfor.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/models/wind.py
--rw-r--r--   0 runner    (1001) docker     (121)     2147 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 12:34:22.912390 threedi_cmd-0.0.8/threedi_cmd/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/plugins/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/plugins/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/test.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 12:34:22.912390 threedi_cmd-0.0.8/threedi_cmd/websockets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2021-04-28 12:33:44.000000 threedi_cmd-0.0.8/threedi_cmd/websockets/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 12:34:22.908390 threedi_cmd-0.0.8/threedi_cmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9125 2021-04-28 12:34:22.000000 threedi_cmd-0.0.8/threedi_cmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2021-04-28 12:34:22.000000 threedi_cmd-0.0.8/threedi_cmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 12:34:22.000000 threedi_cmd-0.0.8/threedi_cmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-04-28 12:34:22.000000 threedi_cmd-0.0.8/threedi_cmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 12:34:22.000000 threedi_cmd-0.0.8/threedi_cmd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-04-28 12:34:22.000000 threedi_cmd-0.0.8/threedi_cmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-04-28 12:34:22.000000 threedi_cmd-0.0.8/threedi_cmd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 14:15:02.349798 threedi_cmd-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9262 2021-05-05 14:15:02.349798 threedi_cmd-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5643 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2021-05-05 14:15:02.349798 threedi_cmd-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 14:15:02.341797 threedi_cmd-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1890 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      857 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/tests/test_scenario_meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2396 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 14:15:02.345798 threedi_cmd-0.0.9/threedi_cmd/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 14:15:02.345798 threedi_cmd-0.0.9/threedi_cmd/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/active_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13740 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/app_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      513 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8665 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/slack_notify.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12282 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/suite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2323 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/console.py
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 14:15:02.349798 threedi_cmd-0.0.9/threedi_cmd/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2628 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6797 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/boundary_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/breach.py
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3956 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/initial_waterlevels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2913 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/lateral.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3252 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/leakage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9469 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4102 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/rain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/rasteredit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/savedstate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5011 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4075 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/sources_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/structure_control.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6910 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/waitfor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/models/wind.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2147 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 14:15:02.349798 threedi_cmd-0.0.9/threedi_cmd/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/plugins/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/plugins/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 14:15:02.349798 threedi_cmd-0.0.9/threedi_cmd/websockets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2021-05-05 14:14:26.000000 threedi_cmd-0.0.9/threedi_cmd/websockets/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 14:15:02.345798 threedi_cmd-0.0.9/threedi_cmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9262 2021-05-05 14:15:01.000000 threedi_cmd-0.0.9/threedi_cmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2021-05-05 14:15:01.000000 threedi_cmd-0.0.9/threedi_cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 14:15:01.000000 threedi_cmd-0.0.9/threedi_cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-05-05 14:15:01.000000 threedi_cmd-0.0.9/threedi_cmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 14:15:01.000000 threedi_cmd-0.0.9/threedi_cmd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-05-05 14:15:01.000000 threedi_cmd-0.0.9/threedi_cmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-05-05 14:15:01.000000 threedi_cmd-0.0.9/threedi_cmd.egg-info/top_level.txt
```

### Comparing `threedi_cmd-0.0.8/HISTORY.rst` & `threedi_cmd-0.0.9/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+0.0.9 (2021-05-05)
+------------------
+
+- Renamed general settings to physical settings
+
+
 0.0.8 (2021-04-28)
 ------------------
 
 - Use auth refresh method from upstream package.
 
 
 0.0.7 (2021-04-14)
```

### Comparing `threedi_cmd-0.0.8/LICENSE` & `threedi_cmd-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/PKG-INFO` & `threedi_cmd-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi_cmd
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python 3Di command line client
 Home-page: https://github.com/nens/threedi-cmd
 Author: Jelle Prins
 Author-email: info@nelen-schuurmans.nl
 License: MIT license
 Description: # The 3Di command line client
         
@@ -196,14 +196,20 @@
         
         
         That's it. Publish your package to [pypi](https://pypi.org/) so that is pip installable. 
         
         
         # History
         
+        0.0.9 (2021-05-05)
+        ------------------
+        
+        - Renamed general settings to physical settings
+        
+        
         0.0.8 (2021-04-28)
         ------------------
         
         - Use auth refresh method from upstream package.
         
         
         0.0.7 (2021-04-14)
```

### Comparing `threedi_cmd-0.0.8/README.md` & `threedi_cmd-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/setup.py` & `threedi_cmd-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/tests/fixtures.py` & `threedi_cmd-0.0.9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/tests/test_cache.py` & `threedi_cmd-0.0.9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/tests/test_scenario_meta.py` & `threedi_cmd-0.0.9/tests/test_scenario_meta.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/tests/test_settings.py` & `threedi_cmd-0.0.9/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/active_simulations.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/active_simulations.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/api.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/api.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/app_definitions.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/app_definitions.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/callbacks.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/callbacks.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/main.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/main.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/scenarios.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/scenarios.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/settings.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/settings.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/suite.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/suite.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/commands/utils.py` & `threedi_cmd-0.0.9/threedi_cmd/commands/utils.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/__init__.py` & `threedi_cmd-0.0.9/threedi_cmd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/actions.py` & `threedi_cmd-0.0.9/threedi_cmd/models/actions.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/base.py` & `threedi_cmd-0.0.9/threedi_cmd/models/base.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/boundary_conditions.py` & `threedi_cmd-0.0.9/threedi_cmd/models/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/initial_waterlevels.py` & `threedi_cmd-0.0.9/threedi_cmd/models/initial_waterlevels.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/lateral.py` & `threedi_cmd-0.0.9/threedi_cmd/models/lateral.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/leakage.py` & `threedi_cmd-0.0.9/threedi_cmd/models/leakage.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/monitor.py` & `threedi_cmd-0.0.9/threedi_cmd/models/monitor.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/rain.py` & `threedi_cmd-0.0.9/threedi_cmd/models/rain.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/rasteredit.py` & `threedi_cmd-0.0.9/threedi_cmd/models/rasteredit.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/savedstate.py` & `threedi_cmd-0.0.9/threedi_cmd/models/savedstate.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/scenario.py` & `threedi_cmd-0.0.9/threedi_cmd/models/scenario.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/settings.py` & `threedi_cmd-0.0.9/threedi_cmd/models/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .base import SettingsWrapper
 from openapi_client import SimulationsApi
 from openapi_client.models import (
-    GeneralSettings,
+    PhysicalSettings,
     NumericalSettings,
     TimeStepSettings,
     AggregationSettings
 )
 
 
-class GeneralSettingsWrapper(SettingsWrapper):
+class PhysicalSettingsWrapper(SettingsWrapper):
     api_class = SimulationsApi
-    model = GeneralSettings
-    api_path: str = "general"
-    scenario_name = "generalsettings"
+    model = PhysicalSettings
+    api_path: str = "physical"
+    scenario_name = "physicalsettings"
 
 
 class NumercialSettingsWrapper(SettingsWrapper):
     api_class = SimulationsApi
     model = NumericalSettings
     api_path: str = "numerical"
     scenario_name = "numericalsettings"
@@ -33,12 +33,12 @@
     api_class = SimulationsApi
     model = AggregationSettings
     api_path: str = "aggregation"
     scenario_name = "aggregationsettings"
 
 
 WRAPPERS = [
-    GeneralSettingsWrapper,
+    PhysicalSettingsWrapper,
     NumercialSettingsWrapper,
     TimeStepSettingsWrapper,
     AggregationSettingsWrapper
 ]
```

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/sources_sinks.py` & `threedi_cmd-0.0.9/threedi_cmd/models/sources_sinks.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/structure_control.py` & `threedi_cmd-0.0.9/threedi_cmd/models/structure_control.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/waitfor.py` & `threedi_cmd-0.0.9/threedi_cmd/models/waitfor.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/models/wind.py` & `threedi_cmd-0.0.9/threedi_cmd/models/wind.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/parser.py` & `threedi_cmd-0.0.9/threedi_cmd/parser.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/plugins/tools.py` & `threedi_cmd-0.0.9/threedi_cmd/plugins/tools.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/test.py` & `threedi_cmd-0.0.9/threedi_cmd/test.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd/websockets/clients.py` & `threedi_cmd-0.0.9/threedi_cmd/websockets/clients.py`

 * *Files identical despite different names*

### Comparing `threedi_cmd-0.0.8/threedi_cmd.egg-info/PKG-INFO` & `threedi_cmd-0.0.9/threedi_cmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-cmd
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python 3Di command line client
 Home-page: https://github.com/nens/threedi-cmd
 Author: Jelle Prins
 Author-email: info@nelen-schuurmans.nl
 License: MIT license
 Description: # The 3Di command line client
         
@@ -196,14 +196,20 @@
         
         
         That's it. Publish your package to [pypi](https://pypi.org/) so that is pip installable. 
         
         
         # History
         
+        0.0.9 (2021-05-05)
+        ------------------
+        
+        - Renamed general settings to physical settings
+        
+        
         0.0.8 (2021-04-28)
         ------------------
         
         - Use auth refresh method from upstream package.
         
         
         0.0.7 (2021-04-14)
```

### Comparing `threedi_cmd-0.0.8/threedi_cmd.egg-info/SOURCES.txt` & `threedi_cmd-0.0.9/threedi_cmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

