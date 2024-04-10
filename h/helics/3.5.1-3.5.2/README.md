# Comparing `tmp/helics-3.5.1.tar.gz` & `tmp/helics-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helics-3.5.1.tar", last modified: Tue Mar 26 03:52:21 2024, max compression
+gzip compressed data, was "helics-3.5.2.tar", last modified: Wed Apr 10 23:44:41 2024, max compression
```

## Comparing `helics-3.5.1.tar` & `helics-3.5.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.044122 helics-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-26 03:51:54.000000 helics-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-26 03:51:54.000000 helics-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-26 03:52:21.044122 helics-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-26 03:51:54.000000 helics-3.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.024123 helics-3.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-26 03:51:54.000000 helics-3.5.1/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-03-26 03:51:54.000000 helics-3.5.1/docs/callbacks.md
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-26 03:51:54.000000 helics-3.5.1/docs/cli-interface.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.024123 helics-3.5.1/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.024123 helics-3.5.1/docs/examples/10-federates-1-topic/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/10-federates-1-topic/pireceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/10-federates-1-topic/pisender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/10-federates-1-topic/runner.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.028123 helics-3.5.1/docs/examples/2-federates-1-topic/
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-1-topic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-1-topic/old-pisender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-1-topic/pireceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-1-topic/pisender.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-1-topic/runner.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.028123 helics-3.5.1/docs/examples/2-federates-3-topics/
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-3-topics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-3-topics/pireceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-3-topics/pisender.py
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-3-topics/profile.txt
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/2-federates-3-topics/runner.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.028123 helics-3.5.1/docs/examples/20-federates-10-topics/
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/20-federates-10-topics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/20-federates-10-topics/pireceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/20-federates-10-topics/pisender.py
--rw-r--r--   0 runner    (1001) docker     (127)    47628 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/20-federates-10-topics/profile.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-26 03:51:54.000000 helics-3.5.1/docs/examples/20-federates-10-topics/runner.json
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-03-26 03:51:54.000000 helics-3.5.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 03:51:54.000000 helics-3.5.1/docs/interface.md
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-03-26 03:51:54.000000 helics-3.5.1/docs/migration-helics2-helics3.md
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-26 03:51:54.000000 helics-3.5.1/docs/pythonic-interface.md
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-26 03:51:54.000000 helics-3.5.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-26 03:51:54.000000 helics-3.5.1/docs/web-interface.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.032122 helics-3.5.1/helics/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-26 03:51:54.000000 helics-3.5.1/helics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-03-26 03:51:54.000000 helics-3.5.1/helics/_build.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 03:51:54.000000 helics-3.5.1/helics/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-26 03:51:54.000000 helics-3.5.1/helics/bin.py
--rw-r--r--   0 runner    (1001) docker     (127)   357886 2024-03-26 03:51:54.000000 helics-3.5.1/helics/capi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-03-26 03:51:54.000000 helics-3.5.1/helics/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-26 03:51:54.000000 helics-3.5.1/helics/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.032122 helics-3.5.1/helics/flaskr/
--rw-r--r--   0 runner    (1001) docker     (127)    19069 2024-03-26 03:51:54.000000 helics-3.5.1/helics/flaskr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-03-26 03:51:54.000000 helics-3.5.1/helics/observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-03-26 03:51:54.000000 helics-3.5.1/helics/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.032122 helics-3.5.1/helics/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.032122 helics-3.5.1/helics/static/_app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.032122 helics-3.5.1/helics/static/_app/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/assets/Dropzone-8e628262.css
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/assets/ScaledSvg.svelte_svelte_type_style_lang-71598278.css
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/assets/fa-29562a41.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.036122 helics-3.5.1/helics/static/_app/assets/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    82948 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/assets/pages/__layout.svelte-b30f8ab5.css
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/assets/pages/profile.svelte-7cbf608b.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.036122 helics-3.5.1/helics/static/_app/chunks/
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/Dropzone-f4be5df7.js
--rw-r--r--   0 runner    (1001) docker     (127)    64905 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/ScaledSvg.svelte_svelte_type_style_lang-3a481e75.js
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/fa-b47ae4c1.js
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/index-d6b53ebe.js
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/index-e4f78b56.js
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/index.es-e33ee127.js
--rw-r--r--   0 runner    (1001) docker     (127)   274503 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/index.min-4cad8088.js
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/preload-helper-e4860ae8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/chunks/stores-43842a59.js
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/error.svelte-f0b69c08.js
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.036122 helics-3.5.1/helics/static/_app/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/pages/__layout.svelte-146b41bd.js
--rw-r--r--   0 runner    (1001) docker     (127)    26271 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/pages/broker.svelte-a984d9f8.js
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/pages/index.svelte-1d030e3b.js
--rw-r--r--   0 runner    (1001) docker     (127)    54195 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/pages/observe.svelte-8c620952.js
--rw-r--r--   0 runner    (1001) docker     (127)    19316 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/pages/profile.svelte-c62e0a3a.js
--rw-r--r--   0 runner    (1001) docker     (127)    36765 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/pages/run.svelte-b0de2dfd.js
--rw-r--r--   0 runner    (1001) docker     (127)    23909 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/start-37b17f1c.js
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/_app/version.json
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-26 03:52:20.000000 helics-3.5.1/helics/static/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-03-26 03:51:54.000000 helics-3.5.1/helics/status_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-26 03:51:54.000000 helics-3.5.1/helics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-26 03:51:54.000000 helics-3.5.1/helics/vcredist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.040122 helics-3.5.1/helics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-26 03:52:21.000000 helics-3.5.1/helics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-03-26 03:52:21.000000 helics-3.5.1/helics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 03:52:21.000000 helics-3.5.1/helics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-26 03:52:21.000000 helics-3.5.1/helics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 03:52:21.000000 helics-3.5.1/helics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-26 03:52:21.000000 helics-3.5.1/helics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-26 03:52:21.000000 helics-3.5.1/helics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 03:52:21.044122 helics-3.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    24240 2024-03-26 03:51:54.000000 helics-3.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:52:21.040122 helics-3.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-26 03:51:54.000000 helics-3.5.1/tests/combinationfederate.json
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-26 03:51:54.000000 helics-3.5.1/tests/filters.json
--rw-r--r--   0 runner    (1001) docker     (127)    17863 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18493 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_badinputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_combinationfederate.py
--rw-r--r--   0 runner    (1001) docker     (127)    35799 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_messagefederate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_messagefilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_pyhelics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24165 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_python_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_systemtests.py
--rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-03-26 03:51:54.000000 helics-3.5.1/tests/test_valuefederate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-26 03:51:54.000000 helics-3.5.1/tests/valuefederate.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.667604 helics-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-10 23:44:05.000000 helics-3.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 23:44:05.000000 helics-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-10 23:44:41.667604 helics-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-10 23:44:05.000000 helics-3.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.651604 helics-3.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 23:44:05.000000 helics-3.5.2/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-10 23:44:05.000000 helics-3.5.2/docs/callbacks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-10 23:44:05.000000 helics-3.5.2/docs/cli-interface.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.647604 helics-3.5.2/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.651604 helics-3.5.2/docs/examples/10-federates-1-topic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/10-federates-1-topic/pireceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/10-federates-1-topic/pisender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/10-federates-1-topic/runner.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.651604 helics-3.5.2/docs/examples/2-federates-1-topic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-1-topic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-1-topic/old-pisender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-1-topic/pireceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-1-topic/pisender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-1-topic/runner.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.651604 helics-3.5.2/docs/examples/2-federates-3-topics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-3-topics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-3-topics/pireceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-3-topics/pisender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-3-topics/profile.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/2-federates-3-topics/runner.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.651604 helics-3.5.2/docs/examples/20-federates-10-topics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/20-federates-10-topics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/20-federates-10-topics/pireceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/20-federates-10-topics/pisender.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47628 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/20-federates-10-topics/profile.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-10 23:44:05.000000 helics-3.5.2/docs/examples/20-federates-10-topics/runner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-10 23:44:05.000000 helics-3.5.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:05.000000 helics-3.5.2/docs/interface.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-10 23:44:05.000000 helics-3.5.2/docs/migration-helics2-helics3.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-10 23:44:05.000000 helics-3.5.2/docs/pythonic-interface.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 23:44:05.000000 helics-3.5.2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-10 23:44:05.000000 helics-3.5.2/docs/web-interface.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.655604 helics-3.5.2/helics/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 23:44:05.000000 helics-3.5.2/helics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-10 23:44:05.000000 helics-3.5.2/helics/_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 23:44:05.000000 helics-3.5.2/helics/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 23:44:05.000000 helics-3.5.2/helics/bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   357886 2024-04-10 23:44:05.000000 helics-3.5.2/helics/capi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-10 23:44:05.000000 helics-3.5.2/helics/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-10 23:44:05.000000 helics-3.5.2/helics/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.655604 helics-3.5.2/helics/flaskr/
+-rw-r--r--   0 runner    (1001) docker     (127)    19069 2024-04-10 23:44:05.000000 helics-3.5.2/helics/flaskr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-10 23:44:05.000000 helics-3.5.2/helics/observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-10 23:44:05.000000 helics-3.5.2/helics/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.655604 helics-3.5.2/helics/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.659604 helics-3.5.2/helics/static/_app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.659604 helics-3.5.2/helics/static/_app/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/assets/Dropzone-8e628262.css
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/assets/ScaledSvg.svelte_svelte_type_style_lang-71598278.css
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/assets/fa-29562a41.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.659604 helics-3.5.2/helics/static/_app/assets/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    82948 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/assets/pages/__layout.svelte-b30f8ab5.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/assets/pages/profile.svelte-7cbf608b.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.659604 helics-3.5.2/helics/static/_app/chunks/
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/Dropzone-f4be5df7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    64905 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/ScaledSvg.svelte_svelte_type_style_lang-3a481e75.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/fa-b47ae4c1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/index-d6b53ebe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/index-e4f78b56.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/index.es-e33ee127.js
+-rw-r--r--   0 runner    (1001) docker     (127)   274503 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/index.min-4cad8088.js
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/preload-helper-e4860ae8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/chunks/stores-43842a59.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/error.svelte-f0b69c08.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.663604 helics-3.5.2/helics/static/_app/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/pages/__layout.svelte-146b41bd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26271 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/pages/broker.svelte-a984d9f8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/pages/index.svelte-1d030e3b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    54195 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/pages/observe.svelte-8c620952.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19316 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/pages/profile.svelte-c62e0a3a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36765 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/pages/run.svelte-b0de2dfd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23909 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/start-17b7a849.js
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/_app/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-10 23:44:41.000000 helics-3.5.2/helics/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-10 23:44:05.000000 helics-3.5.2/helics/status_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-10 23:44:05.000000 helics-3.5.2/helics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-10 23:44:05.000000 helics-3.5.2/helics/vcredist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.667604 helics-3.5.2/helics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-10 23:44:41.000000 helics-3.5.2/helics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-10 23:44:41.000000 helics-3.5.2/helics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:44:41.000000 helics-3.5.2/helics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 23:44:41.000000 helics-3.5.2/helics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:44:41.000000 helics-3.5.2/helics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 23:44:41.000000 helics-3.5.2/helics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 23:44:41.000000 helics-3.5.2/helics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:44:41.667604 helics-3.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24240 2024-04-10 23:44:05.000000 helics-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:44:41.663604 helics-3.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-10 23:44:05.000000 helics-3.5.2/tests/combinationfederate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-10 23:44:05.000000 helics-3.5.2/tests/filters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17863 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18493 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_badinputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_combinationfederate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35799 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_messagefederate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_messagefilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_pyhelics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24165 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_python_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_systemtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20688 2024-04-10 23:44:05.000000 helics-3.5.2/tests/test_valuefederate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-10 23:44:05.000000 helics-3.5.2/tests/valuefederate.json
```

### Comparing `helics-3.5.1/LICENSE` & `helics-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/PKG-INFO` & `helics-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helics
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python HELICS bindings
 Home-page: https://github.com/GMLC-TDC/pyhelics
 Author: Dheepak Krishnamurthy
 Author-email: me@kdheepak.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/GMLC-TDC/pyhelics/issues
 Keywords: helics,co-simulation
```

### Comparing `helics-3.5.1/README.md` & `helics-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/callbacks.md` & `helics-3.5.2/docs/callbacks.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/cli-interface.md` & `helics-3.5.2/docs/cli-interface.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/10-federates-1-topic/pireceiver.py` & `helics-3.5.2/docs/examples/10-federates-1-topic/pireceiver.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/10-federates-1-topic/pisender.py` & `helics-3.5.2/docs/examples/10-federates-1-topic/pisender.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/10-federates-1-topic/runner.json` & `helics-3.5.2/docs/examples/10-federates-1-topic/runner.json`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-1-topic/README.md` & `helics-3.5.2/docs/examples/2-federates-1-topic/README.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-1-topic/old-pisender.py` & `helics-3.5.2/docs/examples/2-federates-1-topic/old-pisender.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-1-topic/pireceiver.py` & `helics-3.5.2/docs/examples/2-federates-1-topic/pireceiver.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-1-topic/pisender.py` & `helics-3.5.2/docs/examples/2-federates-1-topic/pisender.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-1-topic/runner.json` & `helics-3.5.2/docs/examples/2-federates-1-topic/runner.json`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-3-topics/README.md` & `helics-3.5.2/docs/examples/2-federates-3-topics/README.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-3-topics/pireceiver.py` & `helics-3.5.2/docs/examples/2-federates-3-topics/pireceiver.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-3-topics/pisender.py` & `helics-3.5.2/docs/examples/2-federates-3-topics/pisender.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-3-topics/profile.txt` & `helics-3.5.2/docs/examples/2-federates-3-topics/profile.txt`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/2-federates-3-topics/runner.json` & `helics-3.5.2/docs/examples/2-federates-3-topics/runner.json`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/20-federates-10-topics/README.md` & `helics-3.5.2/docs/examples/20-federates-10-topics/README.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/20-federates-10-topics/pireceiver.py` & `helics-3.5.2/docs/examples/20-federates-10-topics/pireceiver.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/20-federates-10-topics/pisender.py` & `helics-3.5.2/docs/examples/20-federates-10-topics/pisender.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/20-federates-10-topics/profile.txt` & `helics-3.5.2/docs/examples/20-federates-10-topics/profile.txt`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/examples/20-federates-10-topics/runner.json` & `helics-3.5.2/docs/examples/20-federates-10-topics/runner.json`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/installation.md` & `helics-3.5.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/migration-helics2-helics3.md` & `helics-3.5.2/docs/migration-helics2-helics3.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/pythonic-interface.md` & `helics-3.5.2/docs/pythonic-interface.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/usage.md` & `helics-3.5.2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/docs/web-interface.md` & `helics-3.5.2/docs/web-interface.md`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/_build.py` & `helics-3.5.2/helics/_build.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/bin.py` & `helics-3.5.2/helics/bin.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/capi.py` & `helics-3.5.2/helics/capi.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/cli.py` & `helics-3.5.2/helics/cli.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/database.py` & `helics-3.5.2/helics/database.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/flaskr/__init__.py` & `helics-3.5.2/helics/flaskr/__init__.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/observer.py` & `helics-3.5.2/helics/observer.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/profile.py` & `helics-3.5.2/helics/profile.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/assets/fa-29562a41.css` & `helics-3.5.2/helics/static/_app/assets/fa-29562a41.css`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/assets/pages/__layout.svelte-b30f8ab5.css` & `helics-3.5.2/helics/static/_app/assets/pages/__layout.svelte-b30f8ab5.css`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/assets/pages/profile.svelte-7cbf608b.css` & `helics-3.5.2/helics/static/_app/assets/pages/profile.svelte-7cbf608b.css`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/Dropzone-f4be5df7.js` & `helics-3.5.2/helics/static/_app/chunks/Dropzone-f4be5df7.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/ScaledSvg.svelte_svelte_type_style_lang-3a481e75.js` & `helics-3.5.2/helics/static/_app/chunks/ScaledSvg.svelte_svelte_type_style_lang-3a481e75.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/fa-b47ae4c1.js` & `helics-3.5.2/helics/static/_app/chunks/fa-b47ae4c1.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/index-d6b53ebe.js` & `helics-3.5.2/helics/static/_app/chunks/index-d6b53ebe.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/index-e4f78b56.js` & `helics-3.5.2/helics/static/_app/chunks/index-e4f78b56.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/index.es-e33ee127.js` & `helics-3.5.2/helics/static/_app/chunks/index.es-e33ee127.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/index.min-4cad8088.js` & `helics-3.5.2/helics/static/_app/chunks/index.min-4cad8088.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/preload-helper-e4860ae8.js` & `helics-3.5.2/helics/static/_app/chunks/preload-helper-e4860ae8.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/chunks/stores-43842a59.js` & `helics-3.5.2/helics/static/_app/chunks/stores-43842a59.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/error.svelte-f0b69c08.js` & `helics-3.5.2/helics/static/_app/error.svelte-f0b69c08.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/manifest.json` & `helics-3.5.2/helics/static/_app/manifest.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970588235294118%*

 * *Differences: {"'.svelte-kit/runtime/client/start.js'": "{'file': 'start-17b7a849.js'}"}*

```diff
@@ -5,15 +5,15 @@
             ".svelte-kit/runtime/components/error.svelte",
             "src/routes/broker.svelte",
             "src/routes/index.svelte",
             "src/routes/observe.svelte",
             "src/routes/profile.svelte",
             "src/routes/run.svelte"
         ],
-        "file": "start-37b17f1c.js",
+        "file": "start-17b7a849.js",
         "imports": [
             "_index-d6b53ebe.js",
             "_index-e4f78b56.js",
             "_preload-helper-e4860ae8.js"
         ],
         "isEntry": true,
         "src": ".svelte-kit/runtime/client/start.js"
```

### Comparing `helics-3.5.1/helics/static/_app/pages/__layout.svelte-146b41bd.js` & `helics-3.5.2/helics/static/_app/pages/__layout.svelte-146b41bd.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/pages/broker.svelte-a984d9f8.js` & `helics-3.5.2/helics/static/_app/pages/broker.svelte-a984d9f8.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/pages/index.svelte-1d030e3b.js` & `helics-3.5.2/helics/static/_app/pages/index.svelte-1d030e3b.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/pages/observe.svelte-8c620952.js` & `helics-3.5.2/helics/static/_app/pages/observe.svelte-8c620952.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/pages/profile.svelte-c62e0a3a.js` & `helics-3.5.2/helics/static/_app/pages/profile.svelte-c62e0a3a.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/pages/run.svelte-b0de2dfd.js` & `helics-3.5.2/helics/static/_app/pages/run.svelte-b0de2dfd.js`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/_app/start-37b17f1c.js` & `helics-3.5.2/helics/static/_app/start-17b7a849.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -618,15 +618,15 @@
     }
 }
 
 function Nt() {
     const {
         set: r,
         subscribe: e
-    } = ue(!1), t = "1711425133547";
+    } = ue(!1), t = "1712792674013";
     let a;
     async function c() {
         clearTimeout(a);
         const u = await fetch(`${Qe}/_app/version.json`, {
             headers: {
                 pragma: "no-cache",
                 "cache-control": "no-cache"
```

### Comparing `helics-3.5.1/helics/static/favicon.png` & `helics-3.5.2/helics/static/favicon.png`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/static/index.html` & `helics-3.5.2/helics/static/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 <html lang="en">
 	<head>
 		<meta charset="utf-8" />
 		<meta name="description" content="" />
 		<link rel="icon" href="./favicon.png" />
 		<meta name="viewport" content="width=device-width, initial-scale=1" />
 		<meta http-equiv="content-security-policy" content="">
-	<link rel="modulepreload" href="/_app/start-37b17f1c.js">
+	<link rel="modulepreload" href="/_app/start-17b7a849.js">
 	<link rel="modulepreload" href="/_app/chunks/index-d6b53ebe.js">
 	<link rel="modulepreload" href="/_app/chunks/index-e4f78b56.js">
 	<link rel="modulepreload" href="/_app/chunks/preload-helper-e4860ae8.js">
 	</head>
 	<body>
 		<div>
 		<script type="module" data-hydrate="45h">
-		import { start } from "/_app/start-37b17f1c.js";
+		import { start } from "/_app/start-17b7a849.js";
 		start({
 			target: document.querySelector('[data-hydrate="45h"]').parentNode,
 			paths: {"base":"","assets":""},
 			session: {},
 			route: true,
 			spa: true,
 			trailing_slash: "never",
```

### Comparing `helics-3.5.1/helics/status_checker.py` & `helics-3.5.2/helics/status_checker.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics/vcredist.py` & `helics-3.5.2/helics/vcredist.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/helics.egg-info/PKG-INFO` & `helics-3.5.2/helics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helics
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python HELICS bindings
 Home-page: https://github.com/GMLC-TDC/pyhelics
 Author: Dheepak Krishnamurthy
 Author-email: me@kdheepak.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/GMLC-TDC/pyhelics/issues
 Keywords: helics,co-simulation
```

### Comparing `helics-3.5.1/helics.egg-info/SOURCES.txt` & `helics-3.5.2/helics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 helics.egg-info/requires.txt
 helics.egg-info/top_level.txt
 helics/flaskr/__init__.py
 helics/static/favicon.png
 helics/static/index.html
 helics/static/_app/error.svelte-f0b69c08.js
 helics/static/_app/manifest.json
-helics/static/_app/start-37b17f1c.js
+helics/static/_app/start-17b7a849.js
 helics/static/_app/version.json
 helics/static/_app/assets/Dropzone-8e628262.css
 helics/static/_app/assets/ScaledSvg.svelte_svelte_type_style_lang-71598278.css
 helics/static/_app/assets/fa-29562a41.css
 helics/static/_app/assets/pages/__layout.svelte-b30f8ab5.css
 helics/static/_app/assets/pages/profile.svelte-7cbf608b.css
 helics/static/_app/chunks/Dropzone-f4be5df7.js
```

### Comparing `helics-3.5.1/setup.py` & `helics-3.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/combinationfederate.json` & `helics-3.5.2/tests/combinationfederate.json`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/filters.json` & `helics-3.5.2/tests/filters.json`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_api.py` & `helics-3.5.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_badinputs.py` & `helics-3.5.2/tests/test_badinputs.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_combinationfederate.py` & `helics-3.5.2/tests/test_combinationfederate.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_filters.py` & `helics-3.5.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_init.py` & `helics-3.5.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_iteration.py` & `helics-3.5.2/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_messagefederate.py` & `helics-3.5.2/tests/test_messagefederate.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_messagefilter.py` & `helics-3.5.2/tests/test_messagefilter.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_python_api.py` & `helics-3.5.2/tests/test_python_api.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_query.py` & `helics-3.5.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_systemtests.py` & `helics-3.5.2/tests/test_systemtests.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/test_valuefederate.py` & `helics-3.5.2/tests/test_valuefederate.py`

 * *Files identical despite different names*

### Comparing `helics-3.5.1/tests/valuefederate.json` & `helics-3.5.2/tests/valuefederate.json`

 * *Files identical despite different names*

