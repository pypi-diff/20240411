# Comparing `tmp/lsst-pex-config-26.2024.800.tar.gz` & `tmp/lsst-pex-config-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-pex-config-26.2024.800.tar", last modified: Thu Feb 22 10:42:28 2024, max compression
+gzip compressed data, was "lsst-pex-config-26.2024.900.tar", last modified: Thu Feb 29 10:20:08 2024, max compression
```

## Comparing `lsst-pex-config-26.2024.800.tar` & `lsst-pex-config-26.2024.900.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.180342 lsst-pex-config-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-22 10:42:28.180342 lsst-pex-config-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.164342 lsst-pex-config-26.2024.800/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.168341 lsst-pex-config-26.2024.800/doc/lsst.pex.config/
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/doc/lsst.pex.config/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/doc/lsst.pex.config/design-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/doc/lsst.pex.config/field-types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/doc/lsst.pex.config/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/doc/lsst.pex.config/inspecting-configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/doc/lsst.pex.config/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/doc/lsst.pex.config/registry-intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/doc/lsst.pex.config/wrapping-cpp-control-objects.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.168341 lsst-pex-config-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.168341 lsst-pex-config-26.2024.800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.168341 lsst-pex-config-26.2024.800/python/lsst/pex/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.172341 lsst-pex-config-26.2024.800/python/lsst/pex/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/_doNotImportMe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/callStack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/choiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)    61518 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23842 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configChoiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configDictField.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configField.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.172341 lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/_configurableAction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/_configurableActionField.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/_configurableActionStructField.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableField.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/dictField.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/listField.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/rangeField.py
--rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:42:27.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/python/lsst/pex/config/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.176342 lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-22 10:42:28.000000 lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-22 10:42:28.000000 lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:42:28.000000 lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-22 10:42:28.000000 lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:42:28.000000 lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:42:27.000000 lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-22 10:42:28.180342 lsst-pex-config-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:42:28.176342 lsst-pex-config-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/testLib.py
--rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test__file__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_configChoiceField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_configDictField.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_configurableActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_configurableField.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_dictField.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_listField.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_ticket1911.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_ticket1914.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_ticket1915.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_ticket1929.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_ticket1995.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_ticket2818.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_ticketDM-7337.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_unloaded_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-02-22 10:42:15.000000 lsst-pex-config-26.2024.800/tests/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.950757 lsst-pex-config-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-29 10:20:08.950757 lsst-pex-config-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.938757 lsst-pex-config-26.2024.900/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.942757 lsst-pex-config-26.2024.900/doc/lsst.pex.config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/doc/lsst.pex.config/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/doc/lsst.pex.config/design-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/doc/lsst.pex.config/field-types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/doc/lsst.pex.config/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/doc/lsst.pex.config/inspecting-configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/doc/lsst.pex.config/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/doc/lsst.pex.config/registry-intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/doc/lsst.pex.config/wrapping-cpp-control-objects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.938757 lsst-pex-config-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.942757 lsst-pex-config-26.2024.900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.942757 lsst-pex-config-26.2024.900/python/lsst/pex/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.946757 lsst-pex-config-26.2024.900/python/lsst/pex/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/_doNotImportMe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/callStack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/choiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61518 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23842 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configChoiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configDictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configField.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.946757 lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/_configurableAction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/_configurableActionField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/_configurableActionStructField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/dictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/listField.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/rangeField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15871 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:20:08.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/python/lsst/pex/config/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.950757 lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-29 10:20:08.000000 lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-29 10:20:08.000000 lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:08.000000 lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-29 10:20:08.000000 lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:20:08.000000 lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:20:08.000000 lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-29 10:20:08.950757 lsst-pex-config-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:20:08.950757 lsst-pex-config-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/testLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22205 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test__file__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_configChoiceField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_configDictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_configurableActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_configurableField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_dictField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_listField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_ticket1911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_ticket1914.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_ticket1915.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_ticket1929.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_ticket1995.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_ticket2818.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_ticketDM-7337.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_unloaded_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-02-29 10:19:54.000000 lsst-pex-config-26.2024.900/tests/test_wrap.py
```

### Comparing `lsst-pex-config-26.2024.800/PKG-INFO` & `lsst-pex-config-26.2024.900/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pex-config
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: A flexible configuration system using Python files.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License, GPLv3+
 Project-URL: Homepage, https://github.com/lsst/pex_config
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-pex-config-26.2024.800/README.rst` & `lsst-pex-config-26.2024.900/README.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/bsd_license.txt` & `lsst-pex-config-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/doc/lsst.pex.config/CHANGES.rst` & `lsst-pex-config-26.2024.900/doc/lsst.pex.config/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/doc/lsst.pex.config/design-notes.rst` & `lsst-pex-config-26.2024.900/doc/lsst.pex.config/design-notes.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/doc/lsst.pex.config/field-types.rst` & `lsst-pex-config-26.2024.900/doc/lsst.pex.config/field-types.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/doc/lsst.pex.config/index.rst` & `lsst-pex-config-26.2024.900/doc/lsst.pex.config/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/doc/lsst.pex.config/inspecting-configs.rst` & `lsst-pex-config-26.2024.900/doc/lsst.pex.config/inspecting-configs.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/doc/lsst.pex.config/overview.rst` & `lsst-pex-config-26.2024.900/doc/lsst.pex.config/overview.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/doc/lsst.pex.config/registry-intro.rst` & `lsst-pex-config-26.2024.900/doc/lsst.pex.config/registry-intro.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/doc/lsst.pex.config/wrapping-cpp-control-objects.rst` & `lsst-pex-config-26.2024.900/doc/lsst.pex.config/wrapping-cpp-control-objects.rst`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/gpl-v3.0.txt` & `lsst-pex-config-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/pyproject.toml` & `lsst-pex-config-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/__init__.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/callStack.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/callStack.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/choiceField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/choiceField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/comparison.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/comparison.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/config.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/config.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configChoiceField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configChoiceField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configDictField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configDictField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/__init__.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/_configurableAction.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/_configurableAction.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/_configurableActionField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/_configurableActionField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/_configurableActionStructField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/_configurableActionStructField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableActions/tests.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableActions/tests.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/configurableField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/configurableField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/convert.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/convert.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/dictField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/dictField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/history.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/history.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/listField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/listField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/rangeField.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/rangeField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/registry.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/registry.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst/pex/config/wrap.py` & `lsst-pex-config-26.2024.900/python/lsst/pex/config/wrap.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/PKG-INFO` & `lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pex-config
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: A flexible configuration system using Python files.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License, GPLv3+
 Project-URL: Homepage, https://github.com/lsst/pex_config
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-pex-config-26.2024.800/python/lsst_pex_config.egg-info/SOURCES.txt` & `lsst-pex-config-26.2024.900/python/lsst_pex_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/testLib.py` & `lsst-pex-config-26.2024.900/tests/testLib.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_Config.py` & `lsst-pex-config-26.2024.900/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test__file__.py` & `lsst-pex-config-26.2024.900/tests/test__file__.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_configChoiceField.py` & `lsst-pex-config-26.2024.900/tests/test_configChoiceField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_configDictField.py` & `lsst-pex-config-26.2024.900/tests/test_configDictField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_configurableActions.py` & `lsst-pex-config-26.2024.900/tests/test_configurableActions.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_configurableField.py` & `lsst-pex-config-26.2024.900/tests/test_configurableField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_dictField.py` & `lsst-pex-config-26.2024.900/tests/test_dictField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_history.py` & `lsst-pex-config-26.2024.900/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_listField.py` & `lsst-pex-config-26.2024.900/tests/test_listField.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_registry.py` & `lsst-pex-config-26.2024.900/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_ticket1911.py` & `lsst-pex-config-26.2024.900/tests/test_ticket1911.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_ticket1914.py` & `lsst-pex-config-26.2024.900/tests/test_ticket1914.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_ticket1915.py` & `lsst-pex-config-26.2024.900/tests/test_ticket1915.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_ticket1929.py` & `lsst-pex-config-26.2024.900/tests/test_ticket1929.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_ticket1995.py` & `lsst-pex-config-26.2024.900/tests/test_ticket1995.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_ticket2818.py` & `lsst-pex-config-26.2024.900/tests/test_ticket2818.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_ticketDM-7337.py` & `lsst-pex-config-26.2024.900/tests/test_ticketDM-7337.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_unloaded_yaml.py` & `lsst-pex-config-26.2024.900/tests/test_unloaded_yaml.py`

 * *Files identical despite different names*

### Comparing `lsst-pex-config-26.2024.800/tests/test_wrap.py` & `lsst-pex-config-26.2024.900/tests/test_wrap.py`

 * *Files identical despite different names*

