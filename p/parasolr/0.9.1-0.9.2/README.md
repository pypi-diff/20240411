# Comparing `tmp/parasolr-0.9.1.tar.gz` & `tmp/parasolr-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parasolr-0.9.1.tar", last modified: Thu Oct  5 20:58:33 2023, max compression
+gzip compressed data, was "parasolr-0.9.2.tar", last modified: Thu Apr 11 21:35:08 2024, max compression
```

## Comparing `parasolr-0.9.1.tar` & `parasolr-0.9.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-05 20:58:22.000000 parasolr-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-05 20:58:22.000000 parasolr-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2023-10-05 20:58:33.888354 parasolr-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2023-10-05 20:58:22.000000 parasolr-0.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.884354 parasolr-0.9.1/parasolr/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/parasolr/django/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/disconnect_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/solrclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/parasolr/django/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/tests/test_django_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/parasolr/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/parasolr/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/management/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/management/commands/solr_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/parasolr/query/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/query/aliased_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27046 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/query/queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/parasolr/solr/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/solr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/solr/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/solr/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/solr/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/solr/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/solr/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/parasolr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10547 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-10-05 20:58:22.000000 parasolr-0.9.1/parasolr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:58:33.888354 parasolr-0.9.1/parasolr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2023-10-05 20:58:33.000000 parasolr-0.9.1/parasolr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-10-05 20:58:33.000000 parasolr-0.9.1/parasolr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 20:58:33.000000 parasolr-0.9.1/parasolr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-05 20:58:33.000000 parasolr-0.9.1/parasolr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-10-05 20:58:33.000000 parasolr-0.9.1/parasolr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-05 20:58:33.000000 parasolr-0.9.1/parasolr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-10-05 20:58:33.888354 parasolr-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-10-05 20:58:22.000000 parasolr-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.600297 parasolr-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 21:35:01.000000 parasolr-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-11 21:35:01.000000 parasolr-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-11 21:35:08.600297 parasolr-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-11 21:35:01.000000 parasolr-0.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.596297 parasolr-0.9.2/parasolr/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.596297 parasolr-0.9.2/parasolr/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/disconnect_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/solrclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.596297 parasolr-0.9.2/parasolr/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/tests/test_django_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.596297 parasolr-0.9.2/parasolr/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.596297 parasolr-0.9.2/parasolr/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/management/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/management/commands/solr_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.600297 parasolr-0.9.2/parasolr/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/query/aliased_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27046 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/query/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.600297 parasolr-0.9.2/parasolr/solr/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/solr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/solr/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/solr/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/solr/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/solr/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/solr/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.600297 parasolr-0.9.2/parasolr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-11 21:35:01.000000 parasolr-0.9.2/parasolr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:35:08.600297 parasolr-0.9.2/parasolr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-11 21:35:08.000000 parasolr-0.9.2/parasolr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-11 21:35:08.000000 parasolr-0.9.2/parasolr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:35:08.000000 parasolr-0.9.2/parasolr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 21:35:08.000000 parasolr-0.9.2/parasolr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-11 21:35:08.000000 parasolr-0.9.2/parasolr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 21:35:08.000000 parasolr-0.9.2/parasolr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 21:35:08.604297 parasolr-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-11 21:35:01.000000 parasolr-0.9.2/setup.py
```

### Comparing `parasolr-0.9.1/LICENSE` & `parasolr-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/PKG-INFO` & `parasolr-0.9.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: parasolr
-Version: 0.9.1
-Summary: Lightweight python library for Solr indexing, searching and schema management with optional Django integration.
-Home-page: https://github.com/Princeton-CDH/parasolr
-Author: The Center for Digital Humanities at Princeton
-Author-email: cdhdevteam@princeton.edu
-License: Apache License, Version 2.0
-Classifier: Environment :: Web Environment
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Pytest
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Database
-Provides-Extra: test
-Provides-Extra: django
-Provides-Extra: dev
-License-File: LICENSE
-
 parasolr
 ==============
 
 .. sphinx-start-marker-do-not-remove
 
 **parasolr** is a lightweight python library for `Apache Solr`_ indexing,
 searching and schema management with optional `Django`_ integration.
@@ -71,26 +42,22 @@
    :target: https://www.codefactor.io/repository/github/princeton-cdh/parasolr
    :alt: CodeFactor
 
   .. image:: https://api.codeclimate.com/v1/badges/73394d05decdf32f12f3/maintainability
    :target: https://codeclimate.com/github/Princeton-CDH/parasolr/maintainability
    :alt: Maintainability
 
-  .. image:: https://requires.io/github/Princeton-CDH/parasolr/requirements.svg?branch=main
-    :target: https://requires.io/github/Princeton-CDH/parasolr/requirements/?branch=main
-    :alt: Requirements Status
-
   .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: code style: Black
 
   .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
-Tested against Python 3.9-3.11, Solr 8.6 and 9.2, and Django 3.2-4.0 and without Django.
+Tested against Python 3.9-3.11, Solr 8.6 and 9.2, and Django 3.2-5.0 and without Django.
 
 
 Installation
 ------------
 
 Install released version from pypi::
 
@@ -128,15 +95,15 @@
 Development instructions
 ------------------------
 
 This git repository uses git flow branching conventions.
 
 Initial setup and installation:
 
-- *Recommmended*: create and activate a Python 3.6 virtualenv::
+- *Recommmended*: create and activate a Python 3.x virtualenv::
 
    python3 -m venv parasolr
    source parasolr/bin/activate
 
 - Install the package with its dependencies as well as development
   dependencies::
 
@@ -190,13 +157,13 @@
 
 
 License
 -------
 
 **parasolr** is distributed under the Apache 2.0 License.
 
-©2019 Trustees of Princeton University.  Permission granted via
+©2019-2024 Trustees of Princeton University.  Permission granted via
 Princeton Docket #20-3619 for distribution online under a standard Open Source
 license.  Ownership rights transferred to Rebecca Koeser provided software
 is distributed online via open source.
```

### Comparing `parasolr-0.9.1/README.rst` & `parasolr-0.9.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,54 @@
+Metadata-Version: 2.1
+Name: parasolr
+Version: 0.9.2
+Summary: Lightweight python library for Solr indexing, searching and schema management with optional Django integration.
+Home-page: https://github.com/Princeton-CDH/parasolr
+Author: The Center for Digital Humanities at Princeton
+Author-email: cdhdevteam@princeton.edu
+License: Apache License, Version 2.0
+Classifier: Environment :: Web Environment
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Database
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: addict
+Requires-Dist: progressbar2
+Provides-Extra: test
+Requires-Dist: pytest>=7; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Provides-Extra: django
+Requires-Dist: django>=3.0; extra == "django"
+Requires-Dist: pytest-django>=3.6; extra == "django"
+Provides-Extra: dev
+Requires-Dist: pytest>=7; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinxcontrib-napoleon; extra == "dev"
+Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: django>=3.0; extra == "dev"
+Requires-Dist: pytest-django>=3.6; extra == "dev"
+
 parasolr
 ==============
 
 .. sphinx-start-marker-do-not-remove
 
 **parasolr** is a lightweight python library for `Apache Solr`_ indexing,
 searching and schema management with optional `Django`_ integration.
@@ -42,26 +89,22 @@
    :target: https://www.codefactor.io/repository/github/princeton-cdh/parasolr
    :alt: CodeFactor
 
   .. image:: https://api.codeclimate.com/v1/badges/73394d05decdf32f12f3/maintainability
    :target: https://codeclimate.com/github/Princeton-CDH/parasolr/maintainability
    :alt: Maintainability
 
-  .. image:: https://requires.io/github/Princeton-CDH/parasolr/requirements.svg?branch=main
-    :target: https://requires.io/github/Princeton-CDH/parasolr/requirements/?branch=main
-    :alt: Requirements Status
-
   .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: code style: Black
 
   .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
-Tested against Python 3.9-3.11, Solr 8.6 and 9.2, and Django 3.2-4.0 and without Django.
+Tested against Python 3.9-3.11, Solr 8.6 and 9.2, and Django 3.2-5.0 and without Django.
 
 
 Installation
 ------------
 
 Install released version from pypi::
 
@@ -99,15 +142,15 @@
 Development instructions
 ------------------------
 
 This git repository uses git flow branching conventions.
 
 Initial setup and installation:
 
-- *Recommmended*: create and activate a Python 3.6 virtualenv::
+- *Recommmended*: create and activate a Python 3.x virtualenv::
 
    python3 -m venv parasolr
    source parasolr/bin/activate
 
 - Install the package with its dependencies as well as development
   dependencies::
 
@@ -161,13 +204,13 @@
 
 
 License
 -------
 
 **parasolr** is distributed under the Apache 2.0 License.
 
-©2019 Trustees of Princeton University.  Permission granted via
+©2019-2024 Trustees of Princeton University.  Permission granted via
 Princeton Docket #20-3619 for distribution online under a standard Open Source
 license.  Ownership rights transferred to Rebecca Koeser provided software
 is distributed online via open source.
```

### Comparing `parasolr-0.9.1/parasolr/django/indexing.py` & `parasolr-0.9.2/parasolr/django/indexing.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/django/queryset.py` & `parasolr-0.9.2/parasolr/django/queryset.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/django/signals.py` & `parasolr-0.9.2/parasolr/django/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -131,34 +131,47 @@
                     signal_name,
                     model,
                 )
                 model_signal.connect(handler, sender=model)
 
     @staticmethod
     def disconnect():
-        """disconnect indexing signal handlers"""
+        """disconnect indexing signal handlers; returns a count of
+        the number of signal handlers disconnected"""
+        total = 0
         for model in ModelIndexable.__subclasses__():
             logger.debug("Disconnecting signal handlers for %s", model)
-            models.signals.post_save.disconnect(
+            # disconnect returns true if anything was disconnected
+            disconnected = models.signals.post_save.disconnect(
                 IndexableSignalHandler.handle_save, sender=model
             )
-            models.signals.post_delete.disconnect(
+            if disconnected:
+                total += 1
+            disconnect = models.signals.post_delete.disconnect(
                 IndexableSignalHandler.handle_delete, sender=model
             )
+            if disconnected:
+                total += 1
 
         for m2m_rel in ModelIndexable.m2m:
             logger.debug("Disconnecting m2m signal handler for %s", m2m_rel)
-            models.signals.m2m_changed.disconnect(
+            disconnect = models.signals.m2m_changed.disconnect(
                 IndexableSignalHandler.handle_relation_change, sender=m2m_rel
             )
+            if disconnected:
+                total += 1
 
         for model, options in ModelIndexable.related:
             for signal_name, handler in options.items():
                 model_signal = getattr(models.signals, signal_name)
                 logger.debug(
                     "Disconnecting %s signal handler for %s", signal_name, model
                 )
-                model_signal.disconnect(handler, sender=model)
+                disconnected = model_signal.disconnect(handler, sender=model)
+                if disconnected:
+                    total += 1
+
+        return total
 
 
 if django:
     IndexableSignalHandler.connect()
```

### Comparing `parasolr-0.9.1/parasolr/django/solrclient.py` & `parasolr-0.9.2/parasolr/django/solrclient.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/django/tests/test_django.py` & `parasolr-0.9.2/parasolr/django/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/django/tests/test_django_signals.py` & `parasolr-0.9.2/parasolr/django/tests/test_django_signals.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,14 +49,28 @@
 
         # testing related handlers based on test models
         post_save_handlers = [item[1] for item in models.signals.post_save.receivers]
         assert ref(test_models.signal_method) in post_save_handlers
         pre_del_handlers = [item[1] for item in models.signals.pre_delete.receivers]
         assert ref(test_models.signal_method) in pre_del_handlers
 
+    def test_disconnect(self):
+        # handlers should already be connected based on test module setup
+        count = IndexableSignalHandler.disconnect()
+        # should return a non-zero count of handlers disconnected
+        # (currently 13, but not sure exact number matters)
+        assert count
+
+        # disconnecting a second time should return zero (nothing disconnected)
+        second_count = IndexableSignalHandler.disconnect()
+        assert not second_count
+
+        # reconnect for other tests
+        IndexableSignalHandler.connect()
+
     def test_handle_save(self):
         instance = test_models.IndexItem()
         with patch.object(instance, "index") as mockindex:
             # call directly
             IndexableSignalHandler.handle_save(Mock(), instance)
             mockindex.assert_any_call()
 
@@ -83,15 +97,14 @@
 
     @pytest.mark.django_db
     def test_handle_relation_change(self):
         instance = test_models.IndexItem()
         with patch.object(instance, "index") as mockindex:
             # call directly - supported actions
             for action in ["post_add", "post_remove", "post_clear"]:
-
                 mockindex.reset_mock()
                 IndexableSignalHandler.handle_relation_change(
                     test_models.IndexItem, instance, action
                 )
                 mockindex.assert_any_call()
 
             # if action is not one we care about, should be ignored
```

### Comparing `parasolr-0.9.1/parasolr/django/tests/test_models.py` & `parasolr-0.9.2/parasolr/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/django/views.py` & `parasolr-0.9.2/parasolr/django/views.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/indexing.py` & `parasolr-0.9.2/parasolr/indexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,15 +160,18 @@
         """
 
         # make sure solr client is initialized
         Indexable._init_solr()
 
         # if this is a queryset, use iterator to get it in chunks
         if QuerySet and isinstance(items, QuerySet):
-            items = items.iterator()
+            # starting in django 4.1, chunk_size is None by default
+            # (previous default was 2000);
+            # chunk size is required when using prefetching
+            items = items.iterator(chunk_size=cls.index_chunk_size)
 
         # if this is a normal list, convert it to an iterator
         # so we don't iterate the same slice over and over
         elif isinstance(items, list):
             items = iter(items)
 
         # index in chunks to support efficiently indexing large numbers
```

### Comparing `parasolr-0.9.1/parasolr/management/commands/index.py` & `parasolr-0.9.2/parasolr/management/commands/index.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/management/commands/solr_schema.py` & `parasolr-0.9.2/parasolr/management/commands/solr_schema.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/pytest_plugin.py` & `parasolr-0.9.2/parasolr/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/query/aliased_queryset.py` & `parasolr-0.9.2/parasolr/query/aliased_queryset.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,20 @@
         self, field: str, exclude: str = "", **kwargs
     ) -> "AliasedSolrQuerySet":
         """Extend :meth:`parasolr.query.queryset.SolrQuerySet.facet_field``
         to support using aliased field names for field parameter."""
         field = self.field_aliases.get(field, field)
         return super().facet_field(field, exclude=exclude, **kwargs)
 
+    def search(self, *args, **kwargs) -> "AliasedSolrQuerySet":
+        """Extend :meth:`parasolr.query.queryset.SolrQuerySet.search`
+        to support using aliased field names for keyword argument keys."""
+        kwargs = self._unalias_kwargs_with_lookups(**kwargs)
+        return super().search(*args, **kwargs)
+
     def order_by(self, *args) -> "AliasedSolrQuerySet":
         """Extend :meth:`parasolr.query.queryset.SolrQuerySet.order_by``
         to support using aliased field names in sort arguments."""
         args = self._unalias_args(*args)
         return super().order_by(*args)
 
     def only(self, *args, **kwargs) -> "AliasedSolrQuerySet":
```

### Comparing `parasolr-0.9.1/parasolr/query/queryset.py` & `parasolr-0.9.2/parasolr/query/queryset.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/schema.py` & `parasolr-0.9.2/parasolr/schema.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/solr/admin.py` & `parasolr-0.9.2/parasolr/solr/admin.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/solr/base.py` & `parasolr-0.9.2/parasolr/solr/base.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/solr/client.py` & `parasolr-0.9.2/parasolr/solr/client.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/solr/schema.py` & `parasolr-0.9.2/parasolr/solr/schema.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/solr/update.py` & `parasolr-0.9.2/parasolr/solr/update.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/tests/test_commands.py` & `parasolr-0.9.2/parasolr/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr/tests/test_indexing.py` & `parasolr-0.9.2/parasolr/tests/test_indexing.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         # progress bar update method should be called once for each chunk
         assert mock_progbar.update.call_count == 2
 
     def test_index_items__queryset(self, mocksolr):
         # index a queryset
         mockqueryset = MagicMock(spec=QuerySet)
         Indexable.index_items(mockqueryset)
-        mockqueryset.iterator.assert_called_with()
+        mockqueryset.iterator.assert_called_with(chunk_size=Indexable.index_chunk_size)
 
     def test_items_to_index(self, mocksolr):
         # assumes django model manager interface by default
 
         # simple object with objects.all interface
         simple_items_to_index = SimpleIndexable.items_to_index()
         assert len(simple_items_to_index) == 5
```

### Comparing `parasolr-0.9.1/parasolr/tests/test_pytest_plugin.py` & `parasolr-0.9.2/parasolr/tests/test_pytest_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,18 +64,14 @@
 def test_configure_django_test_solr(testdir):
     """Basic check of django solr pytest fixture."""
 
     solr_url = settings.SOLR_CONNECTIONS["default"]["URL"]
     solr_test_collection = settings.SOLR_CONNECTIONS["default"]["TEST"]["COLLECTION"]
     solr_commit_within = settings.SOLR_CONNECTIONS["default"]["TEST"]["COMMITWITHIN"]
 
-    # NOTE: can't figure out how to get the plugin test to use
-    # test-local test settings, so testing against project
-    # testsettings for now
-
     # create a temporary pytest test file
     testdir.makepyfile(
         """
         from parasolr.django import SolrClient
 
         # causes "Plugin already registered" error on travis...
         # pytest_plugins = "parasolr.pytest_plugin"
@@ -91,25 +87,32 @@
             # core should exist
             assert solr.core_admin.status(core=test_collection)
 
     """
         % (solr_url, solr_test_collection, solr_commit_within)
     )
 
+    # copy local test settings into the test dir
+    testdir.copy_example("testsettings.py")
+
     # run all tests with pytest with all pytest-django plugins turned off
     # result = testdir.runpytest('-p', 'no:django')
     result = testdir.runpytest_subprocess("--capture", "no")
     # check that test case passed
     result.assert_outcomes(passed=1)
 
 
 @skipif_no_django
 def test_not_configured(testdir):
     """skip without error if not configured."""
 
+    # copy local test settings into the test dir,
+    # or else pytest-django complains about not finding django project
+    testdir.copy_example("testsettings.py")
+
     with override_settings(SOLR_CONNECTIONS=None):
         assert not get_test_solr_config()
 
         # create a temporary pytest test file with no solr use
         testdir.makepyfile(
             """
         def test_unrelated():
@@ -130,19 +133,18 @@
         mockapps.is_installed.return_value = False
         assert not get_test_solr_config()
         mockapps.is_installed.assert_called_with("parasolr")
 
 
 @skipif_no_django
 def test_empty_solr(testdir):
-    """Check empty_solr pytest fixture."""
+    """Check empty_solr pytest fixture."""
 
-    # NOTE: can't figure out how to get the plugin test to use
-    # test-local test settings, so testing against project
-    # testsettings for now
+    # copy local test settings into the test dir
+    testdir.copy_example("testsettings.py")
 
     # create a temporary pytest test file
     testdir.makepyfile(
         """
         from parasolr.django import SolrClient
 
         # causes "Plugin already registered" error on travis...
@@ -197,14 +199,17 @@
     mock_qs = mock_qs_cls()
     assert mock_qs.custom_method.return_value == mock_qs
 
 
 def test_get_mock_solr_queryset_class_scope(testdir):
     # test class scope logic when using mock solr queryset fixture
 
+    # copy local test settings into the test dir
+    testdir.copy_example("testsettings.py")
+
     # create a temporary pytest test file
     testdir.makepyfile(
         """
         import pytest
         # causes "Plugin already registered" error on travis...
         # pytest_plugins = "parasolr.pytest_plugin"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `parasolr-0.9.1/parasolr/tests/test_schema.py` & `parasolr-0.9.2/parasolr/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/parasolr.egg-info/PKG-INFO` & `parasolr-0.9.2/parasolr.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 Metadata-Version: 2.1
 Name: parasolr
-Version: 0.9.1
+Version: 0.9.2
 Summary: Lightweight python library for Solr indexing, searching and schema management with optional Django integration.
 Home-page: https://github.com/Princeton-CDH/parasolr
 Author: The Center for Digital Humanities at Princeton
 Author-email: cdhdevteam@princeton.edu
 License: Apache License, Version 2.0
 Classifier: Environment :: Web Environment
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Database
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: addict
+Requires-Dist: progressbar2
 Provides-Extra: test
+Requires-Dist: pytest>=7; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: django
+Requires-Dist: django>=3.0; extra == "django"
+Requires-Dist: pytest-django>=3.6; extra == "django"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: pytest>=7; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinxcontrib-napoleon; extra == "dev"
+Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: django>=3.0; extra == "dev"
+Requires-Dist: pytest-django>=3.6; extra == "dev"
 
 parasolr
 ==============
 
 .. sphinx-start-marker-do-not-remove
 
 **parasolr** is a lightweight python library for `Apache Solr`_ indexing,
@@ -71,26 +89,22 @@
    :target: https://www.codefactor.io/repository/github/princeton-cdh/parasolr
    :alt: CodeFactor
 
   .. image:: https://api.codeclimate.com/v1/badges/73394d05decdf32f12f3/maintainability
    :target: https://codeclimate.com/github/Princeton-CDH/parasolr/maintainability
    :alt: Maintainability
 
-  .. image:: https://requires.io/github/Princeton-CDH/parasolr/requirements.svg?branch=main
-    :target: https://requires.io/github/Princeton-CDH/parasolr/requirements/?branch=main
-    :alt: Requirements Status
-
   .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: code style: Black
 
   .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
-Tested against Python 3.9-3.11, Solr 8.6 and 9.2, and Django 3.2-4.0 and without Django.
+Tested against Python 3.9-3.11, Solr 8.6 and 9.2, and Django 3.2-5.0 and without Django.
 
 
 Installation
 ------------
 
 Install released version from pypi::
 
@@ -128,15 +142,15 @@
 Development instructions
 ------------------------
 
 This git repository uses git flow branching conventions.
 
 Initial setup and installation:
 
-- *Recommmended*: create and activate a Python 3.6 virtualenv::
+- *Recommmended*: create and activate a Python 3.x virtualenv::
 
    python3 -m venv parasolr
    source parasolr/bin/activate
 
 - Install the package with its dependencies as well as development
   dependencies::
 
@@ -190,13 +204,13 @@
 
 
 License
 -------
 
 **parasolr** is distributed under the Apache 2.0 License.
 
-©2019 Trustees of Princeton University.  Permission granted via
+©2019-2024 Trustees of Princeton University.  Permission granted via
 Princeton Docket #20-3619 for distribution online under a standard Open Source
 license.  Ownership rights transferred to Rebecca Koeser provided software
 is distributed online via open source.
```

### Comparing `parasolr-0.9.1/parasolr.egg-info/SOURCES.txt` & `parasolr-0.9.2/parasolr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parasolr-0.9.1/setup.py` & `parasolr-0.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 REQUIREMENTS = ["requests", "addict", "progressbar2"]
 # NOTE: progressbar only needed for django index script; make optional?
-TEST_REQUIREMENTS = ["pytest>5.2", "pytest-cov"]
+TEST_REQUIREMENTS = ["pytest>=7", "pytest-cov"]
 DEV_REQUIREMENTS = [
     "sphinx",
     "sphinxcontrib-napoleon",
     "sphinx-autodoc-typehints",
     "pre-commit",
 ]
 # django integration is optional
-DJANGO_REQUIREMENTS = ["django>=2.2", "pytest-django>=3.6"]
+DJANGO_REQUIREMENTS = ["django>=3.0", "pytest-django>=3.6"]
 
 setup(
     name="parasolr",
     version=__version__,
     packages=find_packages(),
     include_package_data=True,
     license="Apache License, Version 2.0",
@@ -40,27 +40,30 @@
         "django": DJANGO_REQUIREMENTS,
         "dev": TEST_REQUIREMENTS + DEV_REQUIREMENTS + DJANGO_REQUIREMENTS,
     },
     author="The Center for Digital Humanities at Princeton",
     author_email="cdhdevteam@princeton.edu",
     classifiers=[
         "Environment :: Web Environment",
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 4 - Beta",
         "Framework :: Django",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Database",
     ],
     entry_points={
         "pytest11": [
             "parasolr = parasolr.pytest_plugin",
         ]
```

