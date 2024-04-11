# Comparing `tmp/logger-36-2024.8.tar.gz` & `tmp/logger-36-2024.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-36-2024.8.tar", last modified: Mon Apr  8 09:26:58 2024, max compression
+gzip compressed data, was "logger-36-2024.9.tar", last modified: Mon Apr  8 09:29:49 2024, max compression
```

## Comparing `logger-36-2024.8.tar` & `logger-36-2024.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.679355 logger-36-2024.8/
--rwx------   0 eric      (1000) users      (984)      139 2024-04-05 17:24:52.000000 logger-36-2024.8/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5577 2024-04-08 09:26:58.676021 logger-36-2024.8/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      642 2024-04-05 16:31:37.000000 logger-36-2024.8/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.8/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     4789 2024-04-05 17:18:38.000000 logger-36-2024.8/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.672688 logger-36-2024.8/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     2244 2024-04-05 17:50:37.000000 logger-36-2024.8/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/
--rwx------   0 eric      (1000) users      (984)     1758 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.672688 logger-36-2024.8/logger_36/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/catalog/config/
--rw-r--r--   0 eric      (1000) users      (984)     2032 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/config/console_rich.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/catalog/handler/
--rw-r--r--   0 eric      (1000) users      (984)     3094 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/handler/console.py
--rwx------   0 eric      (1000) users      (984)     6513 2024-04-05 17:23:55.000000 logger-36-2024.8/logger_36/catalog/handler/console_rich.py
--rwx------   0 eric      (1000) users      (984)     3509 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/handler/file.py
--rwx------   0 eric      (1000) users      (984)     6050 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/handler/generic.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/catalog/logging/
--rw-r--r--   0 eric      (1000) users      (984)     1816 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/logging/chronos.py
--rw-r--r--   0 eric      (1000) users      (984)     2467 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/logging/gpu.py
--rw-r--r--   0 eric      (1000) users      (984)     4040 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/logging/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2449 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/catalog/logging/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/config/
--rw-r--r--   0 eric      (1000) users      (984)     1639 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/config/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     1589 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/config/memory.py
--rwx------   0 eric      (1000) users      (984)     2058 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/config/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1849 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/config/system.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1616 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/generic.py
--rwx------   0 eric      (1000) users      (984)     1683 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/handler.py
--rw-r--r--   0 eric      (1000) users      (984)     1658 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/issue.py
--rw-r--r--   0 eric      (1000) users      (984)     2152 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/logger.py
--rw-r--r--   0 eric      (1000) users      (984)     1797 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     2086 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1683 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/record.py
--rw-r--r--   0 eric      (1000) users      (984)     1802 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/constant/system.py
--rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/instance.py
--rwx------   0 eric      (1000) users      (984)     6692 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/task/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/task/format/
--rw-r--r--   0 eric      (1000) users      (984)     3612 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/format/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     3513 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/format/message.py
--rw-r--r--   0 eric      (1000) users      (984)     1970 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/format/rule.py
--rwx------   0 eric      (1000) users      (984)     4399 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/inspection.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/task/measure/
--rwx------   0 eric      (1000) users      (984)     2255 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/measure/chronos.py
--rwx------   0 eric      (1000) users      (984)     1876 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/measure/memory.py
--rw-r--r--   0 eric      (1000) users      (984)     5028 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/task/storage.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36/type/
--rwx------   0 eric      (1000) users      (984)     5200 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/type/extension.py
--rw-r--r--   0 eric      (1000) users      (984)     2153 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/type/issue.py
--rw-r--r--   0 eric      (1000) users      (984)    12768 2024-04-05 16:31:15.000000 logger-36-2024.8/logger_36/type/logger.py
--rwx------   0 eric      (1000) users      (984)     1577 2024-04-08 09:24:16.000000 logger-36-2024.8/logger_36/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:26:58.676021 logger-36-2024.8/logger_36.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5577 2024-04-08 09:26:58.000000 logger-36-2024.8/logger_36.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-08 09:26:58.000000 logger-36-2024.8/logger_36.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-08 09:26:58.000000 logger-36-2024.8/logger_36.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-08 09:26:58.000000 logger-36-2024.8/logger_36.egg-info/top_level.txt
--rwx------   0 eric      (1000) users      (984)       92 2024-04-08 09:25:57.000000 logger-36-2024.8/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-08 09:26:58.679355 logger-36-2024.8/setup.cfg
--rwx------   0 eric      (1000) users      (984)     6205 2024-04-08 09:18:18.000000 logger-36-2024.8/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/
+-rwx------   0 eric      (1000) users      (984)      139 2024-04-05 17:24:52.000000 logger-36-2024.9/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5569 2024-04-08 09:29:49.216017 logger-36-2024.9/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      642 2024-04-05 16:31:37.000000 logger-36-2024.9/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 logger-36-2024.9/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4781 2024-04-08 09:29:09.000000 logger-36-2024.9/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.212684 logger-36-2024.9/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     2244 2024-04-05 17:50:37.000000 logger-36-2024.9/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/
+-rwx------   0 eric      (1000) users      (984)     1758 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.212684 logger-36-2024.9/logger_36/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/catalog/config/
+-rw-r--r--   0 eric      (1000) users      (984)     2032 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/catalog/config/console_rich.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/catalog/handler/
+-rw-r--r--   0 eric      (1000) users      (984)     3094 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/catalog/handler/console.py
+-rwx------   0 eric      (1000) users      (984)     6513 2024-04-05 17:23:55.000000 logger-36-2024.9/logger_36/catalog/handler/console_rich.py
+-rwx------   0 eric      (1000) users      (984)     3509 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/catalog/handler/file.py
+-rwx------   0 eric      (1000) users      (984)     6050 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/catalog/handler/generic.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/catalog/logging/
+-rw-r--r--   0 eric      (1000) users      (984)     1816 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/catalog/logging/chronos.py
+-rw-r--r--   0 eric      (1000) users      (984)     2467 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/catalog/logging/gpu.py
+-rw-r--r--   0 eric      (1000) users      (984)     4040 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/catalog/logging/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2449 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/catalog/logging/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/config/
+-rw-r--r--   0 eric      (1000) users      (984)     1639 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/config/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     1589 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/config/memory.py
+-rwx------   0 eric      (1000) users      (984)     2058 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/config/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1849 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/config/system.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1616 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/constant/generic.py
+-rwx------   0 eric      (1000) users      (984)     1683 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/constant/handler.py
+-rw-r--r--   0 eric      (1000) users      (984)     1658 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/constant/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)     2152 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/constant/logger.py
+-rw-r--r--   0 eric      (1000) users      (984)     1797 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/constant/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     2086 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/constant/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1683 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/constant/record.py
+-rw-r--r--   0 eric      (1000) users      (984)     1802 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/constant/system.py
+-rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/instance.py
+-rwx------   0 eric      (1000) users      (984)     6692 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/task/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/task/format/
+-rw-r--r--   0 eric      (1000) users      (984)     3612 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/task/format/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     3513 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/task/format/message.py
+-rw-r--r--   0 eric      (1000) users      (984)     1970 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/task/format/rule.py
+-rwx------   0 eric      (1000) users      (984)     4399 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/task/inspection.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/task/measure/
+-rwx------   0 eric      (1000) users      (984)     2255 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/task/measure/chronos.py
+-rwx------   0 eric      (1000) users      (984)     1876 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/task/measure/memory.py
+-rw-r--r--   0 eric      (1000) users      (984)     5028 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/task/storage.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36/type/
+-rwx------   0 eric      (1000) users      (984)     5200 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/type/extension.py
+-rw-r--r--   0 eric      (1000) users      (984)     2153 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/type/issue.py
+-rw-r--r--   0 eric      (1000) users      (984)    12768 2024-04-05 16:31:15.000000 logger-36-2024.9/logger_36/type/logger.py
+-rwx------   0 eric      (1000) users      (984)     1577 2024-04-08 09:29:31.000000 logger-36-2024.9/logger_36/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-08 09:29:49.216017 logger-36-2024.9/logger_36.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5569 2024-04-08 09:29:49.000000 logger-36-2024.9/logger_36.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     1320 2024-04-08 09:29:49.000000 logger-36-2024.9/logger_36.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-08 09:29:49.000000 logger-36-2024.9/logger_36.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       10 2024-04-08 09:29:49.000000 logger-36-2024.9/logger_36.egg-info/top_level.txt
+-rwx------   0 eric      (1000) users      (984)       92 2024-04-08 09:25:57.000000 logger-36-2024.9/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-08 09:29:49.216017 logger-36-2024.9/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     6205 2024-04-08 09:18:18.000000 logger-36-2024.9/setup.py
```

### Comparing `logger-36-2024.8/PKG-INFO` & `logger-36-2024.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.8
+Version: 2024.9
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
@@ -55,15 +55,15 @@
 .. |PYPI_NAME_LITERAL| replace:: ``logger-36``
 .. |PYPI_PROJECT_URL|  replace:: https://pypi.org/project/logger-36/
 .. _PYPI_PROJECT_URL:  https://pypi.org/project/logger-36/
 
 .. |DOCUMENTATION_URL| replace:: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 .. _DOCUMENTATION_URL: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 
-.. |DEPENDENCIES_MANDATORY| replace:: platformdirs
+.. |DEPENDENCIES_MANDATORY| replace:: None
 .. |DEPENDENCIES_OPTIONAL|  replace:: psutil, rich
 
 
 
 ===================================
 |PROJECT_NAME|: |SHORT_DESCRIPTION|
 ===================================
```

### Comparing `logger-36-2024.8/README-COPYRIGHT-utf8.txt` & `logger-36-2024.9/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/README-LICENCE-utf8.txt` & `logger-36-2024.9/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/README.rst` & `logger-36-2024.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 .. |PYPI_NAME_LITERAL| replace:: ``logger-36``
 .. |PYPI_PROJECT_URL|  replace:: https://pypi.org/project/logger-36/
 .. _PYPI_PROJECT_URL:  https://pypi.org/project/logger-36/
 
 .. |DOCUMENTATION_URL| replace:: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 .. _DOCUMENTATION_URL: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 
-.. |DEPENDENCIES_MANDATORY| replace:: platformdirs
+.. |DEPENDENCIES_MANDATORY| replace:: None
 .. |DEPENDENCIES_OPTIONAL|  replace:: psutil, rich
 
 
 
 ===================================
 |PROJECT_NAME|: |SHORT_DESCRIPTION|
 ===================================
```

### Comparing `logger-36-2024.8/documentation/wiki/description.asciidoc` & `logger-36-2024.9/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/__init__.py` & `logger-36-2024.9/logger_36/__init__.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/config/console_rich.py` & `logger-36-2024.9/logger_36/catalog/config/console_rich.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/handler/console.py` & `logger-36-2024.9/logger_36/catalog/handler/console.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/handler/console_rich.py` & `logger-36-2024.9/logger_36/catalog/handler/console_rich.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/handler/file.py` & `logger-36-2024.9/logger_36/catalog/handler/file.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/handler/generic.py` & `logger-36-2024.9/logger_36/catalog/handler/generic.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/logging/chronos.py` & `logger-36-2024.9/logger_36/catalog/logging/chronos.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/logging/gpu.py` & `logger-36-2024.9/logger_36/catalog/logging/gpu.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/logging/memory.py` & `logger-36-2024.9/logger_36/catalog/logging/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/catalog/logging/system.py` & `logger-36-2024.9/logger_36/catalog/logging/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/config/issue.py` & `logger-36-2024.9/logger_36/config/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/config/memory.py` & `logger-36-2024.9/logger_36/config/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/config/message.py` & `logger-36-2024.9/logger_36/config/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/config/system.py` & `logger-36-2024.9/logger_36/config/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/constant/generic.py` & `logger-36-2024.9/logger_36/constant/generic.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/constant/handler.py` & `logger-36-2024.9/logger_36/constant/handler.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/constant/issue.py` & `logger-36-2024.9/logger_36/constant/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/constant/logger.py` & `logger-36-2024.9/logger_36/constant/logger.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/constant/memory.py` & `logger-36-2024.9/logger_36/constant/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/constant/message.py` & `logger-36-2024.9/logger_36/constant/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/constant/record.py` & `logger-36-2024.9/logger_36/constant/record.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/constant/system.py` & `logger-36-2024.9/logger_36/constant/system.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/instance.py` & `logger-36-2024.9/logger_36/instance.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/main.py` & `logger-36-2024.9/logger_36/main.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/task/format/memory.py` & `logger-36-2024.9/logger_36/task/format/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/task/format/message.py` & `logger-36-2024.9/logger_36/task/format/message.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/task/format/rule.py` & `logger-36-2024.9/logger_36/task/format/rule.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/task/inspection.py` & `logger-36-2024.9/logger_36/task/inspection.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/task/measure/chronos.py` & `logger-36-2024.9/logger_36/task/measure/chronos.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/task/measure/memory.py` & `logger-36-2024.9/logger_36/task/measure/memory.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/task/storage.py` & `logger-36-2024.9/logger_36/task/storage.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/type/extension.py` & `logger-36-2024.9/logger_36/type/extension.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/type/issue.py` & `logger-36-2024.9/logger_36/type/issue.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/type/logger.py` & `logger-36-2024.9/logger_36/type/logger.py`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/logger_36/version.py` & `logger-36-2024.9/logger_36/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.8"
+__version__ = "2024.9"
```

### Comparing `logger-36-2024.8/logger_36.egg-info/PKG-INFO` & `logger-36-2024.9/logger_36.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-36
-Version: 2024.8
+Version: 2024.9
 Summary: Simple logger with a catalog of handlers
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/logger-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/logger-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/logger-36/
@@ -55,15 +55,15 @@
 .. |PYPI_NAME_LITERAL| replace:: ``logger-36``
 .. |PYPI_PROJECT_URL|  replace:: https://pypi.org/project/logger-36/
 .. _PYPI_PROJECT_URL:  https://pypi.org/project/logger-36/
 
 .. |DOCUMENTATION_URL| replace:: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 .. _DOCUMENTATION_URL: https://src.koda.cnrs.fr/eric.debreuve/logger-36/-/wikis/home
 
-.. |DEPENDENCIES_MANDATORY| replace:: platformdirs
+.. |DEPENDENCIES_MANDATORY| replace:: None
 .. |DEPENDENCIES_OPTIONAL|  replace:: psutil, rich
 
 
 
 ===================================
 |PROJECT_NAME|: |SHORT_DESCRIPTION|
 ===================================
```

### Comparing `logger-36-2024.8/logger_36.egg-info/SOURCES.txt` & `logger-36-2024.9/logger_36.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logger-36-2024.8/setup.py` & `logger-36-2024.9/setup.py`

 * *Files identical despite different names*

