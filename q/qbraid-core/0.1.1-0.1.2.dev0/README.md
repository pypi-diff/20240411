# Comparing `tmp/qbraid-core-0.1.1.tar.gz` & `tmp/qbraid-core-0.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-core-0.1.1.tar", last modified: Wed Apr 10 00:15:27 2024, max compression
+gzip compressed data, was "qbraid-core-0.1.2.dev0.tar", last modified: Thu Apr 11 20:00:37 2024, max compression
```

## Comparing `qbraid-core-0.1.1.tar` & `qbraid-core-0.1.2.dev0.tar`

### file list

```diff
@@ -1,92 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.918968 qbraid-core-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-10 00:15:27.918968 qbraid-core-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.906968 qbraid-core-0.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.910968 qbraid-core-0.1.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.910968 qbraid-core-0.1.1/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.910968 qbraid-core-0.1.1/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.910968 qbraid-core-0.1.1/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/qbraid_core/system/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 00:15:27.000000 qbraid-core-0.1.1/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 00:15:27.918968 qbraid-core-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tests/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:15:27.914968 qbraid-core-0.1.1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-10 00:15:23.000000 qbraid-core-0.1.1/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.802847 qbraid-core-0.1.2.dev0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.802847 qbraid-core-0.1.2.dev0/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.802847 qbraid-core-0.1.2.dev0/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.806846 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.806846 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.806846 qbraid-core-0.1.2.dev0/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_create_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_create_local_venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_delete_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_installed_envs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_system_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_system_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_update_install_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/.github/workflows/docs.yml` & `qbraid-core-0.1.2.dev0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/.github/workflows/format.yml` & `qbraid-core-0.1.2.dev0/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/.github/workflows/main.yml` & `qbraid-core-0.1.2.dev0/.github/workflows/main.yml`

 * *Files 14% similar despite different names*

```diff
@@ -32,17 +32,18 @@
         uses: actions/upload-artifact@v3
         with:
           name: built-package
           path: dist/*.whl
 
   test:
     needs: build
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
+        os: [ubuntu-latest, windows-latest]
         python-version: ['3.9', '3.10', '3.11', '3.12']
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
@@ -51,15 +52,20 @@
       - name: Download built package
         uses: actions/download-artifact@v3
         with:
           name: built-package
           path: dist
       - name: Install package
         run: |
-          pip install dist/*.whl
+          if ($env:RUNNER_OS -eq "Windows") {
+            Get-ChildItem dist/*.whl | ForEach-Object { pip install $_.FullName }
+          } else {
+            pip install dist/*.whl
+          }
+        shell: pwsh
       - name: Install testing dependencies
         run: |
           pip install pytest
       - name: Run tests with pytest
         run: |
           pytest
         env:
```

### Comparing `qbraid-core-0.1.1/.github/workflows/publish.yml` & `qbraid-core-0.1.2.dev0/.github/workflows/test-publish.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-name: Publish to PyPI
+name: Publish to TestPyPI
 
 on:
-  release:
-    types: [published]
   workflow_dispatch:
 
 jobs:
   pypi-publish:
-    name: Build dist & upload to PyPI
+    name: Build dist & upload to TestPyPI
     runs-on: ubuntu-latest
     environment: publish
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 1
 
@@ -20,13 +18,13 @@
         with:
           python-version: '3.11'
 
       - name: Build binary wheel + source tarball
         run: |
           python3 -m pip install --upgrade pip build
           python3 -m build
-
-      - name: Publish package to PyPI
+      - name: Publish package to TestPyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+          repository-url: https://test.pypi.org/legacy/
```

### Comparing `qbraid-core-0.1.1/.github/workflows/test-publish.yml` & `qbraid-core-0.1.2.dev0/.github/workflows/publish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-name: Publish to TestPyPI
+name: Publish to PyPI
 
 on:
+  # release:
+  #   types: [published]
   workflow_dispatch:
 
 jobs:
   pypi-publish:
-    name: Build dist & upload to TestPyPI
+    name: Build dist & upload to PyPI
     runs-on: ubuntu-latest
     environment: publish
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 1
 
@@ -18,13 +20,13 @@
         with:
           python-version: '3.11'
 
       - name: Build binary wheel + source tarball
         run: |
           python3 -m pip install --upgrade pip build
           python3 -m build
-      - name: Publish package to TestPyPI
+
+      - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository-url: https://test.pypi.org/legacy/
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `qbraid-core-0.1.1/.gitignore` & `qbraid-core-0.1.2.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/LICENSE` & `qbraid-core-0.1.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/PKG-INFO` & `qbraid-core-0.1.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.1
+Version: 0.1.2.dev0
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.1/README.md` & `qbraid-core-0.1.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/Makefile` & `qbraid-core-0.1.2.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/_static/cards/jupyter.png` & `qbraid-core-0.1.2.dev0/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/_static/cards/python.png` & `qbraid-core-0.1.2.dev0/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/_static/cards/terminal.png` & `qbraid-core-0.1.2.dev0/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/_static/css/custom.css` & `qbraid-core-0.1.2.dev0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/_static/css/s4defs-roles.css` & `qbraid-core-0.1.2.dev0/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/_static/favicon.ico` & `qbraid-core-0.1.2.dev0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/_static/logo.png` & `qbraid-core-0.1.2.dev0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/conf.py` & `qbraid-core-0.1.2.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/index.rst` & `qbraid-core-0.1.2.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/docs/make.bat` & `qbraid-core-0.1.2.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/pyproject.toml` & `qbraid-core-0.1.2.dev0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.1"
+version = "0.1.2.dev0"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
@@ -39,14 +39,15 @@
 docs = ["sphinx~=7.2.6", "sphinx-rtd-theme>=1.3,<2.1", "sphinx-autodoc-typehints>=1.24,<2.1", "docutils<0.21"]
 
 [tool.setuptools_scm]
 write_to = "qbraid_core/_version.py"
 
 [tool.black]
 line-length = 100
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
```

### Comparing `qbraid-core-0.1.1/qbraid_core/__init__.py` & `qbraid-core-0.1.2.dev0/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/_compat.py` & `qbraid-core-0.1.2.dev0/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/client.py` & `qbraid-core-0.1.2.dev0/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/config.py` & `qbraid-core-0.1.2.dev0/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/exceptions.py` & `qbraid-core-0.1.2.dev0/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/registry.py` & `qbraid-core-0.1.2.dev0/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/retry.py` & `qbraid-core-0.1.2.dev0/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/environments/__init__.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/environments/client.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/environments/create.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/environments/paths.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 
 from qbraid_core.system import is_valid_python
 
 from .validate import is_valid_slug
 
 logger = logging.getLogger(__name__)
 
+DEFAULT_LOCAL_ENVS_PATH = Path.home() / ".qbraid" / "environments"
+
 
 def get_default_envs_paths() -> List[Path]:
     """
     Returns a list of paths to qBraid environments.
 
     If the QBRAID_ENVS_PATH environment variable is set, it splits the variable by ':' to
     accommodate multiple paths. If QBRAID_ENVS_PATH is not set, returns a list containing
     the default qBraid environments path (~/.qbraid/environments).
 
     Returns:
         A list of pathlib.Path objects representing the qBraid environments paths.
     """
-    qbraid_envs_path = os.getenv("QBRAID_ENVS_PATH", str(Path.home() / ".qbraid" / "environments"))
-    return [Path(path) for path in qbraid_envs_path.split(":")]
+    qbraid_envs_path = os.getenv("QBRAID_ENVS_PATH", str(DEFAULT_LOCAL_ENVS_PATH))
+    return [Path(path) for path in qbraid_envs_path.split(os.pathsep)]
 
 
 def get_env_path(slug: str) -> Path:
     """Return path to qbraid environment.
 
     Args:
         slug (str): The environment directory to search for.
```

### Comparing `qbraid-core-0.1.1/qbraid_core/services/environments/state.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/environments/validate.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/quantum/__init__.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/quantum/adapter.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/quantum/client.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/services/quantum/proxy.py` & `qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/sessions.py` & `qbraid-core-0.1.2.dev0/qbraid_core/sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/system/__init__.py` & `qbraid-core-0.1.2.dev0/qbraid_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/system/generic.py` & `qbraid-core-0.1.2.dev0/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core/system/packages.py` & `qbraid-core-0.1.2.dev0/qbraid_core/system/packages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
 Module for serving information about Python packages.
 
 """
+import ast
 import logging
 import site
+import subprocess
 import sys
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
 
 import requests
 
 from .exceptions import QbraidSystemError
-from .executables import get_python_version_from_cfg, get_python_version_from_exe
+from .executables import (
+    get_active_python_path,
+    get_python_version_from_cfg,
+    get_python_version_from_exe,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def get_venv_site_packages_path(venv_path: Path) -> Path:
     """
     Determines the site-packages directory for a given virtual environment in an OS-agnostic manner.
@@ -53,32 +59,59 @@
 
     major_minor_version = ".".join(python_version.split(".")[:2])
     lib_python_dir = venv_path / f"lib/python{major_minor_version}"
     return lib_python_dir / "site-packages"
 
 
 def get_active_site_packages_path() -> Path:
-    """Retrieves the site-packages path of the current Python environment."""
+    """
+    Retrieves the site-packages path of the current Python environment,
+    respecting active virtual environments, as well.
+
+    """
+
+    current_python_path = Path(sys.executable)
+    shell_python_path = get_active_python_path()
 
-    # List of all site-packages directories as Path objects
-    site_packages_paths = [Path(path) for path in site.getsitepackages()]
+    if shell_python_path == current_python_path:
+        site_packages_paths = [Path(path) for path in site.getsitepackages()]
 
+    else:
+        try:
+            result = subprocess.run(
+                [shell_python_path, "-c", "import site; print(site.getsitepackages())"],
+                capture_output=True,
+                text=True,
+                check=True,
+            )
+        except subprocess.CalledProcessError as err:
+            raise QbraidSystemError(
+                "Failed to get user site-packages directory from the shell's Python interpreter."
+            ) from err
+
+        paths = ast.literal_eval(result.stdout.strip())
+        site_packages_paths = [Path(path) for path in paths]
+
+    # Common logic for finding the correct site-packages path
     if len(site_packages_paths) == 1:
         return site_packages_paths[0]
 
-    # Path to the currently running Python interpreter
-    python_executable_path = Path(sys.executable)
-
     # Base path of the Python environment
-    env_base_path = python_executable_path.parent.parent
+    shell_base_path = shell_python_path.parent.parent
+    sys_base_path = current_python_path.parent.parent
+
+    base_paths = [shell_base_path]
+    if shell_base_path != sys_base_path:
+        base_paths.append(sys_base_path)
 
     # Find the site-packages path that is within the same environment
-    for path in site_packages_paths:
-        if env_base_path in path.parents:
-            return path
+    for base_path in base_paths:
+        for path in site_packages_paths:
+            if base_path in path.parents:
+                return path
 
     raise QbraidSystemError("Failed to find site-packages path.")
 
 
 def get_local_package_path(package: str) -> Path:
     """Retrieves the local path of a package."""
     try:
```

### Comparing `qbraid-core-0.1.1/qbraid_core/system/threader.py` & `qbraid-core-0.1.2.dev0/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/qbraid_core.egg-info/PKG-INFO` & `qbraid-core-0.1.2.dev0/qbraid_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.1
+Version: 0.1.2.dev0
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.1/qbraid_core.egg-info/SOURCES.txt` & `qbraid-core-0.1.2.dev0/qbraid_core.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -60,13 +60,20 @@
 qbraid_core/system/packages.py
 qbraid_core/system/threader.py
 tests/__init__.py
 tests/conftest.py
 tests/test_client.py
 tests/test_compat.py
 tests/test_config.py
+tests/test_create_environment.py
+tests/test_create_local_venv.py
+tests/test_delete_environment.py
 tests/test_environments.py
+tests/test_installed_envs_data.py
+tests/test_replace_str.py
 tests/test_session.py
-tests/test_system.py
+tests/test_system_executables.py
+tests/test_system_packages.py
+tests/test_update_install_status.py
 tests/fixtures/__init__.py
 tests/fixtures/environments.py
 tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.1/tests/fixtures/environments.py` & `qbraid-core-0.1.2.dev0/tests/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/tests/test_client.py` & `qbraid-core-0.1.2.dev0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/tests/test_compat.py` & `qbraid-core-0.1.2.dev0/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/tests/test_config.py` & `qbraid-core-0.1.2.dev0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/tests/test_environments.py` & `qbraid-core-0.1.2.dev0/tests/test_environments.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,25 +85,28 @@
         slug = env["slug"]
         assert is_valid_slug(slug)
 
 
 def test_get_default_envs_paths_with_env_var_set(monkeypatch):
     """Test the get_qbraid_envs_paths function when QBRAID_ENVS_PATH is set."""
     # Mocking QBRAID_ENVS_PATH with two paths for the test
-    mock_envs_path = "/path/to/envs1:/path/to/envs2"
+    mock_path_1, mock_path_2 = "/path/to/envs1", "/path/to/envs2"
+    mock_envs_path = mock_path_1 + os.pathsep + mock_path_2
     monkeypatch.setenv("QBRAID_ENVS_PATH", mock_envs_path)
 
-    expected_paths = [Path("/path/to/envs1"), Path("/path/to/envs2")]
+    expected_paths = [Path(mock_path_1), Path(mock_path_2)]
+    default_paths = get_default_envs_paths()
     assert (
-        get_default_envs_paths() == expected_paths
+        default_paths == expected_paths
     ), "Should return paths from QBRAID_ENVS_PATH environment variable"
 
 
 def test_get_qbraid_envs_paths_with_no_env_var_set(monkeypatch):
     """Test the get_qbraid_envs_paths function when QBRAID_ENVS_PATH is not set."""
     # Removing QBRAID_ENVS_PATH to simulate it not being set
     monkeypatch.delenv("QBRAID_ENVS_PATH", raising=False)
 
-    expected_path = Path.home() / ".qbraid" / "environments"
-    assert get_default_envs_paths() == [
-        expected_path
-    ], "Should return the default path when QBRAID_ENVS_PATH is not set"
+    expected_paths = [str(Path.home() / ".qbraid" / "environments")]
+    default_paths = [str(path) for path in get_default_envs_paths()]
+    assert (
+        default_paths == expected_paths
+    ), "Should return the default path when QBRAID_ENVS_PATH is not set"
```

### Comparing `qbraid-core-0.1.1/tests/test_session.py` & `qbraid-core-0.1.2.dev0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.1/tools/verify_headers.py` & `qbraid-core-0.1.2.dev0/tools/verify_headers.py`

 * *Files identical despite different names*

